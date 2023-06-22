# Comparing `tmp/oc_ocdm-7.2.0.tar.gz` & `tmp/oc_ocdm-7.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oc_ocdm-7.2.0.tar", max compression
+gzip compressed data, was "oc_ocdm-7.3.0.tar", max compression
```

## Comparing `oc_ocdm-7.2.0.tar` & `oc_ocdm-7.3.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0      795 2022-12-20 14:08:57.539390 oc_ocdm-7.2.0/LICENSE.md
--rw-r--r--   0        0        0      932 2022-12-20 14:08:57.555020 oc_ocdm-7.2.0/oc_ocdm/__init__.py
--rw-r--r--   0        0        0     8012 2023-01-31 16:12:47.420934 oc_ocdm-7.2.0/oc_ocdm/abstract_entity.py
--rw-r--r--   0        0        0     2890 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/abstract_set.py
--rw-r--r--   0        0        0     1082 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/counter_handler/__init__.py
--rw-r--r--   0        0        0     6419 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/counter_handler/counter_handler.py
--rw-r--r--   0        0        0    16145 2023-02-01 15:10:49.023094 oc_ocdm-7.2.0/oc_ocdm/counter_handler/filesystem_counter_handler.py
--rw-r--r--   0        0        0    12543 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/counter_handler/in_memory_counter_handler.py
--rw-r--r--   0        0        0     3676 2023-06-08 09:32:26.643046 oc_ocdm-7.2.0/oc_ocdm/counter_handler/sqlite_counter_handler.py
--rw-r--r--   0        0        0     2647 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/decorators.py
--rw-r--r--   0        0        0      937 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/__init__.py
--rw-r--r--   0        0        0      974 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/__init__.py
--rw-r--r--   0        0        0     1680 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     8436 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/agent_role.py
--rw-r--r--   0        0        0     9064 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
--rw-r--r--   0        0        0    49262 2023-06-15 09:24:33.053664 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
--rw-r--r--   0        0        0    16277 2023-03-08 10:55:02.484160 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/citation.py
--rw-r--r--   0        0        0    21579 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/discourse_element.py
--rw-r--r--   0        0        0     6313 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/pointer_list.py
--rw-r--r--   0        0        0     4907 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
--rw-r--r--   0        0        0    10131 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
--rw-r--r--   0        0        0    10359 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
--rw-r--r--   0        0        0     8831 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
--rw-r--r--   0        0        0     6582 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic_entity.py
--rw-r--r--   0        0        0    18802 2023-06-15 09:27:55.194188 oc_ocdm-7.2.0/oc_ocdm/graph/entities/identifier.py
--rw-r--r--   0        0        0    15524 2023-06-15 09:19:46.065312 oc_ocdm-7.2.0/oc_ocdm/graph/graph_entity.py
--rw-r--r--   0        0        0    19992 2023-03-08 11:57:00.994531 oc_ocdm-7.2.0/oc_ocdm/graph/graph_set.py
--rw-r--r--   0        0        0      955 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/__init__.py
--rw-r--r--   0        0        0      959 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/entities/__init__.py
--rw-r--r--   0        0        0    19262 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/entities/dataset.py
--rw-r--r--   0        0        0    12483 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/entities/distribution.py
--rw-r--r--   0        0        0     7586 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/metadata_entity.py
--rw-r--r--   0        0        0     6549 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/metadata/metadata_set.py
--rw-r--r--   0        0        0      931 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/prov/__init__.py
--rw-r--r--   0        0        0      905 2022-12-20 14:08:57.570646 oc_ocdm-7.2.0/oc_ocdm/prov/entities/__init__.py
--rw-r--r--   0        0        0    13642 2023-01-31 14:34:56.084004 oc_ocdm-7.2.0/oc_ocdm/prov/entities/snapshot_entity.py
--rw-r--r--   0        0        0     3759 2023-03-08 15:28:49.049031 oc_ocdm-7.2.0/oc_ocdm/prov/prov_entity.py
--rw-r--r--   0        0        0    16537 2023-06-08 09:32:26.643046 oc_ocdm-7.2.0/oc_ocdm/prov/prov_set.py
--rw-r--r--   0        0        0    11895 2023-06-08 09:32:26.644056 oc_ocdm-7.2.0/oc_ocdm/reader.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/resources/__init__.py
--rw-r--r--   0        0        0     1361 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/resources/querymap.txt
--rw-r--r--   0        0        0    22001 2023-03-01 17:12:50.977316 oc_ocdm-7.2.0/oc_ocdm/resources/shacle.ttl
--rw-r--r--   0        0        0    12513 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/resources/shexc.txt
--rw-r--r--   0        0        0    12611 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/resources/shexc_closed.txt
--rw-r--r--   0        0        0    16523 2023-06-08 09:32:26.645057 oc_ocdm-7.2.0/oc_ocdm/storer.py
--rw-r--r--   0        0        0     1354 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/support/__init__.py
--rw-r--r--   0        0        0     3539 2023-03-05 18:46:51.846163 oc_ocdm-7.2.0/oc_ocdm/support/query_utils.py
--rw-r--r--   0        0        0     2615 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/support/reporter.py
--rw-r--r--   0        0        0    15049 2023-06-15 09:14:53.068272 oc_ocdm-7.2.0/oc_ocdm/support/support.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/__init__.py
--rw-r--r--   0        0        0     8681 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
--rw-r--r--   0        0        0    11192 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
--rw-r--r--   0        0        0    69632 2023-03-05 14:39:21.650226 oc_ocdm-7.2.0/oc_ocdm/test/coverage/.coverage
--rw-r--r--   0        0        0      109 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/coverage/.coveragerc
--rw-r--r--   0        0        0      925 2023-03-03 14:13:32.590309 oc_ocdm-7.2.0/oc_ocdm/test/coverage/coverage.svg
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/__init__.py
--rw-r--r--   0        0        0     2679 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
--rw-r--r--   0        0        0     2209 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
--rw-r--r--   0        0        0    12671 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
--rw-r--r--   0        0        0     6887 2023-03-08 14:23:54.735495 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
--rw-r--r--   0        0        0     4915 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
--rw-r--r--   0        0        0     1908 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
--rw-r--r--   0        0        0     1740 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
--rw-r--r--   0        0        0     2501 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
--rw-r--r--   0        0        0     2990 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
--rw-r--r--   0        0        0     2535 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
--rw-r--r--   0        0        0     2980 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
--rw-r--r--   0        0        0     8109 2023-03-08 11:33:47.672369 oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/test_identifier.py
--rw-r--r--   0        0        0      964 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/graph/test_graph_entity.py
--rw-r--r--   0        0        0     6675 2023-01-31 16:12:47.427934 oc_ocdm-7.2.0/oc_ocdm/test/graph/test_graph_set.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/metadata/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/__init__.py
--rw-r--r--   0        0        0     4691 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/test_dataset.py
--rw-r--r--   0        0        0     3601 2022-12-20 14:08:57.586271 oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/test_distribution.py
--rw-r--r--   0        0        0     2738 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/metadata/test_metadata_set.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/prov/__init__.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/prov/entities/__init__.py
--rw-r--r--   0        0        0     4248 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/prov/entities/test_snapshot_entity.py
--rw-r--r--   0        0        0    12288 2023-03-08 15:11:17.576967 oc_ocdm-7.2.0/oc_ocdm/test/prov/prov_counter.db
--rw-r--r--   0        0        0    13027 2023-06-08 09:32:26.647057 oc_ocdm-7.2.0/oc_ocdm/test/prov/test_prov_set.py
--rw-r--r--   0        0        0        0 2023-03-05 14:27:05.796485 oc_ocdm-7.2.0/oc_ocdm/test/reader/__init__.py
--rw-r--r--   0        0        0     2542 2023-03-05 17:46:14.507023 oc_ocdm-7.2.0/oc_ocdm/test/reader/br.nt
--rw-r--r--   0        0        0     1898 2023-03-05 17:47:28.794428 oc_ocdm-7.2.0/oc_ocdm/test/reader/test_reader.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/resources/__init__.py
--rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.2.0/oc_ocdm/test/resources/data.json
--rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.2.0/oc_ocdm/test/resources/data_reader.json
--rw-r--r--   0        0        0     6628 2023-03-03 13:05:35.809618 oc_ocdm-7.2.0/oc_ocdm/test/resources/data_reader_invalid.json
--rw-r--r--   0        0        0     2531 2023-03-03 13:43:32.199458 oc_ocdm-7.2.0/oc_ocdm/test/resources/test_shacle.py
--rw-r--r--   0        0        0      841 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/storer/__init__.py
--rw-r--r--   0        0        0    11519 2023-06-08 09:32:26.648059 oc_ocdm-7.2.0/oc_ocdm/test/storer/test_storer.py
--rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.2.0/oc_ocdm/test/support/__init__.py
--rw-r--r--   0        0        0     5485 2023-01-31 16:12:50.030419 oc_ocdm-7.2.0/oc_ocdm/test/support/test_support.py
--rw-r--r--   0        0        0     1590 2023-06-15 09:33:17.989306 oc_ocdm-7.2.0/pyproject.toml
--rw-r--r--   0        0        0     4373 2022-12-20 14:08:57.539390 oc_ocdm-7.2.0/README.md
--rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 oc_ocdm-7.2.0/setup.py
--rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 oc_ocdm-7.2.0/PKG-INFO
+-rw-r--r--   0        0        0      795 2022-12-20 14:08:57.539390 oc_ocdm-7.3.0/LICENSE.md
+-rw-r--r--   0        0        0      932 2022-12-20 14:08:57.555020 oc_ocdm-7.3.0/oc_ocdm/__init__.py
+-rw-r--r--   0        0        0     8012 2023-01-31 16:12:47.420934 oc_ocdm-7.3.0/oc_ocdm/abstract_entity.py
+-rw-r--r--   0        0        0     2890 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/abstract_set.py
+-rw-r--r--   0        0        0     1082 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/counter_handler/__init__.py
+-rw-r--r--   0        0        0     6419 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/counter_handler/counter_handler.py
+-rw-r--r--   0        0        0    16145 2023-02-01 15:10:49.023094 oc_ocdm-7.3.0/oc_ocdm/counter_handler/filesystem_counter_handler.py
+-rw-r--r--   0        0        0    12543 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/counter_handler/in_memory_counter_handler.py
+-rw-r--r--   0        0        0     3676 2023-06-08 09:32:26.643046 oc_ocdm-7.3.0/oc_ocdm/counter_handler/sqlite_counter_handler.py
+-rw-r--r--   0        0        0     2647 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/decorators.py
+-rw-r--r--   0        0        0      937 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/__init__.py
+-rw-r--r--   0        0        0      974 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/__init__.py
+-rw-r--r--   0        0        0     1680 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     8436 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/agent_role.py
+-rw-r--r--   0        0        0     9064 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py
+-rw-r--r--   0        0        0    49262 2023-06-15 09:24:33.053664 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py
+-rw-r--r--   0        0        0    16277 2023-03-08 10:55:02.484160 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/citation.py
+-rw-r--r--   0        0        0    21579 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/discourse_element.py
+-rw-r--r--   0        0        0     6313 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/pointer_list.py
+-rw-r--r--   0        0        0     4907 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/reference_annotation.py
+-rw-r--r--   0        0        0    10131 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/reference_pointer.py
+-rw-r--r--   0        0        0    10359 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py
+-rw-r--r--   0        0        0     8831 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/responsible_agent.py
+-rw-r--r--   0        0        0     6582 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic_entity.py
+-rw-r--r--   0        0        0    19588 2023-06-22 15:17:47.267645 oc_ocdm-7.3.0/oc_ocdm/graph/entities/identifier.py
+-rw-r--r--   0        0        0    15574 2023-06-22 15:17:01.790488 oc_ocdm-7.3.0/oc_ocdm/graph/graph_entity.py
+-rw-r--r--   0        0        0    19992 2023-03-08 11:57:00.994531 oc_ocdm-7.3.0/oc_ocdm/graph/graph_set.py
+-rw-r--r--   0        0        0      955 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/metadata/__init__.py
+-rw-r--r--   0        0        0      959 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/metadata/entities/__init__.py
+-rw-r--r--   0        0        0    19262 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/metadata/entities/dataset.py
+-rw-r--r--   0        0        0    12483 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/metadata/entities/distribution.py
+-rw-r--r--   0        0        0     7586 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/metadata/metadata_entity.py
+-rw-r--r--   0        0        0     6549 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/metadata/metadata_set.py
+-rw-r--r--   0        0        0      931 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/prov/__init__.py
+-rw-r--r--   0        0        0      905 2022-12-20 14:08:57.570646 oc_ocdm-7.3.0/oc_ocdm/prov/entities/__init__.py
+-rw-r--r--   0        0        0    13642 2023-01-31 14:34:56.084004 oc_ocdm-7.3.0/oc_ocdm/prov/entities/snapshot_entity.py
+-rw-r--r--   0        0        0     3759 2023-03-08 15:28:49.049031 oc_ocdm-7.3.0/oc_ocdm/prov/prov_entity.py
+-rw-r--r--   0        0        0    16537 2023-06-08 09:32:26.643046 oc_ocdm-7.3.0/oc_ocdm/prov/prov_set.py
+-rw-r--r--   0        0        0    11895 2023-06-08 09:32:26.644056 oc_ocdm-7.3.0/oc_ocdm/reader.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/resources/__init__.py
+-rw-r--r--   0        0        0     1361 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/resources/querymap.txt
+-rw-r--r--   0        0        0    22001 2023-03-01 17:12:50.977316 oc_ocdm-7.3.0/oc_ocdm/resources/shacle.ttl
+-rw-r--r--   0        0        0    12513 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/resources/shexc.txt
+-rw-r--r--   0        0        0    12611 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/resources/shexc_closed.txt
+-rw-r--r--   0        0        0    16523 2023-06-08 09:32:26.645057 oc_ocdm-7.3.0/oc_ocdm/storer.py
+-rw-r--r--   0        0        0     1354 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/support/__init__.py
+-rw-r--r--   0        0        0     3539 2023-03-05 18:46:51.846163 oc_ocdm-7.3.0/oc_ocdm/support/query_utils.py
+-rw-r--r--   0        0        0     2615 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/support/reporter.py
+-rw-r--r--   0        0        0    15049 2023-06-15 09:14:53.068272 oc_ocdm-7.3.0/oc_ocdm/support/support.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/counter_handler/__init__.py
+-rw-r--r--   0        0        0     8681 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py
+-rw-r--r--   0        0        0    11192 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py
+-rw-r--r--   0        0        0    69632 2023-03-05 14:39:21.650226 oc_ocdm-7.3.0/oc_ocdm/test/coverage/.coverage
+-rw-r--r--   0        0        0      109 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/coverage/.coveragerc
+-rw-r--r--   0        0        0      925 2023-03-03 14:13:32.590309 oc_ocdm-7.3.0/oc_ocdm/test/coverage/coverage.svg
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/__init__.py
+-rw-r--r--   0        0        0     2679 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py
+-rw-r--r--   0        0        0     2209 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py
+-rw-r--r--   0        0        0    12671 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py
+-rw-r--r--   0        0        0     6887 2023-03-08 14:23:54.735495 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_citation.py
+-rw-r--r--   0        0        0     4915 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py
+-rw-r--r--   0        0        0     1908 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py
+-rw-r--r--   0        0        0     1740 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py
+-rw-r--r--   0        0        0     2501 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py
+-rw-r--r--   0        0        0     2990 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py
+-rw-r--r--   0        0        0     2535 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py
+-rw-r--r--   0        0        0     2980 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/test_bibliographic_entity.py
+-rw-r--r--   0        0        0     8109 2023-03-08 11:33:47.672369 oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/test_identifier.py
+-rw-r--r--   0        0        0      964 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/graph/test_graph_entity.py
+-rw-r--r--   0        0        0     6675 2023-01-31 16:12:47.427934 oc_ocdm-7.3.0/oc_ocdm/test/graph/test_graph_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/metadata/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/metadata/entities/__init__.py
+-rw-r--r--   0        0        0     4691 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/metadata/entities/test_dataset.py
+-rw-r--r--   0        0        0     3601 2022-12-20 14:08:57.586271 oc_ocdm-7.3.0/oc_ocdm/test/metadata/entities/test_distribution.py
+-rw-r--r--   0        0        0     2738 2022-12-20 14:08:57.601896 oc_ocdm-7.3.0/oc_ocdm/test/metadata/test_metadata_set.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.3.0/oc_ocdm/test/prov/__init__.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.3.0/oc_ocdm/test/prov/entities/__init__.py
+-rw-r--r--   0        0        0     4248 2022-12-20 14:08:57.601896 oc_ocdm-7.3.0/oc_ocdm/test/prov/entities/test_snapshot_entity.py
+-rw-r--r--   0        0        0    12288 2023-03-08 15:11:17.576967 oc_ocdm-7.3.0/oc_ocdm/test/prov/prov_counter.db
+-rw-r--r--   0        0        0    13027 2023-06-08 09:32:26.647057 oc_ocdm-7.3.0/oc_ocdm/test/prov/test_prov_set.py
+-rw-r--r--   0        0        0        0 2023-03-05 14:27:05.796485 oc_ocdm-7.3.0/oc_ocdm/test/reader/__init__.py
+-rw-r--r--   0        0        0     2542 2023-03-05 17:46:14.507023 oc_ocdm-7.3.0/oc_ocdm/test/reader/br.nt
+-rw-r--r--   0        0        0     1898 2023-03-05 17:47:28.794428 oc_ocdm-7.3.0/oc_ocdm/test/reader/test_reader.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.3.0/oc_ocdm/test/resources/__init__.py
+-rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.3.0/oc_ocdm/test/resources/data.json
+-rw-r--r--   0        0        0     6627 2023-03-01 17:12:20.402368 oc_ocdm-7.3.0/oc_ocdm/test/resources/data_reader.json
+-rw-r--r--   0        0        0     6628 2023-03-03 13:05:35.809618 oc_ocdm-7.3.0/oc_ocdm/test/resources/data_reader_invalid.json
+-rw-r--r--   0        0        0     2531 2023-03-03 13:43:32.199458 oc_ocdm-7.3.0/oc_ocdm/test/resources/test_shacle.py
+-rw-r--r--   0        0        0      841 2022-12-20 14:08:57.601896 oc_ocdm-7.3.0/oc_ocdm/test/storer/__init__.py
+-rw-r--r--   0        0        0    11519 2023-06-08 09:32:26.648059 oc_ocdm-7.3.0/oc_ocdm/test/storer/test_storer.py
+-rw-r--r--   0        0        0      837 2022-12-20 14:08:57.601896 oc_ocdm-7.3.0/oc_ocdm/test/support/__init__.py
+-rw-r--r--   0        0        0     5485 2023-01-31 16:12:50.030419 oc_ocdm-7.3.0/oc_ocdm/test/support/test_support.py
+-rw-r--r--   0        0        0     1590 2023-06-22 15:19:55.747227 oc_ocdm-7.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4373 2022-12-20 14:08:57.539390 oc_ocdm-7.3.0/README.md
+-rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 oc_ocdm-7.3.0/setup.py
+-rw-r--r--   0        0        0     5687 1970-01-01 00:00:00.000000 oc_ocdm-7.3.0/PKG-INFO
```

### Comparing `oc_ocdm-7.2.0/LICENSE.md` & `oc_ocdm-7.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/abstract_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/abstract_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/abstract_set.py` & `oc_ocdm-7.3.0/oc_ocdm/abstract_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/counter_handler/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/counter_handler/counter_handler.py` & `oc_ocdm-7.3.0/oc_ocdm/counter_handler/counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/counter_handler/filesystem_counter_handler.py` & `oc_ocdm-7.3.0/oc_ocdm/counter_handler/filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/counter_handler/in_memory_counter_handler.py` & `oc_ocdm-7.3.0/oc_ocdm/counter_handler/in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/counter_handler/sqlite_counter_handler.py` & `oc_ocdm-7.3.0/oc_ocdm/counter_handler/sqlite_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/decorators.py` & `oc_ocdm-7.3.0/oc_ocdm/decorators.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/agent_role.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/citation.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/discourse_element.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/pointer_list.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/reference_annotation.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/reference_pointer.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic/responsible_agent.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic/responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/bibliographic_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/entities/identifier.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/entities/identifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -329,14 +329,31 @@
         :type string: str
         :raises TypeError: if the parameter is of the wrong type
         :return: None
         """
         self._associate_identifier_with_scheme(string, GraphEntity.iri_wikipedia)
 
     @accepts_only('literal')
+    def create_arxiv(self, string: str) -> None:
+        """
+        Setter method corresponding to both the ``literal:hasLiteralValue`` and the
+        ``datacite:usesIdentifierScheme`` RDF predicate.
+        It implicitly sets the object value ``datacite:crossref`` for the
+        ``datacite:usesIdentifierScheme`` RDF predicate.
+
+        **WARNING: this is a functional property, hence any existing value will be overwritten!**
+
+        :param string: The value that will be set as the object of the property related to this method
+        :type string: str
+        :raises TypeError: if the parameter is of the wrong type
+        :return: None
+        """
+        self._associate_identifier_with_scheme(string, GraphEntity.iri_arxiv)
+
+    @accepts_only('literal')
     def create_crossref(self, string: str) -> None:
         """
         Setter method corresponding to both the ``literal:hasLiteralValue`` and the
         ``datacite:usesIdentifierScheme`` RDF predicate.
         It implicitly sets the object value ``datacite:crossref`` for the
         ``datacite:usesIdentifierScheme`` RDF predicate.
```

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/graph_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/graph_entity.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     iri_singleloc_pointer_list: ClassVar[URIRef] = C4O.SingleLocationPointerList
     iri_has_element: ClassVar[URIRef] = CO.element
     iri_citation: ClassVar[URIRef] = CITO.Citation
     iri_cites: ClassVar[URIRef] = CITO.cites
     iri_citation_characterisation: ClassVar[URIRef] = CITO.hasCitationCharacterisation
     iri_has_citing_entity: ClassVar[URIRef] = CITO.hasCitingEntity
     iri_has_cited_entity: ClassVar[URIRef] = CITO.hasCitedEntity
+    iri_arxiv: ClassVar[URIRef] = DATACITE.arxiv
     iri_oci: ClassVar[URIRef] = DATACITE.oci
     iri_doi: ClassVar[URIRef] = DATACITE.doi
     iri_pmid: ClassVar[URIRef] = DATACITE.pmid
     iri_pmcid: ClassVar[URIRef] = DATACITE.pmcid
     iri_orcid: ClassVar[URIRef] = DATACITE.orcid
     iri_xpath: ClassVar[URIRef] = DATACITE["local-resource-identifier-scheme"]
     iri_intrepid: ClassVar[URIRef] = DATACITE.intrepid
```

### Comparing `oc_ocdm-7.2.0/oc_ocdm/graph/graph_set.py` & `oc_ocdm-7.3.0/oc_ocdm/graph/graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/metadata/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/metadata/entities/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/metadata/entities/dataset.py` & `oc_ocdm-7.3.0/oc_ocdm/metadata/entities/dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/metadata/entities/distribution.py` & `oc_ocdm-7.3.0/oc_ocdm/metadata/entities/distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/metadata/metadata_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/metadata/metadata_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/metadata/metadata_set.py` & `oc_ocdm-7.3.0/oc_ocdm/metadata/metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/prov/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/prov/entities/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/prov/entities/snapshot_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/prov/entities/snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/prov/prov_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/prov/prov_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/prov/prov_set.py` & `oc_ocdm-7.3.0/oc_ocdm/prov/prov_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/reader.py` & `oc_ocdm-7.3.0/oc_ocdm/reader.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/resources/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/resources/querymap.txt` & `oc_ocdm-7.3.0/oc_ocdm/resources/querymap.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/resources/shacle.ttl` & `oc_ocdm-7.3.0/oc_ocdm/resources/shacle.ttl`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/resources/shexc.txt` & `oc_ocdm-7.3.0/oc_ocdm/resources/shexc.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/resources/shexc_closed.txt` & `oc_ocdm-7.3.0/oc_ocdm/resources/shexc_closed.txt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/storer.py` & `oc_ocdm-7.3.0/oc_ocdm/storer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/support/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/support/query_utils.py` & `oc_ocdm-7.3.0/oc_ocdm/support/query_utils.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/support/reporter.py` & `oc_ocdm-7.3.0/oc_ocdm/support/reporter.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/support/support.py` & `oc_ocdm-7.3.0/oc_ocdm/support/support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/counter_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py` & `oc_ocdm-7.3.0/oc_ocdm/test/counter_handler/test_filesystem_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py` & `oc_ocdm-7.3.0/oc_ocdm/test/counter_handler/test_in_memory_counter_handler.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/coverage/.coverage` & `oc_ocdm-7.3.0/oc_ocdm/test/coverage/.coverage`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/coverage/coverage.svg` & `oc_ocdm-7.3.0/oc_ocdm/test/coverage/coverage.svg`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_agent_role.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_reference.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_bibliographic_resource.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_citation.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_citation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_discourse_element.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_pointer_list.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_annotation.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_reference_pointer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_resource_embodiment.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/bibliographic/test_responsible_agent.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/test_bibliographic_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/test_bibliographic_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/entities/test_identifier.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/entities/test_identifier.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/test_graph_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/test_graph_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/graph/test_graph_set.py` & `oc_ocdm-7.3.0/oc_ocdm/test/graph/test_graph_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/metadata/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/metadata/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/test_dataset.py` & `oc_ocdm-7.3.0/oc_ocdm/test/metadata/entities/test_dataset.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/metadata/entities/test_distribution.py` & `oc_ocdm-7.3.0/oc_ocdm/test/metadata/entities/test_distribution.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/metadata/test_metadata_set.py` & `oc_ocdm-7.3.0/oc_ocdm/test/metadata/test_metadata_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/prov/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/prov/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/prov/entities/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/prov/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/prov/entities/test_snapshot_entity.py` & `oc_ocdm-7.3.0/oc_ocdm/test/prov/entities/test_snapshot_entity.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/prov/prov_counter.db` & `oc_ocdm-7.3.0/oc_ocdm/test/prov/prov_counter.db`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/prov/test_prov_set.py` & `oc_ocdm-7.3.0/oc_ocdm/test/prov/test_prov_set.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/reader/br.nt` & `oc_ocdm-7.3.0/oc_ocdm/test/reader/br.nt`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/reader/test_reader.py` & `oc_ocdm-7.3.0/oc_ocdm/test/reader/test_reader.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/resources/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/resources/data.json` & `oc_ocdm-7.3.0/oc_ocdm/test/resources/data.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/resources/data_reader.json` & `oc_ocdm-7.3.0/oc_ocdm/test/resources/data_reader.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/resources/data_reader_invalid.json` & `oc_ocdm-7.3.0/oc_ocdm/test/resources/data_reader_invalid.json`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/resources/test_shacle.py` & `oc_ocdm-7.3.0/oc_ocdm/test/resources/test_shacle.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/storer/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/storer/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/storer/test_storer.py` & `oc_ocdm-7.3.0/oc_ocdm/test/storer/test_storer.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/support/__init__.py` & `oc_ocdm-7.3.0/oc_ocdm/test/support/__init__.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/oc_ocdm/test/support/test_support.py` & `oc_ocdm-7.3.0/oc_ocdm/test/support/test_support.py`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/pyproject.toml` & `oc_ocdm-7.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oc_ocdm"
-version = "7.2.0"
+version = "7.3.0"
 description = "Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel."
 authors = [
     "Silvio Peroni <essepuntato@gmail.com>",
     "Marilena Daquino <marilena.daquino2@unibo.it>",
     "Fabio Mariani <fabio.mariani6@studio.unibo.it>",
     "Simone Persiani <iosonopersia@gmail.com>",
     "Arcangelo Massari <arcangelo.massari@unibo.it>"
```

### Comparing `oc_ocdm-7.2.0/README.md` & `oc_ocdm-7.3.0/README.md`

 * *Files identical despite different names*

### Comparing `oc_ocdm-7.2.0/setup.py` & `oc_ocdm-7.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
  'rdflib>=6.0.0,<7.0.0']
 
 entry_points = \
 {'console_scripts': ['test = scripts:main']}
 
 setup_kwargs = {
     'name': 'oc-ocdm',
-    'version': '7.2.0',
+    'version': '7.3.0',
     'description': 'Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel.',
     'long_description': '# oc_ocdm\n[<img src="https://img.shields.io/badge/powered%20by-OpenCitations-%239931FC?labelColor=2D22DE" />](http://opencitations.net)\n[![Run tests](https://github.com/opencitations/oc_ocdm/actions/workflows/run_tests.yml/badge.svg)](https://github.com/opencitations/oc_ocdm/actions/workflows/run_tests.yml)\n![Coverage](https://raw.githubusercontent.com/opencitations/oc_ocdm/master/oc_ocdm/test/coverage/coverage.svg)\n[![Documentation Status](https://readthedocs.org/projects/oc-ocdm/badge/?version=latest)](https://oc-ocdm.readthedocs.io/en/latest/?badge=latest)\n[![PyPI version](https://badge.fury.io/py/oc-ocdm.svg)](https://badge.fury.io/py/oc-ocdm)\n![PyPI](https://img.shields.io/pypi/pyversions/oc_meta)\n\n[![DOI](https://zenodo.org/badge/322327342.svg)](https://zenodo.org/badge/latestdoi/322327342)\n[![License: ISC](https://img.shields.io/badge/License-ISC-blue.svg)](https://opensource.org/licenses/ISC)\n\nDocumentation can be found here: [https://oc-ocdm.readthedocs.io](https://oc-ocdm.readthedocs.io).\n\n**oc_ocdm** is a Python &ge;3.7 library that enables the user to import, produce, modify and export RDF data\nstructures which are compliant with the [OCDM v2.0.1](https://figshare.com/articles/Metadata_for_the_OpenCitations_Corpus/3443876) specification.\n\n## User\'s guide\nThis package can be simply installed with **pip**:\n``` bash\n    pip install oc_ocdm\n```\n**Please, have a look at the notebooks [available here](https://github.com/opencitations/oc_ocdm/blob/master/notebooks/).**\n\n## Developer\'s guide\n\n### First steps\n  1. Install Poetry:\n``` bash\n    pip install poetry\n```\n  2. Clone this repository:\n``` bash\n    git clone https://github.com/iosonopersia/oc_ocdm\n    cd ./oc_ocdm\n```\n  3. Install all the dependencies:\n``` bash\n    poetry install\n```\n  4. Build the package (_output dir:_ `dist`):\n``` bash\n    poetry build\n```\n  5. Globally install the package (_alternatively, you can also install it inside a virtual-env,\n  by providing the full path to the .tar.gz archive_):\n``` bash\n    pip install ./dist/oc_ocdm-<VERSION>.tar.gz\n```\n  6. If everything went the right way, than you should be able to use the `oc_ocdm` library in your Python modules as follows:\n``` python\n    from oc_ocdm.graph import GraphSet\n    from oc_ocdm.graph.entities.bibliographic import AgentRole\n    # ...\n```\n\n### How to run the tests\nJust run the following command inside the root project folder:\n``` bash\n    poetry run test\n```\n\n### How to manage the project using Poetry\nSee [Poetry commands documentation](https://python-poetry.org/docs/cli/).\n\n**AAA: when adding a non-dev dependency via `poetry add`, always remember to add\nthat same dependency to the `autodoc_mock_imports` list in `docs/source/conf.py`**\n(otherwise "Read the Docs" won\'t be able to compile the documentation correctly!).\n\n### How to publish the package onto Pypi\n``` bash\n    poetry publish --build\n```\n### Install dependencies needed for the documentation\n``` bash\n    pip install Sphinx sphinx_rtd_theme\n```\n### How to generate the documentation\n``` bash\n    rm ./docs/source/modules/*\n    sphinx-apidoc  -o ./docs/source/modules oc_ocdm *test*\n```\n\n### How to build the documentation\n___\n**Warning! In order to avoid getting the following `WARNING: html_static_path entry \'_static\' does not exist`, you\'ll\nneed to manually create an empty `_static` folder with the command:**\n``` bash\n    mkdir docs/source/_static\n```\n___\n  1. Always remember to move inside the `docs` folder:\n``` bash\n    cd docs\n```\n  2. Use the Makefile provided to build the docs:\n      + _on Windows_\n        ```\n            make.bat html\n        ```\n      + _on Linux and MacOs_\n        ```\n            make html\n        ```\n  3. Open the `build/html/index.html` file with a web browser of your choice!\n\n## Acknowledgements\nThis work has been funded by the project “Open Biomedical Citations in Context Corpus”\n(Wellcome Trust, Grant n. 214471/Z/18/Z) and the project “Wikipedia Citations in Wikidata”\n(Wikimedia Foundation, https://meta.wikimedia.org/wiki/Wikicite/grant/Wikipedia_Citations_in_Wikidata).\n\nWe would like to thank (in alphabetic order) Fabio Mariani (@FabioMariani), Arcangelo\nMassari (@arcangelo7), and Gabriele Pisciotta (@GabrielePisciotta) for the constructive feedback.\n',
     'author': 'Silvio Peroni',
     'author_email': 'essepuntato@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://opencitations.net',
```

### Comparing `oc_ocdm-7.2.0/PKG-INFO` & `oc_ocdm-7.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oc-ocdm
-Version: 7.2.0
+Version: 7.3.0
 Summary: Object mapping library for manipulating RDF graphs that are compliant with the OpenCitations datamodel.
 Home-page: https://opencitations.net
 License: ISC
 Keywords: opencitations,openscience,datamodel,mapping
 Author: Silvio Peroni
 Author-email: essepuntato@gmail.com
 Requires-Python: >=3.7.4,<4.0.0
```

