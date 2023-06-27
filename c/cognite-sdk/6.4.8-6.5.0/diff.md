# Comparing `tmp/cognite_sdk-6.4.8.tar.gz` & `tmp/cognite_sdk-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.4.8.tar", max compression
+gzip compressed data, was "cognite_sdk-6.5.0.tar", max compression
```

## Comparing `cognite_sdk-6.4.8.tar` & `cognite_sdk-6.5.0.tar`

### file list

```diff
@@ -1,114 +1,115 @@
--rw-r--r--   0        0        0    11349 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/README.md
--rw-r--r--   0        0        0      574 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49083 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     7917 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     8418 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    26302 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6455 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     7862 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11025 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21276 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17192 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41485 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45301 2023-06-23 11:04:57.462317 cognite_sdk-6.4.8/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49823 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9466 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27887 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21811 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4589 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9525 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38099 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     3629 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0    12057 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7395 2023-06-23 11:04:57.466318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4019 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     6593 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    29220 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0     2582 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14836 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6037 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7684 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-23 11:04:57.470318 cognite_sdk-6.4.8/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-23 11:04:57.474318 cognite_sdk-6.4.8/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/README.md
+-rw-r--r--   0        0        0      574 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     7558 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49210 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     8056 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8429 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    37786 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6503 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7897 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11115 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87544 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21384 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17504 2023-06-27 12:38:07.730688 cognite_sdk-6.5.0/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41584 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45636 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    50175 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9619 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6088 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24756 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22919 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    38200 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7936 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    28258 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19276 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    22021 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     5083 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4691 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9705 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1881 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38099 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-06-27 12:38:07.734688 cognite_sdk-6.5.0/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     4087 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0     5065 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/aggregations.py
+-rw-r--r--   0        0        0    11348 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7395 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4710 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     6593 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    30982 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0     2582 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    15081 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6037 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-06-27 12:38:07.738688 cognite_sdk-6.5.0/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7684 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-27 12:38:07.742689 cognite_sdk-6.5.0/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-27 12:38:07.746689 cognite_sdk-6.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.5.0/PKG-INFO
```

### Comparing `cognite_sdk-6.4.8/LICENSE` & `cognite_sdk-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/README.md` & `cognite_sdk-6.5.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/__init__.py` & `cognite_sdk-6.5.0/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/annotations.py` & `cognite_sdk-6.5.0/cognite/client/_api/annotations.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         ...
 
     @overload
     def create(self, annotations: Sequence[Annotation]) -> AnnotationList:
         ...
 
     def create(self, annotations: Union[Annotation, Sequence[Annotation]]) -> Union[Annotation, AnnotationList]:
-        """Create annotations
+        """`Create annotations <https://developer.cognite.com/api#tag/Annotations/operation/annotationsCreate>`_
 
         Args:
             annotations (Union[Annotation, Sequence[Annotation]]): annotation(s) to create
 
         Returns:
             Union[Annotation, AnnotationList]: created annotation(s)
         """
@@ -42,15 +42,15 @@
         ...
 
     @overload
     def suggest(self, annotations: Sequence[Annotation]) -> AnnotationList:
         ...
 
     def suggest(self, annotations: Union[Annotation, Sequence[Annotation]]) -> Union[Annotation, AnnotationList]:
-        """Suggest annotations
+        """`Suggest annotations <https://developer.cognite.com/api#tag/Annotations/operation/annotationsSuggest>`_
 
         Args:
             annotations (Union[Annotation, Sequence[Annotation]]): annotation(s) to suggest. They must have status set to "suggested".
 
         Returns:
             Union[Annotation, AnnotationList]: suggested annotation(s)
         """
@@ -75,15 +75,15 @@
         if "status" in item:
             if item["status"] != "suggested":
                 raise ValueError("status field for Annotation suggestions must be set to 'suggested'")
             del item["status"]
         return item
 
     def list(self, filter: Union[AnnotationFilter, Dict], limit: int = LIST_LIMIT_DEFAULT) -> AnnotationList:
-        """List annotations.
+        """`List annotations. <https://developer.cognite.com/api#tag/Annotations/operation/annotationsFilter>`_
 
         Args:
             limit (int): Maximum number of annotations to return. Defaults to 25.
             filter (AnnotationFilter): Return annotations with parameter values that matches what is specified. Note that annotated_resource_type and annotated_resource_ids are always required.
 
         Returns:
             AnnotationList: list of annotations
@@ -125,45 +125,45 @@
     @overload
     def update(self, item: Sequence[Union[Annotation, AnnotationUpdate]]) -> AnnotationList:
         ...
 
     def update(
         self, item: Union[Annotation, AnnotationUpdate, Sequence[Union[Annotation, AnnotationUpdate]]]
     ) -> Union[Annotation, AnnotationList]:
-        """Update annotations
+        """`Update annotations <https://developer.cognite.com/api#tag/Annotations/operation/annotationsUpdate>`_
 
         Args:
             item (Union[Annotation, AnnotationUpdate, Sequence[Union[Annotation, AnnotationUpdate]]]): Annotation or list of annotations to update (or patch or list of patches to apply)
         """
         return self._update_multiple(
             list_cls=AnnotationList, resource_cls=Annotation, update_cls=AnnotationUpdate, items=item
         )
 
     def delete(self, id: Union[int, Sequence[int]]) -> None:
-        """Delete annotations
+        """`Delete annotations <https://developer.cognite.com/api#tag/Annotations/operation/annotationsDelete>`_
 
         Args:
             id (Union[int, Sequence[int]]): ID or list of IDs to be deleted
         """
         self._delete_multiple(identifiers=IdentifierSequence.load(ids=id), wrap_ids=True)
 
     def retrieve_multiple(self, ids: Sequence[int]) -> AnnotationList:
-        """Retrieve annotations by IDs
+        """`Retrieve annotations by IDs <https://developer.cognite.com/api#tag/Annotations/operation/annotationsByids>`_`
 
         Args:
             ids (Sequence[int]]: list of IDs to be retrieved
 
         Returns:
             AnnotationList: list of annotations
         """
         identifiers = IdentifierSequence.load(ids=ids, external_ids=None)
         return self._retrieve_multiple(list_cls=AnnotationList, resource_cls=Annotation, identifiers=identifiers)
 
     def retrieve(self, id: int) -> Optional[Annotation]:
-        """Retrieve an annotation by id
+        """`Retrieve an annotation by id <https://developer.cognite.com/api#tag/Annotations/operation/annotationsGet>`_
 
         Args:
             id (int): id of the annotation to be retrieved
 
         Returns:
             Annotation: annotation requested
         """
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/assets.py` & `cognite_sdk-6.5.0/cognite/client/_api/assets.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,15 +151,15 @@
 
         Yields:
             Asset: yields Assets one by one.
         """
         return cast(Iterator[Asset], self())
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[Asset]:
-        """`Retrieve a single asset by id. <https://docs.cognite.com/api/v1/#operation/getAsset>`_
+        """`Retrieve a single asset by id. <https://developer.cognite.com/api#tag/Assets/operation/getAsset>`_
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
 
         Returns:
             Optional[Asset]: Requested asset or None if it does not exist.
@@ -183,15 +183,15 @@
 
     def retrieve_multiple(
         self,
         ids: Optional[Sequence[int]] = None,
         external_ids: Optional[Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> AssetList:
-        """`Retrieve multiple assets by id. <https://docs.cognite.com/api/v1/#operation/byIdsAssets>`_
+        """`Retrieve multiple assets by id. <https://developer.cognite.com/api#tag/Assets/operation/byIdsAssets>`_
 
         Args:
             ids (Sequence[int], optional): IDs
             external_ids (Sequence[str], optional): External IDs
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -233,15 +233,15 @@
         last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
         root: bool = None,
         external_id_prefix: str = None,
         aggregated_properties: Sequence[str] = None,
         partitions: int = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> AssetList:
-        """`List assets <https://docs.cognite.com/api/v1/#operation/listAssets>`_
+        """`List assets <https://developer.cognite.com/api#tag/Assets/operation/listAssets>`_
 
         Args:
             name (str): Name of asset. Often referred to as tag.
             parent_ids (Sequence[int]): Return only the direct descendants of the specified assets.
             parent_external_ids (Sequence[str]): Return only the direct descendants of the specified assets.
             asset_subtree_ids (Union[int, Sequence[int]]): Asset subtree id or list of asset subtree ids to filter on.
             asset_subtree_external_ids (Union[str, Sequence[str]]): Asset subtree external id or list of asset subtree external ids to filter on.
@@ -325,15 +325,15 @@
             limit=limit,
             filter=filter,
             other_params={"aggregatedProperties": aggregated_properties} if aggregated_properties else {},
             partitions=partitions,
         )
 
     def aggregate(self, filter: Union[AssetFilter, dict] = None) -> List[AssetAggregate]:
-        """`Aggregate assets <https://docs.cognite.com/api/v1/#operation/aggregateAssets>`_
+        """`Aggregate assets <https://developer.cognite.com/api#tag/Assets/operation/aggregateAssets>`_
 
         Args:
             filter (Union[AssetFilter, Dict]): Filter on assets filter with exact match
 
         Returns:
             List[AssetAggregate]: List of asset aggregates
 
@@ -344,15 +344,15 @@
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> aggregate_by_prefix = c.assets.aggregate(filter={"external_id_prefix": "prefix"})
         """
         return self._aggregate(filter=filter, cls=AssetAggregate)
 
     def aggregate_metadata_keys(self, filter: Union[AssetFilter, dict] = None) -> Sequence[AggregateBucketResult]:
-        """`Aggregate assets <https://docs.cognite.com/api/v1/#operation/aggregateAssets>`_
+        """`Aggregate assets <https://developer.cognite.com/api#tag/Assets/operation/aggregateAssets>`_
 
         Note:
             In the case of text fields, the values are aggregated in a case-insensitive manner
 
         Args:
             filter (Union[AssetFilter, Dict]): Filter on assets filter with exact match
 
@@ -368,15 +368,15 @@
                 >>> aggregate_by_prefix = c.assets.aggregate_metadata_keys(filter={"external_id_prefix": "prefix"})
         """
         return self._aggregate(filter=filter, aggregate="metadataKeys", cls=AggregateBucketResult)
 
     def aggregate_metadata_values(
         self, keys: Sequence[str], filter: Union[AssetFilter, dict] = None
     ) -> Sequence[AggregateBucketResult]:
-        """`Aggregate assets <https://docs.cognite.com/api/v1/#operation/aggregateAssets>`_
+        """`Aggregate assets <https://developer.cognite.com/api#tag/Assets/operation/aggregateAssets>`_
 
         Note:
             In the case of text fields, the values are aggregated in a case-insensitive manner
 
         Args:
             filter (Union[AssetFilter, Dict]): Filter on assets filter with exact match
             keys (Sequence[str]): Metadata key(s) to apply the aggregation on. Currently supports exactly one key per request.
@@ -402,15 +402,15 @@
         ...
 
     @overload
     def create(self, asset: Asset) -> Asset:
         ...
 
     def create(self, asset: Union[Asset, Sequence[Asset]]) -> Union[Asset, AssetList]:
-        """`Create one or more assets. <https://docs.cognite.com/api/v1/#operation/createAssets>`_
+        """`Create one or more assets. <https://developer.cognite.com/api#tag/Assets/operation/createAssets>`_
 
         You can create an arbitrary number of assets, and the SDK will split the request into multiple requests.
         When specifying parent-child relation between assets using `parentExternalId` the link will be resvoled into an internal ID and stored as `parentId`.
 
         Args:
             asset (Union[Asset, Sequence[Asset]]): Asset or list of assets to create.
 
@@ -573,15 +573,15 @@
     def delete(
         self,
         id: Union[int, Sequence[int]] = None,
         external_id: Union[str, Sequence[str]] = None,
         recursive: bool = False,
         ignore_unknown_ids: bool = False,
     ) -> None:
-        """`Delete one or more assets <https://doc.cognitedata.com/api/v1/#operation/deleteAssets>`_
+        """`Delete one or more assets <https://developer.cognite.com/api#tag/Assets/operation/deleteAssets>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
             recursive (bool): Recursively delete whole asset subtrees under given ids. Defaults to False.
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
@@ -607,15 +607,15 @@
         ...
 
     @overload
     def update(self, item: Union[Asset, AssetUpdate]) -> Asset:
         ...
 
     def update(self, item: Union[Asset, AssetUpdate, Sequence[Union[Asset, AssetUpdate]]]) -> Union[Asset, AssetList]:
-        """`Update one or more assets <https://docs.cognite.com/api/v1/#operation/updateAssets>`_
+        """`Update one or more assets <https://developer.cognite.com/api#tag/Assets/operation/updateAssets>`_
         Labels can be added, removed or replaced (set). Note that set operation deletes all the existing labels and adds the new specified labels.
 
         Args:
             item (Union[Asset, AssetUpdate, Sequence[Union[Asset, AssetUpdate]]]): Asset(s) to update
 
         Returns:
             Union[Asset, AssetList]: Updated asset(s)
@@ -674,15 +674,15 @@
         self,
         name: str = None,
         description: str = None,
         query: str = None,
         filter: Union[AssetFilter, Dict] = None,
         limit: int = 100,
     ) -> AssetList:
-        """`Search for assets <https://docs.cognite.com/api/v1/#operation/searchAssets>`_
+        """`Search for assets <https://developer.cognite.com/api#tag/Assets/operation/searchAssets>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             name (str): Fuzzy match on name.
             description (str): Fuzzy match on description.
             query (str): Whitespace-separated terms to search for in assets. Does a best-effort fuzzy search in relevant fields (currently name and description) for variations of any of the search terms, and orders results by relevance.
             filter (Union[AssetFilter, Dict]): Filter to apply. Performs exact match on these fields.
@@ -939,15 +939,17 @@
         # Since we enforce XID given and 'no ID', there's no point in "renaming xid to itself":
         dct_update.pop("externalId")
         if patch:
             if "metadata" in dumped:
                 dct_update["metadata"]["add"] = dct_update["metadata"].pop("set")
             if "labels" in dumped:
                 dct_update["labels"]["add"] = dct_update["labels"].pop("set")
-        (upd := AssetUpdate(external_id=dumped["externalId"]))._update_object = dct_update
+
+        upd = AssetUpdate(external_id=dumped["externalId"])
+        upd._update_object = dct_update
         return upd
 
     @cached_property
     def clear_all_update(self) -> MappingProxyType[str, Dict[str, Any]]:
         props = set(map(to_camel_case, AssetUpdate._get_update_properties()))
         # Does not support setNull:
         props -= {"name", "parentExternalId", "parentId"}
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,15 +85,15 @@
         ...
 
     @overload
     def retrieve(self, ids: Sequence[ContainerIdentifier]) -> ContainerList:
         ...
 
     def retrieve(self, ids: ContainerIdentifier | Sequence[ContainerIdentifier]) -> Container | ContainerList | None:
-        """`Retrieve one or more container by id(s). <https://docs.cognite.com/api/v1/#operation/byExternalIdsContainers>`_
+        """`Retrieve one or more container by id(s). <https://developer.cognite.com/api#tag/Containers/operation/byExternalIdsContainers>`_
 
         Args:
             ids (ContainerId | Sequence[ContainerId]): Identifier for container(s).
 
         Returns:
             Optional[Container]: Requested container or None if it does not exist.
 
@@ -102,23 +102,23 @@
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.containers.retrieve(('mySpace', 'myContainer'))
 
             Fetch using the ContainerId::
 
                 >>> from cognite.client import CogniteClient
-                >>> from cognite.client.data_modeling import ContainerId
+                >>> from cognite.client.data_classes.data_modeling import ContainerId
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.containers.retrieve(ContainerId(space='mySpace', external_id='myContainer'))
         """
         identifier = _load_identifier(ids, "container")
         return self._retrieve_multiple(list_cls=ContainerList, resource_cls=Container, identifiers=identifier)
 
     def delete(self, id: ContainerIdentifier | Sequence[ContainerIdentifier]) -> list[ContainerId]:
-        """`Delete one or more containers <https://docs.cognite.com/api/v1/#operation/deleteContainers>`_
+        """`Delete one or more containers <https://developer.cognite.com/api#tag/Containers/operation/deleteContainers>`_
 
         Args:
             id (ContainerId | Sequence[ContainerId): The container identifier(s).
         Returns:
             The container(s) which has been deleted. Empty list if nothing was deleted.
         Examples:
 
@@ -133,15 +133,15 @@
             self._delete_multiple(identifiers=_load_identifier(id, "container"), wrap_ids=True, returns_items=True),
         )
         return [ContainerId(space=item["space"], external_id=item["externalId"]) for item in deleted_containers]
 
     def list(
         self, space: str | None = None, limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT, include_global: bool = False
     ) -> ContainerList:
-        """`List containers <https://docs.cognite.com/api/v1/#operation/listContainers>`_
+        """`List containers <https://developer.cognite.com/api#tag/Containers/operation/listContainers>`_
 
         Args:
             space (int, optional): The space to query
             limit (int, optional): Maximum number of containers to return. Default to 10. Set to -1, float("inf") or None
                 to return all items.
             include_global (bool, optional): Whether the global containers should be returned.
 
@@ -185,28 +185,29 @@
         ...
 
     @overload
     def apply(self, container: ContainerApply) -> Container:
         ...
 
     def apply(self, container: ContainerApply | Sequence[ContainerApply]) -> Container | ContainerList:
-        """`Add or update (upsert) containers. <https://docs.cognite.com/api/v1/#operation/ApplyContainers>`_
+        """`Add or update (upsert) containers. <https://developer.cognite.com/api#tag/Containers/operation/ApplyContainers>`_
 
         Args:
             container (container: ContainerApply | Sequence[ContainerApply]): Container or containers of containers to create or update.
 
         Returns:
             Container | ContainerList: Created container(s)
 
         Examples:
 
             Create new containers:
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_classes.data_modeling as models
+                >>> from cognite.client.data_classes.data_modeling import ContainerApply, ContainerProperty, Text
                 >>> c = CogniteClient()
-                >>> containers = [models.ContainerApply(space="mySpace",properties={"name": models.ContainerProperty(type=models.TextType, name="name")})]
-                >>> res = c.data_modeling.containers.apply(containers)
+                >>> container = [ContainerApply(space="mySpace", external_id="myContainer",
+                ...     properties={"name": ContainerProperty(type=Text(), name="name")})]
+                >>> res = c.data_modeling.containers.apply(container)
         """
         return self._create_multiple(
             list_cls=ContainerList, resource_cls=Container, items=container, input_resource_cls=ContainerApply
         )
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/data_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
         Yields:
             DataModel: yields DataModels one by one.
         """
         return cast(Iterator[DataModel], self())
 
     def retrieve(self, ids: DataModelIdentifier | Sequence[DataModelIdentifier]) -> DataModelList:
-        """`Retrieve data_model(s) by id(s). <https://docs.cognite.com/api/v1/#operation/byExternalIdsDataModels>`_
+        """`Retrieve data_model(s) by id(s). <https://developer.cognite.com/api#tag/Data-models/operation/byExternalIdsDataModels>`_
 
         Args:
             ids (DataModelId | Sequence[DataModelId]): Data Model identifier(s).
 
         Returns:
             Optional[DataModel]: Requested data_model or None if it does not exist.
 
@@ -106,15 +106,15 @@
                 >>> res = c.data_modeling.data_models.retrieve(("mySpace", "myDataModel", "v1"))
 
         """
         identifier = _load_identifier(ids, "data_model")
         return self._retrieve_multiple(list_cls=DataModelList, resource_cls=DataModel, identifiers=identifier)
 
     def delete(self, ids: DataModelIdentifier | Sequence[DataModelIdentifier]) -> list[DataModelId]:
-        """`Delete one or more data model <https://docs.cognite.com/api/v1/#operation/deleteDataModels>`_
+        """`Delete one or more data model <https://developer.cognite.com/api#tag/Data-models/operation/deleteDataModels>`_
 
         Args:
             ids (DataModelId | Sequence[DataModelId]): Data Model identifier(s).
         Returns:
             The data_model(s) which has been deleted. None if nothing was deleted.
         Examples:
 
@@ -134,15 +134,15 @@
         self,
         limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT,
         space: str | None = None,
         inline_views: bool = False,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> DataModelList:
-        """`List data models <https://docs.cognite.com/api/v1/#operation/listDataModels>`_
+        """`List data models <https://developer.cognite.com/api#tag/Data-models/operation/listDataModels>`_
 
         Args:
             limit (int, optional): Maximum number of data model to return. Default to 10. Set to -1, float("inf") or None
                 to return all items.
             space: (str | None): The space to query.
             inline_views (bool): Whether to expand the referenced views inline in the returned result.
             all_versions (bool): Whether to return all versions. If false, only the newest version is returned,
@@ -189,29 +189,29 @@
         ...
 
     @overload
     def apply(self, data_model: DataModelApply) -> DataModel:
         ...
 
     def apply(self, data_model: DataModelApply | Sequence[DataModelApply]) -> DataModel | DataModelList:
-        """`Create or update one or more data model. <https://docs.cognite.com/api/v1/#operation/createDataModels>`_
+        """`Create or update one or more data model. <https://developer.cognite.com/api#tag/Data-models/operation/createDataModels>`_
 
         Args:
             data_model (data_model: DataModelApply | Sequence[DataModelApply]): DataModel or data model to create or update (upsert).
 
         Returns:
             DataModel | DataModelList: Created data_model(s)
 
         Examples:
 
             Create new data model::
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_classes.data_modeling as models
+                >>> from cognite.client.data_classes.data_modeling import DataModelApply
                 >>> c = CogniteClient()
-                >>> data_models = [models.DataModelApply(space="mySpace",external_id="myDataModel",version="v1",is_global=,last_updated_time=),
-                ... DataModelApply(space="mySpace",external_id="myOtherDataModel",version="v1",is_global=,last_updated_time=)]
+                >>> data_models = [DataModelApply(space="mySpace",external_id="myDataModel",version="v1"),
+                ... DataModelApply(space="mySpace",external_id="myOtherDataModel",version="v1")]
                 >>> res = c.data_modeling.data_models.apply(data_models)
         """
         return self._create_multiple(
             list_cls=DataModelList, resource_cls=DataModel, items=data_model, input_resource_cls=DataModelApply
         )
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/instances.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
 
 import json
-from typing import TYPE_CHECKING, Any, Iterator, List, Literal, Sequence, Union, cast, overload
+from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Literal, Sequence, Type, Union, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import INSTANCES_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes._base import CogniteResourceList
+from cognite.client.data_classes.data_modeling.aggregations import Aggregation, Histogram, HistogramValue
 from cognite.client.data_classes.data_modeling.filters import Filter
 from cognite.client.data_classes.data_modeling.ids import (
     EdgeId,
     NodeId,
     ViewId,
     ViewIdentifier,
     _load_identifier,
 )
 from cognite.client.data_classes.data_modeling.instances import (
     Edge,
     EdgeApply,
     EdgeApplyResult,
     EdgeApplyResultList,
     EdgeList,
+    InstanceAggregationResultList,
     InstancesApplyResult,
     InstancesDeleteResult,
     InstanceSort,
     InstancesResult,
     Node,
     NodeApply,
     NodeApplyResult,
@@ -99,16 +101,16 @@
 
 class InstancesAPI(APIClient):
     _RESOURCE_PATH = "/models/instances"
 
     @overload
     def __call__(
         self,
-        chunk_size: None,
-        instance_type: Literal["node"],
+        chunk_size: None = None,
+        instance_type: Literal["node"] = "node",
         limit: int | None = None,
         include_typing: bool = False,
         sources: list[ViewId] | ViewId | None = None,
         sort: list[InstanceSort | dict] | InstanceSort | dict | None = None,
         filter: Filter | dict | None = None,
     ) -> Iterator[Node]:
         ...
@@ -126,15 +128,15 @@
     ) -> Iterator[Edge]:
         ...
 
     @overload
     def __call__(
         self,
         chunk_size: int,
-        instance_type: Literal["node"],
+        instance_type: Literal["node"] = "node",
         limit: int | None = None,
         include_typing: bool = False,
         sources: list[ViewId] | ViewId | None = None,
         sort: list[InstanceSort | dict] | InstanceSort | dict | None = None,
         filter: Filter | dict | None = None,
     ) -> Iterator[NodeList]:
         ...
@@ -214,15 +216,15 @@
     def retrieve(
         self,
         nodes: NodeId | Sequence[NodeId] | tuple[str, str] | Sequence[tuple[str, str]] | None = None,
         edges: EdgeId | Sequence[EdgeId] | tuple[str, str] | Sequence[tuple[str, str]] | None = None,
         sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         include_typing: bool = False,
     ) -> InstancesResult:
-        """`Retrieve one or more instance by id(s). <https://docs.cognite.com/api/v1/#tag/Instances/operation/byExternalIdsInstances>`_
+        """`Retrieve one or more instance by id(s). <https://developer.cognite.com/api#tag/Instances/tag/Instances/operation/byExternalIdsInstances>`_
 
         Args:
             nodes (NodeId | Sequence[NodeId] | tuple[str, str] | Sequence[tuple[str, str]] | None): Node ids
             edges (EdgeId | Sequence[EdgeId] | tuple[str, str] | Sequence[tuple[str, str]] | None): Edge ids
             sources (ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence(View) None): Retrieve properties from the listed - by reference - views.
             include_typing (bool): Whether to return property type information as part of the result.
 
@@ -239,29 +241,29 @@
                 ...                                          edges=("mySpace", "myEdgeExternalId"),
                 ...                                          sources=("mySpace", "myViewExternalId", "myViewVersion")
                 ...                                         )
 
             Retrieve nodes an edges using the built in data class
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_modeling as dm
+                >>> from cognite.client.data_classes.data_modeling import NodeId, EdgeId, ViewId
                 >>> c = CogniteClient()
-                >>> res = c.data_modeling.instances.retrieve(dm.NodeId("mySpace", "myNode"),
-                ...                                          dm.EdgeId("mySpace", "myEdge"),
-                ...                                          dm.ViewId("mySpace", "myViewExternalId", "myViewVersion")
+                >>> res = c.data_modeling.instances.retrieve(NodeId("mySpace", "myNode"),
+                ...                                          EdgeId("mySpace", "myEdge"),
+                ...                                          ViewId("mySpace", "myViewExternalId", "myViewVersion")
                 ...                                         )
 
             Retrieve nodes an edges using the the view object as source
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_modeling as dm
+                >>> from cognite.client.data_classes.data_modeling import NodeId, EdgeId
                 >>> c = CogniteClient()
-                >>> res = c.data_modeling.instances.retrieve(dm.NodeId("mySpace", "myNode"),
-                ...                                          dm.EdgeId("mySpace", "myEdge"),
-                ...                                          sources='myView')
+                >>> res = c.data_modeling.instances.retrieve(NodeId("mySpace", "myNode"),
+                ...                                          EdgeId("mySpace", "myEdge"),
+                ...                                          sources=("myspace", "myView")
                 ...                                         )
         """
         identifiers = self._load_node_and_edge_ids(nodes, edges)
         other_params = self._create_other_params(
             include_typing=include_typing,
             sources=sources,
             sort=None,
@@ -306,15 +308,15 @@
         return DataModelingIdentifierSequence(identifiers, is_singleton=False)
 
     def delete(
         self,
         nodes: NodeId | Sequence[NodeId] | tuple[str, str] | Sequence[tuple[str, str]] | None = None,
         edges: EdgeId | Sequence[EdgeId] | tuple[str, str] | Sequence[tuple[str, str]] | None = None,
     ) -> InstancesDeleteResult:
-        """`Delete one or more instances <https://docs.cognite.com/api/v1/#tag/Instances/operation/deleteBulk>`_
+        """`Delete one or more instances <https://developer.cognite.com/api#tag/Instances/tag/Instances/operation/deleteBulk>`_
 
         Args:
             nodes (NodeId | Sequence[NodeId] | tuple[str, str] | Sequence[tuple[str, str]] | None): Node ids
             edges (EdgeId | Sequence[EdgeId] | tuple[str, str] | Sequence[tuple[str, str]] | None): Edge ids
 
         Returns:
             The instance(s) which has been deleted. Empty list if nothing was deleted.
@@ -326,30 +328,30 @@
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.data_modeling.instances.delete(nodes=("myNode", "mySpace"))
 
             Delete nodes and edges using the built in data class
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_modeling as dm
+                >>> from cognite.client.data_classes.data_modeling import NodeId, EdgeId
                 >>> c = CogniteClient()
-                >>> c.data_modeling.instances.delete(dm.NodeId('mySpace', 'myNode'), dm.EdgeId('mySpace', 'myEdge'))
+                >>> c.data_modeling.instances.delete(NodeId('mySpace', 'myNode'), EdgeId('mySpace', 'myEdge'))
         """
         identifiers = self._load_node_and_edge_ids(nodes, edges)
         deleted_instances = cast(List, self._delete_multiple(identifiers, wrap_ids=True, returns_items=True))
         node_ids = [NodeId.load(item) for item in deleted_instances if item["instanceType"] == "node"]
         edge_ids = [EdgeId.load(item) for item in deleted_instances if item["instanceType"] == "edge"]
         return InstancesDeleteResult(node_ids, edge_ids)
 
     @classmethod
     def _create_other_params(
         cls,
         *,
         include_typing: bool,
-        sort: list[InstanceSort | dict] | InstanceSort | dict | None,
+        sort: Sequence[InstanceSort | dict] | InstanceSort | dict | None,
         sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None,
         instance_type: Literal["node", "edge"] | None,
     ) -> dict[str, Any]:
         other_params: dict[str, Any] = {"includeTyping": include_typing}
         if sources:
             other_params["sources"] = (
                 [cls._dump_instance_source(source) for source in sources]
@@ -384,15 +386,15 @@
         edges: EdgeApply | Sequence[EdgeApply] | None = None,
         auto_create_start_nodes: bool = False,
         auto_create_end_nodes: bool = False,
         auto_create_direct_relations: bool = True,
         skip_on_version_conflict: bool = False,
         replace: bool = False,
     ) -> InstancesApplyResult:
-        """`Add or update (upsert) instances. <https://docs.cognite.com/api/v1/#tag/Instances/operation/applyNodeAndEdges>`_
+        """`Add or update (upsert) instances. <https://developer.cognite.com/api#tag/Instances/tag/Instances/operation/applyNodeAndEdges>`_
 
         Args:
             nodes (NodeApply | Sequence[NodeApply] | None = None): Nodes to apply
             edges (EdgeApply | Sequence[EdgeApply] | None = None): Edges to apply
             auto_create_start_nodes (bool): Whether to create missing start nodes for edges when ingesting. By default,
                                             the start node of an edge must exist before it can be ingestested.
             auto_create_end_nodes (bool): Whether to create missing end nodes for edges when ingesting. By default,
@@ -411,55 +413,55 @@
             InstancesApplyResult: Created instance(s)
 
         Examples:
 
             Create new node without data:
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_modeling as dm
+                >>> from cognite.client.data_classes.data_modeling import EdgeApply, NodeOrEdgeData, NodeApply
                 >>> c = CogniteClient()
-                >>> nodes = [dm.ApplyNode("mySpace", "myNodeId")]
+                >>> nodes = [NodeApply("mySpace", "myNodeId")]
                 >>> res = c.data_modeling.instances.apply(nodes)
 
             Create two nodes with data with an one to many edge, and a one to one edge
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_modeling as dm
-                >>> person = dm.NodeApply("mySpace", "person:arnold_schwarzenegger", sources=[
-                ...                        dm.NodeOrEdgeData(
-                ...                               dm.ViewId("mySpace", "PersonView", "v1"),
+                >>> from cognite.client.data_classes.data_modeling import EdgeApply, NodeOrEdgeData, NodeApply, ViewId
+                >>> person = NodeApply("mySpace", "person:arnold_schwarzenegger", sources=[
+                ...                        NodeOrEdgeData(
+                ...                               ViewId("mySpace", "PersonView", "v1"),
                 ...                               {"name": "Arnold Schwarzenegger", "birthYear": 1947})
                 ... ])
-                >>> actor = dm.NodeApply("mySpace", "actor:arnold_schwarzenegger", sources=[
-                ...                        dm.NodeOrEdgeData(
-                ...                               dm.ViewId("mySpace", "ActorView", "v1"),
+                >>> actor = NodeApply("mySpace", "actor:arnold_schwarzenegger", sources=[
+                ...                        NodeOrEdgeData(
+                ...                               ViewId("mySpace", "ActorView", "v1"),
                 ...                               {"wonOscar": False,
                 ...                               # This is a one-to-one edge from actor to person
                 ...                                "person": {"space": "mySpace", "externalId": "person:arnold_schwarzenegger"}})
                 ... ])
                 >>> # This is one to many edge, in this case from Person to role
                 >>> # (a person can have multiple roles, in this model for example Actor and Director)
-                >>> person_to_actor = dm.EdgeApply(space="mySpace",
+                >>> person_to_actor = EdgeApply(space="mySpace",
                 ...                                       external_id="relation:arnold_schwarzenegger:actor",
-                ...                                       type="Person.roles",
-                ...                                       start_node="person:arnold_schwarzenegger",
-                ...                                       end_node="actor:arnold_schwarzenegger",
+                ...                                       type=("Person", "roles"),
+                ...                                       start_node=("person", "arnold_schwarzenegger"),
+                ...                                       end_node=("actor", "arnold_schwarzenegger"),
                 ... )
                 >>> res = c.data_modeling.instances.apply([person, actor], [person_to_actor])
 
             Create new edge an automatically create end nodes.
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_modeling as dm
+                >>> from cognite.client.data_classes.data_modeling import EdgeApply
                 >>> c = CogniteClient()
-                >>> edge = dm.EdgeApply(space="mySpace",
+                >>> edge = EdgeApply(space="mySpace",
                 ...                            external_id="relation:sylvester_stallone:actor",
-                ...                            type="Person.roles",
-                ...                            start_node="person:sylvester_stallone",
-                ...                            end_node="actor:sylvester_stallone",
+                ...                            type=("Person", "roles"),
+                ...                            start_node=("person", "sylvester_stallone"),
+                ...                            end_node=("actor", "sylvester_stallone"),
                 ... )
                 >>> res = c.data_modeling.instances.apply(edges=edge, auto_create_start_nodes=True, auto_create_end_nodes=True)
 
         """
         other_parameters = {
             "autoCreateStartNodes": auto_create_start_nodes,
             "autoCreateEndNodes": auto_create_end_nodes,
@@ -482,55 +484,296 @@
         )
         return InstancesApplyResult(
             nodes=NodeApplyResultList([item for item in res if isinstance(item, NodeApplyResult)]),
             edges=EdgeApplyResultList([item for item in res if isinstance(item, EdgeApplyResult)]),
         )
 
     @overload
+    def search(
+        self,
+        view: ViewId,
+        query: str,
+        instance_type: Literal["node"] = "node",
+        properties: list[str] | None = None,
+        filter: Filter | dict | None = None,
+        limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
+    ) -> NodeList:
+        ...
+
+    @overload
+    def search(
+        self,
+        view: ViewId,
+        query: str,
+        instance_type: Literal["edge"],
+        properties: list[str] | None = None,
+        filter: Filter | dict | None = None,
+        limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
+    ) -> EdgeList:
+        ...
+
+    def search(
+        self,
+        view: ViewId,
+        query: str,
+        instance_type: Literal["node", "edge"] = "node",
+        properties: list[str] | None = None,
+        filter: Filter | dict | None = None,
+        limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
+    ) -> NodeList | EdgeList:
+        """`Search instances <https://developer.cognite.com/api/v1/#tag/Instances/operation/searchInstances>`_
+
+        Args:
+            view (ViewId): View to search in.
+            query (str): Query string that will be parsed and used for search.
+            instance_type (Literal["node", "edge"]): Whether to search for nodes or edges.
+            properties (list[str]): Optional array of properties you want to search through.
+                                    If you do not specify one or more properties, the service will
+                                    search all text fields within the view.
+            filter (dict | Filter): Advnanced filtering of instances.
+            limit (int, optional): Maximum number of instances to return. Default to 1000. Set to -1, float("inf") or None
+                to return all items.
+
+        Returns:
+            EdgeList | NodeList: Search result with matching nodes or edges.
+
+        Examples:
+
+            Search for Arnold in the person view in the name property:
+
+                >>> from cognite.client import CogniteClient
+                >>> from cognite.client.data_classes.data_modeling import ViewId
+                >>> c = CogniteClient()
+                >>> res = c.data_modeling.instances.search(ViewId("mySpace", "PersonView", "v1"), query="Arnold", properties=["name"])
+
+            Search for Quentin in the person view in the name property, but only born before 1970:
+
+                >>> from cognite.client import CogniteClient
+                >>> from cognite.client.data_classes.data_modeling import ViewId
+                >>> import cognite.client.data_classes.data_modeling.filters as filters
+                >>> c = CogniteClient()
+                >>> born_after_1970 = filters.Range(["mySpace", "PersonView/v1", "birthYear"], gt=1970)
+                >>> res = c.data_modeling.instances.search(ViewId("mySpace", "PersonView", "v1"),
+                ... query="Quentin", properties=["name"], filter=born_after_1970)
+
+        """
+        if instance_type == "node":
+            list_cls: Union[Type[NodeList], Type[EdgeList]] = NodeList
+        elif instance_type == "edge":
+            list_cls = EdgeList
+        else:
+            raise ValueError(f"Invalid instance type: {instance_type}")
+
+        body = {"view": view.dump(camel_case=True), "query": query, "instanceType": instance_type, "limit": limit}
+        if properties:
+            body["properties"] = properties
+        if filter:
+            body["filter"] = filter.dump() if isinstance(filter, Filter) else filter
+
+        res = self._post(url_path=self._RESOURCE_PATH + "/search", json=body)
+        return list_cls._load(res.json()["items"], cognite_client=None)
+
+    def aggregate(
+        self,
+        view: ViewId,
+        aggregates: Aggregation | dict | Sequence[Aggregation | dict],
+        instance_type: Literal["node", "edge"] = "node",
+        group_by: Sequence[str] | None = None,
+        query: str | None = None,
+        properties: Sequence[str] | None = None,
+        filter: Filter | None = None,
+        limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
+    ) -> InstanceAggregationResultList:
+        """`Aggregate data across nodes/edges <https://developer.cognite.com/api/v1/#tag/Instances/operation/aggregateInstances>`_
+
+        Args:
+            view (ViewId): View to to aggregate over.
+            aggregates (Aggregation | dict | Sequence[Aggregation | dict]):  The properties to aggregate over.
+            instance_type (Literal["node", "edge"]): Whether to search for nodes or edges.
+            group_by (Optional[Sequence[str]]): The selection of fields to group the results by when doing aggregations.
+                                  You can specify up to 5 items to group by.
+            query (Optional[str]): Query string that will be parsed and used for search.
+            properties (Optional[Sequence[str]]): Optional array of properties you want to search through.
+                                    If you do not specify one or more properties, the service will
+                                    search all text fields within the view.
+            filter (Optional[Filter]): Advnanced filtering of instances.
+            limit (int, optional): Maximum number of instances to return. Default to 1000. Set to -1, float("inf") or None
+                to return all items.
+
+        Returns:
+            InstanceAggregationResultList: Node or edge aggregation results.
+
+        Examples:
+
+            Get the average run time in minutes for movies grouped by release year:
+
+                >>> from cognite.client import CogniteClient
+                >>> from cognite.client.data_classes.data_modeling import ViewId, aggregations as aggs
+                >>> c = CogniteClient()
+                >>> avg_run_time = aggs.Avg("runTimeMinutes")
+                >>> view_id = ViewId("mySpace", "PersonView", "v1")
+                >>> res = c.data_modeling.instances.aggregate(view_id, [avg_run_time], group_by=["releaseYear"])
+
+        """
+        if instance_type not in ("node", "edge"):
+            raise ValueError(f"Invalid instance type: {instance_type}")
+        body: Dict[str, Any] = {"view": view.dump(camel_case=True), "instanceType": instance_type, "limit": limit}
+        aggregate_seq: Sequence[Aggregation | dict] = aggregates if isinstance(aggregates, Sequence) else [aggregates]
+        body["aggregates"] = [
+            agg.dump(camel_case=True) if isinstance(agg, Aggregation) else agg for agg in aggregate_seq
+        ]
+        if group_by:
+            body["groupBy"] = group_by
+        if filter:
+            body["filter"] = filter.dump() if isinstance(filter, Filter) else filter
+        if query:
+            body["query"] = query
+        if properties:
+            body["properties"] = properties
+
+        res = self._post(url_path=self._RESOURCE_PATH + "/aggregate", json=body)
+        return InstanceAggregationResultList._load(res.json()["items"], cognite_client=None)
+
+    @overload
+    def histogram(
+        self,
+        view: ViewId,
+        histograms: Histogram,
+        instance_type: Literal["node", "edge"] = "node",
+        query: str | None = None,
+        properties: Sequence[str] | None = None,
+        filter: Filter | None = None,
+        limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
+    ) -> HistogramValue:
+        ...
+
+    @overload
+    def histogram(
+        self,
+        view: ViewId,
+        histograms: Sequence[Histogram],
+        instance_type: Literal["node", "edge"] = "node",
+        query: str | None = None,
+        properties: Sequence[str] | None = None,
+        filter: Filter | None = None,
+        limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
+    ) -> list[HistogramValue]:
+        ...
+
+    def histogram(
+        self,
+        view: ViewId,
+        histograms: Histogram | Sequence[Histogram],
+        instance_type: Literal["node", "edge"] = "node",
+        query: str | None = None,
+        properties: Sequence[str] | None = None,
+        filter: Filter | None = None,
+        limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
+    ) -> HistogramValue | list[HistogramValue]:
+        """`Produces histograms for nodes/edges <https://developer.cognite.com/api/v1/#tag/Instances/operation/aggregateInstances>`_
+
+        Args:
+            view (ViewId): View to to aggregate over.
+            histograms (Histogram | Sequence[Histogram]):  The properties to aggregate over.
+            instance_type (Literal["node", "edge"]): Whether to search for nodes or edges.
+            query (Optional[str]): Query string that will be parsed and used for search.
+            properties (Optional[Sequence[str]]): Optional array of properties you want to search through.
+                                    If you do not specify one or more properties, the service will
+                                    search all text fields within the view.
+            filter (Optional[Filter]): Advnanced filtering of instances.
+            limit (int, optional): Maximum number of instances to return. Default to 1000. Set to -1, float("inf") or None
+                to return all items.
+
+        Returns:
+            list[HistogramValue]: Node or edge aggregation results.
+
+        Examples:
+
+            Find the number of people born per decade:
+
+                >>> from cognite.client import CogniteClient
+                >>> from cognite.client.data_classes.data_modeling import aggregations as aggs, ViewId
+                >>> c = CogniteClient()
+                >>> birth_by_decade = aggs.Histogram("birthYear", interval=10.0)
+                >>> view_id = ViewId("mySpace", "PersonView", "v1")
+                >>> res = c.data_modeling.instances.histogram(view_id, birth_by_decade)
+        """
+        if instance_type not in ("node", "edge"):
+            raise ValueError(f"Invalid instance type: {instance_type}")
+        body: Dict[str, Any] = {"view": view.dump(camel_case=True), "instanceType": instance_type, "limit": limit}
+
+        if isinstance(histograms, Sequence):
+            histogram_seq: Sequence[Histogram] = histograms
+            is_singleton = False
+        elif isinstance(histograms, Histogram):
+            histogram_seq = [histograms]
+            is_singleton = True
+        else:
+            raise TypeError(f"Expected Histogram or sequence of Histograms, got {type(histograms)}")
+
+        for histogram in histogram_seq:
+            if not isinstance(histogram, Histogram):
+                raise ValueError(f"Not a histogram: {histogram}")
+
+        body["aggregates"] = [histogram.dump(camel_case=True) for histogram in histogram_seq]
+        if filter:
+            body["filter"] = filter.dump() if isinstance(filter, Filter) else filter
+        if query:
+            body["query"] = query
+        if properties:
+            body["properties"] = properties
+
+        res = self._post(url_path=self._RESOURCE_PATH + "/aggregate", json=body)
+        if is_singleton:
+            return HistogramValue.load(res.json()["items"][0]["aggregates"][0])
+        else:
+            return [HistogramValue.load(item["aggregates"][0]) for item in res.json()["items"]]
+
+    @overload
     def list(
         self,
         instance_type: Literal["node"] = "node",
         include_typing: bool = False,
         sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
-        sort: list[InstanceSort | dict] | InstanceSort | dict | None = None,
+        sort: Sequence[InstanceSort | dict] | InstanceSort | dict | None = None,
         filter: Filter | dict | None = None,
     ) -> NodeList:
         ...
 
     @overload
     def list(
         self,
         instance_type: Literal["edge"],
         include_typing: bool = False,
         sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
-        sort: list[InstanceSort | dict] | InstanceSort | dict | None = None,
+        sort: Sequence[InstanceSort | dict] | InstanceSort | dict | None = None,
         filter: Filter | dict | None = None,
     ) -> EdgeList:
         ...
 
     def list(
         self,
         instance_type: Literal["node", "edge"] = "node",
         include_typing: bool = False,
         sources: ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence[View] | None = None,
         limit: int = INSTANCES_LIST_LIMIT_DEFAULT,
-        sort: list[InstanceSort | dict] | InstanceSort | dict | None = None,
+        sort: Sequence[InstanceSort | dict] | InstanceSort | dict | None = None,
         filter: Filter | dict | None = None,
     ) -> NodeList | EdgeList:
-        """`List instances <https://docs.cognite.com/api/v1/#tag/Instances/operation/advancedListInstance>`_
+        """`List instances <https://developer.cognite.com/api#tag/Instances/tag/Instances/operation/advancedListInstance>`_
 
         Args:
             instance_type(Literal["node", "edge"]): Whether to query for nodes or edges.
             include_typing (bool): Whether to return property type information as part of the result.
             sources (ViewIdentifier | Sequence[ViewIdentifier] | View | Sequence(View) | None): Views to retrieve properties from.
             limit (int, optional): Maximum number of instances to return. Default to 1000. Set to -1, float("inf") or None
                 to return all items.
-            sort (list[InstanceSost] | InstanceSort | dict): How you want the listed instances information ordered.
+            sort (Sequence[InstanceSost] | InstanceSort | dict): How you want the listed instances information ordered.
             filter (dict | Filter): Advanced filtering of instances.
 
         Returns:
             Union[EdgeList, NodeList]: List of requested instances
 
         Examples:
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/spaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         ...
 
     @overload
     def retrieve(self, space: Sequence[str]) -> SpaceList:
         ...
 
     def retrieve(self, space: str | Sequence[str]) -> Space | SpaceList | None:
-        """`Retrieve space by id. <https://docs.cognite.com/api/v1/#operation/bySpaceIdsSpaces>`_
+        """`Retrieve space by id. <https://developer.cognite.com/api#tag/Spaces/operation/bySpaceIdsSpaces>`_
 
         Args:
             space (str): Space ID
 
         Returns:
             Optional[Space]: Requested space or None if it does not exist.
 
@@ -91,15 +91,15 @@
                 >>> res = c.data_modeling.spaces.retrieve(spaces=["MySpace", "MyAwesomeSpace", "MyOtherSpace"])
 
         """
         identifier = DataModelingIdentifierSequence.load_spaces(spaces=space)
         return self._retrieve_multiple(list_cls=SpaceList, resource_cls=Space, identifiers=identifier)
 
     def delete(self, space: str | Sequence[str]) -> list[str]:
-        """`Delete one or more spaces <https://docs.cognite.com/api/v1/#operation/deleteSpacesV3>`_
+        """`Delete one or more spaces <https://developer.cognite.com/api#tag/Spaces/operation/deleteSpacesV3>`_
 
         Args:
             space (str | Sequence[str]): ID or ID list ids of spaces.
         Returns:
             list[str]: The space(s) which has been deleted.
         Examples:
 
@@ -117,15 +117,15 @@
         )
         return [item["space"] for item in deleted_spaces]
 
     def list(
         self,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> SpaceList:
-        """`List spaces <https://docs.cognite.com/api/v1/#operation/listSpacesV3>`_
+        """`List spaces <https://developer.cognite.com/api#tag/Spaces/operation/listSpacesV3>`_
 
         Args:
             limit (int, optional): Maximum number of spaces to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
         Returns:
             SpaceList: List of requested spaces
@@ -164,15 +164,15 @@
         ...
 
     @overload
     def apply(self, space: SpaceApply) -> Space:
         ...
 
     def apply(self, space: SpaceApply | Sequence[SpaceApply]) -> Space | SpaceList:
-        """`Create or patch one or more spaces. <https://docs.cognite.com/api/v1/#operation/ApplySpaces>`_
+        """`Create or patch one or more spaces. <https://developer.cognite.com/api#tag/Spaces/operation/ApplySpaces>`_
 
         Args:
             space (space: Space | Sequence[Space]): Space or spaces of spacesda to create or update.
 
         Returns:
             Space | SpaceList: Created space(s)
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.5.0/cognite/client/_api/data_modeling/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
         Yields:
             View: yields Views one by one.
         """
         return cast(Iterator[View], self())
 
     def retrieve(self, ids: ViewIdentifier | Sequence[ViewIdentifier]) -> ViewList:
-        """`Retrieve a single view by id. <https://docs.cognite.com/api/v1/#operation/byExternalIdsViews>`_
+        """`Retrieve a single view by id. <https://developer.cognite.com/api#tag/Views/operation/byExternalIdsViews>`_
 
         Args:
             ids (ViewId | Sequence[ViewId]): View dentifier(s)
 
         Returns:
             Optional[View]: Requested view or None if it does not exist.
 
@@ -100,15 +100,15 @@
                 >>> res = c.data_modeling.views.retrieve(('mySpace', 'myView', 'v1'))
 
         """
         identifier = _load_identifier(ids, "view")
         return self._retrieve_multiple(list_cls=ViewList, resource_cls=View, identifiers=identifier)
 
     def delete(self, ids: ViewIdentifier | Sequence[ViewIdentifier]) -> list[ViewId]:
-        """`Delete one or more views <https://docs.cognite.com/api/v1/#operation/deleteViews>`_
+        """`Delete one or more views <https://developer.cognite.com/api#tag/Views/operation/deleteViews>`_
 
         Args:
             ids (ViewId | Sequence[ViewId]): View dentifier(s)
         Returns:
             The identifier for the view(s) which has been deleted. Empty list if nothing was deleted.
         Examples:
 
@@ -132,15 +132,15 @@
         self,
         limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT,
         space: str | None = None,
         include_inherited_properties: bool = True,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> ViewList:
-        """`List views <https://docs.cognite.com/api/v1/#operation/listViews>`_
+        """`List views <https://developer.cognite.com/api#tag/Views/operation/listViews>`_
 
         Args:
             limit (int, optional): Maximum number of views to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
             space: (str | None): The space to query.
             include_inherited_properties (bool): Whether to include properties inherited from views this view implements.
             all_versions (bool): Whether to return all versions. If false, only the newest version is returned,
@@ -183,27 +183,27 @@
         ...
 
     @overload
     def apply(self, view: ViewApply) -> View:
         ...
 
     def apply(self, view: ViewApply | Sequence[ViewApply]) -> View | ViewList:
-        """`Create or update (upsert) one or more views. <https://docs.cognite.com/api/v1/#operation/ApplyViews>`_
+        """`Create or update (upsert) one or more views. <https://developer.cognite.com/api#tag/Views/operation/ApplyViews>`_
 
         Args:
             view (view: ViewApply | Sequence[ViewApply]): View or views of views to create or update.
 
         Returns:
             View | ViewList: Created view(s)
 
         Examples:
 
             Create new views::
 
                 >>> from cognite.client import CogniteClient
-                >>> import cognite.client.data_classes.data_modeling as models
+                >>> from cognite.client.data_classes.data_modeling import ViewApply
                 >>> c = CogniteClient()
-                >>> views = [models.ViewApply(space="mySpace",external_id="myView",version="v1"),
-                ... models.ViewApply(space="mySpace",external_id="myOtherView",version="v1")]
+                >>> views = [ViewApply(space="mySpace",external_id="myView",version="v1"),
+                ... ViewApply(space="mySpace",external_id="myOtherView",version="v1")]
                 >>> res = c.data_modeling.views.apply(views)
         """
         return self._create_multiple(list_cls=ViewList, resource_cls=View, items=view, input_resource_cls=ViewApply)
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/data_sets.py` & `cognite_sdk-6.5.0/cognite/client/_api/data_sets.py`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
         Yields:
             Event: yields DataSet one by one.
         """
         return cast(Iterator[DataSet], self())
 
     def create(self, data_set: Union[DataSet, Sequence[DataSet]]) -> Union[DataSet, DataSetList]:
-        """`Create one or more data sets. <https://docs.cognite.com/api/v1/#operation/createDataSets>`_
+        """`Create one or more data sets. <https://developer.cognite.com/api#tag/Data-sets/operation/createDataSets>`_
 
         Args:
             data_set: Union[DataSet, Sequence[DataSet]]: Data set or list of data sets to create.
 
         Returns:
             Union[DataSet, DataSetList]: Created data set(s)
 
@@ -91,15 +91,15 @@
                 >>> c = CogniteClient()
                 >>> data_sets = [DataSet(name="1st level"), DataSet(name="2nd level")]
                 >>> res = c.data_sets.create(data_sets)
         """
         return self._create_multiple(list_cls=DataSetList, resource_cls=DataSet, items=data_set)
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[DataSet]:
-        """`Retrieve a single data set by id. <https://docs.cognite.com/api/v1/#operation/getDataSets>`_
+        """`Retrieve a single data set by id. <https://developer.cognite.com/api#tag/Data-sets/operation/getDataSets>`_
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
 
         Returns:
             Optional[DataSet]: Requested data set or None if it does not exist.
@@ -123,15 +123,15 @@
 
     def retrieve_multiple(
         self,
         ids: Optional[Sequence[int]] = None,
         external_ids: Optional[Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> DataSetList:
-        """`Retrieve multiple data sets by id. <https://docs.cognite.com/api/v1/#operation/getDataSets>`_
+        """`Retrieve multiple data sets by id. <https://developer.cognite.com/api#tag/Data-sets/operation/getDataSets>`_
 
         Args:
             ids (Sequence[int], optional): IDs
             external_ids (Sequence[str], optional): External IDs
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -161,15 +161,15 @@
         metadata: Dict[str, str] = None,
         created_time: Union[Dict[str, Any], TimestampRange] = None,
         last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
         external_id_prefix: str = None,
         write_protected: bool = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> DataSetList:
-        """`List data sets <https://docs.cognite.com/api/v1/#operation/listDataSets>`_
+        """`List data sets <https://developer.cognite.com/api#tag/Data-sets/operation/listDataSets>`_
 
         Args:
             metadata (Dict[str, str]): Custom, application-specific metadata. String key -> String value.
             created_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
             last_updated_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
             external_id_prefix (str): Filter by this (case-sensitive) prefix for the external ID.
             write_protected (bool): Specify whether the filtered data sets are write-protected, or not. Set to True to only list write-protected data sets.
@@ -208,15 +208,15 @@
             last_updated_time=last_updated_time,
             external_id_prefix=external_id_prefix,
             write_protected=write_protected,
         ).dump(camel_case=True)
         return self._list(list_cls=DataSetList, resource_cls=DataSet, method="POST", limit=limit, filter=filter)
 
     def aggregate(self, filter: Union[DataSetFilter, Dict] = None) -> List[DataSetAggregate]:
-        """`Aggregate data sets <https://docs.cognite.com/api/v1/#operation/aggregateDataSets>`_
+        """`Aggregate data sets <https://developer.cognite.com/api#tag/Data-sets/operation/aggregateDataSets>`_
 
         Args:
             filter (Union[DataSetFilter, Dict]): Filter on data set filter with exact match
 
         Returns:
             List[DataSetAggregate]: List of data set aggregates
 
@@ -230,15 +230,15 @@
         """
 
         return self._aggregate(filter=filter, cls=DataSetAggregate)
 
     def update(
         self, item: Union[DataSet, DataSetUpdate, Sequence[Union[DataSet, DataSetUpdate]]]
     ) -> Union[DataSet, DataSetList]:
-        """`Update one or more data sets <https://docs.cognite.com/api/v1/#operation/updateDataSets>`_
+        """`Update one or more data sets <https://developer.cognite.com/api#tag/Data-sets/operation/updateDataSets>`_
 
         Args:
             item: Union[DataSet, DataSetUpdate, Sequence[Union[DataSet, DataSetUpdate]]]: Data set(s) to update
 
         Returns:
             Union[DataSet, DataSetList]: Updated data set(s)
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.5.0/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/datapoints.py` & `cognite_sdk-6.5.0/cognite/client/_api/datapoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,15 +607,15 @@
         end: int | str | datetime | None = None,
         aggregates: Aggregate | str | list[Aggregate | str] | None = None,
         granularity: Optional[str] = None,
         limit: Optional[int] = None,
         include_outside_points: bool = False,
         ignore_unknown_ids: bool = False,
     ) -> None | Datapoints | DatapointsList:
-        """`Retrieve datapoints for one or more time series. <https://docs.cognite.com/api/v1/#operation/getMultiTimeSeriesDatapoints>`_
+        """`Retrieve datapoints for one or more time series. <https://developer.cognite.com/api#tag/Time-series/operation/getMultiTimeSeriesDatapoints>`_
 
         **Performance guide**:
             In order to retrieve millions of datapoints as efficiently as possible, here are a few guidelines:
 
             1. For best speed, and significantly lower memory usage, consider using `retrieve_arrays(...)` which uses `numpy.ndarrays` for data storage.
             2. Unlimited queries are fastest as they are trivial to parallelize. Thus, specifying a very large finite `limit`, e.g. 1 million, comes with a performance penalty.
             3. Try to avoid specifying `start` and `end` to be very far from the actual data: If you have data from 2000 to 2015, don't set start=0 (1970).
@@ -793,15 +793,15 @@
         end: int | str | datetime | None = None,
         aggregates: Aggregate | str | list[Aggregate | str] | None = None,
         granularity: Optional[str] = None,
         limit: Optional[int] = None,
         include_outside_points: bool = False,
         ignore_unknown_ids: bool = False,
     ) -> None | DatapointsArray | DatapointsArrayList:
-        """`Retrieve datapoints for one or more time series. <https://docs.cognite.com/api/v1/#operation/getMultiTimeSeriesDatapoints>`_
+        """`Retrieve datapoints for one or more time series. <https://developer.cognite.com/api#tag/Time-series/operation/getMultiTimeSeriesDatapoints>`_
 
         **Note**: This method requires `numpy` to be installed.
 
         Args:
             start (Union[int, str, datetime, None]): Inclusive start. Default: 1970-01-01 UTC.
             end (Union[int, str, datetime, None]): Exclusive end. Default: "now"
             id (Union[None, int, Dict[str, Any], List[Union[int, Dict[str, Any]]]]): Id, dict (with id) or (mixed) sequence of these. See examples below.
@@ -1174,15 +1174,15 @@
     def retrieve_latest(
         self,
         id: int | LatestDatapointQuery | list[int | LatestDatapointQuery] | None = None,
         external_id: str | LatestDatapointQuery | list[str | LatestDatapointQuery] | None = None,
         before: None | int | str | datetime = None,
         ignore_unknown_ids: bool = False,
     ) -> Datapoints | DatapointsList | None:
-        """`Get the latest datapoint for one or more time series <https://docs.cognite.com/api/v1/#operation/getLatest>`_
+        """`Get the latest datapoint for one or more time series <https://developer.cognite.com/api#tag/Time-series/operation/getLatest>`_
 
         Args:
             id (Union[int, LatestDatapointQuery, List[Union[int, LatestDatapointQuery]]]): Id or list of ids.
             external_id (Union[str, LatestDatapointQuery, List[Union[str, LatestDatapointQuery]]]): External id or list of external ids.
             before: (Union[int, str, datetime]): Get latest datapoint before this time. Not used when passing 'LatestDatapointQuery'.
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
@@ -1301,15 +1301,15 @@
             dps_to_post = datapoints
 
         post_dps_object["datapoints"] = dps_to_post
         dps_poster = DatapointsPoster(self)
         dps_poster.insert([post_dps_object])
 
     def insert_multiple(self, datapoints: list[dict[str, str | int | list | Datapoints | DatapointsArray]]) -> None:
-        """`Insert datapoints into multiple time series <https://docs.cognite.com/api/v1/#operation/postMultiTimeSeriesDatapoints>`_
+        """`Insert datapoints into multiple time series <https://developer.cognite.com/api#tag/Time-series/operation/postMultiTimeSeriesDatapoints>`_
 
         Args:
             datapoints (List[Dict]): The datapoints you wish to insert along with the ids of the time series. See examples below.
 
         Returns:
             None
 
@@ -1373,15 +1373,15 @@
         assert end > start, "end must be larger than start"
 
         identifier = Identifier.of_either(id, external_id).as_dict()
         delete_dps_object = {**identifier, "inclusiveBegin": start, "exclusiveEnd": end}
         self._delete_datapoints_ranges([delete_dps_object])
 
     def delete_ranges(self, ranges: list[dict[str, Any]]) -> None:
-        """`Delete a range of datapoints from multiple time series. <https://docs.cognite.com/api/v1/#operation/deleteDatapoints>`_
+        """`Delete a range of datapoints from multiple time series. <https://developer.cognite.com/api#tag/Time-series/operation/deleteDatapoints>`_
 
         Args:
             ranges (List[Dict[str, Any]]): The list of datapoint ids along with time range to delete. See examples below.
 
         Returns:
             None
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/diagrams.py` & `cognite_sdk-6.5.0/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.5.0/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/events.py` & `cognite_sdk-6.5.0/cognite/client/_api/events.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 
         Yields:
             Event: yields Events one by one.
         """
         return cast(Iterator[Event], self())
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[Event]:
-        """`Retrieve a single event by id. <https://docs.cognite.com/api/v1/#operation/getEventByInternalId>`_
+        """`Retrieve a single event by id. <https://developer.cognite.com/api#tag/Events/operation/getEventByInternalId>`_
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
 
         Returns:
             Optional[Event]: Requested event or None if it does not exist.
@@ -145,15 +145,15 @@
 
     def retrieve_multiple(
         self,
         ids: Optional[Sequence[int]] = None,
         external_ids: Optional[Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> EventList:
-        """`Retrieve multiple events by id. <https://docs.cognite.com/api/v1/#operation/byIdsEvents>`_
+        """`Retrieve multiple events by id. <https://developer.cognite.com/api#tag/Events/operation/byIdsEvents>`_
 
         Args:
             ids (Sequence[int], optional): IDs
             external_ids (Sequence[str], optional): External IDs
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -196,15 +196,15 @@
         created_time: Union[Dict[str, Any], TimestampRange] = None,
         last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
         external_id_prefix: str = None,
         sort: Sequence[str] = None,
         partitions: int = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> EventList:
-        """`List events <https://docs.cognite.com/api/v1/#operation/advancedListEvents>`_
+        """`List events <https://developer.cognite.com/api#tag/Events/operation/advancedListEvents>`_
 
         Args:
             start_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
             end_time (Union[Dict[str, Any], TimestampRange]): Range between two timestamps.
             active_at_time (Union[Dict[str, Any], TimestampRange]): Event is considered active from its startTime to endTime inclusive. If startTime is null, event is never active. If endTime is null, event is active from startTime onwards. activeAtTime filter will match all events that are active at some point from min to max, from min, or to max, depending on which of min and max parameters are specified.
             type (str): Type of the event, e.g 'failure'.
             subtype (str): Subtype of the event, e.g 'electrical'.
@@ -281,15 +281,15 @@
             limit=limit,
             filter=filter,
             partitions=partitions,
             sort=sort,
         )
 
     def aggregate(self, filter: Union[EventFilter, Dict] = None) -> List[AggregateResult]:
-        """`Aggregate events <https://docs.cognite.com/api/v1/#operation/aggregateEvents>`_
+        """`Aggregate events <https://developer.cognite.com/api#tag/Events/operation/aggregateEvents>`_
 
         Args:
             filter (Union[EventFilter, Dict]): Filter on events filter with exact match
 
         Returns:
             List[AggregateResult]: List of event aggregates
 
@@ -303,15 +303,15 @@
         """
 
         return self._aggregate(filter=filter, cls=AggregateResult)
 
     def aggregate_unique_values(
         self, filter: Union[EventFilter, Dict] = None, fields: Sequence[str] = None
     ) -> List[AggregateUniqueValuesResult]:
-        """`Aggregate unique values for events <https://docs.cognite.com/api/v1/#operation/aggregateEvents>`_
+        """`Aggregate unique values for events <https://developer.cognite.com/api#tag/Events/operation/aggregateEvents>`_
 
         Args:
             filter (Union[EventFilter, Dict]): Filter on events filter with exact match
             fields (Sequence[str]): The field name(s) to apply the aggregation on. Currently limited to one field.
 
         Returns:
             List[AggregateUniqueValuesResult]: List of event aggregates
@@ -332,15 +332,15 @@
         ...
 
     @overload
     def create(self, event: Event) -> Event:
         ...
 
     def create(self, event: Union[Event, Sequence[Event]]) -> Union[Event, EventList]:
-        """`Create one or more events. <https://docs.cognite.com/api/v1/#operation/createEvents>`_
+        """`Create one or more events. <https://developer.cognite.com/api#tag/Events/operation/createEvents>`_
 
         Args:
             event (Union[Event, Sequence[Event]]): Event or list of events to create.
 
         Returns:
             Union[Event, EventList]: Created event(s)
 
@@ -358,15 +358,15 @@
 
     def delete(
         self,
         id: Union[int, Sequence[int]] = None,
         external_id: Union[str, Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> None:
-        """`Delete one or more events <https://docs.cognite.com/api/v1/#operation/deleteEvents>`_
+        """`Delete one or more events <https://developer.cognite.com/api#tag/Events/operation/deleteEvents>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -390,15 +390,15 @@
         ...
 
     @overload
     def update(self, item: Union[Event, EventUpdate]) -> Event:
         ...
 
     def update(self, item: Union[Event, EventUpdate, Sequence[Union[Event, EventUpdate]]]) -> Union[Event, EventList]:
-        """`Update one or more events <https://docs.cognite.com/api/v1/#operation/updateEvents>`_
+        """`Update one or more events <https://developer.cognite.com/api#tag/Events/operation/updateEvents>`_
 
         Args:
             item (Union[Event, EventUpdate, Sequence[Union[Event, EventUpdate]]]): Event(s) to update
 
         Returns:
             Union[Event, EventList]: Updated event(s)
 
@@ -419,15 +419,15 @@
                 >>> c = CogniteClient()
                 >>> my_update = EventUpdate(id=1).description.set("New description").metadata.add({"key": "value"})
                 >>> res = c.events.update(my_update)
         """
         return self._update_multiple(list_cls=EventList, resource_cls=Event, update_cls=EventUpdate, items=item)
 
     def search(self, description: str = None, filter: Union[EventFilter, Dict] = None, limit: int = 100) -> EventList:
-        """`Search for events <https://docs.cognite.com/api/v1/#operation/searchEvents>`_
+        """`Search for events <https://developer.cognite.com/api#tag/Events/operation/searchEvents>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             description (str): Fuzzy match on description.
             filter (Union[EventFilter, Dict]): Filter to apply. Performs exact match on these fields.
             limit (int): Maximum number of results to return.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.5.0/cognite/client/_api/extractionpipelines.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self.runs = ExtractionPipelineRunsAPI(config, api_version, cognite_client)
         self.config = ExtractionPipelineConfigsAPI(config, api_version, cognite_client)
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[ExtractionPipeline]:
-        """`Retrieve a single extraction pipeline by id. <https://docs.cognite.com/api/v1/#operation/showExtPipe>`_
+        """`Retrieve a single extraction pipeline by id. <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/showExtPipe>`_
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
 
         Returns:
             Optional[ExtractionPipeline]: Requested extraction pipeline or None if it does not exist.
@@ -64,15 +64,15 @@
 
     def retrieve_multiple(
         self,
         ids: Optional[Sequence[int]] = None,
         external_ids: Optional[Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> ExtractionPipelineList:
-        """`Retrieve multiple extraction pipelines by ids and external ids. <https://docs.cognite.com/api/v1/#operation/byidsExtPipes>`_
+        """`Retrieve multiple extraction pipelines by ids and external ids. <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/byidsExtPipes>`_
 
         Args:
             ids (Sequence[int], optional): IDs
             external_ids (Sequence[str], optional): External IDs
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -97,15 +97,15 @@
             list_cls=ExtractionPipelineList,
             resource_cls=ExtractionPipeline,
             identifiers=identifiers,
             ignore_unknown_ids=ignore_unknown_ids,
         )
 
     def list(self, limit: int = LIST_LIMIT_DEFAULT) -> ExtractionPipelineList:
-        """`List extraction pipelines <https://docs.cognite.com/api/v1/#operation/listExtPipes>`_
+        """`List extraction pipelines <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/listExtPipes>`_
 
         Args:
             limit (int, optional): Maximum number of ExtractionPipelines to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
         Returns:
             ExtractionPipelineList: List of requested ExtractionPipelines
@@ -128,15 +128,15 @@
     @overload
     def create(self, extraction_pipeline: Sequence[ExtractionPipeline]) -> ExtractionPipelineList:
         ...
 
     def create(
         self, extraction_pipeline: Union[ExtractionPipeline, Sequence[ExtractionPipeline]]
     ) -> Union[ExtractionPipeline, ExtractionPipelineList]:
-        """`Create one or more extraction pipelines. <https://docs.cognite.com/api/v1/#operation/createExtPipes>`_
+        """`Create one or more extraction pipelines. <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/createExtPipes>`_
 
         You can create an arbitrary number of extraction pipelines, and the SDK will split the request into multiple requests if necessary.
 
         Args:
             extraction_pipeline (Union[ExtractionPipeline, List[ExtractionPipeline]]): Extraction pipeline or list of extraction pipelines to create.
 
         Returns:
@@ -154,15 +154,15 @@
         """
         utils._auxiliary.assert_type(extraction_pipeline, "extraction_pipeline", [ExtractionPipeline, Sequence])
         return self._create_multiple(
             list_cls=ExtractionPipelineList, resource_cls=ExtractionPipeline, items=extraction_pipeline
         )
 
     def delete(self, id: Union[int, Sequence[int]] = None, external_id: Union[str, Sequence[str]] = None) -> None:
-        """`Delete one or more extraction pipelines <https://docs.cognite.com/api/v1/#operation/deleteExtPipes>`_
+        """`Delete one or more extraction pipelines <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/deleteExtPipes>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
 
         Returns:
             None
@@ -187,15 +187,15 @@
 
     def update(
         self,
         item: Union[
             ExtractionPipeline, ExtractionPipelineUpdate, Sequence[Union[ExtractionPipeline, ExtractionPipelineUpdate]]
         ],
     ) -> Union[ExtractionPipeline, ExtractionPipelineList]:
-        """`Update one or more extraction pipelines <https://docs.cognite.com/api/v1/#operation/updateExtPipes>`_
+        """`Update one or more extraction pipelines <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/updateExtPipes>`_
 
         Args:
             item (Union[ExtractionPipeline, ExtractionPipelineUpdate, Sequence[Union[ExtractionPipeline, ExtractionPipelineUpdate]]]): Extraction pipeline(s) to update
 
         Returns:
             Union[ExtractionPipeline, ExtractionPipelineList]: Updated extraction pipeline(s)
 
@@ -224,15 +224,15 @@
         self,
         external_id: str,
         statuses: Sequence[str] = None,
         message_substring: str = None,
         created_time: Union[Dict[str, Any], TimestampRange] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> ExtractionPipelineRunList:
-        """`List runs for an extraction pipeline with given external_id <https://docs.cognite.com/api/v1/#operation/filterRuns>`_
+        """`List runs for an extraction pipeline with given external_id <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/filterRuns>`_
 
         Args:
             external_id (str): Extraction pipeline external Id.
             statuses (Sequence[str]): One or more among "success" / "failure" / "seen".
             message_substring (str): Failure message part.
             created_time (int): The number of milliseconds since 00:00:00 Thursday, 1 January 1970, Coordinated Universal Time (UTC), minus leap seconds.
             limit (int, optional): Maximum number of ExtractionPipelines to return. Defaults to 25. Set to -1, float("inf") or None
@@ -286,15 +286,15 @@
     @overload
     def create(self, run: Sequence[ExtractionPipelineRun]) -> ExtractionPipelineRunList:
         ...
 
     def create(
         self, run: Union[ExtractionPipelineRun, Sequence[ExtractionPipelineRun]]
     ) -> Union[ExtractionPipelineRun, ExtractionPipelineRunList]:
-        """`Create one or more extraction pipeline runs. <https://docs.cognite.com/api/v1/#operation/createRuns>`_
+        """`Create one or more extraction pipeline runs. <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/createRuns>`_
 
         You can create an arbitrary number of extraction pipeline runs, and the SDK will split the request into multiple requests.
 
         Args:
             run (Union[ExtractionPipelineRun, Sequence[ExtractionPipelineRun]]): Extraction pipeline or list of extraction pipeline runs to create.
 
         Returns:
@@ -316,15 +316,15 @@
 
 class ExtractionPipelineConfigsAPI(APIClient):
     _RESOURCE_PATH = "/extpipes/config"
 
     def retrieve(
         self, external_id: str, revision: Optional[int] = None, active_at_time: Optional[int] = None
     ) -> ExtractionPipelineConfig:
-        """`Retrieve a specific configuration revision, or the latest by default <https://docs.cognite.com/api/v1/#operation/getExtPipeConfigRevision>`
+        """`Retrieve a specific configuration revision, or the latest by default <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/getExtPipeConfigRevision>`
 
         By default the latest configuration revision is retrieved, or you can specify a timestamp or a revision number.
 
         Args:
             external_id (str): External id of the extraction pipeline to retrieve config from.
             revision (Optional[int]): Optionally specify a revision number to retrieve.
             active_at_time (Optional[int]): Optionally specify a timestamp the configuration revision should be active.
@@ -342,15 +342,15 @@
         """
         response = self._get(
             "/extpipes/config", params={"externalId": external_id, "activeAtTime": active_at_time, "revision": revision}
         )
         return ExtractionPipelineConfig._load(response.json(), cognite_client=self._cognite_client)
 
     def list(self, external_id: str) -> ExtractionPipelineConfigRevisionList:
-        """`Retrieve all configuration revisions from an extraction pipeline <https://docs.cognite.com/api/v1/#operation/listExtPipeConfigRevisions>`
+        """`Retrieve all configuration revisions from an extraction pipeline <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/listExtPipeConfigRevisions>`
 
         Args:
             external_id (str): External id of the extraction pipeline to retrieve config from.
 
         Returns:
             ExtractionPipelineConfigRevisionList: Retrieved extraction pipeline configuration revisions
 
@@ -362,15 +362,15 @@
                 >>> c = CogniteClient()
                 >>> res = c.extraction_pipelines.config.list("extId")
         """
         response = self._get("/extpipes/config/revisions", params={"externalId": external_id})
         return ExtractionPipelineConfigRevisionList._load(response.json()["items"], cognite_client=self._cognite_client)
 
     def create(self, config: ExtractionPipelineConfig) -> ExtractionPipelineConfig:
-        """`Create a new configuration revision <https://docs.cognite.com/api/v1/#operation/createExtPipeConfig>`
+        """`Create a new configuration revision <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/createExtPipeConfig>`
 
         Args:
             config (ExtractionPipelineConfig): Configuration revision to create.
 
         Returns:
             ExtractionPipelineConfig: Created extraction pipeline configuration revision
 
@@ -383,15 +383,15 @@
                 >>> c = CogniteClient()
                 >>> res = c.extraction_pipelines.config.create(ExtractionPipelineConfig(external_id="extId", config="my config contents"))
         """
         response = self._post("/extpipes/config", json=config.dump(camel_case=True))
         return ExtractionPipelineConfig._load(response.json(), cognite_client=self._cognite_client)
 
     def revert(self, external_id: str, revision: int) -> ExtractionPipelineConfig:
-        """`Revert to a previous configuration revision <https://docs.cognite.com/api/v1/#operation/createExtPipeConfig>`
+        """`Revert to a previous configuration revision <https://developer.cognite.com/api#tag/Extraction-Pipelines/operation/createExtPipeConfig>`
 
         Args:
             external_id (str): External id of the extraction pipeline to revert revision for.
             revision (int): Revision to revert to.
 
         Returns:
             ExtractionPipelineConfig: New latest extraction pipeline configuration revision.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/files.py` & `cognite_sdk-6.5.0/cognite/client/_api/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         )
         returned_file_metadata = res.json()
         upload_url = returned_file_metadata["uploadUrl"]
         file_metadata = FileMetadata._load(returned_file_metadata)
         return (file_metadata, upload_url)
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[FileMetadata]:
-        """`Retrieve a single file metadata by id. <https://docs.cognite.com/api/v1/#operation/getFileByInternalId>`_
+        """`Retrieve a single file metadata by id. <https://developer.cognite.com/api#tag/Files/operation/getFileByInternalId>`_
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
 
         Returns:
             Optional[FileMetadata]: Requested file metadata or None if it does not exist.
@@ -206,15 +206,15 @@
 
     def retrieve_multiple(
         self,
         ids: Optional[Sequence[int]] = None,
         external_ids: Optional[Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> FileMetadataList:
-        """`Retrieve multiple file metadatas by id. <https://docs.cognite.com/api/v1/#operation/byIdsFiles>`_
+        """`Retrieve multiple file metadatas by id. <https://developer.cognite.com/api#tag/Files/operation/byIdsFiles>`_
 
         Args:
             ids (Sequence[int], optional): IDs
             external_ids (Sequence[str], optional): External IDs
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -262,15 +262,15 @@
         source_modified_time: Union[Dict[str, Any], TimestampRange] = None,
         uploaded_time: Union[Dict[str, Any], TimestampRange] = None,
         external_id_prefix: str = None,
         directory_prefix: str = None,
         uploaded: bool = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> FileMetadataList:
-        """`List files <https://docs.cognite.com/api/v1/#operation/advancedListFiles>`_
+        """`List files <https://developer.cognite.com/api#tag/Files/operation/advancedListFiles>`_
 
         Args:
             name (str): Name of the file.
             mime_type (str): File type. E.g. text/plain, application/pdf, ..
             metadata (Dict[str, str]): Custom, application specific metadata. String key -> String value
             asset_ids (Sequence[int]): Only include files that reference these specific asset IDs.
             asset_subtree_external_ids (Sequence[str]): Only include files that reference these specific asset external IDs.
@@ -358,15 +358,15 @@
         ).dump(camel_case=True)
 
         return self._list(
             list_cls=FileMetadataList, resource_cls=FileMetadata, method="POST", limit=limit, filter=filter
         )
 
     def aggregate(self, filter: Union[FileMetadataFilter, Dict] = None) -> List[FileAggregate]:
-        """`Aggregate files <https://docs.cognite.com/api/v1/#operation/aggregateFiles>`_
+        """`Aggregate files <https://developer.cognite.com/api#tag/Files/operation/aggregateFiles>`_
 
         Args:
             filter (Union[FileMetadataFilter, Dict]): Filter on file metadata filter with exact match
 
         Returns:
             List[FileAggregate]: List of file aggregates
 
@@ -378,15 +378,15 @@
                 >>> c = CogniteClient()
                 >>> aggregate_uploaded = c.files.aggregate(filter={"uploaded": True})
         """
 
         return self._aggregate(filter=filter, cls=FileAggregate)
 
     def delete(self, id: Union[int, Sequence[int]] = None, external_id: Union[str, Sequence[str]] = None) -> None:
-        """`Delete files <https://docs.cognite.com/api/v1/#operation/deleteFiles>`_
+        """`Delete files <https://developer.cognite.com/api#tag/Files/operation/deleteFiles>`_
 
         Args:
             id (Union[int, Sequence[int]]): Id or list of ids
             external_id (Union[str, Sequence[str]]): str or list of str
 
         Returns:
             None
@@ -408,15 +408,15 @@
     @overload
     def update(self, item: Sequence[Union[FileMetadata, FileMetadataUpdate]]) -> FileMetadataList:
         ...
 
     def update(
         self, item: Union[FileMetadata, FileMetadataUpdate, Sequence[Union[FileMetadata, FileMetadataUpdate]]]
     ) -> Union[FileMetadata, FileMetadataList]:
-        """`Update files <https://docs.cognite.com/api/v1/#operation/updateFiles>`_
+        """`Update files <https://developer.cognite.com/api#tag/Files/operation/updateFiles>`_
         Currently, a full replacement of labels on a file is not supported (only partial add/remove updates). See the example below on how to perform partial labels update.
 
         Args:
             item (Union[FileMetadata, FileMetadataUpdate, Sequence[Union[FileMetadata, FileMetadataUpdate]]]): file(s) to update.
 
         Returns:
             Union[FileMetadata, FileMetadataList]: The updated files.
@@ -462,15 +462,15 @@
             resource_path=self._RESOURCE_PATH,
             items=item,
         )
 
     def search(
         self, name: str = None, filter: Optional[Union[FileMetadataFilter, dict]] = None, limit: int = 100
     ) -> FileMetadataList:
-        """`Search for files. <https://docs.cognite.com/api/v1/#operation/searchFiles>`_
+        """`Search for files. <https://developer.cognite.com/api#tag/Files/operation/searchFiles>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             name (str, optional): Prefix and fuzzy search on name.
             filter (Union[FileMetadataFilter, dict], optional): Filter to apply. Performs exact match on these fields.
             limit (int, optional): Max number of results to return.
 
@@ -509,15 +509,15 @@
         data_set_id: int = None,
         labels: Sequence[Label] = None,
         geo_location: GeoLocation = None,
         security_categories: Sequence[int] = None,
         recursive: bool = False,
         overwrite: bool = False,
     ) -> Union[FileMetadata, FileMetadataList]:
-        """`Upload a file <https://docs.cognite.com/api/v1/#operation/initFileUpload>`_
+        """`Upload a file <https://developer.cognite.com/api#tag/Files/operation/initFileUpload>`_
 
         Args:
             path (str): Path to the file you wish to upload. If path is a directory, this method will upload all files in that directory.
             external_id (str): The external ID provided by the client. Must be unique within the project.
             name (str): Name of the file.
             source (str): The source of the file.
             mime_type (str): File type. E.g. text/plain, application/pdf, ...
@@ -739,15 +739,15 @@
 
     def download(
         self,
         directory: Union[str, Path],
         id: Union[int, Sequence[int]] = None,
         external_id: Union[str, Sequence[str]] = None,
     ) -> None:
-        """`Download files by id or external id. <https://docs.cognite.com/api/v1/#operation/downloadLinks>`_
+        """`Download files by id or external id. <https://developer.cognite.com/api#tag/Files/operation/downloadLinks>`_
 
         This method will stream all files to disk, never keeping more than 2MB in memory per worker.
         The files will be stored in the provided directory using the name retrieved from the file metadata in CDF.
 
 
         Args:
             directory (str): Directory to download the file(s) to.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/functions.py` & `cognite_sdk-6.5.0/cognite/client/_api/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         cpu: Optional[Number] = None,
         memory: Optional[Number] = None,
         runtime: Optional[str] = None,
         metadata: Optional[Dict] = None,
         index_url: Optional[str] = None,
         extra_index_urls: Optional[List[str]] = None,
     ) -> Function:
-        """`When creating a function, <https://docs.cognite.com/api/v1/#operation/postFunctions>`_
+        """`When creating a function, <https://developer.cognite.com/api#tag/Functions/operation/postFunctions>`_
         the source code can be specified in one of three ways:\n
         - Via the `folder` argument, which is the path to the folder where the source code is located. `function_path` must point to a python file in the folder within which a function named `handle` must be defined.\n
         - Via the `file_id` argument, which is the ID of a zip-file uploaded to the files API. `function_path` must point to a python file in the zipped folder within which a function named `handle` must be defined.\n
         - Via the `function_handle` argument, which is a reference to a function object, which must be named `handle`.\n
 
         The function named `handle` is the entrypoint of the created function. Valid arguments to `handle` are `data`, `client`, `secrets` and `function_call_info`:\n
         - If the user calls the function with input data, this is passed through the `data` argument.\n
@@ -214,15 +214,15 @@
             function["indexUrl"] = index_url
 
         body = {"items": [function]}
         res = self._post(url, json=body)
         return Function._load(res.json()["items"][0], cognite_client=self._cognite_client)
 
     def delete(self, id: Union[int, Sequence[int]] = None, external_id: Union[str, Sequence[str]] = None) -> None:
-        """`Delete one or more functions. <https://docs.cognite.com/api/v1/#operation/deleteFunctions>`_
+        """`Delete one or more functions. <https://developer.cognite.com/api#tag/Functions/operation/deleteFunctions>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids.
             external_id (Union[str, Sequence[str]]): External ID or list of external ids.
 
         Returns:
             None
@@ -243,15 +243,15 @@
         owner: str = None,
         file_id: int = None,
         status: str = None,
         external_id_prefix: str = None,
         created_time: Union[Dict[str, int], TimestampRange] = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> FunctionList:
-        """`List all functions. <https://docs.cognite.com/api/v1/#operation/listFunctions>`_
+        """`List all functions. <https://developer.cognite.com/api#tag/Functions/operation/listFunctions>`_
 
         Args:
             name (str): The name of the function.
             owner (str): Owner of the function.
             file_id (int): The file ID of the zip-file used to create the function.
             status (str): Status of the function. Possible values: ["Queued", "Deploying", "Ready", "Failed"].
             external_id_prefix (str): External ID prefix to filter on.
@@ -283,15 +283,15 @@
         res = self._post(url_path=f"{self._RESOURCE_PATH}/list", json={"filter": filter, "limit": limit})
 
         return FunctionList._load(res.json()["items"], cognite_client=self._cognite_client)
 
     def retrieve(
         self, id: Optional[int] = None, external_id: Optional[str] = None
     ) -> Union[FunctionList, Function, None]:
-        """`Retrieve a single function by id. <https://docs.cognite.com/api/v1/#operation/byIdsFunctions>`_
+        """`Retrieve a single function by id. <https://developer.cognite.com/api#tag/Functions/operation/byIdsFunctions>`_
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
 
         Returns:
             Optional[Function]: Requested function or None if it does not exist.
@@ -312,15 +312,15 @@
         """
         identifiers = IdentifierSequence.load(ids=id, external_ids=external_id).as_singleton()
         return self._retrieve_multiple(identifiers=identifiers, resource_cls=Function, list_cls=FunctionList)
 
     def retrieve_multiple(
         self, ids: Optional[Sequence[int]] = None, external_ids: Optional[Sequence[str]] = None
     ) -> Union[FunctionList, Function, None]:
-        """`Retrieve multiple functions by id. <https://docs.cognite.com/api/v1/#operation/byIdsFunctions>`_
+        """`Retrieve multiple functions by id. <https://developer.cognite.com/api#tag/Functions/operation/byIdsFunctions>`_
 
         Args:
             ids (Sequence[int], optional): IDs
             external_ids (Sequence[str], optional): External IDs
 
         Returns:
             FunctionList: The requested functions.
@@ -350,15 +350,15 @@
     def call(
         self,
         id: Optional[int] = None,
         external_id: Optional[str] = None,
         data: Optional[Dict] = None,
         wait: bool = True,
     ) -> FunctionCall:
-        """`Call a function by its ID or external ID. <https://docs.cognite.com/api/v1/#operation/postFunctionsCall>`_.
+        """`Call a function by its ID or external ID. <https://developer.cognite.com/api#tag/Functions/operation/postFunctionsCall>`_.
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
             data (Union[str, dict], optional): Input data to the function (JSON serializable). This data is passed deserialized into the function through one of the arguments called data. **WARNING:** Secrets or other confidential information should not be passed via this argument. There is a dedicated `secrets` argument in FunctionsAPI.create() for this purpose.'
             wait (bool): Wait until the function call is finished. Defaults to True.
 
@@ -393,15 +393,15 @@
         function_call = FunctionCall._load(res.json(), cognite_client=self._cognite_client)
         if wait:
             function_call.wait()
 
         return function_call
 
     def limits(self) -> FunctionsLimits:
-        """`Get service limits. <https://docs.cognite.com/api/v1/#operation/functionsLimits>`_.
+        """`Get service limits. <https://developer.cognite.com/api#tag/Functions/operation/functionsLimits>`_.
 
         Returns:
             FunctionsLimits: A function limits object.
 
         Examples:
 
             Call a function by id::
@@ -474,15 +474,15 @@
             raise TypeError(
                 "Exactly one of the arguments folder, file_id and handle is required, but "
                 + ", ".join(given_source_code_options)
                 + " were given."
             )
 
     def activate(self) -> FunctionsStatus:
-        """`Activate functions for the Project. <https://docs.cognite.com/api/v1/#operation/postFunctionsStatus>`_.
+        """`Activate functions for the Project. <https://developer.cognite.com/api#tag/Functions/operation/postFunctionsStatus>`_.
 
         Returns:
             FunctionsStatus: A function activation status.
 
         Examples:
 
             Call activate::
@@ -491,15 +491,15 @@
                 >>> c = CogniteClient()
                 >>> status = c.functions.activate()
         """
         res = self._post("/functions/status")
         return FunctionsStatus._load(res.json())
 
     def status(self) -> FunctionsStatus:
-        """`Functions activation status for the Project. <https://docs.cognite.com/api/v1/#operation/getFunctionsStatus>`_.
+        """`Functions activation status for the Project. <https://developer.cognite.com/api#tag/Functions/operation/getFunctionsStatus>`_.
 
         Returns:
             FunctionsStatus: A function activation status.
 
         Examples:
 
             Call status::
@@ -667,15 +667,15 @@
         function_external_id: Optional[str] = None,
         status: Optional[str] = None,
         schedule_id: Optional[int] = None,
         start_time: Optional[Dict[str, int]] = None,
         end_time: Optional[Dict[str, int]] = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> FunctionCallList:
-        """`List all calls associated with a specific function id. <https://docs.cognite.com/api/v1/#operation/listFunctionCalls>`_ Either function_id or function_external_id must be specified.
+        """`List all calls associated with a specific function id. <https://developer.cognite.com/api#tag/Function-calls/operation/listFunctionCalls>`_ Either function_id or function_external_id must be specified.
 
         Args:
             function_id (int, optional): ID of the function on which the calls were made.
             function_external_id (str, optional): External ID of the function on which the calls were made.
             status (str, optional): Status of the call. Possible values ["Running", "Failed", "Completed", "Timeout"].
             schedule_id (int, optional): Schedule id from which the call belongs (if any).
             start_time (Dict[str, int], optional): Start time of the call. Possible keys are `min` and `max`, with values given as time stamps in ms.
@@ -715,15 +715,15 @@
             resource_cls=FunctionCall,
             list_cls=FunctionCallList,
         )
 
     def retrieve(
         self, call_id: int, function_id: Optional[int] = None, function_external_id: Optional[str] = None
     ) -> Union[FunctionCallList, FunctionCall, None]:
-        """`Retrieve a single function call by id. <https://docs.cognite.com/api/v1/#operation/byIdsFunctionCalls>`_
+        """`Retrieve a single function call by id. <https://developer.cognite.com/api#tag/Function-calls/operation/byIdsFunctionCalls>`_
 
         Args:
             call_id (int): ID of the call.
             function_id (int, optional): ID of the function on which the call was made.
             function_external_id (str, optional): External ID of the function on which the call was made.
 
         Returns:
@@ -757,15 +757,15 @@
             resource_cls=FunctionCall,
             list_cls=FunctionCallList,
         )
 
     def get_response(
         self, call_id: int, function_id: Optional[int] = None, function_external_id: Optional[str] = None
     ) -> Optional[Dict]:
-        """`Retrieve the response from a function call. <https://docs.cognite.com/api/v1/#operation/getFunctionCallResponse>`_
+        """`Retrieve the response from a function call. <https://developer.cognite.com/api#tag/Function-calls/operation/getFunctionCallResponse>`_
 
         Args:
             call_id (int): ID of the call.
             function_id (int, optional): ID of the function on which the call was made.
             function_external_id (str, optional): External ID of the function on which the call was made.
 
         Returns:
@@ -792,15 +792,15 @@
 
         resource_path = self._RESOURCE_PATH_RESPONSE.format(function_id, call_id)
         return self._get(resource_path).json().get("response")
 
     def get_logs(
         self, call_id: int, function_id: Optional[int] = None, function_external_id: Optional[str] = None
     ) -> FunctionCallLog:
-        """`Retrieve logs for function call. <https://docs.cognite.com/api/v1/#operation/getFunctionCalls>`_
+        """`Retrieve logs for function call. <https://developer.cognite.com/api#tag/Function-calls/operation/getFunctionCalls>`_
 
         Args:
             call_id (int): ID of the call.
             function_id (int, optional): ID of the function on which the call was made.
             function_external_id (str, optional): External ID of the function on which the call was made.
 
         Returns:
@@ -833,15 +833,15 @@
     _RESOURCE_PATH = "/functions/schedules"
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self._LIST_LIMIT_CEILING = 10_000
 
     def retrieve(self, id: int) -> Union[FunctionSchedule, FunctionSchedulesList, None]:
-        """`Retrieve a single function schedule by id. <https://docs.cognite.com/api/v1/#operation/byIdsFunctionSchedules>`_
+        """`Retrieve a single function schedule by id. <https://developer.cognite.com/api#tag/Function-schedules/operation/byIdsFunctionSchedules>`_
 
         Args:
             id (int): ID
 
         Returns:
             Optional[FunctionSchedule]: Requested function schedule.
 
@@ -863,15 +863,15 @@
         name: str = None,
         function_id: int = None,
         function_external_id: str = None,
         created_time: Union[Dict[str, int], TimestampRange] = None,
         cron_expression: str = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> FunctionSchedulesList:
-        """`List all schedules associated with a specific project. <https://docs.cognite.com/api/v1/#operation/listFunctionSchedules>`_
+        """`List all schedules associated with a specific project. <https://developer.cognite.com/api#tag/Function-schedules/operation/listFunctionSchedules>`_
 
         Args:
             name (str): Name of the function schedule.
             function_id (int): ID of the function the schedules are linked to.
             function_external_id (str): External ID of the function the schedules are linked to.
             created_time (Union[Dict[str, int], TimestampRange]):  Range between two timestamps. Possible keys are `min` and `max`, with values given as time stamps in ms.
             cron_expression (str): Cron expression.
@@ -923,15 +923,15 @@
         cron_expression: str,
         function_id: Optional[int] = None,
         function_external_id: Optional[str] = None,
         client_credentials: Union[Dict, ClientCredentials, None] = None,
         description: str = "",
         data: Optional[Dict] = None,
     ) -> FunctionSchedule:
-        """`Create a schedule associated with a specific project. <https://docs.cognite.com/api/v1/#operation/postFunctionSchedules>`_
+        """`Create a schedule associated with a specific project. <https://developer.cognite.com/api#tag/Function-schedules/operation/postFunctionSchedules>`_
 
         Args:
             name (str): Name of the schedule.
             function_id (optional, int): Id of the function. This is required if the schedule is created with client_credentials.
             function_external_id (optional, str): External id of the function. **NOTE**: This is deprecated and will be removed in a future major version.
             description (str): Description of the schedule.
             cron_expression (str): Cron expression.
@@ -995,15 +995,15 @@
         if data:
             body["items"][0]["data"] = data
 
         res = self._post(self._RESOURCE_PATH, json=body)
         return FunctionSchedule._load(res.json()["items"][0], cognite_client=self._cognite_client)
 
     def delete(self, id: int) -> None:
-        """`Delete a schedule associated with a specific project. <https://docs.cognite.com/api/v1/#operation/deleteFunctionSchedules>`_
+        """`Delete a schedule associated with a specific project. <https://developer.cognite.com/api#tag/Function-schedules/operation/deleteFunctionSchedules>`_
 
         Args:
             id (int): Id of the schedule
 
         Returns:
             None
 
@@ -1017,15 +1017,15 @@
 
         """
         body = {"items": [{"id": id}]}
         url = f"{self._RESOURCE_PATH}/delete"
         self._post(url, json=body)
 
     def get_input_data(self, id: int) -> Optional[Dict]:
-        """`Retrieve the input data to the associated function. <https://docs.cognite.com/api/v1/#operation/getFunctionScheduleInputData>`_
+        """`Retrieve the input data to the associated function. <https://developer.cognite.com/api#tag/Function-schedules/operation/getFunctionScheduleInputData>`_
         Args:
             id (int): Id of the schedule
 
         Returns:
             Optional[Dict]: Input data to the associated function or None if not set. This data is passed
             deserialized into the function through the data argument.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/geospatial.py` & `cognite_sdk-6.5.0/cognite/client/_api/geospatial.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def create_feature_types(self, feature_type: Sequence[FeatureType]) -> FeatureTypeList:
         ...
 
     def create_feature_types(
         self, feature_type: Union[FeatureType, Sequence[FeatureType]]
     ) -> Union[FeatureType, FeatureTypeList]:
         """`Creates feature types`
-        <https://docs.cognite.com/api/v1/#operation/createFeatureTypes>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/createFeatureTypes>
 
         Args:
             feature_type (Union[FeatureType, Sequence[FeatureType]]): feature type definition or list of feature type definitions to create.
 
         Returns:
             Union[FeatureType, FeatureTypeList]: Created feature type definition(s)
 
@@ -92,15 +92,15 @@
             resource_cls=FeatureType,
             items=feature_type,
             resource_path=f"{self._RESOURCE_PATH}/featuretypes",
         )
 
     def delete_feature_types(self, external_id: Union[str, Sequence[str]], recursive: bool = False) -> None:
         """`Delete one or more feature type`
-        <https://docs.cognite.com/api/v1/#operation/GeospatialDeleteFeatureTypes>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/GeospatialDeleteFeatureTypes>
 
         Args:
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
             recursive (bool): if `true` the features will also be dropped
 
         Returns:
             None
@@ -119,15 +119,15 @@
             wrap_ids=True,
             resource_path=f"{self._RESOURCE_PATH}/featuretypes",
             extra_body_fields=extra_body_fields,
         )
 
     def list_feature_types(self) -> FeatureTypeList:
         """`List feature types`
-        <https://docs.cognite.com/api/v1/#operation/listFeatureTypes>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/listFeatureTypes>
 
         Returns:
             FeatureTypeList: List of feature types
 
         Examples:
 
             Iterate over feature type definitions:
@@ -150,15 +150,15 @@
 
     @overload
     def retrieve_feature_types(self, external_id: List[str]) -> FeatureTypeList:
         ...
 
     def retrieve_feature_types(self, external_id: Union[str, List[str]]) -> Union[FeatureType, FeatureTypeList]:
         """`Retrieve feature types`
-        <https://docs.cognite.com/api/v1/#operation/getFeatureTypesByIds>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/getFeatureTypesByIds>
 
         Args:
             external_id (Union[str, List[str]]): External ID
 
         Returns:
             FeatureTypeList: Requested Type or None if it does not exist.
 
@@ -176,15 +176,15 @@
             resource_cls=FeatureType,
             identifiers=identifiers.as_singleton() if identifiers.is_singleton() else identifiers,
             resource_path=f"{self._RESOURCE_PATH}/featuretypes",
         )
 
     def update_feature_types(self, update: Union[FeatureTypeUpdate, Sequence[FeatureTypeUpdate]]) -> FeatureTypeList:
         """`Update feature types (Deprecated)`
-        <https://docs.cognite.com/api/v1/#operation/updateFeatureTypes>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/updateFeatureTypes>
 
         Args:
             update (Union[FeatureTypeUpdate, Sequence[FeatureTypeUpdate]]): the update to apply
 
         Returns:
             FeatureTypeList: The updated feature types.
 
@@ -232,15 +232,15 @@
 
         json = {"items": [{"externalId": it.external_id, "update": mapper(it)} for it in update]}
         res = self._post(url_path=f"{self._RESOURCE_PATH}/featuretypes/update", json=json)
         return FeatureTypeList._load(res.json()["items"], cognite_client=self._cognite_client)
 
     def patch_feature_types(self, patch: Union[FeatureTypePatch, Sequence[FeatureTypePatch]]) -> FeatureTypeList:
         """`Patch feature types`
-        <https://docs.cognite.com/api/v1/#operation/updateFeatureTypes>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/updateFeatureTypes>
 
         Args:
             patch (Union[FeatureTypePatch, Sequence[FeatureTypePatch]]): the patch to apply
 
         Returns:
             FeatureTypeList: The patched feature types.
 
@@ -314,15 +314,15 @@
         self,
         feature_type_external_id: str,
         feature: Union[Feature, Sequence[Feature], FeatureList],
         allow_crs_transformation: bool = False,
         chunk_size: int = None,
     ) -> Union[Feature, FeatureList]:
         """`Creates features`
-        <https://docs.cognite.com/api/v1/#operation/createFeatures>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/createFeatures>
 
         Args:
             feature_type_external_id: Feature type definition for the features to create.
             feature: one feature or a list of features to create or a FeatureList object
             allow_crs_transformation: If true, then input geometries will be transformed into the Coordinate Reference
                 System defined in the feature type specification. When it is false, then requests with geometries in
                 Coordinate Reference System different from the ones defined in the feature type will result in
@@ -370,15 +370,15 @@
             resource_path=resource_path,
             extra_body_fields=extra_body_fields,
             limit=chunk_size,
         )
 
     def delete_features(self, feature_type_external_id: str, external_id: Union[str, Sequence[str]] = None) -> None:
         """`Delete one or more feature`
-        <https://docs.cognite.com/api/v1/#operation/deleteFeatures>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/deleteFeatures>
 
         Args:
             feature_type_external_id : Feature type external id for the features to delete.
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
 
         Returns:
             None
@@ -420,15 +420,15 @@
     def retrieve_features(
         self,
         feature_type_external_id: str,
         external_id: Union[str, List[str]],
         properties: Dict[str, Any] = None,
     ) -> Union[FeatureList, Feature]:
         """`Retrieve features`
-        <https://docs.cognite.com/api/v1/#operation/getFeaturesByIds>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/getFeaturesByIds>
 
         Args:
             feature_type_external_id : Feature type external id for the features to retrieve.
             external_id (Union[str, List[str]]): External ID or list of external ids
             properties (Dict[str, Any]): the output property selection
 
         Returns:
@@ -459,15 +459,15 @@
         self,
         feature_type_external_id: str,
         feature: Union[Feature, Sequence[Feature]],
         allow_crs_transformation: bool = False,
         chunk_size: int = None,
     ) -> FeatureList:
         """`Update features`
-        <https://docs.cognite.com/api/v1/#operation/updateFeatures>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/updateFeatures>
 
         Args:
             feature_type_external_id : Feature type definition for the features to update.
             feature (Union[Feature, Sequence[Feature]]): feature or list of features.
             allow_crs_transformation: If true, then input geometries will be transformed into the Coordinate Reference
                 System defined in the feature type specification. When it is false, then requests with geometries in
                 Coordinate Reference System different from the ones defined in the feature type will result in
@@ -517,15 +517,15 @@
         feature_type_external_id: str,
         filter: Optional[Dict[str, Any]] = None,
         properties: Dict[str, Any] = None,
         limit: int = 100,
         allow_crs_transformation: bool = False,
     ) -> FeatureList:
         """`List features`
-        <https://docs.cognite.com/api/v1/#operation/listFeatures>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/listFeatures>
 
         This method allows to filter all features.
 
         Args:
             feature_type_external_id: the feature type to list features for
             filter (Dict[str, Any]): the list filter
             limit (int, optional): Maximum number of features to return. Defaults to 25. Set to -1, float("inf") or None
@@ -600,15 +600,15 @@
         filter: Optional[Dict[str, Any]] = None,
         properties: Dict[str, Any] = None,
         limit: int = 100,
         order_by: Sequence[OrderSpec] = None,
         allow_crs_transformation: bool = False,
     ) -> FeatureList:
         """`Search for features`
-        <https://docs.cognite.com/api/v1/#operation/searchFeatures>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/searchFeatures>
 
         This method allows to order the result by one or more of the properties of the feature type.
         However, the number of items returned is  limited to 1000 and there is no support for cursors yet.
         If you need to return more than 1000 items, use the `stream_features(...)` method instead.
 
         Args:
             feature_type_external_id: the feature type to search for
@@ -719,15 +719,15 @@
         self,
         feature_type_external_id: str,
         filter: Optional[Dict[str, Any]] = None,
         properties: Dict[str, Any] = None,
         allow_crs_transformation: bool = False,
     ) -> Generator[Feature, None, None]:
         """`Stream features`
-        <https://docs.cognite.com/api/v1/#operation/searchFeaturesStreaming>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/searchFeaturesStreaming>
 
         This method allows to return any number of items until the underlying
         api calls times out. The order of the result items is not deterministic.
         If you need to order the results, use the `search_features(...)` method instead.
 
         Args:
             feature_type_external_id: the feature type to search for
@@ -789,15 +789,15 @@
         aggregates: Sequence[str] = None,
         filter: Optional[Dict[str, Any]] = None,
         group_by: Sequence[str] = None,
         order_by: Sequence[OrderSpec] = None,
         output: Dict[str, Any] = None,
     ) -> FeatureAggregateList:
         """`Aggregate filtered features`
-        <https://docs.cognite.com/api/v1/#operation/aggregateFeatures>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/aggregateFeatures>
 
         Args:
             feature_type_external_id: the feature type to filter features from
             filter (Dict[str, Any]): the search filter
             property (str): the property for which aggregates should be calculated
             aggregates (Sequence[str]): list of aggregates to be calculated
             group_by (Sequence[str]): list of properties to group by with
@@ -853,15 +853,15 @@
                 "output": output,
             },
         )
         return cls._load(res.json()["items"], cognite_client=self._cognite_client)
 
     def get_coordinate_reference_systems(self, srids: Union[int, Sequence[int]]) -> CoordinateReferenceSystemList:
         """`Get Coordinate Reference Systems`
-        <https://docs.cognite.com/api/v1/#operation/getCoordinateReferenceSystem>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/getCoordinateReferenceSystem>
 
         Args:
             srids: (Union[int, Sequence[int]]): SRID or list of SRIDs
 
         Returns:
             CoordinateReferenceSystemList: Requested CRSs.
 
@@ -881,15 +881,15 @@
         res = self._post(
             url_path=f"{self._RESOURCE_PATH}/crs/byids", json={"items": [{"srid": srid} for srid in srids_processed]}
         )
         return CoordinateReferenceSystemList._load(res.json()["items"], cognite_client=self._cognite_client)
 
     def list_coordinate_reference_systems(self, only_custom: bool = False) -> CoordinateReferenceSystemList:
         """`List Coordinate Reference Systems`
-        <https://docs.cognite.com/api/v1/#operation/listGeospatialCoordinateReferenceSystems>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/listGeospatialCoordinateReferenceSystems>
 
         Args:
             only_custom (bool): list only custom CRSs or not
 
         Returns:
             CoordinateReferenceSystemList: list of CRSs.
 
@@ -904,15 +904,15 @@
         res = self._get(url_path=f"{self._RESOURCE_PATH}/crs", params={"filterCustom": only_custom})
         return CoordinateReferenceSystemList._load(res.json()["items"], cognite_client=self._cognite_client)
 
     def create_coordinate_reference_systems(
         self, crs: Union[CoordinateReferenceSystem, Sequence[CoordinateReferenceSystem]]
     ) -> CoordinateReferenceSystemList:
         """`Create Coordinate Reference System`
-        <https://docs.cognite.com/api/v1/#operation/createGeospatialCoordinateReferenceSystems>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/createGeospatialCoordinateReferenceSystems>
 
         Args:
             crs: a CoordinateReferenceSystem or a list of CoordinateReferenceSystem
 
         Returns:
             CoordinateReferenceSystemList: list of CRSs.
 
@@ -963,15 +963,15 @@
         res = self._post(
             url_path=f"{self._RESOURCE_PATH}/crs", json={"items": [it.dump(camel_case=True) for it in crs]}
         )
         return CoordinateReferenceSystemList._load(res.json()["items"], cognite_client=self._cognite_client)
 
     def delete_coordinate_reference_systems(self, srids: Union[int, Sequence[int]]) -> None:
         """`Delete Coordinate Reference System`
-        <https://docs.cognite.com/api/v1/#operation/deleteGeospatialCoordinateReferenceSystems>
+        <https://developer.cognite.com/api#tag/Geospatial/operation/deleteGeospatialCoordinateReferenceSystems>
 
         Args:
             srids: (Union[int, Sequence[int]]): SRID or list of SRIDs
 
         Returns:
             None
 
@@ -1000,15 +1000,15 @@
         raster_format: str,
         raster_srid: int,
         file: str,
         allow_crs_transformation: bool = False,
         raster_scale_x: Optional[float] = None,
         raster_scale_y: Optional[float] = None,
     ) -> RasterMetadata:
-        """`Put raster <https://docs.cognite.com/api/v1/#operation/putRaster>`
+        """`Put raster <https://developer.cognite.com/api#tag/Geospatial/operation/putRaster>`
 
         Args:
             feature_type_external_id : Feature type definition for the features to create.
             feature_external_id: one feature or a list of features to create
             raster_property_name: the raster property name
             raster_format: the raster input format
             raster_srid: the associated SRID for the raster
@@ -1055,15 +1055,15 @@
 
     def delete_raster(
         self,
         feature_type_external_id: str,
         feature_external_id: str,
         raster_property_name: str,
     ) -> None:
-        """`Delete raster <https://docs.cognite.com/api/v1/#operation/deleteRaster>`
+        """`Delete raster <https://developer.cognite.com/api#tag/Geospatial/operation/deleteRaster>`
 
         Args:
             feature_type_external_id : Feature type definition for the features to create.
             feature_external_id: one feature or a list of features to create
             raster_property_name: the raster property name
 
         Returns:
@@ -1097,15 +1097,15 @@
         raster_format: str,
         raster_options: Dict[str, Any] = None,
         raster_srid: Optional[int] = None,
         raster_scale_x: Optional[float] = None,
         raster_scale_y: Optional[float] = None,
         allow_crs_transformation: bool = False,
     ) -> bytes:
-        """`Get raster <https://docs.cognite.com/api/v1/#operation/getRaster>`
+        """`Get raster <https://developer.cognite.com/api#tag/Geospatial/operation/getRaster>`
 
         Args:
             feature_type_external_id: Feature type definition for the features to create.
             feature_external_id: one feature or a list of features to create
             raster_property_name: the raster property name
             raster_format: the raster output format
             raster_options: GDAL raster creation key-value options
@@ -1146,15 +1146,15 @@
         )
         return res.content
 
     def compute(
         self,
         output: Dict[str, GeospatialComputeFunction],
     ) -> GeospatialComputedResponse:
-        """`Compute <https://docs.cognite.com/api/v1/#operation/compute>`
+        """`Compute <https://developer.cognite.com/api#tag/Geospatial/operation/compute>`
 
         Args:
             output : Mapping of keys to compute functions.
 
         Returns:
             dict: Mapping of keys to computed items.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/iam.py` & `cognite_sdk-6.5.0/cognite/client/_api/iam.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         self.token = TokenAPI(config, api_version=None, cognite_client=cognite_client)
 
 
 class GroupsAPI(APIClient):
     _RESOURCE_PATH = "/groups"
 
     def list(self, all: bool = False) -> GroupList:
-        """`List groups. <https://docs.cognite.com/api/v1/#operation/getGroups>`_
+        """`List groups. <https://developer.cognite.com/api#tag/Groups/operation/getGroups>`_
 
         Args:
             all (bool): Whether to get all groups, only available with the groups:list acl.
 
         Returns:
             GroupList: List of groups.
 
@@ -53,15 +53,15 @@
                 >>> c = CogniteClient()
                 >>> res = c.iam.groups.list()
         """
         res = self._get(self._RESOURCE_PATH, params={"all": all})
         return GroupList._load(res.json()["items"])
 
     def create(self, group: Union[Group, Sequence[Group]]) -> Union[Group, GroupList]:
-        """`Create one or more groups. <https://docs.cognite.com/api/v1/#operation/createGroups>`_
+        """`Create one or more groups. <https://developer.cognite.com/api#tag/Groups/operation/createGroups>`_
 
         Args:
             group (Union[Group, Sequence[Group]]): Group or list of groups to create.
         Returns:
             Union[Group, GroupList]: The created group(s).
 
         Example:
@@ -74,15 +74,15 @@
                 >>> my_capabilities = [{"groupsAcl": {"actions": ["LIST"],"scope": {"all": { }}}}]
                 >>> my_group = Group(name="My Group", capabilities=my_capabilities)
                 >>> res = c.iam.groups.create(my_group)
         """
         return self._create_multiple(list_cls=GroupList, resource_cls=Group, items=group)
 
     def delete(self, id: Union[int, Sequence[int]]) -> None:
-        """`Delete one or more groups. <https://docs.cognite.com/api/v1/#operation/deleteGroups>`_
+        """`Delete one or more groups. <https://developer.cognite.com/api#tag/Groups/operation/deleteGroups>`_
 
         Args:
             id (Union[int, Sequence[int]]): ID or list of IDs of groups to delete.
 
         Returns:
             None
 
@@ -97,15 +97,15 @@
         self._delete_multiple(identifiers=IdentifierSequence.load(ids=id), wrap_ids=False)
 
 
 class SecurityCategoriesAPI(APIClient):
     _RESOURCE_PATH = "/securitycategories"
 
     def list(self, limit: int = LIST_LIMIT_DEFAULT) -> SecurityCategoryList:
-        """`List security categories. <https://docs.cognite.com/api/v1/#operation/getSecurityCategories>`_
+        """`List security categories. <https://developer.cognite.com/api#tag/Security-categories/operation/getSecurityCategories>`_
 
         Args:
             limit (int): Max number of security categories to return. Defaults to 25.
 
         Returns:
             SecurityCategoryList: List of security categories
 
@@ -118,15 +118,15 @@
                 >>> res = c.iam.security_categories.list()
         """
         return self._list(list_cls=SecurityCategoryList, resource_cls=SecurityCategory, method="GET", limit=limit)
 
     def create(
         self, security_category: Union[SecurityCategory, Sequence[SecurityCategory]]
     ) -> Union[SecurityCategory, SecurityCategoryList]:
-        """`Create one or more security categories. <https://docs.cognite.com/api/v1/#operation/createSecurityCategories>`_
+        """`Create one or more security categories. <https://developer.cognite.com/api#tag/Security-categories/operation/createSecurityCategories>`_
 
         Args:
             security_category (Union[SecurityCategory, Sequence[SecurityCategory]]): Security category or list of categories to create.
 
         Returns:
             Union[SecurityCategory, SecurityCategoryList]: The created security category or categories.
 
@@ -141,15 +141,15 @@
                 >>> res = c.iam.security_categories.create(my_category)
         """
         return self._create_multiple(
             list_cls=SecurityCategoryList, resource_cls=SecurityCategory, items=security_category
         )
 
     def delete(self, id: Union[int, Sequence[int]]) -> None:
-        """`Delete one or more security categories. <https://docs.cognite.com/api/v1/#operation/deleteSecurityCategories>`_
+        """`Delete one or more security categories. <https://developer.cognite.com/api#tag/Security-categories/operation/deleteSecurityCategories>`_
 
         Args:
             id (Union[int, Sequence[int]]): ID or list of IDs of security categories to delete.
 
         Returns:
             None
 
@@ -188,15 +188,15 @@
     _RESOURCE_PATH = "/sessions"
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self._LIST_LIMIT = 100
 
     def create(self, client_credentials: Optional[ClientCredentials] = None) -> CreatedSession:
-        """`Create a session. <https://docs.cognite.com/api/v1/#operation/createSessions>`_
+        """`Create a session. <https://developer.cognite.com/api#tag/Sessions/operation/createSessions>`_
 
         Args:
             client_credentials (Optional[ClientCredentials]): The client credentials to create the session. If set to None,
                 a session will be created using the credentials used to instantiate -this- CogniteClient object. If that
                 was done using a token, a session will be created using token exchange. Similarly, if the credentials were
                 client credentials, a session will be created using client credentials. This method does not work when
                 using client certificates (not supported server-side).
@@ -207,29 +207,29 @@
         if client_credentials is None and isinstance((creds := self._config.credentials), OAuthClientCredentials):
             client_credentials = ClientCredentials(creds.client_id, creds.client_secret)
 
         items = {"tokenExchange": True} if client_credentials is None else client_credentials.dump(camel_case=True)
         return CreatedSession._load(self._post(self._RESOURCE_PATH, {"items": [items]}).json()["items"][0])
 
     def revoke(self, id: Union[int, Sequence[int]]) -> SessionList:
-        """`Revoke access to a session. Revocation of a session may in some cases take up to 1 hour to take effect. <https://docs.cognite.com/api/v1/#operation/revokeSessions>`_
+        """`Revoke access to a session. Revocation of a session may in some cases take up to 1 hour to take effect. <https://developer.cognite.com/api#tag/Sessions/operation/revokeSessions>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of session ids
 
         Returns:
             SessionList: List of revoked sessions. If the user does not have the sessionsAcl:LIST capability, then only the session IDs will be present in the response.
         """
         identifiers = IdentifierSequence.load(ids=id, external_ids=None)
         items = {"items": identifiers.as_dicts()}
 
         return SessionList._load(self._post(self._RESOURCE_PATH + "/revoke", items).json()["items"])
 
     def list(self, status: Optional[str] = None) -> SessionList:
-        """`List all sessions in the current project. <https://docs.cognite.com/api/v1/#operation/listSessions>`_
+        """`List all sessions in the current project. <https://developer.cognite.com/api#tag/Sessions/operation/listSessions>`_
 
         Args:
             status (Optional[str]): If given, only sessions with the given status are returned.
 
         Returns:
             SessionList: a list of sessions in the current project.
         """
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/labels.py` & `cognite_sdk-6.5.0/cognite/client/_api/labels.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self,
         name: str = None,
         external_id_prefix: str = None,
         data_set_ids: Union[int, Sequence[int]] = None,
         data_set_external_ids: Union[str, Sequence[str]] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> LabelDefinitionList:
-        """`List Labels <https://docs.cognite.com/api/v1/#operation/listLabels>`_
+        """`List Labels <https://developer.cognite.com/api#tag/Labels/operation/listLabels>`_
 
         Args:
             name (str): returns the label definitions matching that name
             data_set_ids (Union[int, Sequence[int]]): return only labels in the data sets with this id / these ids.
             data_set_external_ids (Union[str, Sequence[str]]): return only labels in the data sets with this external id / these external ids.
             external_id_prefix (str): filter label definitions with external ids starting with the prefix specified
             limit (int, optional): Maximum number of label definitions to return.
@@ -95,15 +95,15 @@
         return self._list(
             list_cls=LabelDefinitionList, resource_cls=LabelDefinition, method="POST", limit=limit, filter=filter
         )
 
     def create(
         self, label: Union[LabelDefinition, Sequence[LabelDefinition]]
     ) -> Union[LabelDefinition, LabelDefinitionList]:
-        """`Create one or more label definitions. <https://docs.cognite.com/api/v1/#operation/createLabelDefinitions>`_
+        """`Create one or more label definitions. <https://developer.cognite.com/api#tag/Labels/operation/createLabelDefinitions>`_
 
         Args:
             Label (Union[LabelDefinition, Sequence[LabelDefinition]]): label definition or a list of label definitions to create.
 
         Returns:
             Union[LabelDefinition, LabelDefinitionList]: Created label definition(s)
 
@@ -121,15 +121,15 @@
             if len(label) > 0 and not isinstance(label[0], LabelDefinition):
                 raise TypeError("'label' must be of type LabelDefinition or Sequence[LabelDefinition]")
         elif not isinstance(label, LabelDefinition):
             raise TypeError("'label' must be of type LabelDefinition or Sequence[LabelDefinition]")
         return self._create_multiple(list_cls=LabelDefinitionList, resource_cls=LabelDefinition, items=label)
 
     def delete(self, external_id: Union[str, Sequence[str]] = None) -> None:
-        """`Delete one or more label definitions <https://docs.cognite.com/api/v1/#operation/deleteLabels>`_
+        """`Delete one or more label definitions <https://developer.cognite.com/api#tag/Labels/operation/deleteLabels>`_
 
         Args:
             external_id (Union[str, Sequence[str]]): One or more label external ids
 
         Returns:
             None
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/raw.py` & `cognite_sdk-6.5.0/cognite/client/_api/raw.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         ...
 
     @overload
     def create(self, name: List[str]) -> DatabaseList:
         ...
 
     def create(self, name: Union[str, List[str]]) -> Union[Database, DatabaseList]:
-        """`Create one or more databases. <https://docs.cognite.com/api/v1/#operation/createDBs>`_
+        """`Create one or more databases. <https://developer.cognite.com/api#tag/Raw/operation/createDBs>`_
 
         Args:
             name (Union[str, List[str]]): A db name or list of db names to create.
 
         Returns:
             Union[Database, DatabaseList]: Database or list of databases that has been created.
 
@@ -72,15 +72,15 @@
         if isinstance(name, str):
             items: Union[Dict[str, Any], List[Dict[str, Any]]] = {"name": name}
         else:
             items = [{"name": n} for n in name]
         return self._create_multiple(list_cls=DatabaseList, resource_cls=Database, items=items)
 
     def delete(self, name: Union[str, Sequence[str]], recursive: bool = False) -> None:
-        """`Delete one or more databases. <https://docs.cognite.com/api/v1/#operation/deleteDBs>`_
+        """`Delete one or more databases. <https://developer.cognite.com/api#tag/Raw/operation/deleteDBs>`_
 
         Args:
             name (Union[str, Sequence[str]]): A db name or list of db names to delete.
             recursive (bool): Recursively delete all tables in the database(s).
 
         Returns:
             None
@@ -104,15 +104,15 @@
         ]
         summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
         summary.raise_compound_exception_if_failed_tasks(
             task_unwrap_fn=lambda task: task["json"]["items"], task_list_element_unwrap_fn=lambda el: el["name"]
         )
 
     def list(self, limit: int = LIST_LIMIT_DEFAULT) -> DatabaseList:
-        """`List databases <https://docs.cognite.com/api/v1/#operation/getDBs>`_
+        """`List databases <https://developer.cognite.com/api#tag/Raw/operation/getDBs>`_
 
         Args:
             limit (int, optional): Maximum number of databases to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
         Returns:
             DatabaseList: List of requested databases.
@@ -172,15 +172,15 @@
         ...
 
     @overload
     def create(self, db_name: str, name: List[str]) -> TableList:
         ...
 
     def create(self, db_name: str, name: Union[str, List[str]]) -> Union[Table, TableList]:
-        """`Create one or more tables. <https://docs.cognite.com/api/v1/#operation/createTables>`_
+        """`Create one or more tables. <https://developer.cognite.com/api#tag/Raw/operation/createTables>`_
 
         Args:
             db_name (str): Database to create the tables in.
             name (Union[str, List[str]]): A table name or list of table names to create.
 
         Returns:
             Union[Table, TableList]: Table or list of tables that has been created.
@@ -203,15 +203,15 @@
             resource_cls=Table,
             resource_path=utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, db_name),
             items=items,
         )
         return self._set_db_name_on_tables(tb, db_name)
 
     def delete(self, db_name: str, name: Union[str, Sequence[str]]) -> None:
-        """`Delete one or more tables. <https://docs.cognite.com/api/v1/#operation/deleteTables>`_
+        """`Delete one or more tables. <https://developer.cognite.com/api#tag/Raw/operation/deleteTables>`_
 
         Args:
             db_name (str): Database to delete tables from.
             name (Union[str, Sequence[str]]): A table name or list of table names to delete.
 
         Returns:
             None
@@ -238,15 +238,15 @@
         ]
         summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
         summary.raise_compound_exception_if_failed_tasks(
             task_unwrap_fn=lambda task: task["json"]["items"], task_list_element_unwrap_fn=lambda el: el["name"]
         )
 
     def list(self, db_name: str, limit: int = LIST_LIMIT_DEFAULT) -> TableList:
-        """`List tables <https://docs.cognite.com/api/v1/#operation/getTables>`_
+        """`List tables <https://developer.cognite.com/api#tag/Raw/operation/getTables>`_
 
         Args:
             db_name (str): The database to list tables from.
             limit (int, optional): Maximum number of tables to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
         Returns:
@@ -338,15 +338,15 @@
                 "columns": self._make_columns_param(columns),
             },
         )
 
     def insert(
         self, db_name: str, table_name: str, row: Union[Sequence[Row], Row, Dict], ensure_parent: bool = False
     ) -> None:
-        """`Insert one or more rows into a table. <https://docs.cognite.com/api/v1/#operation/postRows>`_
+        """`Insert one or more rows into a table. <https://developer.cognite.com/api#tag/Raw/operation/postRows>`_
 
         Args:
             db_name (str): Name of the database.
             table_name (str): Name of the table.
             row (Union[Sequence[Row], Row, Dict]): The row(s) to insert
             ensure_parent (bool): Create database/table if they don't already exist.
 
@@ -374,15 +374,15 @@
         ]
         summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
         summary.raise_compound_exception_if_failed_tasks(
             task_unwrap_fn=lambda task: task["json"]["items"], task_list_element_unwrap_fn=lambda row: row.get("key")
         )
 
     def insert_dataframe(self, db_name: str, table_name: str, dataframe: Any, ensure_parent: bool = False) -> None:
-        """`Insert pandas dataframe into a table <https://docs.cognite.com/api/v1/#operation/postRows>`_
+        """`Insert pandas dataframe into a table <https://developer.cognite.com/api#tag/Raw/operation/postRows>`_
 
         Use index as rowkeys.
 
         Args:
             db_name (str): Name of the database.
             table_name (str): Name of the table.
             dataframe (pandas.DataFrame): The dataframe to insert. Index will be used as rowkeys.
@@ -419,15 +419,15 @@
                 else:
                     raise TypeError("list elements must be Row objects.")
         elif isinstance(row, Row):
             rows.append(row.dump(camel_case=True))
         return utils._auxiliary.split_into_chunks(rows, self._CREATE_LIMIT)
 
     def delete(self, db_name: str, table_name: str, key: Union[str, Sequence[str]]) -> None:
-        """`Delete rows from a table. <https://docs.cognite.com/api/v1/#operation/deleteRows>`_
+        """`Delete rows from a table. <https://developer.cognite.com/api#tag/Raw/operation/deleteRows>`_
 
         Args:
             db_name (str): Name of the database.
             table_name (str): Name of the table.
             key (Union[str, Sequence[str]]): The key(s) of the row(s) to delete.
 
         Returns:
@@ -459,15 +459,15 @@
         ]
         summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
         summary.raise_compound_exception_if_failed_tasks(
             task_unwrap_fn=lambda task: task["json"]["items"], task_list_element_unwrap_fn=lambda el: el["key"]
         )
 
     def retrieve(self, db_name: str, table_name: str, key: str) -> Optional[Row]:
-        """`Retrieve a single row by key. <https://docs.cognite.com/api/v1/#operation/getRow>`_
+        """`Retrieve a single row by key. <https://developer.cognite.com/api#tag/Raw/operation/getRow>`_
 
         Args:
             db_name (str): Name of the database.
             table_name (str): Name of the table.
             key (str): The key of the row to retrieve.
 
         Returns:
@@ -492,15 +492,15 @@
         db_name: str,
         table_name: str,
         min_last_updated_time: int = None,
         max_last_updated_time: int = None,
         columns: List[str] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> RowList:
-        """`List rows in a table. <https://docs.cognite.com/api/v1/#operation/getRows>`_
+        """`List rows in a table. <https://developer.cognite.com/api#tag/Raw/operation/getRows>`_
 
         Args:
             db_name (str): Name of the database.
             table_name (str): Name of the table.
             min_last_updated_time (int): Rows must have been last updated after this time (exclusive). ms since epoch.
             max_last_updated_time (int): Rows must have been last updated before this time (inclusive). ms since epoch.
             columns (List[str]): List of column keys. Set to `None` for retrieving all, use [] to retrieve only row keys.
@@ -580,15 +580,15 @@
         db_name: str,
         table_name: str,
         min_last_updated_time: int = None,
         max_last_updated_time: int = None,
         columns: List[str] = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> pandas.DataFrame:
-        """`Retrieve rows in a table as a pandas dataframe. <https://docs.cognite.com/api/v1/#operation/getRows>`_
+        """`Retrieve rows in a table as a pandas dataframe. <https://developer.cognite.com/api#tag/Raw/operation/getRows>`_
 
         Rowkeys are used as the index.
 
         Args:
             db_name (str): Name of the database.
             table_name (str): Name of the table.
             min_last_updated_time (int): Rows must have been last updated after this time. ms since epoch.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/relationships.py` & `cognite_sdk-6.5.0/cognite/client/_api/relationships.py`

 * *Files 3% similar despite different names*

```diff
@@ -167,15 +167,15 @@
             list_cls=RelationshipList,
             resource_cls=Relationship,
             identifiers=identifiers,
             other_params={"fetchResources": fetch_resources},
         )
 
     def retrieve_multiple(self, external_ids: Sequence[str], fetch_resources: bool = False) -> RelationshipList:
-        """`Retrieve multiple relationships by external id.  <https://docs.cognite.com/api/v1/#operation/byidsRelationships>`_
+        """`Retrieve multiple relationships by external id.  <https://developer.cognite.com/api#tag/Relationships/operation/byidsRelationships>`_
 
         Args:
             external_ids (Sequence[str]): External IDs
             fetch_resources (bool): if true, will try to return the full resources referenced by the relationship in the
                 source and target fields.
 
         Returns:
@@ -212,15 +212,15 @@
         created_time: Dict[str, int] = None,
         active_at_time: Dict[str, int] = None,
         labels: LabelFilter = None,
         limit: int = 100,
         partitions: int = None,
         fetch_resources: bool = False,
     ) -> RelationshipList:
-        """`Lists relationships stored in the project based on a query filter given in the payload of this request. Up to 1000 relationships can be retrieved in one operation.  <https://docs.cognite.com/api/v1/#operation/listRelationships>`_
+        """`Lists relationships stored in the project based on a query filter given in the payload of this request. Up to 1000 relationships can be retrieved in one operation.  <https://developer.cognite.com/api#tag/Relationships/operation/listRelationships>`_
 
         Args:
             source_external_ids (Sequence[str]): Include relationships that have any of these values in their source External Id field
             source_types (Sequence[str]): Include relationships that have any of these values in their source Type field
             target_external_ids (Sequence[str]): Include relationships that have any of these values in their target External Id field
             target_types (Sequence[str]): Include relationships that have any of these values in their target Type field
             data_set_ids (Union[int, Sequence[int]]): Return only relationships in the specified data set(s) with this id / these ids.
@@ -318,15 +318,15 @@
             filter=filter,
             other_params={"fetchResources": fetch_resources},
         )
 
     def create(
         self, relationship: Union[Relationship, Sequence[Relationship]]
     ) -> Union[Relationship, RelationshipList]:
-        """`Create one or more relationships. <https://docs.cognite.com/api/v1/#operation/createRelationships>`_
+        """`Create one or more relationships. <https://developer.cognite.com/api#tag/Relationships/operation/createRelationships>`_
 
         Args:
             relationship (Union[Relationship, Sequence[Relationship]]): Relationship or list of relationships to create.
 
         Returns:
             Union[Relationship, RelationshipList]: Created relationship(s)
 
@@ -368,15 +368,15 @@
             relationship = relationship._validate_resource_types()
 
         return self._create_multiple(list_cls=RelationshipList, resource_cls=Relationship, items=relationship)
 
     def update(
         self, item: Union[Relationship, RelationshipUpdate, Sequence[Union[Relationship, RelationshipUpdate]]]
     ) -> Union[Relationship, RelationshipList]:
-        """`Update one or more relationships <https://docs.cognite.com/api/v1/#operation/updateRelationships>`_
+        """`Update one or more relationships <https://developer.cognite.com/api#tag/Relationships/operation/updateRelationships>`_
         Currently, a full replacement of labels on a relationship is not supported (only partial add/remove updates). See the example below on how to perform partial labels update.
 
         Args:
             item (Union[Relationship, RelationshipUpdate, Sequence[Union[Relationship, RelationshipUpdate]]]): Relationship(s) to update
 
         Returns:
             Union[Relationship, RelationshipList]: Updated relationship(s)
@@ -418,15 +418,15 @@
                 >>> res = c.relationships.update(my_update)
         """
         return self._update_multiple(
             list_cls=RelationshipList, resource_cls=Relationship, update_cls=RelationshipUpdate, items=item
         )
 
     def delete(self, external_id: Union[str, Sequence[str]], ignore_unknown_ids: bool = False) -> None:
-        """`Delete one or more relationships. <https://docs.cognite.com/api/v1/#operation/deleteRelationships>`_
+        """`Delete one or more relationships. <https://developer.cognite.com/api#tag/Relationships/operation/deleteRelationships>`_
 
         Args:
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
             ignore_unknown_ids (bool): Ignore external IDs that are not found rather than throw an exception.
         Returns:
             None
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/sequences.py` & `cognite_sdk-6.5.0/cognite/client/_api/sequences.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
         Yields:
             Sequence: yields Sequence one by one.
         """
         return cast(Iterator[Sequence], self())
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[Sequence]:
-        """`Retrieve a single sequence by id. <https://docs.cognite.com/api/v1/#operation/getSequenceById>`_
+        """`Retrieve a single sequence by id. <https://developer.cognite.com/api#tag/Sequences/operation/getSequenceById>`_
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
 
         Returns:
             Optional[Sequence]: Requested sequences or None if it does not exist.
@@ -133,15 +133,15 @@
 
     def retrieve_multiple(
         self,
         ids: Optional[SequenceType[int]] = None,
         external_ids: Optional[SequenceType[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> SequenceList:
-        """`Retrieve multiple sequences by id. <https://docs.cognite.com/api/v1/#operation/getSequenceById>`_
+        """`Retrieve multiple sequences by id. <https://developer.cognite.com/api#tag/Sequences/operation/getSequenceById>`_
 
         Args:
             ids (SequenceType[int], optional): IDs
             external_ids (SequenceType[str], optional): External IDs
             ignore_unknown_ids (bool, optional): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -176,15 +176,15 @@
         asset_subtree_external_ids: Union[str, SequenceType[str]] = None,
         data_set_ids: Union[int, SequenceType[int]] = None,
         data_set_external_ids: Union[str, SequenceType[str]] = None,
         created_time: (Union[Dict[str, Any], TimestampRange]) = None,
         last_updated_time: (Union[Dict[str, Any], TimestampRange]) = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> SequenceList:
-        """`Iterate over sequences <https://docs.cognite.com/api/v1/#operation/advancedListSequences>`_
+        """`Iterate over sequences <https://developer.cognite.com/api#tag/Sequences/operation/advancedListSequences>`_
 
         Fetches sequences as they are iterated over, so you keep a limited number of objects in memory.
 
         Args:
             name (str): Filter out sequences that do not have this *exact* name.
             external_id_prefix (str): Filter out sequences that do not have this string as the start of the externalId
             metadata (Dict[str, Any]): Filter out sequences that do not match these metadata fields and values (case-sensitive). Format is {"key1":"value1","key2":"value2"}.
@@ -235,15 +235,15 @@
             created_time=created_time,
             last_updated_time=last_updated_time,
             data_set_ids=data_set_ids_processed,
         ).dump(camel_case=True)
         return self._list(list_cls=SequenceList, resource_cls=Sequence, method="POST", filter=filter, limit=limit)
 
     def aggregate(self, filter: Union[SequenceFilter, Dict] = None) -> List[SequenceAggregate]:
-        """`Aggregate sequences <https://docs.cognite.com/api/v1/#operation/aggregateSequences>`_
+        """`Aggregate sequences <https://developer.cognite.com/api#tag/Sequences/operation/aggregateSequences>`_
 
         Args:
             filter (Union[SequenceFilter, Dict]): Filter on sequence filter with exact match
 
         Returns:
             List[SequenceAggregate]: List of sequence aggregates
 
@@ -263,15 +263,15 @@
         ...
 
     @overload
     def create(self, sequence: SequenceType[Sequence]) -> SequenceList:
         ...
 
     def create(self, sequence: Union[Sequence, SequenceType[Sequence]]) -> Union[Sequence, SequenceList]:
-        """`Create one or more sequences. <https://docs.cognite.com/api/v1/#operation/createSequence>`_
+        """`Create one or more sequences. <https://developer.cognite.com/api#tag/Sequences/operation/createSequence>`_
 
         Args:
             sequence (Union[Sequence, SequenceType[Sequence]]): Sequence or list of Sequence to create.
                 The Sequence columns parameter is a list of objects with fields
                 `externalId` (external id of the column, when omitted, they will be given ids of 'column0, column1, ...'),
                 `valueType` (data type of the column, either STRING, LONG, or DOUBLE, with default DOUBLE),
                 `name`, `description`, `metadata` (optional fields to describe and store information about the data in the column).
@@ -318,15 +318,15 @@
             if sequence.columns[i].get("valueType"):
                 sequence.columns[i]["valueType"] = sequence.columns[i]["valueType"].upper()
         return sequence
 
     def delete(
         self, id: Union[int, SequenceType[int]] = None, external_id: Union[str, SequenceType[str]] = None
     ) -> None:
-        """`Delete one or more sequences. <https://docs.cognite.com/api/v1/#operation/deleteSequences>`_
+        """`Delete one or more sequences. <https://developer.cognite.com/api#tag/Sequences/operation/deleteSequences>`_
 
         Args:
             id (Union[int, SequenceType[int]): Id or list of ids
             external_id (Union[str, SequenceType[str]]): External ID or list of external ids
 
         Returns:
             None
@@ -348,15 +348,15 @@
     @overload
     def update(self, item: SequenceType[Union[Sequence, SequenceUpdate]]) -> SequenceList:
         ...
 
     def update(
         self, item: Union[Sequence, SequenceUpdate, SequenceType[Union[Sequence, SequenceUpdate]]]
     ) -> Union[Sequence, SequenceList]:
-        """`Update one or more sequences. <https://docs.cognite.com/api/v1/#operation/updateSequences>`_
+        """`Update one or more sequences. <https://developer.cognite.com/api#tag/Sequences/operation/updateSequences>`_
 
         Args:
             item (Union[Sequence, SequenceUpdate, SequenceType[Union[Sequence, SequenceUpdate]]]): Sequences to update
 
         Returns:
             Union[Sequence, SequenceList]: Updated sequences.
 
@@ -440,15 +440,15 @@
         self,
         name: str = None,
         description: str = None,
         query: str = None,
         filter: Union[SequenceFilter, Dict] = None,
         limit: int = 100,
     ) -> SequenceList:
-        """`Search for sequences. <https://docs.cognite.com/api/v1/#operation/searchSequences>`_
+        """`Search for sequences. <https://developer.cognite.com/api#tag/Sequences/operation/searchSequences>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             name (str, optional): Prefix and fuzzy search on name.
             description (str, optional): Prefix and fuzzy search on description.
             query (str, optional): Search on name and description using wildcard search on each of the words (separated
                 by spaces). Retrieves results where at least one word must match. Example: 'some other'
@@ -491,15 +491,15 @@
             SequenceType[Dict[str, Any]],
             SequenceData,
         ],
         column_external_ids: Optional[SequenceType[str]],
         id: int = None,
         external_id: str = None,
     ) -> None:
-        """`Insert rows into a sequence <https://docs.cognite.com/api/v1/#operation/postSequenceData>`_
+        """`Insert rows into a sequence <https://developer.cognite.com/api#tag/Sequences/operation/postSequenceData>`_
 
         Args:
             column_external_ids (Optional[SequenceType[str]]): List of external id for the columns of the sequence.
             rows (Union[ Dict[int, SequenceType[Union[int, float, str]]], SequenceType[Tuple[int, SequenceType[Union[int, float, str]]]], SequenceType[Dict[str,Any]], SequenceData]):  The rows you wish to insert.
                 Can either be a list of tuples, a list of {"rowNumber":... ,"values": ...} objects, a dictionary of rowNumber: data, or a SequenceData object. See examples below.
             id (int): Id of sequence to insert rows into.
             external_id (str): External id of sequence to insert rows into.
@@ -562,15 +562,15 @@
 
         row_objs = [{"rows": all_rows[i : i + rows_per_request]} for i in range(0, len(all_rows), rows_per_request)]
         tasks = [({**base_obj, **rows},) for rows in row_objs]  # type: ignore
         summary = utils._concurrency.execute_tasks(self._insert_data, tasks, max_workers=self._config.max_workers)
         summary.raise_compound_exception_if_failed_tasks()
 
     def insert_dataframe(self, dataframe: pandas.DataFrame, id: int = None, external_id: str = None) -> None:
-        """`Insert a Pandas dataframe. <https://docs.cognite.com/api/v1/#operation/postSequenceData>`_
+        """`Insert a Pandas dataframe. <https://developer.cognite.com/api#tag/Sequences/operation/postSequenceData>`_
 
         The index of the dataframe must contain the row numbers. The names of the remaining columns specify the column external ids.
         The sequence and columns must already exist.
 
         Args:
             dataframe (pandas.DataFrame):  Pandas DataFrame object containing the sequence data.
             id (int): Id of sequence to insert rows into.
@@ -592,15 +592,15 @@
         column_external_ids = [str(s) for s in dataframe.columns]
         self.insert(rows=data, column_external_ids=column_external_ids, id=id, external_id=external_id)
 
     def _insert_data(self, task: Dict[str, Any]) -> None:
         self._post(url_path=self._DATA_PATH, json={"items": [task]})
 
     def delete(self, rows: SequenceType[int], id: int = None, external_id: str = None) -> None:
-        """`Delete rows from a sequence <https://docs.cognite.com/api/v1/#operation/deleteSequenceData>`_
+        """`Delete rows from a sequence <https://developer.cognite.com/api#tag/Sequences/operation/deleteSequenceData>`_
 
         Args:
             rows (SequenceType[int]): List of row numbers.
             id (int): Id of sequence to delete rows from.
             external_id (str): External id of sequence to delete rows from.
 
         Returns:
@@ -614,15 +614,15 @@
         """
         post_obj = Identifier.of_either(id, external_id).as_dict()
         post_obj["rows"] = rows
 
         self._post(url_path=self._DATA_PATH + "/delete", json={"items": [post_obj]})
 
     def delete_range(self, start: int, end: Union[int, None], id: int = None, external_id: str = None) -> None:
-        """`Delete a range of rows from a sequence. Note this operation is potentially slow, as retrieves each row before deleting. <https://docs.cognite.com/api/v1/#operation/deleteSequenceData>`_
+        """`Delete a range of rows from a sequence. Note this operation is potentially slow, as retrieves each row before deleting. <https://developer.cognite.com/api#tag/Sequences/operation/deleteSequenceData>`_
 
         Args:
             start (int): Row number to start from (inclusive).
             end (Union[int, None]): Upper limit on the row number (exclusive).
                 Set to None or -1 to delete all rows until end of sequence.
             id (int): Id of sequence to delete rows from.
             external_id (str): External id of sequence to delete rows from.
@@ -650,15 +650,15 @@
         start: int,
         end: Union[int, None],
         column_external_ids: Optional[SequenceType[str]] = None,
         external_id: Union[str, SequenceType[str]] = None,
         id: Union[int, SequenceType[int]] = None,
         limit: int = None,
     ) -> Union[SequenceData, SequenceDataList]:
-        """`Retrieve data from a sequence <https://docs.cognite.com/api/v1/#operation/getSequenceData>`_
+        """`Retrieve data from a sequence <https://developer.cognite.com/api#tag/Sequences/operation/getSequenceData>`_
 
         Args:
             start (int): Row number to start from (inclusive).
             end (Union[int, None]): Upper limit on the row number (exclusive). Set to None or -1 to get all rows
                 until end of sequence.
             column_external_ids (Optional[SequenceType[str]]): List of external id for the columns of the sequence. If 'None' is passed, all columns will be retrieved.
             id (int): Id of sequence.
@@ -706,15 +706,15 @@
     def retrieve_latest(
         self,
         id: int = None,
         external_id: str = None,
         column_external_ids: Optional[SequenceType[str]] = None,
         before: int = None,
     ) -> SequenceData:
-        """`Retrieves the last row (i.e the row with the highest row number) in a sequence. <https://docs.cognite.com/api/v1/#operation/getLatestSequenceRow>`_
+        """`Retrieves the last row (i.e the row with the highest row number) in a sequence. <https://developer.cognite.com/api#tag/Sequences/operation/getLatestSequenceRow>`_
 
         Args:
             id (optional, int): Id or list of ids.
             external_id (optional, str): External id or list of external ids.
             column_external_ids: (optional, SequenceType[str]): external ids of columns to include. Omitting wil return all columns.
             before: (optional, int): Get latest datapoint before this row number.
 
@@ -741,15 +741,15 @@
         end: Union[int, None],
         column_external_ids: Optional[List[str]] = None,
         external_id: str = None,
         column_names: str = None,
         id: int = None,
         limit: int = None,
     ) -> pandas.DataFrame:
-        """`Retrieve data from a sequence as a pandas dataframe <https://docs.cognite.com/api/v1/#operation/getSequenceData>`_
+        """`Retrieve data from a sequence as a pandas dataframe <https://developer.cognite.com/api#tag/Sequences/operation/getSequenceData>`_
 
         Args:
             start (int): (inclusive) row number to start from.
             end (Union[int, None]): (exclusive) upper limit on the row number. Set to None or -1 to get all rows
                 until end of sequence.
             column_external_ids (Optional[SequenceType[str]]): List of external id for the columns of the sequence.  If 'None' is passed, all columns will be retrieved.
             id (int): Id of sequence
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.5.0/cognite/client/_api/synthetic_time_series.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         start: Union[int, str, datetime],
         end: Union[int, str, datetime],
         limit: int = None,
         variables: Dict[str, Union[str, TimeSeries]] = None,
         aggregate: str = None,
         granularity: str = None,
     ) -> Union[Datapoints, DatapointsList]:
-        """`Calculate the result of a function on time series. <https://docs.cognite.com/api/v1/#operation/querySyntheticTimeseries>`_
+        """`Calculate the result of a function on time series. <https://developer.cognite.com/api#tag/Synthetic-Time-Series/operation/querySyntheticTimeseries>`_
 
         Args:
             expressions (Union[str, sympy.Expr, Sequence[Union[str, sympy.Expr]]]): Functions to be calculated. Supports both strings and sympy expressions. Strings can have either the API `ts{}` syntax, or contain variable names to be replaced using the `variables` parameter.
             start (Union[int, str, datetime]): Inclusive start.
             end (Union[int, str, datetime]): Exclusive end
             limit (int): Number of datapoints per expression to retrieve.
             variables (Dict[str,Union[str,TimeSeries]]): An optional map of symbol replacements.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/templates.py` & `cognite_sdk-6.5.0/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/three_d.py` & `cognite_sdk-6.5.0/cognite/client/_api/three_d.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 
         Yields:
             ThreeDModel: yields models one by one.
         """
         return cast(Iterator[ThreeDModel], self())
 
     def retrieve(self, id: int) -> Optional[ThreeDModel]:
-        """`Retrieve a 3d model by id <https://docs.cognite.com/api/v1/#operation/get3DModel>`_
+        """`Retrieve a 3d model by id <https://developer.cognite.com/api#tag/3D-Models/operation/get3DModel>`_
 
         Args:
             id (int): Get the model with this id.
 
         Returns:
             ThreeDModel: The requested 3d model.
 
@@ -86,15 +86,15 @@
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.three_d.models.retrieve(id=1)
         """
         return self._retrieve(cls=ThreeDModel, identifier=InternalId(id))
 
     def list(self, published: bool = None, limit: int = LIST_LIMIT_DEFAULT) -> ThreeDModelList:
-        """`List 3d models. <https://docs.cognite.com/api/v1/#operation/get3DModels>`_
+        """`List 3d models. <https://developer.cognite.com/api#tag/3D-Models/operation/get3DModels>`_
 
         Args:
             published (bool): Filter based on whether or not the model has published revisions.
             limit (int): Maximum number of models to retrieve. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
         Returns:
@@ -127,15 +127,15 @@
             resource_cls=ThreeDModel,
             method="GET",
             filter={"published": published},
             limit=limit,
         )
 
     def create(self, name: Union[str, Sequence[str]]) -> Union[ThreeDModel, ThreeDModelList]:
-        """`Create new 3d models. <https://docs.cognite.com/api/v1/#operation/create3DModels>`_
+        """`Create new 3d models. <https://developer.cognite.com/api#tag/3D-Models/operation/create3DModels>`_
 
         Args:
             name (Union[str, Sequence[str]): The name of the 3d model(s) to create.
 
         Returns:
             Union[ThreeDModel, ThreeDModelList]: The created 3d model(s).
 
@@ -153,15 +153,15 @@
         else:
             name_processed = [{"name": n} for n in name]
         return self._create_multiple(list_cls=ThreeDModelList, resource_cls=ThreeDModel, items=name_processed)
 
     def update(
         self, item: Union[ThreeDModel, ThreeDModelUpdate, Sequence[Union[ThreeDModel, ThreeDModelUpdate]]]
     ) -> Union[ThreeDModel, ThreeDModelList]:
-        """`Update 3d models. <https://docs.cognite.com/api/v1/#operation/update3DModels>`_
+        """`Update 3d models. <https://developer.cognite.com/api#tag/3D-Models/operation/update3DModels>`_
 
         Args:
             item (Union[ThreeDModel, ThreeDModelUpdate, Sequence[Union[ThreeDModel, ThreeDModelUpdate]]]): ThreeDModel(s) to update
 
         Returns:
             Union[ThreeDModel, ThreeDModelList]: Updated ThreeDModel(s)
 
@@ -185,15 +185,15 @@
 
         """
         return self._update_multiple(
             list_cls=ThreeDModelList, resource_cls=ThreeDModel, update_cls=ThreeDModelUpdate, items=item
         )
 
     def delete(self, id: Union[int, Sequence[int]]) -> None:
-        """`Delete 3d models. <https://docs.cognite.com/api/v1/#operation/delete3DModels>`_
+        """`Delete 3d models. <https://developer.cognite.com/api#tag/3D-Models/operation/delete3DModels>`_
 
         Args:
             id (Union[int, Sequence[int]]): ID or list of IDs to delete.
 
         Returns:
             None
 
@@ -235,15 +235,15 @@
             method="GET",
             chunk_size=chunk_size,
             filter={"published": published},
             limit=limit,
         )
 
     def retrieve(self, model_id: int, id: int) -> Optional[ThreeDModelRevision]:
-        """`Retrieve a 3d model revision by id <https://docs.cognite.com/api/v1/#operation/get3DRevision>`_
+        """`Retrieve a 3d model revision by id <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/get3DRevision>`_
 
         Args:
             model_id (int): Get the revision under the model with this id.
             id (int): Get the model revision with this id.
 
         Returns:
             Optional[ThreeDModelRevision]: The requested 3d model revision.
@@ -261,15 +261,15 @@
             resource_path=utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, model_id),
             identifier=InternalId(id),
         )
 
     def create(
         self, model_id: int, revision: Union[ThreeDModelRevision, Sequence[ThreeDModelRevision]]
     ) -> Union[ThreeDModelRevision, ThreeDModelRevisionList]:
-        """`Create a revisions for a specified 3d model. <https://docs.cognite.com/api/v1/#operation/create3DRevisions>`_
+        """`Create a revisions for a specified 3d model. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/create3DRevisions>`_
 
         Args:
             model_id (int): Create revisions for this model.
             revision (Union[ThreeDModelRevision, Sequence[ThreeDModelRevision]]): The revision(s) to create.
 
         Returns:
             Union[ThreeDModelRevision, ThreeDModelRevisionList]: The created revision(s)
@@ -288,15 +288,15 @@
             list_cls=ThreeDModelRevisionList,
             resource_cls=ThreeDModelRevision,
             resource_path=utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, model_id),
             items=revision,
         )
 
     def list(self, model_id: int, published: bool = False, limit: int = LIST_LIMIT_DEFAULT) -> ThreeDModelRevisionList:
-        """`List 3d model revisions. <https://docs.cognite.com/api/v1/#operation/get3DRevisions>`_
+        """`List 3d model revisions. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/get3DRevisions>`_
 
         Args:
             model_id (int): List revisions under the model with this id.
             published (bool): Filter based on whether or not the revision is published.
             limit (int): Maximum number of models to retrieve. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
 
@@ -325,15 +325,15 @@
         model_id: int,
         item: Union[
             ThreeDModelRevision,
             ThreeDModelRevisionUpdate,
             Sequence[Union[ThreeDModelRevision, ThreeDModelRevisionUpdate]],
         ],
     ) -> Union[ThreeDModelRevision, ThreeDModelRevisionList]:
-        """`Update 3d model revisions. <https://docs.cognite.com/api/v1/#operation/update3DRevisions>`_
+        """`Update 3d model revisions. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/update3DRevisions>`_
 
         Args:
             model_id (int): Update the revision under the model with this id.
             item (Union[ThreeDModelRevision, ThreeDModelRevisionUpdate, Sequence[Union[ThreeDModelRevision, ThreeDModelRevisionUpdate]]]):
                 ThreeDModelRevision(s) to update
 
         Returns:
@@ -362,15 +362,15 @@
             resource_cls=ThreeDModelRevision,
             update_cls=ThreeDModelRevisionUpdate,
             resource_path=utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, model_id),
             items=item,
         )
 
     def delete(self, model_id: int, id: Union[int, Sequence[int]]) -> None:
-        """`Delete 3d model revisions. <https://docs.cognite.com/api/v1/#operation/delete3DRevisions>`_
+        """`Delete 3d model revisions. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/delete3DRevisions>`_
 
         Args:
             model_id (int): Delete the revision under the model with this id.
             id (Union[int, Sequence[int]]): ID or list of IDs to delete.
 
         Returns:
             None
@@ -386,15 +386,15 @@
         self._delete_multiple(
             resource_path=utils._auxiliary.interpolate_and_url_encode(self._RESOURCE_PATH, model_id),
             identifiers=IdentifierSequence.load(ids=id),
             wrap_ids=True,
         )
 
     def update_thumbnail(self, model_id: int, revision_id: int, file_id: int) -> None:
-        """`Update a revision thumbnail. <https://docs.cognite.com/api/v1/#operation/updateThumbnail>`_
+        """`Update a revision thumbnail. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/updateThumbnail>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
             file_id (int): Id of the thumbnail file in the Files API.
 
         Returns:
@@ -420,15 +420,15 @@
         revision_id: int,
         node_id: int = None,
         depth: int = None,
         sort_by_node_id: bool = False,
         partitions: int = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> ThreeDNodeList:
-        """`Retrieves a list of nodes from the hierarchy in the 3D Model. <https://docs.cognite.com/api/v1/#operation/get3DNodes>`_
+        """`Retrieves a list of nodes from the hierarchy in the 3D Model. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/get3DNodes>`_
 
         You can also request a specific subtree with the 'nodeId' query parameter and limit the depth of
         the resulting subtree with the 'depth' query parameter.
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
@@ -468,15 +468,15 @@
         self,
         model_id: int,
         revision_id: int,
         properties: Dict[str, Dict[str, Sequence[str]]] = None,
         limit: int = LIST_LIMIT_DEFAULT,
         partitions: int = None,
     ) -> ThreeDNodeList:
-        """`List nodes in a revision, filtered by node property values. <https://docs.cognite.com/api/v1/#operation/filter3DNodes>`_
+        """`List nodes in a revision, filtered by node property values. <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/filter3DNodes>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
             properties (Dict[str, Dict[str, Sequence[str]]]): Properties for filtering. The object contains one or more category. Each category references one or more properties. Each property is associated with a list of values. For a node to satisfy the filter, it must, for each category/property in the filter, contain the catogery+property combination with a value that is contained within the corresponding list in the filter.
             limit (int): Maximun number of nodes to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
@@ -505,15 +505,15 @@
             filter={"properties": properties},
             partitions=partitions,
         )
 
     def list_ancestor_nodes(
         self, model_id: int, revision_id: int, node_id: int = None, limit: int = LIST_LIMIT_DEFAULT
     ) -> ThreeDNodeList:
-        """`Retrieves a list of ancestor nodes of a given node, including itself, in the hierarchy of the 3D model <https://docs.cognite.com/api/v1/#operation/get3DNodeAncestors>`_
+        """`Retrieves a list of ancestor nodes of a given node, including itself, in the hierarchy of the 3D model <https://developer.cognite.com/api#tag/3D-Model-Revisions/operation/get3DNodeAncestors>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
             node_id (int): ID of the node to get the ancestors of.
             limit (int): Maximun number of nodes to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
@@ -542,15 +542,15 @@
         )
 
 
 class ThreeDFilesAPI(APIClient):
     _RESOURCE_PATH = "/3d/files"
 
     def retrieve(self, id: int) -> bytes:
-        """`Retrieve the contents of a 3d file by id. <https://docs.cognite.com/api/v1/#operation/get3DFile>`_
+        """`Retrieve the contents of a 3d file by id. <https://developer.cognite.com/api#tag/3D-Files/operation/get3DFile>`_
 
         Args:
             id (int): The id of the file to retrieve.
 
         Returns:
             bytes: The contents of the file.
 
@@ -573,15 +573,15 @@
         self,
         model_id: int,
         revision_id: int,
         node_id: int = None,
         asset_id: int = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> ThreeDAssetMappingList:
-        """`List 3D node asset mappings. <https://docs.cognite.com/api/v1/#operation/get3DMappings>`_
+        """`List 3D node asset mappings. <https://developer.cognite.com/api#tag/3D-Asset-Mapping/operation/get3DMappings>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
             node_id (int): List only asset mappings associated with this node.
             asset_id (int): List only asset mappings associated with this asset.
             limit (int): Maximum number of asset mappings to return. Defaults to 25. Set to -1, float("inf") or None
@@ -607,15 +607,15 @@
             filter={"nodeId": node_id, "assetId": asset_id},
             limit=limit,
         )
 
     def create(
         self, model_id: int, revision_id: int, asset_mapping: Union[ThreeDAssetMapping, Sequence[ThreeDAssetMapping]]
     ) -> Union[ThreeDAssetMapping, ThreeDAssetMappingList]:
-        """`Create 3d node asset mappings. <https://docs.cognite.com/api/v1/#operation/create3DMappings>`_
+        """`Create 3d node asset mappings. <https://developer.cognite.com/api#tag/3D-Asset-Mapping/operation/create3DMappings>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
             asset_mapping (Union[ThreeDAssetMapping, Sequence[ThreeDAssetMapping]]): The asset mapping(s) to create.
 
         Returns:
@@ -635,15 +635,15 @@
         return self._create_multiple(
             list_cls=ThreeDAssetMappingList, resource_cls=ThreeDAssetMapping, resource_path=path, items=asset_mapping
         )
 
     def delete(
         self, model_id: int, revision_id: int, asset_mapping: Union[ThreeDAssetMapping, Sequence[ThreeDAssetMapping]]
     ) -> None:
-        """`Delete 3d node asset mappings. <https://docs.cognite.com/api/v1/#operation/delete3DMappings>`_
+        """`Delete 3d node asset mappings. <https://developer.cognite.com/api#tag/3D-Asset-Mapping/operation/delete3DMappings>`_
 
         Args:
             model_id (int): Id of the model.
             revision_id (int): Id of the revision.
             asset_mapping (Union[ThreeDAssetMapping, Sequence[ThreeDAssetMapping]]): The asset mapping(s) to delete.
 
         Returns:
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/time_series.py` & `cognite_sdk-6.5.0/cognite/client/_api/time_series.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
         Yields:
             TimeSeries: yields TimeSeries one by one.
         """
         return cast(Iterator[TimeSeries], self())
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[TimeSeries]:
-        """`Retrieve a single time series by id. <https://docs.cognite.com/api/v1/#operation/getTimeSeriesByIds>`_
+        """`Retrieve a single time series by id. <https://developer.cognite.com/api#tag/Time-series/operation/getTimeSeriesByIds>`_
 
         Args:
             id (int, optional): ID
             external_id (str, optional): External ID
 
         Returns:
             Optional[TimeSeries]: Requested time series or None if it does not exist.
@@ -139,15 +139,15 @@
 
     def retrieve_multiple(
         self,
         ids: Optional[Sequence[int]] = None,
         external_ids: Optional[Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> TimeSeriesList:
-        """`Retrieve multiple time series by id. <https://docs.cognite.com/api/v1/#operation/getTimeSeriesByIds>`_
+        """`Retrieve multiple time series by id. <https://developer.cognite.com/api#tag/Time-series/operation/getTimeSeriesByIds>`_
 
         Args:
             ids (Sequence[int], optional): IDs
             external_ids (Sequence[str], optional): External IDs
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -190,15 +190,15 @@
         metadata: Dict[str, Any] = None,
         external_id_prefix: str = None,
         created_time: Dict[str, Any] = None,
         last_updated_time: Dict[str, Any] = None,
         partitions: int = None,
         limit: int = LIST_LIMIT_DEFAULT,
     ) -> TimeSeriesList:
-        """`List over time series <https://docs.cognite.com/api/v1/#operation/listTimeSeries>`_
+        """`List over time series <https://developer.cognite.com/api#tag/Time-series/operation/listTimeSeries>`_
 
         Fetches time series as they are iterated over, so you keep a limited number of objects in memory.
 
         Args:
             name (str): Name of the time series. Often referred to as tag.
             unit (str): Unit of the time series.
             is_string (bool): Whether the time series is an string time series.
@@ -265,15 +265,15 @@
             method="POST",
             filter=filter,
             limit=limit,
             partitions=partitions,
         )
 
     def aggregate(self, filter: Union[TimeSeriesFilter, Dict] = None) -> List[TimeSeriesAggregate]:
-        """`Aggregate time series <https://docs.cognite.com/api/v1/#operation/aggregateTimeSeries>`_
+        """`Aggregate time series <https://developer.cognite.com/api#tag/Time-series/operation/aggregateTimeSeries>`_
 
         Args:
             filter (Union[TimeSeriesFilter, Dict]): Filter on time series filter with exact match
 
         Returns:
             List[TimeSeriesAggregate]: List of sequence aggregates
 
@@ -293,15 +293,15 @@
         ...
 
     @overload
     def create(self, time_series: TimeSeries) -> TimeSeries:
         ...
 
     def create(self, time_series: Union[TimeSeries, Sequence[TimeSeries]]) -> Union[TimeSeries, TimeSeriesList]:
-        """`Create one or more time series. <https://docs.cognite.com/api/v1/#operation/postTimeSeries>`_
+        """`Create one or more time series. <https://developer.cognite.com/api#tag/Time-series/operation/postTimeSeries>`_
 
         Args:
             time_series (Union[TimeSeries, Sequence[TimeSeries]]): TimeSeries or list of TimeSeries to create.
 
         Returns:
             Union[TimeSeries, TimeSeriesList]: The created time series.
 
@@ -318,15 +318,15 @@
 
     def delete(
         self,
         id: Union[int, Sequence[int]] = None,
         external_id: Union[str, Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> None:
-        """`Delete one or more time series. <https://docs.cognite.com/api/v1/#operation/deleteTimeSeries>`_
+        """`Delete one or more time series. <https://developer.cognite.com/api#tag/Time-series/operation/deleteTimeSeries>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -353,15 +353,15 @@
     @overload
     def update(self, item: Union[TimeSeries, TimeSeriesUpdate]) -> TimeSeries:
         ...
 
     def update(
         self, item: Union[TimeSeries, TimeSeriesUpdate, Sequence[Union[TimeSeries, TimeSeriesUpdate]]]
     ) -> Union[TimeSeries, TimeSeriesList]:
-        """`Update one or more time series. <https://docs.cognite.com/api/v1/#operation/alterTimeSeries>`_
+        """`Update one or more time series. <https://developer.cognite.com/api#tag/Time-series/operation/alterTimeSeries>`_
 
         Args:
             item (Union[TimeSeries, TimeSeriesUpdate, Sequence[Union[TimeSeries, TimeSeriesUpdate]]]): Time series to update
 
         Returns:
             Union[TimeSeries, TimeSeriesList]: Updated time series.
 
@@ -391,15 +391,15 @@
         self,
         name: str = None,
         description: str = None,
         query: str = None,
         filter: Union[TimeSeriesFilter, Dict] = None,
         limit: int = 100,
     ) -> TimeSeriesList:
-        """`Search for time series. <https://docs.cognite.com/api/v1/#operation/searchTimeSeries>`_
+        """`Search for time series. <https://developer.cognite.com/api#tag/Time-series/operation/searchTimeSeries>`_
         Primarily meant for human-centric use-cases and data exploration, not for programs, since matching and ordering may change over time. Use the `list` function if stable or exact matches are required.
 
         Args:
             name (str, optional): Prefix and fuzzy search on name.
             description (str, optional): Prefix and fuzzy search on description.
             query (str, optional): Search on name and description using wildcard search on each of the words (separated
                 by spaces). Retrieves results where at least one word must match. Example: 'some other'
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.5.0/cognite/client/_api/transformations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.schedules = TransformationSchedulesAPI(config, api_version, cognite_client)
         self.schema = TransformationSchemaAPI(config, api_version, cognite_client)
         self.notifications = TransformationNotificationsAPI(config, api_version, cognite_client)
 
     def create(
         self, transformation: Union[Transformation, Sequence[Transformation]]
     ) -> Union[Transformation, TransformationList]:
-        """`Create one or more transformations. <https://docs.cognite.com/api/v1/#operation/createTransformations>`_
+        """`Create one or more transformations. <https://developer.cognite.com/api#tag/Transformations/operation/createTransformations>`_
 
         Args:
             transformation (Union[Transformation, List[Transformation]]): Transformation or list of transformations to create.
 
         Returns:
             Created transformation(s)
 
@@ -116,15 +116,15 @@
 
     def delete(
         self,
         id: Union[int, Sequence[int]] = None,
         external_id: Union[str, Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> None:
-        """`Delete one or more transformations. <https://docs.cognite.com/api/v1/#operation/deleteTransformations>`_
+        """`Delete one or more transformations. <https://developer.cognite.com/api#tag/Transformations/operation/deleteTransformations>`_
 
         Args:
             id (Union[int, List[int]): Id or list of ids.
             external_id (Union[str, List[str]]): External ID or list of external ids.
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -156,15 +156,15 @@
         created_time: Union[Dict[str, Any], TimestampRange] = None,
         last_updated_time: Union[Dict[str, Any], TimestampRange] = None,
         data_set_ids: List[int] = None,
         data_set_external_ids: List[str] = None,
         tags: Optional[TagsFilter] = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> TransformationList:
-        """`List all transformations. <https://docs.cognite.com/api/v1/#operation/getTransformations>`_
+        """`List all transformations. <https://developer.cognite.com/api#tag/Transformations/operation/getTransformations>`_
 
         Args:
             include_public (bool): Whether public transformations should be included in the results. (default true).
             name_regex (str): Regex expression to match the transformation name
             query_regex (str): Regex expression to match the transformation query
             destination_type (str): Transformation destination resource name to filter by.
             conflict_mode (str): Filters by a selected transformation action type: abort/create, upsert, update, delete
@@ -215,15 +215,15 @@
             method="POST",
             url_path=f"{self._RESOURCE_PATH}/filter",
             limit=limit,
             filter=filter,
         )
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[Transformation]:
-        """`Retrieve a single transformation by id. <https://docs.cognite.com/api/v1/#operation/getTransformationsByIds>`_
+        """`Retrieve a single transformation by id. <https://developer.cognite.com/api#tag/Transformations/operation/getTransformationsByIds>`_
 
         Args:
             id (int, optional): ID
 
         Returns:
             Optional[Transformation]: Requested transformation or None if it does not exist.
 
@@ -247,15 +247,15 @@
             resource_cls=Transformation,
             identifiers=identifiers,
         )
 
     def retrieve_multiple(
         self, ids: Sequence[int] = None, external_ids: Sequence[str] = None, ignore_unknown_ids: bool = False
     ) -> TransformationList:
-        """`Retrieve multiple transformations. <https://docs.cognite.com/api/v1/#operation/getTransformationsByIds>`_
+        """`Retrieve multiple transformations. <https://developer.cognite.com/api#tag/Transformations/operation/getTransformationsByIds>`_
 
         Args:
             ids (List[int]): List of ids to retrieve.
             external_ids (List[str]): List of external ids to retrieve.
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -276,15 +276,15 @@
             identifiers=identifiers,
             ignore_unknown_ids=ignore_unknown_ids,
         )
 
     def update(
         self, item: Union[Transformation, TransformationUpdate, Sequence[Union[Transformation, TransformationUpdate]]]
     ) -> Union[Transformation, TransformationList]:
-        """`Update one or more transformations <https://docs.cognite.com/api/v1/#operation/updateTransformations>`_
+        """`Update one or more transformations <https://developer.cognite.com/api#tag/Transformations/operation/updateTransformations>`_
 
         Args:
             item (Union[Transformation, TransformationUpdate, List[Union[Transformation, TransformationUpdate]]]): Transformation(s) to update
 
         Returns:
             Union[Transformation, TransformationList]: Updated transformation(s)
 
@@ -332,15 +332,15 @@
     def run(
         self,
         transformation_id: int = None,
         transformation_external_id: str = None,
         wait: bool = True,
         timeout: Optional[float] = None,
     ) -> TransformationJob:
-        """`Run a transformation. <https://docs.cognite.com/api/v1/#operation/runTransformation>`_
+        """`Run a transformation. <https://developer.cognite.com/api#tag/Transformations/operation/runTransformation>`_
 
         Args:
             transformation_id (int): Transformation internal id
             transformation_external_id (str): Transformation external id
             wait (bool): Wait until the transformation run is finished. Defaults to True.
             timeout (Optional[float]): maximum time (s) to wait, default is None (infinite time). Once the timeout is reached, it returns with the current status. Won't have any effect if wait is False.
 
@@ -374,15 +374,15 @@
             return job.wait(timeout=timeout)
 
         return job
 
     async def run_async(
         self, transformation_id: int = None, transformation_external_id: str = None, timeout: Optional[float] = None
     ) -> TransformationJob:
-        """`Run a transformation to completion asynchronously. <https://docs.cognite.com/api/v1/#operation/runTransformation>`_
+        """`Run a transformation to completion asynchronously. <https://developer.cognite.com/api#tag/Transformations/operation/runTransformation>`_
 
         Args:
             transformation_id (int): internal Transformation id
             transformation_external_id (str): external Transformation id
             timeout (Optional[float]): maximum time (s) to wait, default is None (infinite time). Once the timeout is reached, it returns with the current status.
 
         Returns:
@@ -407,15 +407,15 @@
 
         job = self.run(
             transformation_id=transformation_id, transformation_external_id=transformation_external_id, wait=False
         )
         return await job.wait_async(timeout=timeout)
 
     def cancel(self, transformation_id: int = None, transformation_external_id: str = None) -> None:
-        """`Cancel a running transformation. <https://docs.cognite.com/api/v1/#operation/cancelTransformation>`_
+        """`Cancel a running transformation. <https://developer.cognite.com/api#tag/Transformations/operation/cancelTransformation>`_
 
         Args:
             transformation_id (int): Transformation internal id
             transformation_external_id (str): Transformation external id
 
         Examples:
 
@@ -439,15 +439,15 @@
         self,
         query: str = None,
         convert_to_string: bool = False,
         limit: int = 100,
         source_limit: Optional[int] = 100,
         infer_schema_limit: Optional[int] = 1000,
     ) -> TransformationPreviewResult:
-        """`Preview the result of a query. <https://docs.cognite.com/api/v1/#operation/runPreview>`_
+        """`Preview the result of a query. <https://developer.cognite.com/api#tag/Transformations/operation/runPreview>`_
 
         Args:
             query (str): SQL query to run for preview.
             convert_to_string (bool): Stringify values in the query results, default is False.
             limit (int): Maximum number of rows to return in the final result, default is 100.
             source_limit (Union[int,str]): Maximum number of items to read from the data source or None to run without limit, default is 100.
             infer_schema_limit: Limit for how many rows that are used for inferring result schema, default is 1000.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.5.0/cognite/client/_api/transformations/jobs.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
     def list(
         self,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
         transformation_id: Optional[int] = None,
         transformation_external_id: Optional[str] = None,
     ) -> TransformationJobList:
-        """`List all running transformation jobs. <https://docs.cognite.com/api/v1/#operation/getTransformationJobs>`_
+        """`List all running transformation jobs. <https://developer.cognite.com/api#tag/Transformation-Jobs/operation/getTransformationJobs>`_
 
         Args:
             limit (int): Limits the number of results to be returned. To retrieve all results use limit=-1, default limit is 25.
             transformation_id (int): Filters the results by the internal transformation id.
             transformation_external_id (str): Filters the results by the external transformation id.
 
         Returns:
@@ -54,15 +54,15 @@
         ).dump(camel_case=True)
 
         return self._list(
             list_cls=TransformationJobList, resource_cls=TransformationJob, method="GET", limit=limit, filter=filter
         )
 
     def retrieve(self, id: int) -> Optional[TransformationJob]:
-        """`Retrieve a single transformation job by id. <https://docs.cognite.com/api/v1/#operation/getTransformationJobsByIds>`_
+        """`Retrieve a single transformation job by id. <https://developer.cognite.com/api#tag/Transformation-Jobs/operation/getTransformationJobsByIds>`_
 
         Args:
             id (int): Job internal Id
 
         Returns:
             Optional[TransformationJob]: Requested transformation job or None if it does not exist.
 
@@ -76,15 +76,15 @@
         """
         identifiers = IdentifierSequence.load(ids=id, external_ids=None).as_singleton()
         return self._retrieve_multiple(
             list_cls=TransformationJobList, resource_cls=TransformationJob, identifiers=identifiers
         )
 
     def list_metrics(self, id: int) -> TransformationJobMetricList:
-        """`List the metrics of a single transformation job. <https://docs.cognite.com/api/v1/#operation/getTransformationJobsMetrics>`_
+        """`List the metrics of a single transformation job. <https://developer.cognite.com/api#tag/Transformation-Jobs/operation/getTransformationJobsMetrics>`_
 
         Args:
             id (int): Job internal Id
 
         Returns:
             TransformationJobMetricList: List of updated metrics of the given job.
 
@@ -103,15 +103,15 @@
             resource_cls=TransformationJobMetric,
             method="GET",
             limit=None,
             resource_path=url_path,
         )
 
     def retrieve_multiple(self, ids: Sequence[int], ignore_unknown_ids: bool = False) -> TransformationJobList:
-        """`Retrieve multiple transformation jobs by id. <https://docs.cognite.com/api/v1/#operation/getTransformationJobsByIds>`_
+        """`Retrieve multiple transformation jobs by id. <https://developer.cognite.com/api#tag/Transformation-Jobs/operation/getTransformationJobsByIds>`_
 
         Args:
             ids (Sequence[int]): Job internal Ids
             ignore_unknown_ids (bool): Ignore IDs that are not found rather than throw an exception.
 
         Returns:
             TransformationJobList: Requested transformation jobs.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.5.0/cognite/client/_api/transformations/notifications.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 class TransformationNotificationsAPI(APIClient):
     _RESOURCE_PATH = "/transformations/notifications"
 
     def create(
         self, notification: Union[TransformationNotification, Sequence[TransformationNotification]]
     ) -> Union[TransformationNotification, TransformationNotificationList]:
-        """`Subscribe for notifications on the transformation errors. <https://docs.cognite.com/api/v1/#operation/createTransformationNotifications>`_
+        """`Subscribe for notifications on the transformation errors. <https://developer.cognite.com/api#tag/Transformation-Notifications/operation/createTransformationNotifications>`_
 
         Args:
             notification (Union[TransformationNotification, Sequence[TransformationNotification]]): Notification or list of notifications to create.
 
         Returns:
             Created notification(s)
 
@@ -42,15 +42,15 @@
     def list(
         self,
         transformation_id: Optional[int] = None,
         transformation_external_id: str = None,
         destination: str = None,
         limit: Optional[int] = LIST_LIMIT_DEFAULT,
     ) -> TransformationNotificationList:
-        """`List notification subscriptions. <https://docs.cognite.com/api/v1/#operation/getTransformationNotifications>`_
+        """`List notification subscriptions. <https://developer.cognite.com/api#tag/Transformation-Notifications/operation/getTransformationNotifications>`_
 
         Args:
             transformation_id (Optional[int]): Filter by transformation internal numeric ID.
             transformation_external_id (str): Filter by transformation externalId.
             destination (str): Filter by notification destination.
             limit (int): Limits the number of results to be returned. To retrieve all results use limit=-1, default limit is 25.
 
@@ -82,15 +82,15 @@
             resource_cls=TransformationNotification,
             method="GET",
             limit=limit,
             filter=filter,
         )
 
     def delete(self, id: Union[int, Sequence[int]] = None) -> None:
-        """`Deletes the specified notification subscriptions on the transformation. Does nothing when the subscriptions already don't exist <https://docs.cognite.com/api/v1/#operation/deleteTransformationNotifications>`_
+        """`Deletes the specified notification subscriptions on the transformation. Does nothing when the subscriptions already don't exist <https://developer.cognite.com/api#tag/Transformation-Notifications/operation/deleteTransformationNotifications>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of transformation notification ids
 
         Returns:
             None
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.5.0/cognite/client/_api/transformations/schedules.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self._CREATE_LIMIT = 5
         self._DELETE_LIMIT = 5
         self._UPDATE_LIMIT = 5
 
     def create(
         self, schedule: Union[TransformationSchedule, Sequence[TransformationSchedule]]
     ) -> Union[TransformationSchedule, TransformationScheduleList]:
-        """`Schedule the specified transformation with the specified configuration(s). <https://docs.cognite.com/api/v1/#operation/createTransformationSchedules>`_
+        """`Schedule the specified transformation with the specified configuration(s). <https://developer.cognite.com/api#tag/Transformation-Schedules/operation/createTransformationSchedules>`_
 
         Args:
             schedule (Union[TransformationSchedule, Sequence[TransformationSchedule]]): Configuration or list of configurations of the schedules to create.
 
         Returns:
             Created schedule(s)
 
@@ -46,15 +46,15 @@
         """
         utils._auxiliary.assert_type(schedule, "schedule", [TransformationSchedule, list])
         return self._create_multiple(
             list_cls=TransformationScheduleList, resource_cls=TransformationSchedule, items=schedule
         )
 
     def retrieve(self, id: Optional[int] = None, external_id: Optional[str] = None) -> Optional[TransformationSchedule]:
-        """`Retrieve a single transformation schedule by the id or external id of its transformation. <https://docs.cognite.com/api/v1/#operation/getTransformationSchedulesByIds>`_
+        """`Retrieve a single transformation schedule by the id or external id of its transformation. <https://developer.cognite.com/api#tag/Transformation-Schedules/operation/getTransformationSchedulesByIds>`_
 
         Args:
             id (int, optional): transformation ID
             external_id (str, optional): transformation External ID
 
         Returns:
             Optional[TransformationSchedule]: Requested transformation schedule or None if it does not exist.
@@ -80,15 +80,15 @@
 
     def retrieve_multiple(
         self,
         ids: Optional[Sequence[int]] = None,
         external_ids: Optional[Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> TransformationScheduleList:
-        """`Retrieve multiple transformation schedules by the ids or external ids of the corresponding transformations. <https://docs.cognite.com/api/v1/#operation/getTransformationSchedulesByIds>`_
+        """`Retrieve multiple transformation schedules by the ids or external ids of the corresponding transformations. <https://developer.cognite.com/api#tag/Transformation-Schedules/operation/getTransformationSchedulesByIds>`_
 
         Args:
             ids (int, optional): transformation IDs
             external_ids (str, optional): transformation External IDs
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -115,15 +115,15 @@
             identifiers=identifiers,
             ignore_unknown_ids=ignore_unknown_ids,
         )
 
     def list(
         self, include_public: bool = True, limit: Optional[int] = LIST_LIMIT_DEFAULT
     ) -> TransformationScheduleList:
-        """`List all transformation schedules. <https://docs.cognite.com/api/v1/#operation/getTransformationSchedules>`_
+        """`List all transformation schedules. <https://developer.cognite.com/api#tag/Transformation-Schedules/operation/getTransformationSchedules>`_
 
         Args:
             include_public (bool): Whether public transformations should be included in the results. (default true).
             cursor (str): Cursor for paging through results.
             limit (int): Limits the number of results to be returned. To retrieve all results use limit=-1, default limit is 25.
 
         Returns:
@@ -149,15 +149,15 @@
 
     def delete(
         self,
         id: Union[int, Sequence[int]] = None,
         external_id: Union[str, Sequence[str]] = None,
         ignore_unknown_ids: bool = False,
     ) -> None:
-        """`Unschedule one or more transformations <https://docs.cognite.com/api/v1/#operation/deleteTransformationSchedules>`_
+        """`Unschedule one or more transformations <https://developer.cognite.com/api#tag/Transformation-Schedules/operation/deleteTransformationSchedules>`_
 
         Args:
             id (Union[int, Sequence[int]): Id or list of ids
             external_id (Union[str, Sequence[str]]): External ID or list of external ids
             ignore_unknown_ids (bool): Ignore IDs and external IDs that are not found rather than throw an exception.
 
         Returns:
@@ -181,15 +181,15 @@
         self,
         item: Union[
             TransformationSchedule,
             TransformationScheduleUpdate,
             Sequence[Union[TransformationSchedule, TransformationScheduleUpdate]],
         ],
     ) -> Union[TransformationSchedule, TransformationScheduleList]:
-        """`Update one or more transformation schedules <https://docs.cognite.com/api/v1/#operation/updateTransformationSchedules>`_
+        """`Update one or more transformation schedules <https://developer.cognite.com/api#tag/Transformation-Schedules/operation/updateTransformationSchedules>`_
 
         Args:
             item (Union[TransformationSchedule, TransformationScheduleUpdate, Sequence[Union[TransformationSchedule, TransformationScheduleUpdate]]]): Transformation schedule(s) to update
 
         Returns:
             Union[TransformationSchedule, TransformationScheduleList]: Updated transformation schedule(s)
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.5.0/cognite/client/_api/transformations/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class TransformationSchemaAPI(APIClient):
     _RESOURCE_PATH = "/transformations/schema"
 
     def retrieve(
         self, destination: TransformationDestination, conflict_mode: Optional[str] = None
     ) -> TransformationSchemaColumnList:
-        """`Get expected schema for a transformation destination. <https://docs.cognite.com/api/v1/#operation/getTransformationSchema>`_
+        """`Get expected schema for a transformation destination. <https://developer.cognite.com/api#tag/Schema/operation/getTransformationSchema>`_
 
         Args:
             destination (TransformationDestination): destination for which the schema is requested.
             conflict_mode (Optional[str]): conflict mode for which the schema is requested.
 
         Returns:
             TransformationSchemaColumnList: List of column descriptions
```

### Comparing `cognite_sdk-6.4.8/cognite/client/_api/vision.py` & `cognite_sdk-6.5.0/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_api_client.py` & `cognite_sdk-6.5.0/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_cognite_client.py` & `cognite_sdk-6.5.0/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_http_client.py` & `cognite_sdk-6.5.0/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.5.0/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.5.0/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.5.0/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.5.0/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.5.0/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/config.py` & `cognite_sdk-6.5.0/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/credentials.py` & `cognite_sdk-6.5.0/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/_base.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/assets.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from cognite.client.data_classes.data_modeling import filters
+from cognite.client.data_classes.data_modeling import aggregations, filters
+from cognite.client.data_classes.data_modeling.aggregations import AggregatedValue, Aggregation
 from cognite.client.data_classes.data_modeling.containers import (
     Constraint,
     Container,
     ContainerApply,
     ContainerApplyList,
-    ContainerDirectRelation,
     ContainerFilter,
     ContainerList,
     ContainerProperty,
     Index,
     RequiresConstraintDefinition,
     UniquenessConstraintDefinition,
 )
@@ -69,50 +69,62 @@
     NodeApplyResultList,
     NodeList,
     NodeOrEdgeData,
 )
 from cognite.client.data_classes.data_modeling.spaces import Space, SpaceApply, SpaceApplyList, SpaceList
 from cognite.client.data_classes.data_modeling.views import (
     ConnectionDefinition,
-    MappedApplyPropertyDefinition,
-    MappedPropertyDefinition,
+    MappedProperty,
+    MappedPropertyApply,
     SingleHopConnectionDefinition,
     View,
     ViewApply,
     ViewApplyList,
     ViewFilter,
     ViewList,
-    ViewPropertyDefinition,
 )
 
+# TODO: Remove these in next major version, there just here to ensure backwards compatibility after renaming and
+#  removing some data classes.
+ViewDirectRelation = DirectRelation
+ContainerDirectRelation = DirectRelation
+MapppedPropertyDefinition = MappedProperty
+MappedApplyPropertyDefinition = MappedPropertyApply
+
 __all__ = [
+    "Aggregation",
+    "AggregatedValue",
+    "aggregations",
     "ViewIdentifier",
     "ViewApply",
     "ViewApplyList",
+    "MappedPropertyApply",
     "MappedApplyPropertyDefinition",
     "VersionedDataModelingId",
     "DataModelingId",
     "ContainerIdentifier",
     "DataModelIdentifier",
     "filters",
     "DirectRelation",
+    "ViewDirectRelation",
+    "ContainerDirectRelation",
     "Filter",
     "DirectRelationReference",
     "DataModel",
     "DataModelList",
     "DataModelsSort",
     "DataModelFilter",
     "DataModelApply",
     "DataModelApplyList",
     "ContainerFilter",
     "ViewFilter",
-    "MappedPropertyDefinition",
+    "MappedProperty",
+    "MapppedPropertyDefinition",
     "ConnectionDefinition",
     "SingleHopConnectionDefinition",
-    "ViewPropertyDefinition",
     "Space",
     "SpaceList",
     "SpaceApply",
     "SpaceApplyList",
     "View",
     "ViewList",
     "Container",
@@ -120,15 +132,14 @@
     "ContainerApply",
     "ContainerApplyList",
     "Index",
     "Constraint",
     "ContainerProperty",
     "Primitive",
     "CDFExternalIdReference",
-    "ContainerDirectRelation",
     "RequiresConstraintDefinition",
     "UniquenessConstraintDefinition",
     "ContainerId",
     "ViewId",
     "DataModelId",
     "Text",
     "Boolean",
```

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -185,46 +185,28 @@
 
     def __init__(self, space: str = None, include_global: bool = False):
         self.space = space
         self.include_global = include_global
 
 
 @dataclass
-class ContainerDirectRelation(DirectRelation):
-    container: Optional[ContainerId] = None
-
-    def dump(self, camel_case: bool = False) -> dict:
-        output = super().dump(camel_case)
-        if "container" in output and isinstance(output["container"], dict):
-            output["container"]["type"] = "container"
-        return output
-
-    @classmethod
-    def load(cls, data: dict) -> ContainerDirectRelation:
-        output = cls(**convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"type"})))
-        if isinstance(data.get("container"), dict):
-            output.container = ContainerId.load(data["container"])
-        return output
-
-
-@dataclass
 class ContainerProperty:
-    type: PropertyType | ContainerDirectRelation
+    type: PropertyType
     nullable: bool = True
     auto_increment: bool = False
     name: Optional[str] = None
     default_value: str | int | dict | None = None
     description: str | None = None
 
     @classmethod
     def load(cls, data: dict[str, Any]) -> ContainerProperty:
         if "type" not in data:
             raise ValueError("Type not specified")
         if data["type"].get("type") == "direct":
-            data["type"] = ContainerDirectRelation.load(data["type"])
+            data["type"] = DirectRelation.load(data["type"])
         else:
             data["type"] = PropertyType.load(data["type"])
         return cls(**convert_all_keys_to_snake_case(data))
 
     def dump(self, camel_case: bool = False) -> dict[str, str | dict]:
         output = asdict(self)
         if "type" in output and isinstance(output["type"], dict):
```

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from abc import ABC
 from dataclasses import asdict, dataclass
-from typing import ClassVar
+from typing import ClassVar, Optional
 
+from cognite.client.data_classes.data_modeling.ids import ContainerId
 from cognite.client.utils._auxiliary import rename_and_exclude_keys
 from cognite.client.utils._text import convert_all_keys_recursive, convert_all_keys_to_snake_case
 
 _PROPERTY_ALIAS = {"list": "isList"}
 _PROPERTY_ALIAS_INV = {"isList": "list", "is_list": "list"}
 
 
@@ -71,15 +72,15 @@
         elif type_ == "timeseries":
             return TimeSeriesReference(**data)
         elif type_ == "file":
             return FileReference(**data)
         elif type_ == "sequence":
             return SequenceReference(**data)
         elif type_ == "direct":
-            return DirectRelation()
+            return DirectRelation(**data)
 
         raise ValueError(f"Invalid type {type_}.")
 
 
 @dataclass
 class ListablePropertyType(PropertyType):
     _type = "listable"
@@ -156,7 +157,21 @@
 class SequenceReference(CDFExternalIdReference):
     _type = "sequence"
 
 
 @dataclass
 class DirectRelation(PropertyType):
     _type = "direct"
+    container: Optional[ContainerId] = None
+
+    def dump(self, camel_case: bool = False) -> dict:
+        output = super().dump(camel_case)
+        if "container" in output and isinstance(output["container"], dict):
+            output["container"]["type"] = "container"
+        return output
+
+    @classmethod
+    def load(cls, data: dict) -> DirectRelation:
+        output = cls(**convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"type"})))
+        if isinstance(data.get("container"), dict):
+            output.container = ContainerId.load(data["container"])
+        return output
```

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/ids.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/instances.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteResourceList,
 )
 from cognite.client.data_classes.data_modeling._core import DataModelingResource
 from cognite.client.data_classes.data_modeling._validation import validate_data_modeling_identifier
+from cognite.client.data_classes.data_modeling.aggregations import AggregatedNumberedValue
 from cognite.client.data_classes.data_modeling.data_types import (
     DirectRelationReference,
 )
 from cognite.client.data_classes.data_modeling.ids import (
     ContainerId,
     ContainerIdentifier,
     EdgeId,
@@ -301,14 +302,67 @@
         super().__init__(space, external_id, instance_type)
         self.version = version
         self.was_modified = was_modified
         self.last_updated_time = last_updated_time
         self.created_time = created_time
 
 
+class InstanceAggregationResult(DataModelingResource):
+    """A node or edge. This represents the update on the instance.
+
+    Args:
+        aggregates (list[AggregatedNumberedValue]) : List of aggregated values.
+        group (dict[str, str | int | float | bool]) : The grouping used for the aggregation.
+    """
+
+    def __init__(self, aggregates: list[AggregatedNumberedValue], group: dict[str, str | int | float | bool]):
+        self.aggregates = aggregates
+        self.group = group
+
+    @classmethod
+    def load(cls, data: dict | str) -> InstanceAggregationResult:
+        """
+        Loads an instance from a json string or dictionary.
+
+        Args:
+            data (dict | str): The json string or dictionary.
+
+        Returns:
+            An instance.
+
+        """
+        data = json.loads(data) if isinstance(data, str) else data
+
+        return cls(
+            aggregates=[AggregatedNumberedValue.load(agg) for agg in data["aggregates"]],
+            group=cast(Dict[str, Union[str, int, float, bool]], data.get("group")),
+        )
+
+    def dump(self, camel_case: bool = False) -> dict[str, Any]:
+        """
+        Dumps the instance to a dictionary.
+
+        Args:
+            camel_case (bool): Whether to convert the keys to camel case.
+
+        Returns:
+            A dictionary.
+
+        """
+        return {
+            "aggregates": [agg.dump(camel_case) for agg in self.aggregates],
+            "group": self.group,
+            ("instanceType" if camel_case else "instance_type"): self.instance_type,
+        }
+
+
+class InstanceAggregationResultList(CogniteResourceList[InstanceAggregationResult]):
+    _RESOURCE = InstanceAggregationResult
+
+
 class NodeApply(InstanceApply):
     """A node. This is the write version of the node.
 
     Args:
         space (str): The workspace for the node.a unique identifier for the space.
         external_id (str): Combined with the space is the unique identifier of the node.
         existing_version (int): Fail the ingestion request if the node's version is greater than or equal to this value.
```

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_modeling/views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 import json
-from abc import ABC
+from abc import ABC, abstractmethod
 from dataclasses import asdict, dataclass
 from typing import Any, Dict, Literal, Optional, Union, cast
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteResourceList,
 )
@@ -14,15 +14,14 @@
 from cognite.client.data_classes.data_modeling.data_types import (
     DirectRelation,
     DirectRelationReference,
     PropertyType,
 )
 from cognite.client.data_classes.data_modeling.filters import Filter
 from cognite.client.data_classes.data_modeling.ids import ContainerId, ViewId
-from cognite.client.utils._auxiliary import rename_and_exclude_keys
 from cognite.client.utils._text import (
     convert_all_keys_to_camel_case_recursive,
     convert_all_keys_to_snake_case,
 )
 
 
 class ViewCore(DataModelingResource):
@@ -92,24 +91,24 @@
         space: str,
         external_id: str,
         version: str,
         description: str = None,
         name: str = None,
         filter: Filter | None = None,
         implements: list[ViewId] = None,
-        properties: dict[str, MappedApplyPropertyDefinition | ConnectionDefinition] = None,
+        properties: dict[str, MappedPropertyApply | ConnectionDefinition] = None,
     ):
         super().__init__(space, external_id, version, description, name, filter, implements)
         self.properties = properties
 
     @classmethod
     def load(cls, resource: dict | str) -> ViewApply:
         data = json.loads(resource) if isinstance(resource, str) else resource
         if "properties" in data and isinstance(data["properties"], dict):
-            data["properties"] = {k: ViewPropertyDefinition.load(v) for k, v in data["properties"].items()} or None
+            data["properties"] = {k: ViewPropertyApply.load(v) for k, v in data["properties"].items()} or None
 
         return cast(ViewApply, super().load(data))
 
     def dump(self, camel_case: bool = False) -> dict[str, Any]:
         output = super().dump(camel_case)
         if "properties" in output:
             output["properties"] = {k: v.dump(camel_case) for k, v in output["properties"].items()}
@@ -137,15 +136,15 @@
     """
 
     def __init__(
         self,
         space: str,
         external_id: str,
         version: str,
-        properties: dict[str, MappedPropertyDefinition | ConnectionDefinition],
+        properties: dict[str, MappedProperty | ConnectionDefinition],
         last_updated_time: int,
         created_time: int,
         description: str = None,
         name: str = None,
         filter: Filter | None = None,
         implements: list[ViewId] = None,
         writable: bool = False,
@@ -169,15 +168,15 @@
         self.last_updated_time = last_updated_time
         self.created_time = created_time
 
     @classmethod
     def load(cls, resource: dict | str) -> View:
         data = json.loads(resource) if isinstance(resource, str) else resource
         if "properties" in data and isinstance(data["properties"], dict):
-            data["properties"] = {k: ViewPropertyDefinition.load(v) for k, v in data["properties"].items()} or None
+            data["properties"] = {k: ViewProperty.load(v) for k, v in data["properties"].items()} or None
 
         return cast(View, super().load(data))
 
     def dump(self, camel_case: bool = False) -> dict[str, Any]:
         output = super().dump(camel_case)
         if "properties" in output:
             output["properties"] = {k: v.dump(camel_case) for k, v in output["properties"].items()}
@@ -186,19 +185,17 @@
 
     def as_apply(self) -> ViewApply:
         """Convert to a view applies.
 
         Returns:
             ViewApply: The view apply.
         """
-        properties: Optional[Dict[str, Union[MappedApplyPropertyDefinition, ConnectionDefinition]]] = None
+        properties: Optional[Dict[str, Union[MappedPropertyApply, ConnectionDefinition]]] = None
         if self.properties:
-            properties = {
-                k: (v.as_apply() if isinstance(v, MappedPropertyDefinition) else v) for k, v in self.properties.items()
-            }
+            properties = {k: (v.as_apply() if isinstance(v, MappedProperty) else v) for k, v in self.properties.items()}
 
         return ViewApply(
             space=self.space,
             external_id=self.external_id,
             version=self.version,
             description=self.description,
             name=self.name,
@@ -252,165 +249,180 @@
     ):
         self.space = space
         self.include_inherited_properties = include_inherited_properties
         self.all_versions = all_versions
         self.include_global = include_global
 
 
-@dataclass
-class ViewDirectRelation(DirectRelation):
-    source: Optional[ViewId] = None
-
+class ViewProperty(ABC):
     @classmethod
-    def load(cls, data: dict) -> ViewDirectRelation:
-        output = cls(**convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"type"})))
-        if isinstance(data.get("source"), dict):
-            output.source = ViewId.load(data["source"])
-        return output
-
-    def dump(self, camel_case: bool = False) -> dict:
-        output = super().dump(camel_case)
-
-        if self.source:
-            output["source"] = self.source.dump(camel_case)
-        return output
+    def load(cls, data: dict[str, Any]) -> ViewProperty:
+        if "direction" in data:
+            return SingleHopConnectionDefinition.load(data)
+        else:
+            return MappedProperty.load(data)
 
+    @abstractmethod
+    def dump(self, camel_case: bool = False) -> dict[str, Any]:
+        raise NotImplementedError
 
-@dataclass
-class ViewPropertyDefinition(ABC):
-    @classmethod
-    def _load(cls, data: dict) -> ViewPropertyDefinition:
-        return cls(**convert_all_keys_to_snake_case(data))
 
+class ViewPropertyApply(ABC):
     @classmethod
-    def load(cls, data: dict) -> MappedPropertyDefinition | ConnectionDefinition | MappedApplyPropertyDefinition:
-        if "container" in data and "source" in data:
-            return MappedApplyPropertyDefinition.load(data)
-        elif "container" in data:
-            return MappedPropertyDefinition.load(data)
-        elif "type" in data:
-            return SingleHopConnectionDefinition.load(data)
+    def load(cls, data: dict[str, Any]) -> ViewPropertyApply:
+        if "direction" in data:
+            return SingleHopConnectionDefinitionApply.load(data)
+        else:
+            return MappedPropertyApply.load(data)
 
-        raise ValueError(f"Unknown type of ViewPropertyDefinition: {data.get('type')}")
-
-    def dump(self, camel_case: bool = False) -> dict:
-        output = asdict(self)
-        return convert_all_keys_to_camel_case_recursive(output) if camel_case else output
+    @abstractmethod
+    def dump(self, camel_case: bool = False) -> dict[str, Any]:
+        raise NotImplementedError
 
 
 @dataclass
-class MappedCorePropertyDefinition(ViewPropertyDefinition):
+class MappedPropertyApply(ViewPropertyApply):
     container: ContainerId
     container_property_identifier: str
     name: str | None = None
     description: str | None = None
+    source: ViewId | None = None
 
     @classmethod
-    def load(cls, data: dict) -> MappedCorePropertyDefinition:  # type: ignore[override]
-        output = cast(MappedCorePropertyDefinition, super()._load(data))
+    def load(cls, data: dict) -> MappedPropertyApply:
+        output = cls(**convert_all_keys_to_snake_case(data))
         if isinstance(data.get("container"), dict):
             output.container = ContainerId.load(data["container"])
+        if isinstance(data.get("source"), dict):
+            output.source = ViewId.load(data["source"])
         return output
 
-    def dump(self, camel_case: bool = False) -> dict:
+    def dump(self, camel_case: bool = False) -> dict[str, Any]:
         output = asdict(self)
-        if self.container:
-            output["container"] = self.container.dump(camel_case)
-
+        output["container"] = self.container.dump(camel_case)
         if camel_case:
-            output = convert_all_keys_to_camel_case_recursive(output)
-
+            return convert_all_keys_to_camel_case_recursive(output)
         return output
 
 
 @dataclass
-class MappedApplyPropertyDefinition(MappedCorePropertyDefinition):
+class MappedProperty(ViewProperty):
+    container: ContainerId
+    container_property_identifier: str
+    type: PropertyType
+    nullable: bool
+    auto_increment: bool
     source: ViewId | None = None
-
-    @classmethod
-    def load(cls, data: dict) -> MappedApplyPropertyDefinition:
-        output = cast(MappedApplyPropertyDefinition, super().load(data))
-        if isinstance(data.get("source"), dict):
-            output.source = ViewId.load(data["source"])
-        return output
-
-    def dump(self, camel_case: bool = False) -> dict:
-        output = super().dump(camel_case)
-        if self.source:
-            output["source"] = self.source.dump(camel_case)
-        return output
-
-
-@dataclass
-class MappedPropertyDefinition(MappedCorePropertyDefinition):
-    type: PropertyType | None = None
-    nullable: bool = True
-    auto_increment: bool = False
     default_value: str | int | dict | None = None
+    name: str | None = None
+    description: str | None = None
 
     @classmethod
-    def load(cls, data: dict) -> MappedPropertyDefinition:
-        output = cast(MappedPropertyDefinition, super().load(data))
+    def load(cls, data: dict[str, Any]) -> MappedProperty:
+        output = cls(**convert_all_keys_to_snake_case(data))
+        if isinstance(data.get("container"), dict):
+            output.container = ContainerId.load(data["container"])
         if "type" in data:
             if data["type"].get("type") == "direct":
-                output.type = ViewDirectRelation.load(data["type"])
+                type_data = data["type"]
+                source = type_data.pop("source", None)
+                output.type = DirectRelation.load(type_data)
+                output.source = ViewId.load(source) if source else None
             else:
                 output.type = PropertyType.load(data["type"])
         return output
 
-    def dump(self, camel_case: bool = False) -> dict:
-        output = super().dump(camel_case)
-        if self.type:
-            try:
-                output["type"] = self.type.dump(camel_case)
-            except AttributeError:
-                raise
+    def dump(self, camel_case: bool = False) -> dict[str, Any]:
+        output = asdict(self)
+        output["type"] = self.type.dump(camel_case)
+        output["type"]["source"] = output.pop("source", None)
+        if camel_case:
+            return convert_all_keys_to_camel_case_recursive(output)
         return output
 
-    def as_apply(self) -> MappedApplyPropertyDefinition:
-        return MappedApplyPropertyDefinition(
+    def as_apply(self) -> MappedPropertyApply:
+        return MappedPropertyApply(
             container=self.container,
             container_property_identifier=self.container_property_identifier,
             name=self.name,
             description=self.description,
         )
 
 
 @dataclass
-class ConnectionDefinition(ViewPropertyDefinition):
+class ConnectionDefinition(ViewProperty):
     ...
 
 
 @dataclass
 class SingleHopConnectionDefinition(ConnectionDefinition):
     type: DirectRelationReference
     source: ViewId
     name: str | None = None
     description: str | None = None
     edge_source: ViewId | None = None
     direction: Literal["outwards", "inwards"] = "outwards"
 
     @classmethod
-    def load(cls, data: dict) -> SingleHopConnectionDefinition:
-        output = cast(SingleHopConnectionDefinition, super()._load(data))
-        if "type" in data:
-            output.type = DirectRelationReference.load(data["type"])
-        if "source" in data:
-            output.source = ViewId.load(data["source"])
-        if "edgeSource" in data or "edge_source" in data:
-            edge_source = data.get("edgeSource", data.get("edge_source"))
-            output.edge_source = ViewId.load(edge_source) if edge_source else None
+    def load(cls, data: dict[str, Any]) -> SingleHopConnectionDefinition:
+        output = cls(**convert_all_keys_to_snake_case(data))
+        if (type_ := data.get("type")) is not None:
+            output.type = DirectRelationReference.load(type_)
+        if (source := data.get("source")) is not None:
+            output.source = ViewId.load(source)
+        if (edge_source := data.get("edgeSource")) is not None:
+            output.edge_source = ViewId.load(edge_source)
+        return output
+
+    def dump(self, camel_case: bool = False) -> dict[str, Any]:
+        output = asdict(self)
+
+        if self.type:
+            output["type"] = self.type.dump(camel_case)
+
+        if self.source:
+            output["source"] = self.source.dump(camel_case)
+
+        if self.edge_source:
+            output["edge_source"] = self.edge_source.dump(camel_case)
+
+        return convert_all_keys_to_camel_case_recursive(output) if camel_case else output
+
+
+@dataclass
+class ConnectionDefinitionApply(ViewPropertyApply):
+    ...
+
+
+@dataclass
+class SingleHopConnectionDefinitionApply(ConnectionDefinitionApply):
+    type: DirectRelationReference
+    source: ViewId
+    name: str | None = None
+    description: str | None = None
+    edge_source: ViewId | None = None
+    direction: Literal["outwards", "inwards"] = "outwards"
+
+    @classmethod
+    def load(cls, data: dict) -> SingleHopConnectionDefinitionApply:
+        output = cls(**convert_all_keys_to_snake_case(data))
+        if (type_ := data.get("type")) is not None:
+            output.type = DirectRelationReference.load(type_)
+        if (source := data.get("source")) is not None:
+            output.source = ViewId.load(source)
+        if (edge_source := data.get("edgeSource")) is not None:
+            output.edge_source = ViewId.load(edge_source)
         return output
 
     def dump(self, camel_case: bool = False) -> dict:
         output = asdict(self)
 
         if self.type:
             output["type"] = self.type.dump(camel_case)
 
         if self.source:
             output["source"] = self.source.dump(camel_case)
 
         if self.edge_source:
-            output["edgeSource" if camel_case else "edge_source"] = self.edge_source.dump(camel_case)
+            output["edge_source"] = self.edge_source.dump(camel_case)
 
         return convert_all_keys_to_camel_case_recursive(output) if camel_case else output
```

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/events.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/files.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/functions.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/iam.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/labels.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/raw.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/shared.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/templates.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.5.0/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/exceptions.py` & `cognite_sdk-6.5.0/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/testing.py` & `cognite_sdk-6.5.0/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/__init__.py` & `cognite_sdk-6.5.0/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.5.0/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.5.0/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_graph.py` & `cognite_sdk-6.5.0/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_identifier.py` & `cognite_sdk-6.5.0/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_logging.py` & `cognite_sdk-6.5.0/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.5.0/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.5.0/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.5.0/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_text.py` & `cognite_sdk-6.5.0/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_time.py` & `cognite_sdk-6.5.0/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_validation.py` & `cognite_sdk-6.5.0/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.5.0/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.8/pyproject.toml` & `cognite_sdk-6.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.4.8"
+version = "6.5.0"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.4.8/PKG-INFO` & `cognite_sdk-6.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.4.8
+Version: 6.5.0
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
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.8 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.5.0 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

