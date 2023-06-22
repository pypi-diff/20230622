# Comparing `tmp/cognite_sdk-6.4.5.tar.gz` & `tmp/cognite_sdk-6.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_sdk-6.4.5.tar", max compression
+gzip compressed data, was "cognite_sdk-6.4.7.tar", max compression
```

## Comparing `cognite_sdk-6.4.5.tar` & `cognite_sdk-6.4.7.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0    11349 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/LICENSE
--rw-r--r--   0        0        0     3945 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/README.md
--rw-r--r--   0        0        0      574 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/__init__.py
--rw-r--r--   0        0        0        0 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/_api/__init__.py
--rw-r--r--   0        0        0     6979 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/_api/annotations.py
--rw-r--r--   0        0        0    49083 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/_api/assets.py
--rw-r--r--   0        0        0     1157 2023-06-21 11:17:08.516638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/__init__.py
--rw-r--r--   0        0        0     7857 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/containers.py
--rw-r--r--   0        0        0     8393 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/data_models.py
--rw-r--r--   0        0        0    26302 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/instances.py
--rw-r--r--   0        0        0     6424 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/spaces.py
--rw-r--r--   0        0        0     7857 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_modeling/views.py
--rw-r--r--   0        0        0    11025 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/data_sets.py
--rw-r--r--   0        0        0    54681 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/datapoint_tasks.py
--rw-r--r--   0        0        0    87459 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/datapoints.py
--rw-r--r--   0        0        0    12424 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/diagrams.py
--rw-r--r--   0        0        0    12245 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/entity_matching.py
--rw-r--r--   0        0        0    21276 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/events.py
--rw-r--r--   0        0        0    17192 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/extractionpipelines.py
--rw-r--r--   0        0        0    41485 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/files.py
--rw-r--r--   0        0        0    45301 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/functions.py
--rw-r--r--   0        0        0    49823 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/geospatial.py
--rw-r--r--   0        0        0     9466 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/iam.py
--rw-r--r--   0        0        0     6052 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/labels.py
--rw-r--r--   0        0        0    24648 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/raw.py
--rw-r--r--   0        0        0    22824 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/relationships.py
--rw-r--r--   0        0        0    37975 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/sequences.py
--rw-r--r--   0        0        0     7909 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/synthetic_time_series.py
--rw-r--r--   0        0        0    32072 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/templates.py
--rw-r--r--   0        0        0    27887 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/three_d.py
--rw-r--r--   0        0        0    19140 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/time_series.py
--rw-r--r--   0        0        0    21811 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/__init__.py
--rw-r--r--   0        0        0     4983 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/jobs.py
--rw-r--r--   0        0        0     4589 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/notifications.py
--rw-r--r--   0        0        0     9525 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/schedules.py
--rw-r--r--   0        0        0     1869 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/transformations/schema.py
--rw-r--r--   0        0        0     5910 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api/vision.py
--rw-r--r--   0        0        0    38099 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_api_client.py
--rw-r--r--   0        0        0     5391 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_cognite_client.py
--rw-r--r--   0        0        0      215 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_constants.py
--rw-r--r--   0        0        0     6937 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_http_client.py
--rw-r--r--   0        0        0      553 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response.proto
--rw-r--r--   0        0        0     1985 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-21 11:17:08.520638 cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0      811 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto/data_points.proto
--rw-r--r--   0        0        0     2495 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto/data_points_pb2.pyi
--rw-r--r--   0        0        0     9509 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_point_list_response_pb2.py
--rw-r--r--   0        0        0     3364 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
--rw-r--r--   0        0        0    15421 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_points_pb2.py
--rw-r--r--   0        0        0     5321 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_points_pb2.pyi
--rw-r--r--   0        0        0       91 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/_version.py
--rw-r--r--   0        0        0      300 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/beta.py
--rw-r--r--   0        0        0     4508 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/config.py
--rw-r--r--   0        0        0    19252 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/credentials.py
--rw-r--r--   0        0        0     8794 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/__init__.py
--rw-r--r--   0        0        0    19074 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/_base.py
--rw-r--r--   0        0        0        0 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/__init__.py
--rw-r--r--   0        0        0     1595 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/images.py
--rw-r--r--   0        0        0     2936 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/primitives.py
--rw-r--r--   0        0        0     8753 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/annotations.py
--rw-r--r--   0        0        0    34185 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/assets.py
--rw-r--r--   0        0        0    33708 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/contextualization.py
--rw-r--r--   0        0        0     3629 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/__init__.py
--rw-r--r--   0        0        0     1224 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/_core.py
--rw-r--r--   0        0        0     1239 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/_validation.py
--rw-r--r--   0        0        0    12076 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/containers.py
--rw-r--r--   0        0        0     7267 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/data_models.py
--rw-r--r--   0        0        0     4019 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/data_types.py
--rw-r--r--   0        0        0     9519 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/filters.py
--rw-r--r--   0        0        0     6238 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/ids.py
--rw-r--r--   0        0        0    28930 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/instances.py
--rw-r--r--   0        0        0     2543 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/spaces.py
--rw-r--r--   0        0        0    14855 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/views.py
--rw-r--r--   0        0        0     6691 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/data_sets.py
--rw-r--r--   0        0        0    33969 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/datapoints.py
--rw-r--r--   0        0        0    11015 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/events.py
--rw-r--r--   0        0        0    14376 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/extractionpipelines.py
--rw-r--r--   0        0        0    13671 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/files.py
--rw-r--r--   0        0        0    16695 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/functions.py
--rw-r--r--   0        0        0    16556 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/geospatial.py
--rw-r--r--   0        0        0     6037 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/iam.py
--rw-r--r--   0        0        0     5885 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/labels.py
--rw-r--r--   0        0        0     4120 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/raw.py
--rw-r--r--   0        0        0    12267 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/relationships.py
--rw-r--r--   0        0        0    17675 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/sequences.py
--rw-r--r--   0        0        0     8699 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/shared.py
--rw-r--r--   0        0        0    16892 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/templates.py
--rw-r--r--   0        0        0    11855 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/three_d.py
--rw-r--r--   0        0        0    12090 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/time_series.py
--rw-r--r--   0        0        0    23040 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/__init__.py
--rw-r--r--   0        0        0    12116 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/common.py
--rw-r--r--   0        0        0    11469 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/jobs.py
--rw-r--r--   0        0        0     2382 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/notifications.py
--rw-r--r--   0        0        0     2475 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/schedules.py
--rw-r--r--   0        0        0     2770 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/data_classes/transformations/schema.py
--rw-r--r--   0        0        0     9383 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/py.typed
--rw-r--r--   0        0        0     9006 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/testing.py
--rw-r--r--   0        0        0      534 2023-06-21 11:17:08.524638 cognite_sdk-6.4.5/cognite/client/utils/__init__.py
--rw-r--r--   0        0        0     8165 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_auxiliary.py
--rw-r--r--   0        0        0     9853 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_concurrency.py
--rw-r--r--   0        0        0     1396 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_graph.py
--rw-r--r--   0        0        0     7684 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_identifier.py
--rw-r--r--   0        0        0     2134 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_logging.py
--rw-r--r--   0        0        0     3548 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_pandas_helpers.py
--rw-r--r--   0        0        0     6188 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_priority_tpe.py
--rw-r--r--   0        0        0     4260 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_pyodide_helpers.py
--rw-r--r--   0        0        0     2981 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_text.py
--rw-r--r--   0        0        0    24536 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_time.py
--rw-r--r--   0        0        0     1820 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_validation.py
--rw-r--r--   0        0        0     3341 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/cognite/client/utils/_version_checker.py
--rw-r--r--   0        0        0     2151 2023-06-21 11:17:08.528638 cognite_sdk-6.4.5/pyproject.toml
--rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.5/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/LICENSE
+-rw-r--r--   0        0        0     3945 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/README.md
+-rw-r--r--   0        0        0      574 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/__init__.py
+-rw-r--r--   0        0        0     6979 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/annotations.py
+-rw-r--r--   0        0        0    49083 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/assets.py
+-rw-r--r--   0        0        0     1157 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/data_modeling/__init__.py
+-rw-r--r--   0        0        0     7860 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/data_modeling/containers.py
+-rw-r--r--   0        0        0     8361 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/data_modeling/data_models.py
+-rw-r--r--   0        0        0    26302 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/data_modeling/instances.py
+-rw-r--r--   0        0        0     6424 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/data_modeling/spaces.py
+-rw-r--r--   0        0        0     7832 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/data_modeling/views.py
+-rw-r--r--   0        0        0    11025 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/data_sets.py
+-rw-r--r--   0        0        0    54681 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/datapoint_tasks.py
+-rw-r--r--   0        0        0    87459 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/datapoints.py
+-rw-r--r--   0        0        0    12424 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/diagrams.py
+-rw-r--r--   0        0        0    12245 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/entity_matching.py
+-rw-r--r--   0        0        0    21276 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/events.py
+-rw-r--r--   0        0        0    17192 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/extractionpipelines.py
+-rw-r--r--   0        0        0    41485 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/files.py
+-rw-r--r--   0        0        0    45301 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/functions.py
+-rw-r--r--   0        0        0    49823 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/geospatial.py
+-rw-r--r--   0        0        0     9466 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/iam.py
+-rw-r--r--   0        0        0     6052 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/labels.py
+-rw-r--r--   0        0        0    24648 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/raw.py
+-rw-r--r--   0        0        0    22824 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/relationships.py
+-rw-r--r--   0        0        0    37975 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/sequences.py
+-rw-r--r--   0        0        0     7909 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/synthetic_time_series.py
+-rw-r--r--   0        0        0    32072 2023-06-22 12:51:49.911110 cognite_sdk-6.4.7/cognite/client/_api/templates.py
+-rw-r--r--   0        0        0    27887 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api/three_d.py
+-rw-r--r--   0        0        0    19140 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api/time_series.py
+-rw-r--r--   0        0        0    21811 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api/transformations/__init__.py
+-rw-r--r--   0        0        0     4983 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api/transformations/jobs.py
+-rw-r--r--   0        0        0     4589 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api/transformations/notifications.py
+-rw-r--r--   0        0        0     9525 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api/transformations/schedules.py
+-rw-r--r--   0        0        0     1869 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api/transformations/schema.py
+-rw-r--r--   0        0        0     5910 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api/vision.py
+-rw-r--r--   0        0        0    38099 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_api_client.py
+-rw-r--r--   0        0        0     5391 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_cognite_client.py
+-rw-r--r--   0        0        0      215 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_constants.py
+-rw-r--r--   0        0        0     6937 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_http_client.py
+-rw-r--r--   0        0        0      553 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto/data_point_list_response.proto
+-rw-r--r--   0        0        0     1985 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0      811 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto/data_points.proto
+-rw-r--r--   0        0        0     2495 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto/data_points_pb2.pyi
+-rw-r--r--   0        0        0     9509 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto_legacy/data_point_list_response_pb2.py
+-rw-r--r--   0        0        0     3364 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi
+-rw-r--r--   0        0        0    15421 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto_legacy/data_points_pb2.py
+-rw-r--r--   0        0        0     5321 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_proto_legacy/data_points_pb2.pyi
+-rw-r--r--   0        0        0       91 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/_version.py
+-rw-r--r--   0        0        0      300 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/beta.py
+-rw-r--r--   0        0        0     4508 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/config.py
+-rw-r--r--   0        0        0    19252 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/credentials.py
+-rw-r--r--   0        0        0     8794 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/__init__.py
+-rw-r--r--   0        0        0    19074 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/_base.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/annotation_types/__init__.py
+-rw-r--r--   0        0        0     1595 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/annotation_types/images.py
+-rw-r--r--   0        0        0     2936 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/annotation_types/primitives.py
+-rw-r--r--   0        0        0     8753 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/annotations.py
+-rw-r--r--   0        0        0    34185 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/assets.py
+-rw-r--r--   0        0        0    33708 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/contextualization.py
+-rw-r--r--   0        0        0     3629 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/__init__.py
+-rw-r--r--   0        0        0     1224 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/_core.py
+-rw-r--r--   0        0        0     1239 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/_validation.py
+-rw-r--r--   0        0        0    12057 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/containers.py
+-rw-r--r--   0        0        0     7395 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/data_models.py
+-rw-r--r--   0        0        0     4019 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/data_types.py
+-rw-r--r--   0        0        0     9519 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/filters.py
+-rw-r--r--   0        0        0     6593 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/ids.py
+-rw-r--r--   0        0        0    28930 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/instances.py
+-rw-r--r--   0        0        0     2527 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/spaces.py
+-rw-r--r--   0        0        0    14836 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/views.py
+-rw-r--r--   0        0        0     6691 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/data_sets.py
+-rw-r--r--   0        0        0    33969 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/datapoints.py
+-rw-r--r--   0        0        0    11015 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/events.py
+-rw-r--r--   0        0        0    14376 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/extractionpipelines.py
+-rw-r--r--   0        0        0    13671 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/files.py
+-rw-r--r--   0        0        0    16695 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/functions.py
+-rw-r--r--   0        0        0    16556 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/geospatial.py
+-rw-r--r--   0        0        0     6037 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/iam.py
+-rw-r--r--   0        0        0     5885 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/labels.py
+-rw-r--r--   0        0        0     4120 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/raw.py
+-rw-r--r--   0        0        0    12267 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/relationships.py
+-rw-r--r--   0        0        0    17675 2023-06-22 12:51:49.915110 cognite_sdk-6.4.7/cognite/client/data_classes/sequences.py
+-rw-r--r--   0        0        0     8699 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/shared.py
+-rw-r--r--   0        0        0    16892 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/templates.py
+-rw-r--r--   0        0        0    11855 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/three_d.py
+-rw-r--r--   0        0        0    12090 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/time_series.py
+-rw-r--r--   0        0        0    23040 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/transformations/__init__.py
+-rw-r--r--   0        0        0    12116 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/transformations/common.py
+-rw-r--r--   0        0        0    11469 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/transformations/jobs.py
+-rw-r--r--   0        0        0     2382 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/transformations/notifications.py
+-rw-r--r--   0        0        0     2475 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/transformations/schedules.py
+-rw-r--r--   0        0        0     2770 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/data_classes/transformations/schema.py
+-rw-r--r--   0        0        0     9383 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/py.typed
+-rw-r--r--   0        0        0     9006 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/testing.py
+-rw-r--r--   0        0        0      534 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/__init__.py
+-rw-r--r--   0        0        0     8165 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_auxiliary.py
+-rw-r--r--   0        0        0     9853 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_concurrency.py
+-rw-r--r--   0        0        0     1396 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_graph.py
+-rw-r--r--   0        0        0     7684 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_identifier.py
+-rw-r--r--   0        0        0     2134 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_logging.py
+-rw-r--r--   0        0        0     3548 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_pandas_helpers.py
+-rw-r--r--   0        0        0     6188 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_priority_tpe.py
+-rw-r--r--   0        0        0     4260 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_pyodide_helpers.py
+-rw-r--r--   0        0        0     2981 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_text.py
+-rw-r--r--   0        0        0    24536 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_time.py
+-rw-r--r--   0        0        0     1820 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_validation.py
+-rw-r--r--   0        0        0     3341 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/cognite/client/utils/_version_checker.py
+-rw-r--r--   0        0        0     2151 2023-06-22 12:51:49.919110 cognite_sdk-6.4.7/pyproject.toml
+-rw-r--r--   0        0        0     5625 1970-01-01 00:00:00.000000 cognite_sdk-6.4.7/PKG-INFO
```

### Comparing `cognite_sdk-6.4.5/LICENSE` & `cognite_sdk-6.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/README.md` & `cognite_sdk-6.4.7/README.md`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/__init__.py` & `cognite_sdk-6.4.7/cognite/client/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/annotations.py` & `cognite_sdk-6.4.7/cognite/client/_api/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/assets.py` & `cognite_sdk-6.4.7/cognite/client/_api/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/__init__.py` & `cognite_sdk-6.4.7/cognite/client/_api/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/containers.py` & `cognite_sdk-6.4.7/cognite/client/_api/data_modeling/containers.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.containers import (
     Container,
     ContainerApply,
     ContainerFilter,
     ContainerList,
 )
-from cognite.client.data_classes.data_modeling.ids import ContainerIdentifier, DataModelingId, _load_identifier
+from cognite.client.data_classes.data_modeling.ids import (
+    ContainerId,
+    ContainerIdentifier,
+    _load_identifier,
+)
 
 
 class ContainersAPI(APIClient):
     _RESOURCE_PATH = "/models/containers"
 
     @overload
     def __call__(
@@ -95,25 +99,25 @@
 
         Examples:
 
                 >>> from cognite.client import CogniteClient
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.containers.retrieve(('mySpace', 'myContainer'))
 
-            Fetch using the DataModelingId::
+            Fetch using the ContainerId::
 
                 >>> from cognite.client import CogniteClient
-                >>> from cognite.client.data_modeling import DataModelingId
+                >>> from cognite.client.data_modeling import ContainerId
                 >>> c = CogniteClient()
-                >>> res = c.data_modeling.containers.retrieve(DataModelingId(space='mySpace', external_id='myContainer'))
+                >>> res = c.data_modeling.containers.retrieve(ContainerId(space='mySpace', external_id='myContainer'))
         """
         identifier = _load_identifier(ids, "container")
         return self._retrieve_multiple(list_cls=ContainerList, resource_cls=Container, identifiers=identifier)
 
-    def delete(self, id: ContainerIdentifier | Sequence[ContainerIdentifier]) -> list[DataModelingId]:
+    def delete(self, id: ContainerIdentifier | Sequence[ContainerIdentifier]) -> list[ContainerId]:
         """`Delete one or more containers <https://docs.cognite.com/api/v1/#operation/deleteContainers>`_
 
         Args:
             id (ContainerId | Sequence[ContainerId): The container identifier(s).
         Returns:
             The container(s) which has been deleted. Empty list if nothing was deleted.
         Examples:
@@ -124,15 +128,15 @@
                 >>> c = CogniteClient()
                 >>> c.data_modeling.containers.delete(("mySpace", "myContainer"))
         """
         deleted_containers = cast(
             list,
             self._delete_multiple(identifiers=_load_identifier(id, "container"), wrap_ids=True, returns_items=True),
         )
-        return [DataModelingId(space=item["space"], external_id=item["externalId"]) for item in deleted_containers]
+        return [ContainerId(space=item["space"], external_id=item["externalId"]) for item in deleted_containers]
 
     def list(
         self, space: str | None = None, limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT, include_global: bool = False
     ) -> ContainerList:
         """`List containers <https://docs.cognite.com/api/v1/#operation/listContainers>`_
 
         Args:
@@ -196,11 +200,11 @@
         Examples:
 
             Create new containers:
 
                 >>> from cognite.client import CogniteClient
                 >>> import cognite.client.data_classes.data_modeling as models
                 >>> c = CogniteClient()
-                >>> containers = [models.Container(space="mySpace",properties={"name": models.ContainerProperty(type=models.TextType, name="name")})]
-                >>> res = c.data_modeling.containers.create(containers)
+                >>> containers = [models.ContainerApply(space="mySpace",properties={"name": models.ContainerProperty(type=models.TextType, name="name")})]
+                >>> res = c.data_modeling.containers.apply(containers)
         """
         return self._create_multiple(list_cls=ContainerList, resource_cls=Container, items=container)
```

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/data_models.py` & `cognite_sdk-6.4.7/cognite/client/_api/data_modeling/data_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
 from cognite.client.data_classes.data_modeling.data_models import (
     DataModel,
     DataModelApply,
     DataModelFilter,
     DataModelList,
 )
-from cognite.client.data_classes.data_modeling.ids import DataModelIdentifier, VersionedDataModelingId, _load_identifier
+from cognite.client.data_classes.data_modeling.ids import (
+    DataModelId,
+    DataModelIdentifier,
+    _load_identifier,
+)
 
 
 class DataModelsAPI(APIClient):
     _RESOURCE_PATH = "/models/datamodels"
 
     @overload
     def __call__(
@@ -101,15 +105,15 @@
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.data_models.retrieve(("mySpace", "myDataModel", "v1"))
 
         """
         identifier = _load_identifier(ids, "data_model")
         return self._retrieve_multiple(list_cls=DataModelList, resource_cls=DataModel, identifiers=identifier)
 
-    def delete(self, ids: DataModelIdentifier | Sequence[DataModelIdentifier]) -> list[VersionedDataModelingId]:
+    def delete(self, ids: DataModelIdentifier | Sequence[DataModelIdentifier]) -> list[DataModelId]:
         """`Delete one or more data model <https://docs.cognite.com/api/v1/#operation/deleteDataModels>`_
 
         Args:
             ids (DataModelId | Sequence[DataModelId]): Data Model identifier(s).
         Returns:
             The data_model(s) which has been deleted. None if nothing was deleted.
         Examples:
@@ -120,17 +124,15 @@
                 >>> c = CogniteClient()
                 >>> c.data_modeling.data_models.delete(("mySpace", "myDataModel", "v1"))
         """
         deleted_data_models = cast(
             list,
             self._delete_multiple(identifiers=_load_identifier(ids, "data_model"), wrap_ids=True, returns_items=True),
         )
-        return [
-            VersionedDataModelingId(item["space"], item["externalId"], item["version"]) for item in deleted_data_models
-        ]
+        return [DataModelId(item["space"], item["externalId"], item["version"]) for item in deleted_data_models]
 
     def list(
         self,
         limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT,
         space: str | None = None,
         inline_views: bool = False,
         all_versions: bool = False,
@@ -202,12 +204,12 @@
         Examples:
 
             Create new data model::
 
                 >>> from cognite.client import CogniteClient
                 >>> import cognite.client.data_classes.data_modeling as models
                 >>> c = CogniteClient()
-                >>> data_models = [models.DataModel(space="mySpace",external_id="myDataModel",version="v1",is_global=,last_updated_time=),
-                ... DataModel(space="mySpace",external_id="myOtherDataModel",version="v1",is_global=,last_updated_time=)]
-                >>> res = c.data_modeling.data_models.create(data_models)
+                >>> data_models = [models.DataModelApply(space="mySpace",external_id="myDataModel",version="v1",is_global=,last_updated_time=),
+                ... DataModelApply(space="mySpace",external_id="myOtherDataModel",version="v1",is_global=,last_updated_time=)]
+                >>> res = c.data_modeling.data_models.apply(data_models)
         """
         return self._create_multiple(list_cls=DataModelList, resource_cls=DataModel, items=data_model)
```

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/instances.py` & `cognite_sdk-6.4.7/cognite/client/_api/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/spaces.py` & `cognite_sdk-6.4.7/cognite/client/_api/data_modeling/spaces.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/data_modeling/views.py` & `cognite_sdk-6.4.7/cognite/client/_api/data_modeling/views.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from __future__ import annotations
 
 from typing import Iterator, Sequence, cast, overload
 
 from cognite.client._api_client import APIClient
 from cognite.client._constants import DATA_MODELING_LIST_LIMIT_DEFAULT
-from cognite.client.data_classes.data_modeling.ids import VersionedDataModelingId, ViewIdentifier, _load_identifier
+from cognite.client.data_classes.data_modeling.ids import (
+    ViewId,
+    ViewIdentifier,
+    _load_identifier,
+)
 from cognite.client.data_classes.data_modeling.views import View, ViewApply, ViewFilter, ViewList
 
 
 class ViewsAPI(APIClient):
     _RESOURCE_PATH = "/models/views"
 
     @overload
@@ -95,15 +99,15 @@
                 >>> c = CogniteClient()
                 >>> res = c.data_modeling.views.retrieve(('mySpace', 'myView', 'v1'))
 
         """
         identifier = _load_identifier(ids, "view")
         return self._retrieve_multiple(list_cls=ViewList, resource_cls=View, identifiers=identifier)
 
-    def delete(self, ids: ViewIdentifier | Sequence[ViewIdentifier]) -> list[VersionedDataModelingId]:
+    def delete(self, ids: ViewIdentifier | Sequence[ViewIdentifier]) -> list[ViewId]:
         """`Delete one or more views <https://docs.cognite.com/api/v1/#operation/deleteViews>`_
 
         Args:
             ids (ViewId | Sequence[ViewId]): View dentifier(s)
         Returns:
             The identifier for the view(s) which has been deleted. Empty list if nothing was deleted.
         Examples:
@@ -118,15 +122,15 @@
             list,
             self._delete_multiple(
                 identifiers=_load_identifier(ids, "view"),
                 wrap_ids=True,
                 returns_items=True,
             ),
         )
-        return [VersionedDataModelingId(item["space"], item["externalId"], item["version"]) for item in deleted_views]
+        return [ViewId(item["space"], item["externalId"], item["version"]) for item in deleted_views]
 
     def list(
         self,
         limit: int = DATA_MODELING_LIST_LIMIT_DEFAULT,
         space: str | None = None,
         include_inherited_properties: bool = True,
         all_versions: bool = False,
@@ -194,12 +198,12 @@
         Examples:
 
             Create new views::
 
                 >>> from cognite.client import CogniteClient
                 >>> import cognite.client.data_classes.data_modeling as models
                 >>> c = CogniteClient()
-                >>> views = [models.View(space="mySpace",external_id="myView",version="v1"),
-                ... models.View(space="mySpace",external_id="myOtherView",version="v1")]
-                >>> res = c.data_modeling.views.create(views)
+                >>> views = [models.ViewApply(space="mySpace",external_id="myView",version="v1"),
+                ... models.ViewApply(space="mySpace",external_id="myOtherView",version="v1")]
+                >>> res = c.data_modeling.views.apply(views)
         """
         return self._create_multiple(list_cls=ViewList, resource_cls=View, items=view)
```

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/data_sets.py` & `cognite_sdk-6.4.7/cognite/client/_api/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/datapoint_tasks.py` & `cognite_sdk-6.4.7/cognite/client/_api/datapoint_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/datapoints.py` & `cognite_sdk-6.4.7/cognite/client/_api/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/diagrams.py` & `cognite_sdk-6.4.7/cognite/client/_api/diagrams.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/entity_matching.py` & `cognite_sdk-6.4.7/cognite/client/_api/entity_matching.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/events.py` & `cognite_sdk-6.4.7/cognite/client/_api/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/extractionpipelines.py` & `cognite_sdk-6.4.7/cognite/client/_api/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/files.py` & `cognite_sdk-6.4.7/cognite/client/_api/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/functions.py` & `cognite_sdk-6.4.7/cognite/client/_api/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/geospatial.py` & `cognite_sdk-6.4.7/cognite/client/_api/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/iam.py` & `cognite_sdk-6.4.7/cognite/client/_api/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/labels.py` & `cognite_sdk-6.4.7/cognite/client/_api/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/raw.py` & `cognite_sdk-6.4.7/cognite/client/_api/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/relationships.py` & `cognite_sdk-6.4.7/cognite/client/_api/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/sequences.py` & `cognite_sdk-6.4.7/cognite/client/_api/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/synthetic_time_series.py` & `cognite_sdk-6.4.7/cognite/client/_api/synthetic_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/templates.py` & `cognite_sdk-6.4.7/cognite/client/_api/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/three_d.py` & `cognite_sdk-6.4.7/cognite/client/_api/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/time_series.py` & `cognite_sdk-6.4.7/cognite/client/_api/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/transformations/__init__.py` & `cognite_sdk-6.4.7/cognite/client/_api/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/transformations/jobs.py` & `cognite_sdk-6.4.7/cognite/client/_api/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/transformations/notifications.py` & `cognite_sdk-6.4.7/cognite/client/_api/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/transformations/schedules.py` & `cognite_sdk-6.4.7/cognite/client/_api/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/transformations/schema.py` & `cognite_sdk-6.4.7/cognite/client/_api/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api/vision.py` & `cognite_sdk-6.4.7/cognite/client/_api/vision.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_api_client.py` & `cognite_sdk-6.4.7/cognite/client/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_cognite_client.py` & `cognite_sdk-6.4.7/cognite/client/_cognite_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_http_client.py` & `cognite_sdk-6.4.7/cognite/client/_http_client.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response.proto` & `cognite_sdk-6.4.7/cognite/client/_proto/data_point_list_response.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response_pb2.py` & `cognite_sdk-6.4.7/cognite/client/_proto/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.7/cognite/client/_proto/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto/data_points.proto` & `cognite_sdk-6.4.7/cognite/client/_proto/data_points.proto`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto/data_points_pb2.py` & `cognite_sdk-6.4.7/cognite/client/_proto/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto/data_points_pb2.pyi` & `cognite_sdk-6.4.7/cognite/client/_proto/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_point_list_response_pb2.py` & `cognite_sdk-6.4.7/cognite/client/_proto_legacy/data_point_list_response_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi` & `cognite_sdk-6.4.7/cognite/client/_proto_legacy/data_point_list_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_points_pb2.py` & `cognite_sdk-6.4.7/cognite/client/_proto_legacy/data_points_pb2.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/_proto_legacy/data_points_pb2.pyi` & `cognite_sdk-6.4.7/cognite/client/_proto_legacy/data_points_pb2.pyi`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/config.py` & `cognite_sdk-6.4.7/cognite/client/config.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/credentials.py` & `cognite_sdk-6.4.7/cognite/client/credentials.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/__init__.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/_base.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/_base.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/images.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/annotation_types/images.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/annotation_types/primitives.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/annotation_types/primitives.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/annotations.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/annotations.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/assets.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/assets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/contextualization.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/contextualization.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/__init__.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/_core.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/_validation.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/containers.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,14 @@
         external_id: str,
         properties: dict[str, ContainerProperty],
         description: str = None,
         name: str = None,
         used_for: Literal["node", "edge", "all"] = None,
         constraints: dict[str, Constraint] = None,
         indexes: dict[str, Index] = None,
-        **_: dict,
     ):
         super().__init__(space, external_id, properties, description, name, used_for, constraints, indexes)
 
 
 class Container(ContainerCore):
     """Represent the physical storage of data. This is the read format of the container
```

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/data_models.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/data_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from cognite.client.data_classes._base import (
     CogniteFilter,
     CogniteResourceList,
 )
 from cognite.client.data_classes.data_modeling._core import DataModelingResource
 from cognite.client.data_classes.data_modeling._validation import validate_data_modeling_identifier
-from cognite.client.data_classes.data_modeling.ids import ViewId
+from cognite.client.data_classes.data_modeling.ids import DataModelId, ViewId
 from cognite.client.data_classes.data_modeling.views import View, ViewApply
 
 
 class DataModelCore(DataModelingResource):
     """A group of views.
 
     Args:
@@ -57,15 +57,14 @@
         self,
         space: str,
         external_id: str,
         version: str,
         description: str = None,
         name: str = None,
         views: list[ViewId | ViewApply] = None,
-        **_: dict,
     ):
         super().__init__(space, external_id, version, description, name)
         self.views = views
 
     @classmethod
     def _load_view(cls, view_data: dict) -> ViewId | ViewApply:
         if "type" in view_data:
@@ -157,14 +156,17 @@
             external_id=self.external_id,
             version=self.version,
             description=self.description,
             name=self.name,
             views=views,
         )
 
+    def as_id(self) -> DataModelId:
+        return DataModelId(space=self.space, external_id=self.external_id, version=self.version)
+
 
 class DataModelApplyList(CogniteResourceList[DataModelApply]):
     _RESOURCE = DataModelApply
 
 
 class DataModelList(CogniteResourceList[DataModel]):
     _RESOURCE = DataModel
```

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/data_types.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/data_types.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/filters.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/filters.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/ids.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/ids.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from __future__ import annotations
 
+from abc import ABC
 from dataclasses import asdict, dataclass, field
-from typing import ClassVar, Literal, Optional, Sequence, Tuple, Type, TypeVar, Union, cast
+from typing import Any, ClassVar, Literal, Optional, Sequence, Tuple, Type, TypeVar, Union, cast
 
 from cognite.client.utils._auxiliary import rename_and_exclude_keys
 from cognite.client.utils._identifier import DataModelingIdentifier, DataModelingIdentifierSequence
 from cognite.client.utils._text import convert_all_keys_recursive, convert_all_keys_to_snake_case
 
 
 @dataclass(frozen=True)
-class DataModelingId:
+class AbstractDataclass(ABC):
+    def __new__(cls, *args: Any, **kwargs: Any) -> Any:
+        if cls == AbstractDataclass or cls.__bases__[0] == AbstractDataclass:
+            raise TypeError("Cannot instantiate abstract class.")
+        return super().__new__(cls)
+
+
+@dataclass(frozen=True)
+class DataModelingId(AbstractDataclass):
     _type: ClassVar[str] = field(init=False)
     space: str
     external_id: str
 
     def as_tuple(self) -> tuple[str, str]:
         return self.space, self.external_id
 
@@ -34,15 +43,15 @@
         raise ValueError(f"Cannot load {data} into {cls}, invalid type={type(data)}")
 
 
 T_DataModelingId = TypeVar("T_DataModelingId", bound=DataModelingId)
 
 
 @dataclass(frozen=True)
-class VersionedDataModelingId:
+class VersionedDataModelingId(AbstractDataclass):
     _type: ClassVar[str] = field(init=False)
     space: str
     external_id: str
     version: Optional[str] = None
 
     def as_tuple(self) -> tuple[str, str, Optional[str]]:
         return self.space, self.external_id, self.version
```

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/instances.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/instances.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/spaces.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/spaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from typing import Any
+
 from cognite.client.data_classes._base import (
     CogniteResourceList,
 )
 from cognite.client.data_classes.data_modeling._core import DataModelingResource
 from cognite.client.data_classes.data_modeling._validation import validate_data_modeling_identifier
 
 
@@ -12,21 +14,15 @@
 
     Args:
         space (str): A unique identifier for space.
         description (str): Textual description of the space
         name (str): Human readable name for the space.
     """
 
-    def __init__(
-        self,
-        space: str,
-        description: str = None,
-        name: str = None,
-        **_: dict,
-    ):
+    def __init__(self, space: str, description: str = None, name: str = None):
         validate_data_modeling_identifier(space)
         self.space = space
         self.description = description
         self.name = name
 
 
 class SpaceApply(SpaceCore):
@@ -51,14 +47,15 @@
         self,
         space: str,
         is_global: bool,
         last_updated_time: int,
         created_time: int,
         description: str = None,
         name: str = None,
+        **_: Any,
     ):
         super().__init__(space, description, name)
         self.is_global = is_global
         self.last_updated_time = last_updated_time
         self.created_time = created_time
 
     def as_apply(self) -> SpaceApply:
```

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_modeling/views.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_modeling/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,14 @@
         external_id: str,
         version: str,
         description: str = None,
         name: str = None,
         filter: Filter | None = None,
         implements: list[ViewId] = None,
         properties: dict[str, MappedApplyPropertyDefinition | ConnectionDefinition] = None,
-        **_: dict,
     ):
         super().__init__(space, external_id, version, description, name, filter, implements)
         self.properties = properties
 
     @classmethod
     def load(cls, resource: dict | str) -> ViewApply:
         data = json.loads(resource) if isinstance(resource, str) else resource
```

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/data_sets.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/data_sets.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/datapoints.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/datapoints.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/events.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/events.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/extractionpipelines.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/extractionpipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/files.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/files.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/functions.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/functions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/geospatial.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/geospatial.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/iam.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/iam.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/labels.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/labels.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/raw.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/raw.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/relationships.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/relationships.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/sequences.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/sequences.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/shared.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/shared.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/templates.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/templates.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/three_d.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/three_d.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/time_series.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/__init__.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/common.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/transformations/common.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/jobs.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/transformations/jobs.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/notifications.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/transformations/notifications.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/schedules.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/transformations/schedules.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/data_classes/transformations/schema.py` & `cognite_sdk-6.4.7/cognite/client/data_classes/transformations/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/exceptions.py` & `cognite_sdk-6.4.7/cognite/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/testing.py` & `cognite_sdk-6.4.7/cognite/client/testing.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/__init__.py` & `cognite_sdk-6.4.7/cognite/client/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_auxiliary.py` & `cognite_sdk-6.4.7/cognite/client/utils/_auxiliary.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_concurrency.py` & `cognite_sdk-6.4.7/cognite/client/utils/_concurrency.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_graph.py` & `cognite_sdk-6.4.7/cognite/client/utils/_graph.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_identifier.py` & `cognite_sdk-6.4.7/cognite/client/utils/_identifier.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_logging.py` & `cognite_sdk-6.4.7/cognite/client/utils/_logging.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_pandas_helpers.py` & `cognite_sdk-6.4.7/cognite/client/utils/_pandas_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_priority_tpe.py` & `cognite_sdk-6.4.7/cognite/client/utils/_priority_tpe.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_pyodide_helpers.py` & `cognite_sdk-6.4.7/cognite/client/utils/_pyodide_helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_text.py` & `cognite_sdk-6.4.7/cognite/client/utils/_text.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_time.py` & `cognite_sdk-6.4.7/cognite/client/utils/_time.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_validation.py` & `cognite_sdk-6.4.7/cognite/client/utils/_validation.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/cognite/client/utils/_version_checker.py` & `cognite_sdk-6.4.7/cognite/client/utils/_version_checker.py`

 * *Files identical despite different names*

### Comparing `cognite_sdk-6.4.5/pyproject.toml` & `cognite_sdk-6.4.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "cognite-sdk"
 
-version = "6.4.5"
+version = "6.4.7"
 
 description = "Cognite Python SDK"
 readme = "README.md"
 documentation = "https://cognite-sdk-python.readthedocs-hosted.com"
 authors = ["Erlend Vollset <erlend.vollset@cognite.com>"]
 license = "Apache-2.0"
```

### Comparing `cognite_sdk-6.4.5/PKG-INFO` & `cognite_sdk-6.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-sdk
-Version: 6.4.5
+Version: 6.4.7
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
-Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.5 Summary: Cognite Python
+Metadata-Version: 2.1 Name: cognite-sdk Version: 6.4.7 Summary: Cognite Python
 SDK License: Apache-2.0 Author: Erlend Vollset Author-email:
 erlend.vollset@cognite.com Requires-Python: >=3.8,<4.0 Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Provides-
 Extra: all Provides-Extra: functions Provides-Extra: geo Provides-Extra: numpy
```

