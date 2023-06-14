# Comparing `tmp/cognite_sdk-6.3.2.tar.gz` & `tmp/cognite_sdk-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.3.2.tar", max compression
+gzip compressed data, was "cognite_sdk-6.4.0.tar", max compression
```

## Comparing `cognite_sdk-6.3.2.tar` & `cognite_sdk-6.4.0.tar`

### file list

```diff
@@ -1,112 +1,114 @@
--rw-r--r--   0        0        0    11349 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/README.md
--rw-r--r--   0        0        0      574 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49083 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1013 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     7924 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     8454 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0     6468 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     7894 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11025 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-08 10:33:03.597142 cognite_sdk-6.3.2/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12474 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21276 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17320 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41397 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45329 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49915 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9466 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27887 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21811 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4589 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9525 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    37722 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      178 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-08 10:33:03.601143 cognite_sdk-6.3.2/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    18565 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8741 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34178 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33582 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     2935 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0    12346 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7240 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     3651 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     3877 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0     2524 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14625 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6682 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33940 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11008 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14299 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13657 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16631 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16465 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6003 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5868 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4098 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12253 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17651 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16814 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11789 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12078 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11425 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2354 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2451 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2742 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/py.typed
--rw-r--r--   0        0        0     8865 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-08 10:33:03.605143 cognite_sdk-6.3.2/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7422 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-08 10:33:03.609143 cognite_sdk-6.3.2/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/README.md
+-rw-r--r--   0        0        0      574 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49083 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     7867 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8393 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    24419 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6424 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7857 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11025 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-12 16:29:40.247142 cognite_sdk-6.4.0/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21276 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17192 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41485 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45301 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49823 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9466 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27887 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21811 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4589 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9525 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38099 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-06-12 16:29:40.251142 cognite_sdk-6.4.0/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33629 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     3689 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0    12373 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7267 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     3739 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     5911 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    28421 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0     2543 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14642 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6037 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7684 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-12 16:29:40.255142 cognite_sdk-6.4.0/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-12 16:29:40.259142 cognite_sdk-6.4.0/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.0/PKG-INFO
```

### Comparing `cognite_sdk-6.3.2/LICENSE` & `cognite_sdk-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/README.md` & `cognite_sdk-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/__init__.py` & `cognite_sdk-6.4.0/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/annotations.py` & `cognite_sdk-6.4.0/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/assets.py` & `cognite_sdk-6.4.0/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.4.0/cognite/client/_api/data_modeling/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
 from cognite.client._api.data_modeling.containers import ContainersAPI
 from cognite.client._api.data_modeling.data_models import DataModelsAPI
+from cognite.client._api.data_modeling.instances import InstancesAPI
 from cognite.client._api.data_modeling.spaces import SpacesAPI
 from cognite.client._api.data_modeling.views import ViewsAPI
 from cognite.client._api_client import APIClient
 
 if TYPE_CHECKING:
     from cognite.client import CogniteClient
     from cognite.client.config import ClientConfig
@@ -16,7 +17,8 @@
 class DataModelingAPI(APIClient):
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
         self.containers = ContainersAPI(config, api_version, cognite_client)
         self.data_models = DataModelsAPI(config, api_version, cognite_client)
         self.spaces = SpacesAPI(config, api_version, cognite_client)
         self.views = ViewsAPI(config, api_version, cognite_client)
+        self.instances = InstancesAPI(config, api_version, cognite_client)
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.4.0/cognite/client/_api/data_modeling/containers.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.containers import (
     Container,
     ContainerApply,
     ContainerFilter,
     ContainerList,
 )
-from cognite.client.data_classes.data_modeling.ids import ContainerIdentifier, DataModelingId, load_identifier
+from cognite.client.data_classes.data_modeling.ids import ContainerIdentifier, DataModelingId, _load_identifier
 
 
 class ContainersAPI(APIClient):
     _RESOURCE_PATH = "/models/containers"
 
     @overload
     def __call__(
@@ -81,15 +81,15 @@
         ...
 
     @overload
     def retrieve(self, ids: Sequence[ContainerIdentifier]) -> ContainerList:
         ...
 
     def retrieve(self, ids: ContainerIdentifier | Sequence[ContainerIdentifier]) -> Container | ContainerList | None:
-        """`Retrieve one or more container by id(s). <https://docs.cognite.com/api/v1/#tag/Containers/operation/byExternalIdsContainers>`_
+        """`Retrieve one or more container by id(s). <https://docs.cognite.com/api/v1/#operation/byExternalIdsContainers>`_
 
         Args:
             ids (ContainerId | Sequence[ContainerId]): Identifier for container(s).
 
         Returns:
             Optional[Container]: Requested container or None if it does not exist.
 
@@ -102,19 +102,19 @@
             Fetch using the DataModelingId::
 
                 >>> from cognite.client import CogniteClient
                 >>> from cognite.client.data_modeling import DataModelingId
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.containers.retrieve(DataModelingId(space='mySpace', external_id='myContainer'))
         """
-        identifier = load_identifier(ids, "container")
+        identifier = _load_identifier(ids, "container")
         return self._retrieve_multiple(list_cls=ContainerList, resource_cls=Container, identifiers=identifier)
 
     def delete(self, id: ContainerIdentifier | Sequence[ContainerIdentifier]) -> list[DataModelingId]:
-        """`Delete one or more containers <https://docs.cognite.com/api/v1/#tag/Containers/operation/deleteContainers>`_
+        """`Delete one or more containers <https://docs.cognite.com/api/v1/#operation/deleteContainers>`_
 
         Args:
             id (ContainerId | Sequence[ContainerId): The container identifier(s).
         Returns:
             The container(s) which has been deleted. Empty list if nothing was deleted.
         Examples:
 
@@ -122,22 +122,22 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.data_modeling.containers.delete(("mySpace", "myContainer"))
         """
         deleted_containers = cast(
             list,
-            self._delete_multiple(identifiers=load_identifier(id, "container"), wrap_ids=True, returns_items=True),
+            self._delete_multiple(identifiers=_load_identifier(id, "container"), wrap_ids=True, returns_items=True),
         )
         return [DataModelingId(space=item["space"], external_id=item["externalId"]) for item in deleted_containers]
 
     def list(
         self, space: str | None = None, limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT, include_global: bool = False
     ) -> ContainerList:
-        """`List containers <https://docs.cognite.com/api/v1/#tag/Containers/operation/listContainers>`_
+        """`List containers <https://docs.cognite.com/api/v1/#operation/listContainers>`_
 
         Args:
             space (int, optional): The space to query
             limit (int, optional): Maximum number of containers to return. Default to 10. Set to -1, float("inf") or None
                 to return all items.
             include_global (bool, optional): Whether the global containers should be returned.
 
@@ -181,15 +181,15 @@
         ...
 
     @overload
     def apply(self, container: ContainerApply) -> Container:
         ...
 
     def apply(self, container: ContainerApply | Sequence[ContainerApply]) -> Container | ContainerList:
-        """`Add or update (upsert) containers. <https://docs.cognite.com/api/v1/#tag/Containers/operation/ApplyContainers>`_
+        """`Add or update (upsert) containers. <https://docs.cognite.com/api/v1/#operation/ApplyContainers>`_
 
         Args:
             container (container: ContainerApply | Sequence[ContainerApply]): Container or containers of containers to create or update.
 
         Returns:
             Container | ContainerList: Created container(s)
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.4.0/cognite/client/_api/data_modeling/data_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.data_models import (
     DataModel,
     DataModelApply,
     DataModelFilter,
     DataModelList,
 )
-from cognite.client.data_classes.data_modeling.ids import DataModelIdentifier, VersionedDataModelingId, load_identifier
+from cognite.client.data_classes.data_modeling.ids import DataModelIdentifier, VersionedDataModelingId, _load_identifier
 
 
 class DataModelsAPI(APIClient):
     _RESOURCE_PATH = "/models/datamodels"
 
     @overload
     def __call__(
@@ -83,34 +83,34 @@
 
         Yields:
             DataModel: yields DataModels one by one.
         """
         return cast(Iterator[DataModel], self())
 
     def retrieve(self, ids: DataModelIdentifier | Sequence[DataModelIdentifier]) -> DataModelList:
-        """`Retrieve data_model(s) by id(s). <https://docs.cognite.com/api/v1/#tag/Data-models/operation/byExternalIdsDataModels>`_
+        """`Retrieve data_model(s) by id(s). <https://docs.cognite.com/api/v1/#operation/byExternalIdsDataModels>`_
 
         Args:
             ids (DataModelId | Sequence[DataModelId]): Data Model identifier(s).
 
         Returns:
             Optional[DataModel]: Requested data_model or None if it does not exist.
 
         Examples:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.data_models.retrieve(("mySpace", "myDataModel", "v1"))
 
         """
-        identifier = load_identifier(ids, "data_model")
+        identifier = _load_identifier(ids, "data_model")
         return self._retrieve_multiple(list_cls=DataModelList, resource_cls=DataModel, identifiers=identifier)
 
     def delete(self, ids: DataModelIdentifier | Sequence[DataModelIdentifier]) -> list[VersionedDataModelingId]:
-        """`Delete one or more data model <https://docs.cognite.com/api/v1/#tag/Data-models/operation/deleteDataModels>`_
+        """`Delete one or more data model <https://docs.cognite.com/api/v1/#operation/deleteDataModels>`_
 
         Args:
             ids (DataModelId | Sequence[DataModelId]): Data Model identifier(s).
         Returns:
             The data_model(s) which has been deleted. None if nothing was deleted.
         Examples:
 
@@ -118,29 +118,29 @@
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.data_modeling.data_models.delete(("mySpace", "myDataModel", "v1"))
         """
         deleted_data_models = cast(
             list,
-            self._delete_multiple(identifiers=load_identifier(ids, "data_model"), wrap_ids=True, returns_items=True),
+            self._delete_multiple(identifiers=_load_identifier(ids, "data_model"), wrap_ids=True, returns_items=True),
         )
         return [
             VersionedDataModelingId(item["space"], item["externalId"], item["version"]) for item in deleted_data_models
         ]
 
     def list(
         self,
         limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT,
         space: str | None = None,
         inline_views: bool = False,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> DataModelList:
-        """`List data models <https://docs.cognite.com/api/v1/#tag/Data-models/operation/listDataModels>`_
+        """`List data models <https://docs.cognite.com/api/v1/#operation/listDataModels>`_
 
         Args:
             limit (int, optional): Maximum number of data model to return. Default to 10. Set to -1, float("inf") or None
                 to return all items.
             space: (str | None): The space to query.
             inline_views (bool): Whether to expand the referenced views inline in the returned result.
             all_versions (bool): Whether to return all versions. If false, only the newest version is returned,
@@ -187,15 +187,15 @@
         ...
 
     @overload
     def apply(self, data_model: DataModelApply) -> DataModel:
         ...
 
     def apply(self, data_model: DataModelApply | Sequence[DataModelApply]) -> DataModel | DataModelList:
-        """`Create or update one or more data model. <https://docs.cognite.com/api/v1/#tag/Data-models/operation/createDataModels>`_
+        """`Create or update one or more data model. <https://docs.cognite.com/api/v1/#operation/createDataModels>`_
 
         Args:
             data_model (data_model: DataModelApply | Sequence[DataModelApply]): DataModel or data model to create or update (upsert).
 
         Returns:
             DataModel | DataModelList: Created data_model(s)
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.4.0/cognite/client/_api/data_modeling/spaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         ...
 
     @overload
     def retrieve(self, space: Sequence[str]) -> SpaceList:
         ...
 
     def retrieve(self, space: str | Sequence[str]) -> Space | SpaceList | None:
-        """`Retrieve space by id. <https://docs.cognite.com/api/v1/#tag/Spaces/operation/bySpaceIdsSpaces>`_
+        """`Retrieve space by id. <https://docs.cognite.com/api/v1/#operation/bySpaceIdsSpaces>`_
 
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
-        """`Delete one or more spaces <https://docs.cognite.com/api/v1/#tag/Spaces/operation/deleteSpacesV3>`_
+        """`Delete one or more spaces <https://docs.cognite.com/api/v1/#operation/deleteSpacesV3>`_
 
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
-        """`List spaces <https://docs.cognite.com/api/v1/#tag/Spaces/operation/listSpacesV3>`_
+        """`List spaces <https://docs.cognite.com/api/v1/#operation/listSpacesV3>`_
 
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
-        """`Create or patch one or more spaces. <https://docs.cognite.com/api/v1/#tag/Spaces/operation/ApplySpaces>`_
+        """`Create or patch one or more spaces. <https://docs.cognite.com/api/v1/#operation/ApplySpaces>`_
 
         Args:
             space (space: Space | Sequence[Space]): Space or spaces of spacesda to create or update.
 
         Returns:
             Space | SpaceList: Created space(s)
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.4.0/cognite/client/_api/data_modeling/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import Iterator, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
-from cognite.client.data_classes.data_modeling.ids import VersionedDataModelingId, ViewIdentifier, load_identifier
+from cognite.client.data_classes.data_modeling.ids import VersionedDataModelingId, ViewIdentifier, _load_identifier
 from cognite.client.data_classes.data_modeling.views import View, ViewApply, ViewFilter, ViewList
 
 
 class ViewsAPI(APIClient):
     _RESOURCE_PATH = "/models/views"
 
     @overload
@@ -77,34 +77,34 @@
 
         Yields:
             View: yields Views one by one.
         """
         return cast(Iterator[View], self())
 
     def retrieve(self, ids: ViewIdentifier | Sequence[ViewIdentifier]) -> ViewList:
-        """`Retrieve a single view by id. <https://docs.cognite.com/api/v1/#tag/Views/operation/byExternalIdsViews>`_
+        """`Retrieve a single view by id. <https://docs.cognite.com/api/v1/#operation/byExternalIdsViews>`_
 
         Args:
             ids (ViewId | Sequence[ViewId]): View dentifier(s)
 
         Returns:
             Optional[View]: Requested view or None if it does not exist.
 
         Examples:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.views.retrieve(('mySpace', 'myView', 'v1'))
 
         """
-        identifier = load_identifier(ids, "view")
+        identifier = _load_identifier(ids, "view")
         return self._retrieve_multiple(list_cls=ViewList, resource_cls=View, identifiers=identifier)
 
     def delete(self, ids: ViewIdentifier | Sequence[ViewIdentifier]) -> list[VersionedDataModelingId]:
-        """`Delete one or more views <https://docs.cognite.com/api/v1/#tag/Views/operation/deleteViews>`_
+        """`Delete one or more views <https://docs.cognite.com/api/v1/#operation/deleteViews>`_
 
         Args:
             ids (ViewId | Sequence[ViewId]): View dentifier(s)
         Returns:
             The identifier for the view(s) which has been deleted. Empty list if nothing was deleted.
         Examples:
 
@@ -113,30 +113,30 @@
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> c.data_modeling.views.delete(('mySpace', 'myView', 'v1'))
         """
         deleted_views = cast(
             list,
             self._delete_multiple(
-                identifiers=load_identifier(ids, "view"),
+                identifiers=_load_identifier(ids, "view"),
                 wrap_ids=True,
                 returns_items=True,
             ),
         )
         return [VersionedDataModelingId(item["space"], item["externalId"], item["version"]) for item in deleted_views]
 
     def list(
         self,
         limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT,
         space: str | None = None,
         include_inherited_properties: bool = True,
         all_versions: bool = False,
         include_global: bool = False,
     ) -> ViewList:
-        """`List views <https://docs.cognite.com/api/v1/#tag/Views/operation/listViews>`_
+        """`List views <https://docs.cognite.com/api/v1/#operation/listViews>`_
 
         Args:
             limit (int, optional): Maximum number of views to return. Defaults to 25. Set to -1, float("inf") or None
                 to return all items.
             space: (str | None): The space to query.
             include_inherited_properties (bool): Whether to include properties inherited from views this view implements.
             all_versions (bool): Whether to return all versions. If false, only the newest version is returned,
@@ -179,15 +179,15 @@
         ...
 
     @overload
     def apply(self, view: ViewApply) -> View:
         ...
 
     def apply(self, view: ViewApply | Sequence[ViewApply]) -> View | ViewList:
-        """`Create or update (upsert) one or more views. <https://docs.cognite.com/api/v1/#tag/Views/operation/ApplyViews>`_
+        """`Create or update (upsert) one or more views. <https://docs.cognite.com/api/v1/#operation/ApplyViews>`_
 
         Args:
             view (view: ViewApply | Sequence[ViewApply]): View or views of views to create or update.
 
         Returns:
             View | ViewList: Created view(s)
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/data_sets.py` & `cognite_sdk-6.4.0/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.4.0/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/datapoints.py` & `cognite_sdk-6.4.0/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/diagrams.py` & `cognite_sdk-6.4.0/cognite/client/_api/diagrams.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 
 
 class DiagramsAPI(APIClient):
     _RESOURCE_PATH = "/context/diagram"
 
     def __init__(self, config: ClientConfig, api_version: Optional[str], cognite_client: CogniteClient) -> None:
         super().__init__(config, api_version, cognite_client)
-        # https://docs.cognite.com/api/playground/#tag/Engineering-diagrams/operation/diagramDetect
+        # https://docs.cognite.com/api/playground/#operation/diagramDetect
         self._DETECT_API_FILE_LIMIT = 50
-        # https://docs.cognite.com/api/playground/#tag/Engineering-diagrams/operation/diagramDetectMultipleResults
+        # https://docs.cognite.com/api/playground/#operation/diagramDetectMultipleResults
         self._DETECT_API_STATUS_JOB_LIMIT = 1000
 
     def _camel_post(
         self,
         context_path: str,
         json: Dict[str, Any] = None,
         params: Dict[str, Any] = None,
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.4.0/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/events.py` & `cognite_sdk-6.4.0/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.4.0/cognite/client/_api/extractionpipelines.py`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
 class ExtractionPipelineConfigsAPI(APIClient):
     _RESOURCE_PATH = "/extpipes/config"
 
     def retrieve(
         self, external_id: str, revision: Optional[int] = None, active_at_time: Optional[int] = None
     ) -> ExtractionPipelineConfig:
-        """`Retrieve a specific configuration revision, or the latest by default <https://docs.cognite.com/api/v1/#tag/Extraction-Pipelines-Config/operation/getExtPipeConfigRevision>`
+        """`Retrieve a specific configuration revision, or the latest by default <https://docs.cognite.com/api/v1/#operation/getExtPipeConfigRevision>`
 
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
-        """`Retrieve all configuration revisions from an extraction pipeline <https://docs.cognite.com/api/v1/#tag/Extraction-Pipelines-Config/operation/listExtPipeConfigRevisions>`
+        """`Retrieve all configuration revisions from an extraction pipeline <https://docs.cognite.com/api/v1/#operation/listExtPipeConfigRevisions>`
 
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
-        """`Create a new configuration revision <https://docs.cognite.com/api/v1/#tag/Extraction-Pipelines-Config/operation/createExtPipeConfig>`
+        """`Create a new configuration revision <https://docs.cognite.com/api/v1/#operation/createExtPipeConfig>`
 
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
-        """`Revert to a previous configuration revision <https://docs.cognite.com/api/v1/#tag/Extraction-Pipelines-Config/operation/createExtPipeConfig>`
+        """`Revert to a previous configuration revision <https://docs.cognite.com/api/v1/#operation/createExtPipeConfig>`
 
         Args:
             external_id (str): External id of the extraction pipeline to revert revision for.
             revision (int): Revision to revert to.
 
         Returns:
             ExtractionPipelineConfig: New latest extraction pipeline configuration revision.
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/files.py` & `cognite_sdk-6.4.0/cognite/client/_api/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -774,18 +774,19 @@
 
     def _get_id_to_metadata_map(self, all_ids: Sequence[Dict]) -> Dict[Union[str, int], FileMetadata]:
         ids = [id["id"] for id in all_ids if "id" in id]
         external_ids = [id["externalId"] for id in all_ids if "externalId" in id]
 
         files_metadata = self.retrieve_multiple(ids=ids, external_ids=external_ids)
 
-        id_to_metadata = {}
+        id_to_metadata: dict[str | int, FileMetadata] = {}
         for f in files_metadata:
-            id_to_metadata[f.id] = f
-            id_to_metadata[f.external_id] = f
+            id_to_metadata[cast(int, f.id)] = f
+            if f.external_id is not None:
+                id_to_metadata[f.external_id] = f
 
         return id_to_metadata
 
     def _download_files_to_directory(
         self,
         directory: Path,
         all_ids: Sequence[Dict[str, Union[int, str]]],
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/functions.py` & `cognite_sdk-6.4.0/cognite/client/_api/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -474,15 +474,15 @@
             raise TypeError(
                 "Exactly one of the arguments folder, file_id and handle is required, but "
                 + ", ".join(given_source_code_options)
                 + " were given."
             )
 
     def activate(self) -> FunctionsStatus:
-        """`Activate functions for the Project. <https://docs.cognite.com/api/v1/#tag/Functions/operation/postFunctionsStatus>`_.
+        """`Activate functions for the Project. <https://docs.cognite.com/api/v1/#operation/postFunctionsStatus>`_.
 
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
-        """`Functions activation status for the Project. <https://docs.cognite.com/api/v1/#tag/Functions/operation/getFunctionsStatus>`_.
+        """`Functions activation status for the Project. <https://docs.cognite.com/api/v1/#operation/getFunctionsStatus>`_.
 
         Returns:
             FunctionsStatus: A function activation status.
 
         Examples:
 
             Call status::
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/geospatial.py` & `cognite_sdk-6.4.0/cognite/client/_api/geospatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1000,16 +1000,15 @@
         raster_format: str,
         raster_srid: int,
         file: str,
         allow_crs_transformation: bool = False,
         raster_scale_x: Optional[float] = None,
         raster_scale_y: Optional[float] = None,
     ) -> RasterMetadata:
-        """`Put raster`
-        <https://docs.cognite.com/api/v1/#tag/Geospatial/operation/putRaster>
+        """`Put raster <https://docs.cognite.com/api/v1/#operation/putRaster>`
 
         Args:
             feature_type_external_id : Feature type definition for the features to create.
             feature_external_id: one feature or a list of features to create
             raster_property_name: the raster property name
             raster_format: the raster input format
             raster_srid: the associated SRID for the raster
@@ -1056,16 +1055,15 @@
 
     def delete_raster(
         self,
         feature_type_external_id: str,
         feature_external_id: str,
         raster_property_name: str,
     ) -> None:
-        """`Delete raster`
-        <https://docs.cognite.com/api/v1/#tag/Geospatial/operation/deleteRaster>
+        """`Delete raster <https://docs.cognite.com/api/v1/#operation/deleteRaster>`
 
         Args:
             feature_type_external_id : Feature type definition for the features to create.
             feature_external_id: one feature or a list of features to create
             raster_property_name: the raster property name
 
         Returns:
@@ -1099,16 +1097,15 @@
         raster_format: str,
         raster_options: Dict[str, Any] = None,
         raster_srid: Optional[int] = None,
         raster_scale_x: Optional[float] = None,
         raster_scale_y: Optional[float] = None,
         allow_crs_transformation: bool = False,
     ) -> bytes:
-        """`Get raster`
-        <https://docs.cognite.com/api/v1/#tag/Geospatial/operation/getRaster>
+        """`Get raster <https://docs.cognite.com/api/v1/#operation/getRaster>`
 
         Args:
             feature_type_external_id: Feature type definition for the features to create.
             feature_external_id: one feature or a list of features to create
             raster_property_name: the raster property name
             raster_format: the raster output format
             raster_options: GDAL raster creation key-value options
@@ -1149,16 +1146,15 @@
         )
         return res.content
 
     def compute(
         self,
         output: Dict[str, GeospatialComputeFunction],
     ) -> GeospatialComputedResponse:
-        """`Compute`
-        <https://docs.cognite.com/api/v1/#tag/Geospatial/operation/compute>
+        """`Compute <https://docs.cognite.com/api/v1/#operation/compute>`
 
         Args:
             output : Mapping of keys to compute functions.
 
         Returns:
             dict: Mapping of keys to computed items.
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/iam.py` & `cognite_sdk-6.4.0/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/labels.py` & `cognite_sdk-6.4.0/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/raw.py` & `cognite_sdk-6.4.0/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/relationships.py` & `cognite_sdk-6.4.0/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/sequences.py` & `cognite_sdk-6.4.0/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.4.0/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/templates.py` & `cognite_sdk-6.4.0/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/three_d.py` & `cognite_sdk-6.4.0/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/time_series.py` & `cognite_sdk-6.4.0/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.4.0/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.4.0/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.4.0/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.4.0/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.4.0/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api/vision.py` & `cognite_sdk-6.4.0/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_api_client.py` & `cognite_sdk-6.4.0/cognite/client/_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,15 +394,17 @@
                     params = filter.copy()
                     params["limit"] = current_limit
                     params["cursor"] = next_cursor
                     if sort is not None:
                         params["sort"] = sort
                     res = self._get(url_path=url_path or resource_path, params=params, headers=headers)
                 elif method == "POST":
-                    body = {"filter": filter, "limit": current_limit, "cursor": next_cursor, **(other_params or {})}
+                    body: dict[str, Any] = {"limit": current_limit, "cursor": next_cursor, **(other_params or {})}
+                    if filter:
+                        body["filter"] = filter
                     if sort is not None:
                         body["sort"] = sort
                     res = self._post(url_path=url_path or resource_path + "/list", json=body, headers=headers)
                 else:
                     raise ValueError(f"_list_generator parameter `method` must be GET or POST, not {method}")
                 last_received_items = res.json()["items"]
                 total_items_retrieved += len(last_received_items)
@@ -588,51 +590,55 @@
             body["keys"] = keys
         res = self._post(url_path=resource_path + "/aggregate", json=body, headers=headers)
         return [cls(**agg) for agg in res.json()["items"]]
 
     @overload
     def _create_multiple(
         self,
-        items: Union[Sequence[T_CogniteResource], Sequence[Dict[str, Any]]],
+        items: Union[Sequence[CogniteResource], Sequence[Dict[str, Any]]],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         resource_path: Optional[str] = None,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         extra_body_fields: Optional[Dict] = None,
         limit: Optional[int] = None,
+        input_resource_cls: Optional[Type[CogniteResource]] = None,
     ) -> T_CogniteResourceList:
         ...
 
     @overload
     def _create_multiple(
         self,
         items: Union[CogniteResource, Dict[str, Any]],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         resource_path: Optional[str] = None,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         extra_body_fields: Optional[Dict] = None,
         limit: Optional[int] = None,
+        input_resource_cls: Optional[Type[CogniteResource]] = None,
     ) -> T_CogniteResource:
         ...
 
     def _create_multiple(
         self,
         items: Union[Sequence[CogniteResource], Sequence[Dict[str, Any]], CogniteResource, Dict[str, Any]],
         list_cls: Type[T_CogniteResourceList],
         resource_cls: Type[T_CogniteResource],
         resource_path: Optional[str] = None,
         params: Optional[Dict] = None,
         headers: Optional[Dict] = None,
         extra_body_fields: Optional[Dict] = None,
         limit: Optional[int] = None,
+        input_resource_cls: Optional[Type[CogniteResource]] = None,
     ) -> Union[T_CogniteResourceList, T_CogniteResource]:
         resource_path = resource_path or self._RESOURCE_PATH
+        input_resource_cls = input_resource_cls or resource_cls
         limit = limit or self._CREATE_LIMIT
         single_item = not isinstance(items, Sequence)
         if single_item:
             items = cast(Union[Sequence[T_CogniteResource], Sequence[Dict[str, Any]]], [items])
         else:
             items = cast(Union[Sequence[T_CogniteResource], Sequence[Dict[str, Any]]], items)
 
@@ -640,15 +646,15 @@
             (resource_path, task_items, params, headers)
             for task_items in self._prepare_item_chunks(items, limit, extra_body_fields)
         ]
         summary = utils._concurrency.execute_tasks(self._post, tasks, max_workers=self._config.max_workers)
 
         def unwrap_element(el: T) -> Union[CogniteResource, T]:
             if isinstance(el, dict):
-                return resource_cls._load(el, cognite_client=self._cognite_client)
+                return input_resource_cls._load(el, cognite_client=self._cognite_client)  # type: ignore[union-attr]
             else:
                 return el
 
         def str_format_element(el: T) -> Union[str, Dict, T]:
             if isinstance(el, CogniteResource):
                 dumped = el.dump()
                 if "external_id" in dumped:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/_cognite_client.py` & `cognite_sdk-6.4.0/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_http_client.py` & `cognite_sdk-6.4.0/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.4.0/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.4.0/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.0/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.4.0/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.4.0/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.4.0/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.4.0/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.0/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.4.0/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.4.0/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/config.py` & `cognite_sdk-6.4.0/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/credentials.py` & `cognite_sdk-6.4.0/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/_base.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,28 @@
 from __future__ import annotations
 
 import json
 from collections import UserList
-from typing import TYPE_CHECKING, Any, Collection, Dict, Generic, List, Optional, Sequence, Type, TypeVar, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Collection,
+    Dict,
+    Generic,
+    Iterator,
+    List,
+    Optional,
+    Sequence,
+    SupportsIndex,
+    Type,
+    TypeVar,
+    Union,
+    cast,
+    overload,
+)
 
 from cognite.client import utils
 from cognite.client.exceptions import CogniteMissingClientError
 from cognite.client.utils._identifier import IdentifierSequence
 from cognite.client.utils._pandas_helpers import convert_nullable_int_cols, notebook_display_with_fallback
 from cognite.client.utils._text import convert_all_keys_to_camel_case, to_snake_case
 from cognite.client.utils._time import convert_time_attributes_to_datetime
@@ -169,15 +185,15 @@
     def _property_setter(self: Any, schema_name: str, value: Any) -> None:
         if value is None:
             self.pop(schema_name, None)
         else:
             self[schema_name] = value
 
 
-class CogniteResourceList(UserList):
+class CogniteResourceList(UserList, Generic[T_CogniteResource]):
     _RESOURCE: Type[CogniteResource]
 
     def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
         for resource in resources:
             if not isinstance(resource, self._RESOURCE):
                 raise TypeError(
                     f"All resources for class '{self.__class__.__name__}' must be of type "
@@ -196,14 +212,28 @@
 
     def __getattribute__(self, item: Any) -> Any:
         attr = super().__getattribute__(item)
         if item == "_cognite_client" and attr is None:
             raise CogniteMissingClientError
         return attr
 
+    def pop(self, i: int = -1) -> T_CogniteResource:
+        return super().pop(i)
+
+    def __iter__(self) -> Iterator[T_CogniteResource]:
+        return super().__iter__()
+
+    @overload
+    def __getitem__(self, item: SupportsIndex) -> T_CogniteResource:
+        ...
+
+    @overload
+    def __getitem__(self, item: slice) -> CogniteResourceList[T_CogniteResource]:
+        ...
+
     def __getitem__(self, item: Any) -> Any:
         value = super().__getitem__(item)
         if isinstance(item, slice):
             c = None
             if super().__getattribute__("_cognite_client") is not None:
                 c = self._cognite_client
             return self.__class__(value, cognite_client=c)
@@ -230,15 +260,15 @@
             camel_case (bool): Use camelCase for attribute names. Defaults to False.
 
         Returns:
             List[Dict[str, Any]]: A list of dicts representing the instance.
         """
         return [resource.dump(camel_case) for resource in self.data]
 
-    def get(self, id: int = None, external_id: str = None) -> Optional[CogniteResource]:
+    def get(self, id: int = None, external_id: str = None) -> Optional[T_CogniteResource]:
         """Get an item from this list by id or exernal_id.
 
         Args:
             id (int): The id of the item to get.
             external_id (str): The external_id of the item to get.
 
         Returns:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,9 +190,9 @@
         return AnnotationUpdate._StrUpdate(self, "status")
 
     @property
     def annotation_type(self) -> AnnotationUpdate._StrUpdate:
         return AnnotationUpdate._StrUpdate(self, "annotationType")
 
 
-class AnnotationList(CogniteResourceList):
+class AnnotationList(CogniteResourceList[Annotation]):
     _RESOURCE = Annotation
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/assets.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/assets.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
         return AssetUpdate._LabelAssetUpdate(self, "labels")
 
     @property
     def geo_location(self) -> _PrimitiveAssetUpdate:
         return AssetUpdate._PrimitiveAssetUpdate(self, "geoLocation")
 
 
-class AssetList(CogniteResourceList):
+class AssetList(CogniteResourceList[Asset]):
     _RESOURCE = Asset
 
     def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
         super().__init__(resources, cognite_client)
         self._retrieve_chunk_size = 100
 
     def time_series(self) -> TimeSeriesList:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/contextualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
         obj._status_path = status_path
         return obj
 
 
 T_ContextualizationJob = TypeVar("T_ContextualizationJob", bound=ContextualizationJob)
 
 
-class ContextualizationJobList(CogniteResourceList):
+class ContextualizationJobList(CogniteResourceList[ContextualizationJob]):
     _RESOURCE = ContextualizationJob
 
 
 class EntityMatchingModel(CogniteResource):
     _RESOURCE_PATH = "/context/entitymatching"
     _STATUS_PATH = _RESOURCE_PATH + "/"
 
@@ -322,15 +322,15 @@
         return EntityMatchingModelUpdate._PrimitiveUpdate(self, "name")
 
     @property
     def description(self) -> _PrimitiveUpdate:
         return EntityMatchingModelUpdate._PrimitiveUpdate(self, "description")
 
 
-class EntityMatchingModelList(CogniteResourceList):
+class EntityMatchingModelList(CogniteResourceList[EntityMatchingModel]):
     _RESOURCE = EntityMatchingModel
 
 
 class FileReference:
     def __init__(
         self,
         file_id: Optional[int] = None,
@@ -364,15 +364,15 @@
     ):
         self.page = page
         self.png_url = png_url
         self.svg_url = svg_url
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class DiagramConvertPageList(CogniteResourceList):
+class DiagramConvertPageList(CogniteResourceList[DiagramConvertPage]):
     _RESOURCE = DiagramConvertPage
 
 
 class DiagramConvertItem(CogniteResource):
     def __init__(
         self,
         file_id: int = None,
@@ -817,15 +817,15 @@
         self,
         creating_user: Optional[str] = None,
         creating_app: Optional[str] = None,
         creating_app_version: Optional[str] = None,
     ) -> Union[Annotation, AnnotationList]:
         """
         Saves all predictions made by the feature extractors in CDF using the Annotations API.
-        See https://docs.cognite.com/api/v1/#tag/Annotations/operation/annotationsSuggest
+        See https://docs.cognite.com/api/v1/#operation/annotationsSuggest
 
         Args:
             creating_app (str, optional): The name of the app from which this annotation was created. Defaults to 'cognite-sdk-python'.
             creating_app_version (str, optional): The version of the app that created this annotation. Must be a valid semantic versioning (SemVer) string. Defaults to client version.
             creating_user: (str, optional): A username, or email, or name. This is not checked nor enforced. If the value is None, it means the annotation was created by a service.
         Returns:
             Union[Annotation, AnnotationList]: (suggested) annotation(s) stored in CDF.
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,19 +156,19 @@
             name=self.name,
             used_for=self.used_for,
             constraints=self.constraints,
             indexes=self.indexes,
         )
 
 
-class ContainerList(CogniteResourceList):
+class ContainerList(CogniteResourceList[Container]):
     _RESOURCE = Container
 
 
-class ContainerApplyList(CogniteResourceList):
+class ContainerApplyList(CogniteResourceList[ContainerApply]):
     _RESOURCE = ContainerApply
 
     def as_apply(self) -> ContainerApplyList:
         """Convert to a container an apply list.
 
         Returns:
             ContainerApplyList: The container apply list.
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,19 +158,19 @@
             version=self.version,
             description=self.description,
             name=self.name,
             views=views,
         )
 
 
-class DataModelApplyList(CogniteResourceList):
+class DataModelApplyList(CogniteResourceList[DataModelApply]):
     _RESOURCE = DataModelApply
 
 
-class DataModelList(CogniteResourceList):
+class DataModelList(CogniteResourceList[DataModel]):
     _RESOURCE = DataModel
 
     def to_data_model_apply_list(self) -> DataModelApplyList:
         return DataModelApplyList(resources=[d.as_apply() for d in self.items])
 
 
 class DataModelFilter(CogniteFilter):
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 
         return convert_all_keys_recursive(output, camel_case)
 
     @classmethod
     def load(cls, data: dict) -> DirectRelationReference:
         return cls(**convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"type"})))
 
+    def as_tuple(self) -> tuple[str, str]:
+        return self.space, self.external_id
+
 
 class PropertyType(ABC):
     _type: ClassVar[str]
 
     def dump(self, camel_case: bool = False) -> dict:
         output = asdict(self)
         output["type"] = self._type
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/ids.py`

 * *Files 27% similar despite different names*

```diff
@@ -66,47 +66,98 @@
         raise ValueError(f"Cannot load {data} into {cls}, invalid type={type(data)}")
 
 
 T_Versioned_DataModeling_Id = TypeVar("T_Versioned_DataModeling_Id", bound=VersionedDataModelingId)
 
 
 @dataclass
+class InstanceId:
+    _instance_type: ClassVar[Literal["node", "edge"]]
+    space: str
+    external_id: str
+
+    def dump(self, camel_case: bool = False, include_instance_type: bool = True) -> dict[str, str]:
+        output = asdict(self)
+        if include_instance_type:
+            output["instanceType" if camel_case else "instance_type"] = self._instance_type
+        return convert_all_keys_recursive(output, camel_case)
+
+    @classmethod
+    def load(cls: Type[T_InstanceId], data: dict) -> T_InstanceId:
+        return cls(
+            **convert_all_keys_to_snake_case(rename_and_exclude_keys(data, exclude={"instanceType", "instance_type"}))
+        )
+
+    @property
+    def instance_type(self) -> Literal["node", "edge"]:
+        return self._instance_type
+
+
+T_InstanceId = TypeVar("T_InstanceId", bound=InstanceId)
+
+
+@dataclass
+class NodeId(InstanceId):
+    _instance_type = "node"  # type: ignore[assignment]
+
+
+@dataclass
+class EdgeId(InstanceId):
+    _instance_type = "edge"  # type: ignore[assignment]
+
+
+@dataclass
 class ContainerId(DataModelingId):
     _type = "container"
 
+    def as_source_identifier(self) -> str:
+        return self.external_id
+
 
 @dataclass
 class ViewId(VersionedDataModelingId):
     _type = "view"
 
+    def as_source_identifier(self) -> str:
+        return f"{self.external_id}/{self.version}"
+
 
 @dataclass
 class DataModelId(VersionedDataModelingId):
     _type = "datamodel"
 
 
 ContainerIdentifier = Union[ContainerId, Tuple[str, str]]
 ViewIdentifier = Union[ViewId, Tuple[str, str], Tuple[str, str, str]]
 DataModelIdentifier = Union[DataModelId, Tuple[str, str], Tuple[str, str, str]]
+NodeIdentifier = Union[NodeId, Tuple[str, str, str]]
+EdgeIdentifier = Union[EdgeId, Tuple[str, str, str]]
 
-Id = Union[Tuple[str, str], Tuple[str, str, str], DataModelingId, VersionedDataModelingId]
+Id = Union[Tuple[str, str], Tuple[str, str, str], DataModelingId, VersionedDataModelingId, NodeId, EdgeId, InstanceId]
 
 
-def load_identifier(
-    ids: Id | Sequence[Id], id_type: Literal["container", "view", "data_model"]
+def _load_identifier(
+    ids: Id | Sequence[Id], id_type: Literal["container", "view", "data_model", "node", "edge", "all"]
 ) -> DataModelingIdentifierSequence:
     is_sequence = isinstance(ids, Sequence) and not (isinstance(ids, tuple) and isinstance(ids[0], str))
     is_view_or_data_model = id_type in {"view", "data_model"}
-
+    is_instance = id_type in {"node", "edge", "all"}
     id_list = cast(Sequence, ids)
     if not is_sequence:
         id_list = [ids]
 
+    def create_args(id_: Id) -> tuple[str, str, Optional[str], Optional[Literal["node", "edge"]]]:
+        if isinstance(id_, tuple) and is_instance:
+            if len(id_) == 3:
+                return id_[1], id_[2], None, id_type  # type: ignore[misc, return-value]
+            raise ValueError("Instance given as a tuple must have three elements, (instanceType, space, externalId)")
+        if isinstance(id_, tuple):
+            return id_[0], id_[1], id_[2] if len(id_) == 3 else None, None  # type: ignore[misc]
+        instance_type = None
+        if is_instance:
+            instance_type = "node" if isinstance(id_, NodeId) else "edge"
+        return id_.space, id_.external_id, getattr(id_, "version", None), instance_type  # type: ignore[return-value]
+
     return DataModelingIdentifierSequence(
-        identifiers=[
-            DataModelingIdentifier(
-                *id_ if isinstance(id_, tuple) else (id_.space, id_.external_id, getattr(id_, "version", None))
-            )
-            for id_ in id_list
-        ],
+        identifiers=[DataModelingIdentifier(*create_args(id_)) for id_ in id_list],
         is_singleton=not is_sequence and not is_view_or_data_model,
     )
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,19 +65,19 @@
         return SpaceApply(
             space=self.space,
             description=self.description,
             name=self.name,
         )
 
 
-class SpaceApplyList(CogniteResourceList):
+class SpaceApplyList(CogniteResourceList[SpaceApply]):
     _RESOURCE = SpaceApply
 
 
-class SpaceList(CogniteResourceList):
+class SpaceList(CogniteResourceList[Space]):
     _RESOURCE = Space
 
     def to_space_apply_list(self) -> SpaceApplyList:
         return SpaceApplyList(
             resources=[item.as_apply() for item in self.items],
             cognite_client=self._cognite_client,
         )
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_modeling/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -205,27 +205,27 @@
             name=self.name,
             filter=self.filter,
             implements=self.implements,
             properties=properties,
         )
 
 
-class ViewList(CogniteResourceList):
+class ViewList(CogniteResourceList[View]):
     _RESOURCE = View
 
     def to_view_apply(self) -> ViewApplyList:
         """Convert to a view an apply list.
 
         Returns:
             ViewApplyList: The view apply list.
         """
         return ViewApplyList(resources=[v.as_apply() for v in self.items])
 
 
-class ViewApplyList(CogniteResourceList):
+class ViewApplyList(CogniteResourceList[ViewApply]):
     _RESOURCE = ViewApply
 
 
 class ViewFilter(CogniteFilter):
     """Represent the filer arguments for the list endpoint.
 
     Args:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/data_sets.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,9 +166,9 @@
     def __init__(self, count: int = None, **kwargs: Any) -> None:
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
-class DataSetList(CogniteResourceList):
+class DataSetList(CogniteResourceList[DataSet]):
     _RESOURCE = DataSet
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/datapoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -637,15 +637,15 @@
         return truncated_datapoints
 
     def _repr_html_(self) -> str:
         is_synthetic_dps = self.error is not None
         return notebook_display_with_fallback(self, include_errors=is_synthetic_dps)
 
 
-class DatapointsArrayList(CogniteResourceList):
+class DatapointsArrayList(CogniteResourceList[DatapointsArray]):
     _RESOURCE = DatapointsArray
 
     def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
         super().__init__(resources, cognite_client)
 
         # Fix what happens for duplicated identifiers:
         ids = [dps.id for dps in self if dps.id is not None]
@@ -756,15 +756,15 @@
 
         Returns:
             List[Dict[str, Any]]: A list of dicts representing the instance.
         """
         return [dps.dump(camel_case, convert_timestamps) for dps in self]
 
 
-class DatapointsList(CogniteResourceList):
+class DatapointsList(CogniteResourceList[Datapoints]):
     _RESOURCE = Datapoints
 
     def __init__(self, resources: Collection[Any], cognite_client: CogniteClient = None):
         super().__init__(resources, cognite_client)
 
         # Fix what happens for duplicated identifiers:
         ids = [dps.id for dps in self if dps.id is not None]
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/events.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,9 +240,9 @@
         return EventUpdate._PrimitiveEventUpdate(self, "type")
 
     @property
     def subtype(self) -> _PrimitiveEventUpdate:
         return EventUpdate._PrimitiveEventUpdate(self, "subtype")
 
 
-class EventList(CogniteResourceList):
+class EventList(CogniteResourceList[Event]):
     _RESOURCE = Event
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/extractionpipelines.py`

 * *Files 2% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         return ExtractionPipelineUpdate._PrimitiveExtractionPipelineUpdate(self, "schedule")
 
     @property
     def contacts(self) -> _ListExtractionPipelineUpdate:
         return ExtractionPipelineUpdate._ListExtractionPipelineUpdate(self, "contacts")
 
 
-class ExtractionPipelineList(CogniteResourceList):
+class ExtractionPipelineList(CogniteResourceList[ExtractionPipeline]):
     _RESOURCE = ExtractionPipeline
 
 
 class ExtractionPipelineRun(CogniteResource):
     """A representation of an extraction pipeline run.
 
     Args:
@@ -244,15 +244,15 @@
         if camel_case:
             dct["externalId"] = dct.pop("extpipeExternalId", None)
         else:
             dct["external_id"] = dct.pop("extpipe_external_id", None)
         return dct
 
 
-class ExtractionPipelineRunList(CogniteResourceList):
+class ExtractionPipelineRunList(CogniteResourceList[ExtractionPipelineRun]):
     _RESOURCE = ExtractionPipelineRun
 
 
 class StringFilter(CogniteFilter):
     """Filter runs on substrings of the message
 
     Args:
@@ -350,9 +350,9 @@
             description=description,
             created_time=created_time,
             cognite_client=cognite_client,
         )
         self.config = config
 
 
-class ExtractionPipelineConfigRevisionList(CogniteResourceList):
+class ExtractionPipelineConfigRevisionList(CogniteResourceList[ExtractionPipelineConfigRevision]):
     _RESOURCE = ExtractionPipelineConfigRevision
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/files.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/files.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,9 +291,9 @@
     def __init__(self, count: int = None, **kwargs: Any) -> None:
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
-class FileMetadataList(CogniteResourceList):
+class FileMetadataList(CogniteResourceList[FileMetadata]):
     _RESOURCE = FileMetadata
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/functions.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,19 +260,19 @@
         self.name = name
         self.function_id = function_id
         self.function_external_id = function_external_id
         self.created_time = created_time
         self.cron_expression = cron_expression
 
 
-class FunctionSchedulesList(CogniteResourceList):
+class FunctionSchedulesList(CogniteResourceList[FunctionSchedule]):
     _RESOURCE = FunctionSchedule
 
 
-class FunctionList(CogniteResourceList):
+class FunctionList(CogniteResourceList[Function]):
     _RESOURCE = Function
 
 
 class FunctionCall(CogniteResource):
     """A representation of a Cognite Function call.
 
     Args:
@@ -337,15 +337,15 @@
 
     def wait(self) -> None:
         while self.status == "Running":
             self.update()
             time.sleep(1.0)
 
 
-class FunctionCallList(CogniteResourceList):
+class FunctionCallList(CogniteResourceList[FunctionCall]):
     _RESOURCE = FunctionCall
 
 
 class FunctionCallLogEntry(CogniteResource):
     """A log entry for a function call.
 
     Args:
@@ -360,15 +360,15 @@
         cognite_client: CogniteClient = None,
     ):
         self.timestamp = timestamp
         self.message = message
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class FunctionCallLog(CogniteResourceList):
+class FunctionCallLog(CogniteResourceList[FunctionCallLogEntry]):
     _RESOURCE = FunctionCallLogEntry
 
 
 class FunctionsLimits(CogniteResponse):
     """Service limits for the associated project.
 
     Args:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/geospatial.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         instance = cls(cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
         return instance
 
 
-class FeatureTypeList(CogniteResourceList):
+class FeatureTypeList(CogniteResourceList[FeatureType]):
     _RESOURCE = FeatureType
 
 
 class PropertyAndSearchSpec:
     """A representation of a feature type property and search spec."""
 
     def __init__(
@@ -169,15 +169,15 @@
     }
 
 
 def _to_feature_property_name(property_name: str) -> str:
     return to_snake_case(property_name) if property_name in RESERVED_PROPERTIES else property_name
 
 
-class FeatureList(CogniteResourceList):
+class FeatureList(CogniteResourceList[Feature]):
     _RESOURCE = Feature
 
     def to_geopandas(self, geometry: str, camel_case: bool = False) -> geopandas.GeoDataFrame:
         """Convert the instance into a GeoPandas GeoDataFrame.
 
         Args:
             geometry (str): The name of the feature type geometry property to use in the GeoDataFrame
@@ -297,15 +297,15 @@
         instance = cls(cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
         return instance
 
 
-class FeatureAggregateList(CogniteResourceList):
+class FeatureAggregateList(CogniteResourceList[FeatureAggregate]):
     _RESOURCE = FeatureAggregate
 
 
 class CoordinateReferenceSystem(CogniteResource):
     """A representation of a feature in the geospatial api."""
 
     def __init__(
@@ -325,15 +325,15 @@
         instance = cls(cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
         return instance
 
 
-class CoordinateReferenceSystemList(CogniteResourceList):
+class CoordinateReferenceSystemList(CogniteResourceList[CoordinateReferenceSystem]):
     _RESOURCE = CoordinateReferenceSystem
 
 
 class OrderSpec:
     """An order specification with respect to an property."""
 
     def __init__(self, property: str, direction: str):
@@ -412,15 +412,15 @@
         instance = cls(resource=resource, cognite_client=cognite_client)
         for key, value in resource.items():
             snake_case_key = to_snake_case(key)
             setattr(instance, snake_case_key, value)
         return instance
 
 
-class GeospatialComputedItemList(CogniteResourceList):
+class GeospatialComputedItemList(CogniteResourceList[GeospatialComputedItem]):
     "A list of items computed from geospatial."
     _RESOURCE = GeospatialComputedItem
 
 
 class GeospatialComputedResponse(CogniteResource):
     "The geospatial compute response."
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/iam.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         self.capabilities = capabilities
         self.id = id
         self.is_deleted = is_deleted
         self.deleted_time = deleted_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class GroupList(CogniteResourceList):
+class GroupList(CogniteResourceList[Group]):
     _RESOURCE = Group
 
 
 class SecurityCategory(CogniteResource):
     """No description.
 
     Args:
@@ -56,15 +56,15 @@
 
     def __init__(self, name: str = None, id: int = None, cognite_client: CogniteClient = None):
         self.name = name
         self.id = id
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class SecurityCategoryList(CogniteResourceList):
+class SecurityCategoryList(CogniteResourceList[SecurityCategory]):
     _RESOURCE = SecurityCategory
 
 
 class ProjectSpec(CogniteResponse):
     """A CDF project spec
 
     Args:
@@ -167,15 +167,15 @@
         self.type = type
         self.status = status
         self.creation_time = creation_time
         self.expiration_time = expiration_time
         self.client_id = client_id
 
 
-class SessionList(CogniteResourceList):
+class SessionList(CogniteResourceList[Session]):
     _RESOURCE = Session
 
 
 class ClientCredentials(CogniteResource):
     """Client credentials for session creation
 
     Args:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/labels.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/labels.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     ):
         self.name = name
         self.external_id_prefix = external_id_prefix
         self.data_set_ids = data_set_ids
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class LabelDefinitionList(CogniteResourceList):
+class LabelDefinitionList(CogniteResourceList[LabelDefinition]):
     _RESOURCE = LabelDefinition
 
 
 class Label(dict):
     """A label assigned to a resource.
 
     Args:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/raw.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/raw.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         Returns:
             pandas.DataFrame: The pandas DataFrame representing this instance.
         """
         pd = cast(Any, utils._auxiliary.local_import("pandas"))
         return pd.DataFrame([self.columns], [self.key])
 
 
-class RowList(CogniteResourceList):
+class RowList(CogniteResourceList[Row]):
     _RESOURCE = Row
 
     def to_pandas(self) -> pandas.DataFrame:  # type: ignore[override]
         """Convert the instance into a pandas DataFrame.
 
         Returns:
             pandas.DataFrame: The pandas DataFrame representing this instance.
@@ -84,15 +84,15 @@
             Union[Row, RowList]: List of tables in this database.
         """
         if key:
             return self._cognite_client.raw.rows.retrieve(db_name=self._db_name, table_name=self.name, key=key)
         return self._cognite_client.raw.rows.list(db_name=self._db_name, table_name=self.name, limit=limit)
 
 
-class TableList(CogniteResourceList):
+class TableList(CogniteResourceList[Table]):
     _RESOURCE = Table
 
 
 class Database(CogniteResource):
     """A NoSQL database to store customer data.
 
     Args:
@@ -114,9 +114,9 @@
 
         Returns:
             TableList: List of tables in this database.
         """
         return self._cognite_client.raw.tables.list(db_name=self.name, limit=limit)
 
 
-class DatabaseList(CogniteResourceList):
+class DatabaseList(CogniteResourceList[Database]):
     _RESOURCE = Database
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/relationships.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,9 +229,9 @@
         return RelationshipUpdate._PrimitiveRelationshipUpdate(self, "confidence")
 
     @property
     def labels(self) -> _LabelRelationshipUpdate:
         return RelationshipUpdate._LabelRelationshipUpdate(self, "labels")
 
 
-class RelationshipList(CogniteResourceList):
+class RelationshipList(CogniteResourceList[Relationship]):
     _RESOURCE = Relationship
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/sequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
     def __init__(self, count: int = None, **kwargs: Any):
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
-class SequenceList(CogniteResourceList):
+class SequenceList(CogniteResourceList[Sequence]):
     _RESOURCE = Sequence
 
 
 class SequenceData(CogniteResource):
     """An object representing a list of rows from a sequence.
 
     Args:
@@ -434,15 +434,15 @@
         Returns:
             List of column value types
         """
         assert self.columns is not None
         return [cast(str, c.get("valueType")) for c in self.columns]
 
 
-class SequenceDataList(CogniteResourceList):
+class SequenceDataList(CogniteResourceList[SequenceData]):
     _RESOURCE = SequenceData
 
     def __str__(self) -> str:
         return json.dumps(self.dump(), indent=4)
 
     def to_pandas(self, column_names: str = "externalId|columnExternalId") -> pandas.DataFrame:  # type: ignore[override]
         """Convert the sequence data list into a pandas DataFrame. Each column will be a sequence.
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/shared.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/templates.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
         self.owners = owners
         self.data_set_id = data_set_id
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class TemplateGroupList(CogniteResourceList):
+class TemplateGroupList(CogniteResourceList[TemplateGroup]):
     _RESOURCE = TemplateGroup
 
 
 class TemplateGroupVersion(CogniteResource):
     """
     A Template Group Version supports specifying different conflict modes, which is used when an existing schema already exists.
 
@@ -83,15 +83,15 @@
         self.version = version
         self.conflict_mode = conflict_mode
         self.created_time = created_time
         self.last_updated_time = last_updated_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class TemplateGroupVersionList(CogniteResourceList):
+class TemplateGroupVersionList(CogniteResourceList[TemplateGroupVersion]):
     _RESOURCE = TemplateGroupVersion
 
 
 class ConstantResolver(CogniteResource):
     """Resolves a field to a constant value. The value can be of any supported JSON type.
 
     Args:
@@ -429,17 +429,17 @@
 class GraphQlResponse(CogniteResource):
     def __init__(self, data: Any = None, errors: List[GraphQlError] = None, cognite_client: CogniteClient = None):
         self.data = data
         self.errors = errors
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class TemplateInstanceList(CogniteResourceList):
+class TemplateInstanceList(CogniteResourceList[TemplateInstance]):
     _RESOURCE = TemplateInstance
 
 
-class ViewList(CogniteResourceList):
+class ViewList(CogniteResourceList[View]):
     _RESOURCE = View
 
 
-class ViewResolveList(CogniteResourceList):
+class ViewResolveList(CogniteResourceList[ViewResolveItem]):
     _RESOURCE = ViewResolveItem
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/three_d.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         return ThreeDModelUpdate._PrimitiveThreeDModelUpdate(self, "name")
 
     @property
     def metadata(self) -> _ObjectThreeDModelUpdate:
         return ThreeDModelUpdate._ObjectThreeDModelUpdate(self, "metadata")
 
 
-class ThreeDModelList(CogniteResourceList):
+class ThreeDModelList(CogniteResourceList[ThreeDModel]):
     _RESOURCE = ThreeDModel
 
 
 class ThreeDModelRevision(CogniteResource):
     """No description.
 
     Args:
@@ -234,15 +234,15 @@
         return ThreeDModelRevisionUpdate._ObjectThreeDModelRevisionUpdate(self, "camera")
 
     @property
     def metadata(self) -> _ObjectThreeDModelRevisionUpdate:
         return ThreeDModelRevisionUpdate._ObjectThreeDModelRevisionUpdate(self, "metadata")
 
 
-class ThreeDModelRevisionList(CogniteResourceList):
+class ThreeDModelRevisionList(CogniteResourceList[ThreeDModelRevision]):
     _RESOURCE = ThreeDModelRevision
 
 
 class ThreeDNode(CogniteResource):
     """No description.
 
     Args:
@@ -284,15 +284,15 @@
         instance = super()._load(resource, cognite_client)
         if isinstance(resource, Dict):
             if instance.bounding_box is not None:
                 instance.bounding_box = BoundingBox3D(**instance.bounding_box)
         return instance
 
 
-class ThreeDNodeList(CogniteResourceList):
+class ThreeDNodeList(CogniteResourceList[ThreeDNode]):
     _RESOURCE = ThreeDNode
 
 
 class ThreeDAssetMapping(CogniteResource):
     """No description.
 
     Args:
@@ -314,9 +314,9 @@
         self.node_id = node_id
         self.asset_id = asset_id
         self.tree_index = tree_index
         self.subtree_size = subtree_size
         self._cognite_client = cast("CogniteClient", cognite_client)
 
 
-class ThreeDAssetMappingList(CogniteResourceList):
+class ThreeDAssetMappingList(CogniteResourceList[ThreeDAssetMapping]):
     _RESOURCE = ThreeDAssetMapping
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/time_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,9 +283,9 @@
     def __init__(self, count: int = None, **kwargs: Any) -> None:
         self.count = count
         self.update(kwargs)
 
     count = CognitePropertyClassUtil.declare_property("count")
 
 
-class TimeSeriesList(CogniteResourceList):
+class TimeSeriesList(CogniteResourceList[TimeSeries]):
     _RESOURCE = TimeSeries
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/transformations/jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     @classmethod
     def _load(cls, resource: Union[Dict, str], cognite_client: CogniteClient = None) -> TransformationJobMetric:
         instance = super()._load(resource, cognite_client)
         return instance
 
 
-class TransformationJobMetricList(CogniteResourceList):
+class TransformationJobMetricList(CogniteResourceList[TransformationJobMetric]):
     _RESOURCE = TransformationJobMetric
 
 
 class TransformationJob(CogniteResource):
     """The transformation job resource allows following the status of execution of a transformation run.
 
     Args:
@@ -252,15 +252,15 @@
             instance.destination = _load_destination_dct(instance.destination)
         return instance
 
     def __hash__(self) -> int:
         return hash(self.id)
 
 
-class TransformationJobList(CogniteResourceList):
+class TransformationJobList(CogniteResourceList[TransformationJob]):
     _RESOURCE = TransformationJob
 
 
 class TransformationJobFilter(CogniteFilter):
     """
 
     Args:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/transformations/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.last_updated_time = last_updated_time
         self._cognite_client = cast("CogniteClient", cognite_client)
 
     def __hash__(self) -> int:
         return hash(self.id)
 
 
-class TransformationNotificationList(CogniteResourceList):
+class TransformationNotificationList(CogniteResourceList[TransformationNotification]):
     _RESOURCE = TransformationNotification
 
 
 class TransformationNotificationFilter(CogniteFilter):
     """
 
     Args:
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/transformations/schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,9 +65,9 @@
         return TransformationScheduleUpdate._PrimitiveTransformationScheduleUpdate(self, "interval")
 
     @property
     def is_paused(self) -> _PrimitiveTransformationScheduleUpdate:
         return TransformationScheduleUpdate._PrimitiveTransformationScheduleUpdate(self, "isPaused")
 
 
-class TransformationScheduleList(CogniteResourceList):
+class TransformationScheduleList(CogniteResourceList[TransformationSchedule]):
     _RESOURCE = TransformationSchedule
```

### Comparing `cognite_sdk-6.3.2/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.4.0/cognite/client/data_classes/transformations/schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,9 +65,9 @@
             elif instance_type == "map":
                 instance.type = TransformationSchemaMapType(**snake_dict)
         elif isinstance(instance.type, str):
             instance.type = TransformationSchemaType(type=instance.type)
         return instance
 
 
-class TransformationSchemaColumnList(CogniteResourceList):
+class TransformationSchemaColumnList(CogniteResourceList[TransformationSchemaColumn]):
     _RESOURCE = TransformationSchemaColumn
```

### Comparing `cognite_sdk-6.3.2/cognite/client/exceptions.py` & `cognite_sdk-6.4.0/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/testing.py` & `cognite_sdk-6.4.0/cognite/client/testing.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from cognite.client import CogniteClient
 from cognite.client._api.annotations import AnnotationsAPI
 from cognite.client._api.assets import AssetsAPI
 from cognite.client._api.data_modeling import DataModelingAPI
 from cognite.client._api.data_modeling.containers import ContainersAPI
 from cognite.client._api.data_modeling.data_models import DataModelsAPI
+from cognite.client._api.data_modeling.instances import InstancesAPI
 from cognite.client._api.data_modeling.spaces import SpacesAPI
 from cognite.client._api.data_modeling.views import ViewsAPI
 from cognite.client._api.data_sets import DataSetsAPI
 from cognite.client._api.datapoints import DatapointsAPI
 from cognite.client._api.diagrams import DiagramsAPI
 from cognite.client._api.entity_matching import EntityMatchingAPI
 from cognite.client._api.events import EventsAPI
@@ -77,14 +78,15 @@
         self.assets = MagicMock(spec_set=AssetsAPI)
 
         self.data_modeling = MagicMock(spec=DataModelingAPI)
         self.data_modeling.containers = MagicMock(spec_set=ContainersAPI)
         self.data_modeling.data_models = MagicMock(spec_set=DataModelsAPI)
         self.data_modeling.spaces = MagicMock(spec_set=SpacesAPI)
         self.data_modeling.views = MagicMock(spec_set=ViewsAPI)
+        self.data_modeling.instances = MagicMock(spec_set=InstancesAPI)
 
         self.data_sets = MagicMock(spec_set=DataSetsAPI)
 
         self.diagrams = MagicMock(spec_set=DiagramsAPI)
         self.entity_matching = MagicMock(spec_set=EntityMatchingAPI)
         self.events = MagicMock(spec_set=EventsAPI)
```

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/__init__.py` & `cognite_sdk-6.4.0/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.4.0/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.4.0/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_graph.py` & `cognite_sdk-6.4.0/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_identifier.py` & `cognite_sdk-6.4.0/cognite/client/utils/_identifier.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numbers
 from typing import (
     Dict,
     Generic,
     Iterable,
     List,
+    Literal,
     NoReturn,
     Optional,
     Protocol,
     Sequence,
     Tuple,
     TypeVar,
     Union,
@@ -74,26 +75,35 @@
         return {self.name(camel_case): self.__value}
 
     def as_tuple(self, camel_case: bool = True) -> Tuple[str, T_ID]:
         return self.name(camel_case), self.__value
 
 
 class DataModelingIdentifier:
-    def __init__(self, space: str, external_id: str | None = None, version: str | None = None):
+    def __init__(
+        self,
+        space: str,
+        external_id: str | None = None,
+        version: str | None = None,
+        instance_type: Literal["node", "edge"] | None = None,
+    ):
         self.__space = space
         self.__external_id = external_id
         self.__version = version
+        self.__instance_type = instance_type
 
     def as_dict(self, camel_case: bool = True) -> dict[str, str]:
         output = {"space": self.__space}
         if self.__external_id is not None:
             key = "externalId" if camel_case else "external_id"
             output[key] = self.__external_id
         if self.__version is not None:
             output["version"] = self.__version
+        if self.__instance_type is not None:
+            output["instanceType"] = self.__instance_type
         return output
 
     def as_primitive(self) -> NoReturn:
         raise AttributeError(f"Not supported for {type(self).__name__} implementation")
 
 
 class ExternalId(Identifier[str]):
```

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_logging.py` & `cognite_sdk-6.4.0/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.4.0/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.4.0/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.4.0/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_text.py` & `cognite_sdk-6.4.0/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_time.py` & `cognite_sdk-6.4.0/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_validation.py` & `cognite_sdk-6.4.0/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.4.0/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.3.2/pyproject.toml` & `cognite_sdk-6.4.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.3.2"
+version = "6.4.0"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.3.2/PKG-INFO` & `cognite_sdk-6.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.3.2
+Version: 6.4.0
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
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.3.2 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.0 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

