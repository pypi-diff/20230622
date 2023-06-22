# Comparing `tmp/muscle3-0.6.0.tar.gz` & `tmp/muscle3-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muscle3-0.6.0.tar", last modified: Tue Jan 17 22:16:13 2023, max compression
+gzip compressed data, was "muscle3-0.7.0.tar", last modified: Thu Jun 22 21:28:15 2023, max compression
```

## Comparing `muscle3-0.6.0.tar` & `muscle3-0.7.0.tar`

### file list

```diff
@@ -1,118 +1,109 @@
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    11357 2022-04-29 20:04:40.000000 muscle3-0.6.0/LICENSE
--rw-rw-r--   0 lourens   (1000) lourens   (1000)       66 2022-04-29 20:04:40.000000 muscle3-0.6.0/MANIFEST.in
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      172 2023-01-17 22:10:28.000000 muscle3-0.6.0/NOTICE
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3257 2023-01-17 22:16:13.417863 muscle3-0.6.0/PKG-INFO
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2460 2023-01-17 22:10:28.000000 muscle3-0.6.0/README.rst
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        6 2023-01-17 22:10:28.000000 muscle3-0.6.0/VERSION
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.413864 muscle3-0.6.0/integration_test/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2018-11-20 12:47:22.000000 muscle3-0.6.0/integration_test/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     7397 2023-01-17 22:10:28.000000 muscle3-0.6.0/integration_test/conftest.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      241 2018-03-26 08:12:44.000000 muscle3-0.6.0/integration_test/include_libmuscle.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2584 2023-01-17 22:10:28.000000 muscle3-0.6.0/integration_test/test_all.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1539 2023-01-17 22:10:28.000000 muscle3-0.6.0/integration_test/test_cpp_macro_micro.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3284 2022-07-15 14:58:45.000000 muscle3-0.6.0/integration_test/test_cpp_mmp_client.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1799 2022-07-15 14:58:45.000000 muscle3-0.6.0/integration_test/test_cpp_tcp_server.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1496 2023-01-17 22:10:28.000000 muscle3-0.6.0/integration_test/test_duplication_mapper.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1617 2023-01-17 22:10:28.000000 muscle3-0.6.0/integration_test/test_fortran_macro_micro.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1828 2022-07-15 14:58:45.000000 muscle3-0.6.0/integration_test/test_logging.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2321 2023-01-17 22:10:28.000000 muscle3-0.6.0/integration_test/test_mpi_macro_micro.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4011 2023-01-17 22:10:28.000000 muscle3-0.6.0/integration_test/test_parameter_overlays.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2591 2022-07-15 14:58:45.000000 muscle3-0.6.0/integration_test/test_registration.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)       86 2019-06-19 11:10:51.000000 muscle3-0.6.0/integration_test/test_version.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.413864 muscle3-0.6.0/libmuscle/
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.413864 muscle3-0.6.0/libmuscle/python/
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/libmuscle/python/libmuscle/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      616 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     8929 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/api_guard.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    10750 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/checkpoint_triggers.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    22909 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/communicator.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3434 2019-04-10 08:41:23.000000 muscle3-0.6.0/libmuscle/python/libmuscle/endpoint.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2232 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/grid.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    50217 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/instance.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2382 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/logging.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1160 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/logging_handler.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/libmuscle/python/libmuscle/manager/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2019-06-18 16:09:06.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     6744 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/instance_manager.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3058 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/instance_registry.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3793 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/instantiator.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4589 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/logger.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4719 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/manager.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    13753 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/mmp_server.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    16395 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/qcgpj_instantiator.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2303 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/run_dir.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    24928 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/snapshot_registry.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2019-06-18 16:59:49.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4128 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/conftest.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1436 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_instance_registry.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      724 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_logger.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    12503 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_mmp_request_handler.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    17815 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_snapshot_registry.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1891 2019-06-18 16:03:44.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_topology_store.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3812 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/manager/topology_store.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2019-05-08 06:55:56.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1183 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/protocol.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3219 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/tcp_transport_client.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4076 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/tcp_transport_server.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1661 2019-10-24 10:24:35.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/tcp_util.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/test/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2019-06-18 16:59:38.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/test/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      738 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/test/conftest.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      779 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/test/test_tcp_transport.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1124 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/test/test_tcp_transport_server.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1220 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/transport_client.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1572 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/transport_server.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      294 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mcp/type_registry.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    10386 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mmp_client.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2020 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mpp_client.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     7976 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/mpp_message.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1131 2020-09-23 19:59:56.000000 muscle3-0.6.0/libmuscle/python/libmuscle/outbox.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4437 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/peer_manager.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/libmuscle/python/libmuscle/planner/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/planner/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    26813 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/planner/planner.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     8084 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/port.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2854 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/post_office.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2461 2020-09-23 19:59:56.000000 muscle3-0.6.0/libmuscle/python/libmuscle/profiler.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2608 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/profiling.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    10104 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/runner.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3732 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/settings_manager.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4695 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/snapshot.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     9022 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/snapshot_manager.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/libmuscle/python/libmuscle/test/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2019-06-18 16:59:33.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      632 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/conftest.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4452 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_api_guard.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     6870 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_checkpoint_triggers.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    25578 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_communicator.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      316 2020-10-09 12:48:58.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_grid.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)    12749 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_instance.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     5741 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_mmp_client.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     6036 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_mpp_message.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1030 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_outbox.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2343 2019-05-08 06:55:56.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_port.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2430 2019-10-24 10:24:35.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_settings_manager.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2992 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_snapshot.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     5069 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_snapshot_manager.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)       57 2019-05-08 06:55:56.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_test.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1163 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/test/test_util.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      699 2022-07-15 14:58:45.000000 muscle3-0.6.0/libmuscle/python/libmuscle/timestamp.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2542 2023-01-17 22:10:28.000000 muscle3-0.6.0/libmuscle/python/libmuscle/util.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)       22 2023-01-17 22:16:13.000000 muscle3-0.6.0/libmuscle/python/libmuscle/version.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/muscle3/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2022-07-15 14:58:45.000000 muscle3-0.6.0/muscle3/__init__.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      241 2022-07-15 14:58:45.000000 muscle3-0.6.0/muscle3/conftest.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     5688 2023-01-17 22:10:28.000000 muscle3-0.6.0/muscle3/muscle3.py
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3358 2023-01-17 22:10:28.000000 muscle3-0.6.0/muscle3/muscle_manager.py
-drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-01-17 22:16:13.417863 muscle3-0.6.0/muscle3.egg-info/
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     3257 2023-01-17 22:16:13.000000 muscle3-0.6.0/muscle3.egg-info/PKG-INFO
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     4350 2023-01-17 22:16:13.000000 muscle3-0.6.0/muscle3.egg-info/SOURCES.txt
--rw-rw-r--   0 lourens   (1000) lourens   (1000)        1 2023-01-17 22:16:13.000000 muscle3-0.6.0/muscle3.egg-info/dependency_links.txt
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      111 2023-01-17 22:16:13.000000 muscle3-0.6.0/muscle3.egg-info/entry_points.txt
--rw-rw-r--   0 lourens   (1000) lourens   (1000)      247 2023-01-17 22:16:13.000000 muscle3-0.6.0/muscle3.egg-info/requires.txt
--rw-rw-r--   0 lourens   (1000) lourens   (1000)       18 2023-01-17 22:16:13.000000 muscle3-0.6.0/muscle3.egg-info/top_level.txt
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     1060 2023-01-17 22:16:13.421864 muscle3-0.6.0/setup.cfg
--rw-rw-r--   0 lourens   (1000) lourens   (1000)     2295 2023-01-17 22:10:28.000000 muscle3-0.6.0/setup.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    11357 2023-01-17 09:30:54.000000 muscle3-0.7.0/LICENSE
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)       66 2023-01-17 09:30:54.000000 muscle3-0.7.0/MANIFEST.in
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      172 2023-02-08 09:57:48.000000 muscle3-0.7.0/NOTICE
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2895 2023-06-22 21:28:15.755963 muscle3-0.7.0/PKG-INFO
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2098 2023-06-22 21:19:55.000000 muscle3-0.7.0/README.rst
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        6 2023-06-22 21:19:55.000000 muscle3-0.7.0/VERSION
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.751963 muscle3-0.7.0/libmuscle/
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.751963 muscle3-0.7.0/libmuscle/python/
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/libmuscle/python/libmuscle/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      706 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/__init__.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     8452 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/api_guard.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    10532 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/checkpoint_triggers.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    24714 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/communicator.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     3347 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/endpoint.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2232 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/grid.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    50269 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/instance.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2382 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/logging.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1169 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/logging_handler.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/libmuscle/python/libmuscle/manager/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/__init__.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     8585 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/instance_manager.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     3504 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/instance_registry.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     3964 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/instantiator.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     5490 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/logger.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     5455 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/manager.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    15571 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/mmp_server.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    18207 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/profile_database.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     9250 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/profile_store.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    16345 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/qcgpj_instantiator.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2303 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/run_dir.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    24825 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/snapshot_registry.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/__init__.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     4397 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/conftest.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1436 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_instance_registry.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      724 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_logger.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    12734 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_mmp_request_handler.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     5371 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_profile_database.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     3964 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_profile_store.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    17815 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_snapshot_registry.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1891 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_topology_store.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     3812 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/manager/topology_store.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/__init__.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1183 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/protocol.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     3762 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/tcp_transport_client.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     4242 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/tcp_transport_server.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1661 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/tcp_util.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/test/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/test/__init__.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      738 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/test/conftest.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      782 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/test/test_tcp_transport.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1124 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/test/test_tcp_transport_server.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1691 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/transport_client.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1773 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/transport_server.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      294 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mcp/type_registry.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    10376 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mmp_client.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2066 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mpp_client.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     7934 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/mpp_message.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1123 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/outbox.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     4425 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/peer_manager.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/libmuscle/python/libmuscle/planner/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/planner/__init__.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    30910 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/planner/planner.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     8074 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/port.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2842 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/post_office.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     3367 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/profiler.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     3749 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/profiling.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    11196 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/runner.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     5289 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/settings_manager.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     4695 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/snapshot.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     8985 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/snapshot_manager.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/libmuscle/python/libmuscle/test/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/__init__.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1440 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/conftest.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     4452 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_api_guard.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     6921 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_checkpoint_triggers.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    25910 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_communicator.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      316 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_grid.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)    12802 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_instance.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     5978 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_mmp_client.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     6036 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_mpp_message.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1030 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_outbox.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2343 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_port.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1452 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_profiler.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     4424 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_settings_manager.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2992 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_snapshot.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     4672 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_snapshot_manager.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)       57 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_test.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1163 2023-01-17 09:30:54.000000 muscle3-0.7.0/libmuscle/python/libmuscle/test/test_util.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      952 2023-06-22 21:19:55.000000 muscle3-0.7.0/libmuscle/python/libmuscle/timestamp.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2542 2023-02-08 09:57:48.000000 muscle3-0.7.0/libmuscle/python/libmuscle/util.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)       22 2023-06-22 21:28:15.000000 muscle3-0.7.0/libmuscle/python/libmuscle/version.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/muscle3/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        0 2023-01-17 09:30:54.000000 muscle3-0.7.0/muscle3/__init__.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      241 2023-01-17 09:30:54.000000 muscle3-0.7.0/muscle3/conftest.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     7877 2023-06-22 21:19:55.000000 muscle3-0.7.0/muscle3/muscle3.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     7670 2023-06-22 21:19:55.000000 muscle3-0.7.0/muscle3/muscle_manager.py
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     5511 2023-06-22 21:19:55.000000 muscle3-0.7.0/muscle3/profiling.py
+drwxrwxr-x   0 lourens   (1000) lourens   (1000)        0 2023-06-22 21:28:15.755963 muscle3-0.7.0/muscle3.egg-info/
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2895 2023-06-22 21:28:15.000000 muscle3-0.7.0/muscle3.egg-info/PKG-INFO
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     4130 2023-06-22 21:28:15.000000 muscle3-0.7.0/muscle3.egg-info/SOURCES.txt
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)        1 2023-06-22 21:28:15.000000 muscle3-0.7.0/muscle3.egg-info/dependency_links.txt
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      111 2023-06-22 21:28:15.000000 muscle3-0.7.0/muscle3.egg-info/entry_points.txt
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)      272 2023-06-22 21:28:15.000000 muscle3-0.7.0/muscle3.egg-info/requires.txt
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)       18 2023-06-22 21:28:15.000000 muscle3-0.7.0/muscle3.egg-info/top_level.txt
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     1067 2023-06-22 21:28:15.759963 muscle3-0.7.0/setup.cfg
+-rw-rw-r--   0 lourens   (1000) lourens   (1000)     2331 2023-06-22 21:19:55.000000 muscle3-0.7.0/setup.py
```

### Comparing `muscle3-0.6.0/LICENSE` & `muscle3-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/PKG-INFO` & `muscle3-0.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muscle3
-Version: 0.6.0
+Version: 0.7.0
 Summary: Version 3 of the MUltiScale Coupling Library and Environment
 Home-page: https://github.com/multiscale/muscle3
 Author: Lourens Veen
 Author-email: l.veen@esciencecenter.nl
 License: Apache License 2.0
 Keywords: multiscale,coupling,MUSCLE
 Platform: UNKNOWN
@@ -20,30 +20,22 @@
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://github.com/multiscale/muscle3/raw/develop/docs/source/muscle3_logo_readme.png
     :alt: MUSCLE3
 
-.. image:: https://readthedocs.org/projects/muscle3/badge/?version=master
-    :target: https://muscle3.readthedocs.io/en/develop/?badge=master
+.. image:: https://readthedocs.org/projects/muscle3/badge/?version=latest
+    :target: https://muscle3.readthedocs.io/en/develop/?badge=latest
     :alt: Documentation Build Status
 
 .. image:: https://github.com/multiscale/muscle3/workflows/continuous_integration/badge.svg?branch=master
     :target: https://github.com/multiscale/muscle3/actions
     :alt: Build Status
 
-.. image:: https://app.codacy.com/project/badge/Coverage/4542a84edcd947ee982a0bfabe617089
-    :target: https://www.codacy.com/gh/multiscale/muscle3/dashboard
-    :alt: Code Coverage
-
-.. image:: https://app.codacy.com/project/badge/Grade/4542a84edcd947ee982a0bfabe617089
-    :target: https://www.codacy.com/gh/multiscale/muscle3/dashboard
-    :alt: Codacy Grade
-
 .. image:: https://zenodo.org/badge/122876985.svg
    :target: https://zenodo.org/badge/latestdoi/122876985
 
 .. image:: https://img.shields.io/badge/rsd-muscle3-00a3e3.svg
    :target: https://www.research-software.nl/software/muscle3
 
 |
```

### Comparing `muscle3-0.6.0/README.rst` & `muscle3-0.7.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 .. image:: https://github.com/multiscale/muscle3/raw/develop/docs/source/muscle3_logo_readme.png
     :alt: MUSCLE3
 
-.. image:: https://readthedocs.org/projects/muscle3/badge/?version=master
-    :target: https://muscle3.readthedocs.io/en/develop/?badge=master
+.. image:: https://readthedocs.org/projects/muscle3/badge/?version=latest
+    :target: https://muscle3.readthedocs.io/en/develop/?badge=latest
     :alt: Documentation Build Status
 
 .. image:: https://github.com/multiscale/muscle3/workflows/continuous_integration/badge.svg?branch=master
     :target: https://github.com/multiscale/muscle3/actions
     :alt: Build Status
 
-.. image:: https://app.codacy.com/project/badge/Coverage/4542a84edcd947ee982a0bfabe617089
-    :target: https://www.codacy.com/gh/multiscale/muscle3/dashboard
-    :alt: Code Coverage
-
-.. image:: https://app.codacy.com/project/badge/Grade/4542a84edcd947ee982a0bfabe617089
-    :target: https://www.codacy.com/gh/multiscale/muscle3/dashboard
-    :alt: Codacy Grade
-
 .. image:: https://zenodo.org/badge/122876985.svg
    :target: https://zenodo.org/badge/latestdoi/122876985
 
 .. image:: https://img.shields.io/badge/rsd-muscle3-00a3e3.svg
    :target: https://www.research-software.nl/software/muscle3
 
 |
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/__init__.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from libmuscle.communicator import Message
 from libmuscle.grid import Grid
 from libmuscle.instance import Instance, InstanceFlags
+from libmuscle.manager.profile_database import ProfileDatabase
 from libmuscle.version import __version__
 from libmuscle import runner
 
 
 # Note that libmuscle.version above is created by the build system; it's okay
 # that it's not present.
 
 __all__ = [
-        '__version__', 'Grid', 'Instance', 'InstanceFlags', 'Message', 'runner']
+        '__version__', 'Grid', 'Instance', 'InstanceFlags', 'Message',
+        'ProfileDatabase', 'runner']
 
 
 # export InstanceFlag members to the module namespace
 # adapted from https://github.com/python/cpython/blob/3.10/Lib/re.py#L179
 globals().update(InstanceFlags.__members__)
 __all__.extend(InstanceFlags.__members__)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/api_guard.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/api_guard.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,14 @@
     in for the case where checkpointing is implemented. By tracking
     the phase that the model should be in, we can detect incorrect API
     usage.
 
     This does not match the yMMSL operators, as it is more
     fine-grained and concerns checkpointing, which is not represented
     in the SEL.
-
-    Note that AFTER_REUSE_INSTANCE and BEFORE_RESUMING refer to the
-    same place in the code. AFTER_REUSE_INSTANCE is used when we
-    don't know yet if the code has checkpointing support, and so we
-    don't know whether the next call is to resuming() or to
-    reuse_instance(). Once a checkpointing function has been called,
-    we know that we should expect resume() after reuse_instance() and
-    we use BEFORE_RESUMING accordingly.
     """
     BEFORE_FIRST_REUSE_INSTANCE = auto()
     """Before the first time calling reuse_instance"""
 
     BEFORE_REUSE_INSTANCE = auto()
     """Before calling reuse_instance"""
 
@@ -55,29 +47,29 @@
     The verify_* functions are called when the corresponding function
     on Instance is called, to check that we're in the right phase. They
     raise a RuntimeError if there's a problem. The *_done functions are
     called to signal that the corresponding function finished
     successfully, and that we are moving on to the next phase.
     """
     def __init__(self, uses_checkpointing: bool) -> None:
-        """Create an APIPhaseTracker.
+        """Create an APIGuard.
 
-        This starts the tracker in BEFORE_FIRST_REUSE_INSTANCE.
+        This starts the tracker in the phase BEFORE_FIRST_REUSE_INSTANCE.
         """
         self._phase = APIPhase.BEFORE_FIRST_REUSE_INSTANCE
         self._uses_checkpointing = uses_checkpointing
 
     def _generic_error_messages(self, verify_phase: str) -> None:
         if self._phase in (
                 APIPhase.BEFORE_FIRST_REUSE_INSTANCE,
                 APIPhase.AFTER_REUSE_LOOP):
             msg = f'Please only call {verify_phase} inside the reuse loop.'
         elif self._phase == APIPhase.BEFORE_REUSE_INSTANCE:
             msg = (
-                    'Please do not call {verify_phase} after'
+                    f'Please do not call {verify_phase} after'
                     ' should_save_final_snapshot. should_save_final_snapshot'
                     ' should be at the end of the reuse loop.')
         elif self._phase == APIPhase.BEFORE_RESUMING:
             msg = 'Inside the reuse loop you must call resuming first.'
         elif self._phase == APIPhase.BEFORE_LOAD_SNAPSHOT:
             msg = (
                     'If resuming returns True, then you must call'
@@ -136,15 +128,14 @@
 
     def resuming_done(self, resuming: bool) -> None:
         """Update phase on successful resuming().
 
         Args:
             resuming: Whether we're resuming or not.
         """
-        self._uses_checkpointing = True
         if resuming:
             self._phase = APIPhase.BEFORE_LOAD_SNAPSHOT
         else:
             self._phase = APIPhase.BEFORE_SHOULD_INIT
 
     def verify_load_snapshot(self) -> None:
         """Check load_snapshot()"""
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/checkpoint_triggers.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/checkpoint_triggers.py`

 * *Files 11% similar despite different names*

```diff
@@ -74,29 +74,26 @@
     as long as ``start + i*step <= stop``.
 
     Stop may be omitted, in which case the range is infinite.
 
     Start may be omitted, in which case the range is equivalent to an "at" rule
     ``[..., -n*step, ..., -step, 0, step, 2*step, ...]`` for as long as
     ``i*step <= stop``.
-
-    Note: the "every" rule is a special case of a range with start and stop
-    omitted, and is handled by this class as well
     """
 
     def __init__(self, range: CheckpointRangeRule) -> None:
         """Create a range of checkpoints
 
         Args:
             range: checkpoint range defining start, stop and step.
         """
         self._start = range.start
         self._stop = range.stop
         self._every = range.every
-        self._last = None  # type: Union[int, float, None]
+        self._last: Union[int, float, None] = None
         if self._stop is not None:
             start = 0 if self._start is None else self._start
             diff = self._stop - start
             self._last = start + (diff // self._every) * self._every
 
     def next_checkpoint(self, cur_time: float) -> Optional[float]:
         if self._start is not None and cur_time < self._start:
@@ -114,25 +111,25 @@
             return float(self._last)
         start = 0 if self._start is None else self._start
         diff = cur_time - start
         return float(start + (diff // self._every) * self._every)
 
 
 class CombinedCheckpointTriggers(CheckpointTrigger):
-    """Checkpoint trigger based on a combination of "every", "at" and "ranges"
+    """Checkpoint trigger based on a combination of "at" and "ranges"
     """
 
     def __init__(self, checkpoint_rules: List[CheckpointRule]) -> None:
         """Create a new combined checkpoint trigger from the given rules
 
         Args:
             checkpoint_rules: checkpoint rules (from ymmsl)
         """
-        self._triggers = []     # type: List[CheckpointTrigger]
-        at_rules = []           # type: List[CheckpointAtRule]
+        self._triggers: List[CheckpointTrigger] = []
+        at_rules: List[CheckpointAtRule] = []
         for rule in checkpoint_rules:
             if isinstance(rule, CheckpointAtRule):
                 if rule.at:
                     at_rules.append(rule)
             elif isinstance(rule, CheckpointRangeRule):
                 self._triggers.append(RangeCheckpointTrigger(rule))
             else:
@@ -161,15 +158,15 @@
 
 class TriggerManager:
     """Manages all checkpoint triggers and checks if a snapshot must be saved.
     """
 
     def __init__(self) -> None:
         self._has_checkpoints = False
-        self._last_triggers = []    # type: List[str]
+        self._last_triggers: List[str] = []
         self._cpts_considered_until = float('-inf')
 
     def set_checkpoint_info(
             self, elapsed: float, checkpoints: Checkpoints) -> None:
         """Register checkpoint info received from the muscle manager.
         """
         self._mono_to_elapsed = elapsed - time.monotonic()
@@ -180,19 +177,19 @@
 
         self._has_checkpoints = True
 
         self._checkpoint_at_end = checkpoints.at_end
 
         self._wall = CombinedCheckpointTriggers(checkpoints.wallclock_time)
         self._prevwall = 0.0
-        self._nextwall = self._wall.next_checkpoint(0.0)  # type: Optional[float]
+        self._nextwall: Optional[float] = self._wall.next_checkpoint(0.0)
 
         self._sim = CombinedCheckpointTriggers(checkpoints.simulation_time)
-        self._prevsim = None        # type: Optional[float]
-        self._nextsim = None        # type: Optional[float]
+        self._prevsim: Optional[float] = None
+        self._nextsim: Optional[float] = None
 
     def elapsed_walltime(self) -> float:
         """Returns elapsed wallclock_time in seconds.
         """
         return time.monotonic() + self._mono_to_elapsed
 
     def checkpoints_considered_until(self) -> float:
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/communicator.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/communicator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
 from typing import Any, Dict, List, Optional, Tuple, cast
 from ymmsl import Conduit, Identifier, Operator, Reference, Settings
 
 from libmuscle.endpoint import Endpoint
 from libmuscle.mpp_message import ClosePort, MPPMessage
 from libmuscle.mpp_client import MPPClient
+from libmuscle.mcp.tcp_util import SocketClosed
 from libmuscle.mcp.transport_server import TransportServer
 from libmuscle.mcp.type_registry import transport_server_types
 from libmuscle.peer_manager import PeerManager
 from libmuscle.post_office import PostOffice
 from libmuscle.port import Port
 from libmuscle.profiler import Profiler
-from libmuscle.profiling import ProfileEventType
+from libmuscle.profiling import (
+        ProfileEvent, ProfileEventType, ProfileTimestamp)
 
 
 _logger = logging.getLogger(__name__)
 
 
 MessageObject = Any
 
@@ -86,24 +88,24 @@
         """
         self._kernel = kernel
         self._index = index
         self._declared_ports = declared_ports
         self._post_office = PostOffice()
         self._profiler = profiler
 
-        self._servers = list()  # type: List[TransportServer]
+        self._servers: List[TransportServer] = []
 
         # indexed by remote instance id
-        self._clients = dict()  # type: Dict[Reference, MPPClient]
+        self._clients: Dict[Reference, MPPClient] = {}
 
         for server_type in transport_server_types:
             server = server_type(self._post_office)
             self._servers.append(server)
 
-        self._ports = dict()   # type: Dict[str, Port]
+        self._ports: Dict[str, Port] = {}
 
     def get_locations(self) -> List[str]:
         """Returns a list of locations that we can be reached at.
 
         These locations are of the form 'protocol:location', where
         the protocol name does not contain a colon and location may
         be an arbitrary string.
@@ -152,15 +154,15 @@
         """Returns a description of the ports this Communicator has.
 
         Returns:
             A dictionary, indexed by Operator, containing lists of
             port names. Operators with no associated ports are not
             included.
         """
-        result = dict()     # type: Dict[Operator, List[str]]
+        result: Dict[Operator, List[str]] = {}
         for port_name, port in self._ports.items():
             if port.operator not in result:
                 result[port.operator] = list()
             result[port.operator].append(port_name)
         return result
 
     def port_exists(self, port_name: str) -> bool:
@@ -193,15 +195,15 @@
             message: The message to be sent.
             slot: The slot to send the message on, if any.
             checkpoints_considered_until: When we last checked if we
                 should save a snapshot (wallclock time).
         """
         if slot is None:
             _logger.debug('Sending message on {}'.format(port_name))
-            slot_list = []  # type: List[int]
+            slot_list: List[int] = []
         else:
             _logger.debug('Sending message on {}[{}]'.format(port_name, slot))
             slot_list = [slot]
             slot_length = self._ports[port_name].get_length()
             if slot_length <= slot:
                 raise RuntimeError(('Slot out of bounds. You are sending on'
                                     ' slot {} of port "{}", which is of length'
@@ -210,41 +212,44 @@
 
         snd_endpoint = self.__get_endpoint(port_name, slot_list)
         if not self._peer_manager.is_connected(snd_endpoint.port):
             # log sending on disconnected port
             return
 
         port = self._ports[port_name]
-        profile_event = self._profiler.start(ProfileEventType.SEND, port,
-                                             None, slot, None)
+        profile_event = ProfileEvent(
+                ProfileEventType.SEND, ProfileTimestamp(), None, port, None,
+                slot, port.get_num_messages(slot), None, message.timestamp)
 
         recv_endpoints = self._peer_manager.get_peer_endpoints(
                 snd_endpoint.port, slot_list)
 
         port_length = None
         if port.is_resizable():
             port_length = port.get_length()
 
         for recv_endpoint in recv_endpoints:
-            mcp_message = MPPMessage(snd_endpoint.ref(), recv_endpoint.ref(),
+            mpp_message = MPPMessage(snd_endpoint.ref(), recv_endpoint.ref(),
                                      port_length,
                                      message.timestamp, message.next_timestamp,
                                      cast(Settings, message.settings),
                                      port.get_num_messages(slot),
                                      checkpoints_considered_until,
                                      message.data)
-            encoded_message = mcp_message.encoded()
+            encoded_message = mpp_message.encoded()
             self._post_office.deposit(recv_endpoint.ref(), encoded_message)
 
         port.increment_num_messages(slot)
 
         profile_event.stop()
         if port.is_vector():
             profile_event.port_length = port.get_length()
         profile_event.message_size = len(encoded_message)
+        if not isinstance(message.data, ClosePort):
+            self._profiler.record_event(profile_event)
 
     def receive_message(self, port_name: str, slot: Optional[int] = None,
                         default: Optional[Message] = None
                         ) -> Tuple[Message, float]:
         """Receive a message and attached settings overlay.
 
         Receiving is a blocking operation. This function will contact
@@ -269,15 +274,15 @@
 
         Raises:
             RuntimeError: If no default was given and the port is not
                 connected.
         """
         if slot is None:
             port_and_slot = port_name
-            slot_list = []      # type: List[int]
+            slot_list: List[int] = []
         else:
             port_and_slot = f"{port_name}[{slot}]"
             slot_list = [slot]
         _logger.debug('Waiting for message on {}'.format(port_and_slot))
 
         recv_endpoint = self.__get_endpoint(port_name, slot_list)
 
@@ -297,40 +302,75 @@
             port = self._ports[port_name]
         else:
             # it's muscle_settings_in here, because we check for unknown
             # user ports in Instance already, and we don't have any other
             # built-in automatic ports.
             port = self._muscle_settings_in
 
-        profile_event = self._profiler.start(ProfileEventType.RECEIVE, port,
-                                             None, slot, None)
+        receive_event = ProfileEvent(
+                ProfileEventType.RECEIVE, ProfileTimestamp(), None, port, None,
+                slot, port.get_num_messages())
 
         # peer_manager already checks that there is at most one snd_endpoint
         # connected to the port we receive on
         snd_endpoint = self._peer_manager.get_peer_endpoints(
                 recv_endpoint.port, slot_list)[0]
         client = self.__get_client(snd_endpoint.instance())
-        mpp_message_bytes = client.receive(recv_endpoint.ref())
+        try:
+            mpp_message_bytes, profile = client.receive(recv_endpoint.ref())
+        except (ConnectionError, SocketClosed) as exc:
+            raise RuntimeError(
+                "Error while receiving a message: connection with peer"
+                f" '{snd_endpoint.kernel}' was lost. Did the peer crash?"
+            ) from exc
+
+        recv_decode_event = ProfileEvent(
+                ProfileEventType.RECEIVE_DECODE, ProfileTimestamp(), None,
+                port, None, slot, port.get_num_messages(),
+                len(mpp_message_bytes))
         mpp_message = MPPMessage.from_bytes(mpp_message_bytes)
+        recv_decode_event.stop()
 
         if mpp_message.port_length is not None:
             if port.is_resizable():
                 port.set_length(mpp_message.port_length)
 
         if isinstance(mpp_message.data, ClosePort):
             port.set_closed(slot)
 
         message = Message(
                 mpp_message.timestamp, mpp_message.next_timestamp,
                 mpp_message.data, mpp_message.settings_overlay)
 
-        profile_event.stop()
+        recv_wait_event = ProfileEvent(
+                ProfileEventType.RECEIVE_WAIT, profile[0], profile[1], port,
+                mpp_message.port_length, slot, port.get_num_messages(),
+                len(mpp_message_bytes), message.timestamp)
+
+        recv_xfer_event = ProfileEvent(
+                ProfileEventType.RECEIVE_TRANSFER, profile[1], profile[2],
+                port, mpp_message.port_length, slot, port.get_num_messages(),
+                len(mpp_message_bytes), message.timestamp)
+
+        recv_decode_event.message_timestamp = message.timestamp
+        receive_event.message_timestamp = message.timestamp
+
         if port.is_vector():
-            profile_event.port_length = port.get_length()
-        profile_event.message_size = len(mpp_message_bytes)
+            receive_event.port_length = port.get_length()
+            recv_wait_event.port_length = port.get_length()
+            recv_xfer_event.port_length = port.get_length()
+            recv_decode_event.port_length = port.get_length()
+
+        receive_event.message_size = len(mpp_message_bytes)
+
+        if not isinstance(mpp_message.data, ClosePort):
+            self._profiler.record_event(recv_wait_event)
+            self._profiler.record_event(recv_xfer_event)
+            self._profiler.record_event(recv_decode_event)
+            self._profiler.record_event(receive_event)
 
         expected_message_number = port.get_num_messages(slot)
         if expected_message_number != mpp_message.message_number:
             if (expected_message_number - 1 == mpp_message.message_number and
                     port.is_resuming(slot)):
                 _logger.debug(f'Discarding received message on {port_and_slot}'
                               ': resuming from weakly consistent snapshot')
@@ -376,28 +416,28 @@
         self._post_office.wait_for_receivers()
 
         for server in self._servers:
             server.close()
 
     def restore_message_counts(self, port_message_counts: Dict[str, List[int]]
                                ) -> None:
-        """Restore message counts on all ports
+        """Restore message counts on all ports.
         """
         for port_name, num_messages in port_message_counts.items():
             if port_name == "muscle_settings_in":
                 self._muscle_settings_in.restore_message_counts(num_messages)
             elif port_name in self._ports:
                 self._ports[port_name].restore_message_counts(num_messages)
             else:
                 raise RuntimeError(f'Unknown port {port_name} in snapshot.'
                                    ' Have your port definitions changed since'
                                    ' the snapshot was taken?')
 
     def get_message_counts(self) -> Dict[str, List[int]]:
-        """Get message counts for all ports on the communicator
+        """Get message counts for all ports on the communicator.
         """
         port_message_counts = {port_name: port.get_message_counts()
                                for port_name, port in self._ports.items()}
         port_message_counts["muscle_settings_in"] = \
             self._muscle_settings_in.get_message_counts()
         return port_message_counts
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/endpoint.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,18 +47,18 @@
 
         Args:
             kernel: Name of an instance's kernel.
             index: Index of the kernel instance.
             port: Name of the port used.
             slot: Slot on which to send or receive.
         """
-        self.kernel = kernel  # type: Reference
-        self.index = index    # type: List[int]
-        self.port = port      # type: Identifier
-        self.slot = slot      # type: List[int]
+        self.kernel = kernel
+        self.index = index
+        self.port = port
+        self.slot = slot
 
     def ref(self) -> Reference:
         """Express as Reference.
 
         This yields a valid Reference of the form
         kernel[index].port[slot], with index and port omitted if they
         are zero-length.
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/grid.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/grid.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/instance.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/instance.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 from libmuscle.communicator import Communicator, Message
 from libmuscle.settings_manager import SettingsManager
 from libmuscle.logging import LogLevel
 from libmuscle.logging_handler import MuscleManagerHandler
 from libmuscle.mpp_message import ClosePort
 from libmuscle.mmp_client import MMPClient
 from libmuscle.profiler import Profiler
-from libmuscle.profiling import ProfileEventType
+from libmuscle.profiling import (
+        ProfileEvent, ProfileEventType, ProfileTimestamp)
 from libmuscle.snapshot_manager import SnapshotManager
 from libmuscle.util import extract_log_file_location
 
 
 _logger = logging.getLogger(__name__)
 
 
@@ -62,32 +63,33 @@
     """Indicate that this instance supports checkpointing.
 
     You may not use any checkpointing API calls when this flag is not supplied.
     """
 
     KEEPS_NO_STATE_FOR_NEXT_USE = auto()
     """Indicate this instance does not carry state between iterations of the
-    reuse loop.
+    reuse loop. Specifying this flag is equivalent to
+    :external:py:attr:`ymmsl.KeepsStateForNextUse.NO`.
 
-    This corresponds to :external:py:attr:`ymmsl.KeepsStateForNextUse.NO`.
-
-    If neither :attr:`KEEPS_NO_STATE_FOR_NEXT_USE` and
-    :attr:`STATE_NOT_REQUIRED_FOR_NEXT_USE` are supplied, this corresponds to
-    :external:py:attr:`ymmsl.KeepsStateForNextUse.REQUIRED`.
+    By default, (if neither :attr:`KEEPS_NO_STATE_FOR_NEXT_USE` nor
+    :attr:`STATE_NOT_REQUIRED_FOR_NEXT_USE` are provided), the instance is assumed
+    to keep state between reuses, and to require that state (equivalent to
+    :external:py:attr:`ymmsl.KeepsStateForNextUse.NECESSARY`).
     """
 
     STATE_NOT_REQUIRED_FOR_NEXT_USE = auto()
     """Indicate this instance carries state between iterations of the
     reuse loop, however this state is not required for restarting.
+    Specifying this flag is equivalent to
+    :external:py:attr:`ymmsl.KeepsStateForNextUse.HELPFUL`.
 
-    This corresponds to :external:py:attr:`ymmsl.KeepsStateForNextUse.HELPFUL`.
-
-    If neither :attr:`KEEPS_NO_STATE_FOR_NEXT_USE` and
-    :attr:`STATE_NOT_REQUIRED_FOR_NEXT_USE` are supplied, this corresponds to
-    :external:py:attr:`ymmsl.KeepsStateForNextUse.REQUIRED`.
+    By default, (if neither :attr:`KEEPS_NO_STATE_FOR_NEXT_USE` nor
+    :attr:`STATE_NOT_REQUIRED_FOR_NEXT_USE` are provided), the instance is assumed
+    to keep state between reuses, and to require that state (equivalent to
+    :external:py:attr:`ymmsl.KeepsStateForNextUse.NECESSARY`).
     """
 
 
 _CHECKPOINT_SUPPORT_MASK = (
         InstanceFlags.USES_CHECKPOINT_API |
         InstanceFlags.KEEPS_NO_STATE_FOR_NEXT_USE |
         InstanceFlags.STATE_NOT_REQUIRED_FOR_NEXT_USE)
@@ -120,96 +122,77 @@
                     ' development: the API may change in a future MUSCLE3'
                     ' release.')
 
         # Note that these are accessed by Muscle3, but otherwise private.
         self._name, self._index = self.__make_full_name()
         """Name and index of this instance."""
 
+        self._instance_id = self._name + self._index
+        """Full id of this instance."""
+
         mmp_location = self.__extract_manager_location()
-        self.__manager = MMPClient(mmp_location)
+        self.__manager = MMPClient(self._instance_id, mmp_location)
         """Client object for talking to the manager."""
 
         self.__set_up_logging()
 
         self._api_guard = APIGuard(
                 InstanceFlags.USES_CHECKPOINT_API in self._flags)
         """Checks that the user uses the API correctly."""
 
-        self._profiler = Profiler(self._instance_name(), self.__manager)
+        self._profiler = Profiler(self.__manager)
         """Profiler for this instance."""
 
         self._communicator = Communicator(
                 self._name, self._index, ports, self._profiler)
         """Communicator for this instance."""
 
         self._declared_ports = ports
         """Declared ports for this instance."""
 
         self._settings_manager = SettingsManager()
         """Settings for this instance."""
 
         self._snapshot_manager = SnapshotManager(
-                self._instance_name(), self.__manager, self._communicator)
+                self._instance_id, self.__manager, self._communicator)
         """Resumes, loads and saves snapshots."""
 
         self._trigger_manager = TriggerManager()
         """Keeps track of checkpoints and triggers snapshots."""
 
-        self._first_run = None          # type: Optional[bool]
+        self._first_run: Optional[bool] = None
         """Whether this is the first iteration of the reuse loop"""
 
-        self._do_reuse = None           # type: Optional[bool]
+        self._do_reuse: Optional[bool] = None
         """Whether to enter this iteration of the reuse loop
 
         This is None during the reuse loop, and set between
         should_save_final_snapshot and reuse_instance.
         """
 
         self._do_resume = False
         """Whether to resume on this iteration of the reuse loop"""
 
         self._do_init = False
         """Whether to do f_init on this iteration of the reuse loop"""
 
-        self._f_init_cache = dict()     # type: _FInitCacheType
+        self._f_init_cache: _FInitCacheType = {}
         """Stores pre-received messages for f_init ports"""
 
         self._register()
         self._connect()
-
-        # Note: get_checkpoint_info needs to have the ports initialized
+        # Note: self._setup_checkpointing() needs to have the ports initialized
         # so it comes after self._connect()
-        checkpoint_info = self.__manager.get_checkpoint_info(
-                self._instance_name())
-
-        elapsed_time, checkpoints = checkpoint_info[0:2]
-        self._trigger_manager.set_checkpoint_info(elapsed_time, checkpoints)
-
-        if checkpoints and not (self._flags & _CHECKPOINT_SUPPORT_MASK):
-            raise RuntimeError(
-                    'The workflow has requested checkpoints, but this instance'
-                    ' does not support checkpointing. Please consult the'
-                    ' MUSCLE3 checkpointing documentation how to add'
-                    ' checkpointing support.')
-
-        resume_snapshot, snapshot_dir = checkpoint_info[2:4]
-        saved_at = self._snapshot_manager.prepare_resume(
-                resume_snapshot, snapshot_dir)
-        # Resume settings overlay
-        overlay = self._snapshot_manager._resume_overlay
-        if overlay is not None:
-            self._settings_manager.overlay = overlay
-
-        if saved_at is not None:
-            self._trigger_manager.update_checkpoints(saved_at)
-
+        self._setup_checkpointing()
+        # profiling and logging need settings, so come after register_()
         self._set_local_log_level()
         self._set_remote_log_level()
+        self._setup_profiling()
 
-    def reuse_instance(self, apply_overlay: Optional[bool] = None) -> bool:
+    def reuse_instance(self) -> bool:
         """Decide whether to run this instance again.
 
         In a multiscale simulation, instances get reused all the time.
         For example, in a macro-micro simulation, the micromodel does a
         complete run for every timestep of the macromodel. Rather than
         starting up a new instance of the micromodel, which could be
         expensive, we reuse a single instance many times.
@@ -242,15 +225,15 @@
         self._api_guard.verify_reuse_instance()
 
         if self._do_reuse is not None:
             # thank you, should_save_final_snapshot, for running this already
             do_reuse = self._do_reuse
             self._do_reuse = None
         else:
-            do_reuse = self._decide_reuse_instance(apply_overlay)
+            do_reuse = self._decide_reuse_instance()
 
         # now _first_run, _do_resume and _do_init are also set correctly
 
         do_implicit_checkpoint = (
                 not self._first_run and
                 InstanceFlags.USES_CHECKPOINT_API not in self._flags and
                 (InstanceFlags.STATE_NOT_REQUIRED_FOR_NEXT_USE in self._flags or
@@ -287,14 +270,24 @@
         supposed to send.
 
         Args:
             message: An error message describing the problem.
         """
         self.__shutdown(message)
 
+    def list_settings(self) -> List[str]:
+        """List settings by name.
+
+        This function returns a list of names of the available settings.
+
+        Return:
+            A list of setting names.
+        """
+        return self._settings_manager.list_settings(self._instance_id)
+
     @overload
     def get_setting(self, name: str, typ: Literal['str']) -> str:
         ...
 
     @overload
     def get_setting(self, name: str, typ: Literal['int']) -> int:
         ...
@@ -335,15 +328,15 @@
 
         Raises:
             KeyError: If no value was set for this setting.
             TypeError: If the type of the setting's value was not
                     as expected.
         """
         return self._settings_manager.get_setting(
-                self._instance_name(), Reference(name), typ)
+                self._instance_id, Reference(name), typ)
 
     def list_ports(self) -> Dict[Operator, List[str]]:
         """Returns a description of the ports that this Instance has.
 
         Note that the result has almost the same format as the port
         declarations you pass when making an Instance. The only
         difference is that the port names never have `[]` at the end,
@@ -525,16 +518,15 @@
 
         This method returns True for the first iteration of the reuse loop after
         resuming from a previously taken snapshot. When resuming from a
         snapshot, the submodel must load its state from the snapshot as returned
         by :meth:`load_snapshot`.
 
         Returns:
-            True iff the submodel must resume from a snapshot instead of the
-            usual F_INIT step during this iteration of the reuse loop.
+            True iff the submodel must resume from a snapshot.
         """
         self._api_guard.verify_resuming()
         self._api_guard.resuming_done(self._do_resume)
         return self._do_resume
 
     def should_init(self) -> bool:
         """Check if this instance should initialize.
@@ -555,15 +547,15 @@
     def load_snapshot(self) -> Message:
         """Load a snapshot.
 
         Must only be called when :meth:`resuming` returns True.
 
         Returns:
             Message object containing the state as saved in a previous run
-            through :meth:`save_snapshot` or :meth:`save_final_snapshot`
+            through :meth:`save_snapshot` or :meth:`save_final_snapshot`.
 
         Raises:
             RuntimeError: if not resuming from a snapshot.
         """
         self._api_guard.verify_load_snapshot()
         result = self._snapshot_manager.load_snapshot()
         self._api_guard.load_snapshot_done()
@@ -573,22 +565,22 @@
         """Check if a snapshot should be saved after the S Operator of the
         submodel.
 
         This method checks if a snapshot should be saved right now, based on the
         provided timestamp and passed wallclock time.
 
         When this method returns True, the submodel must also save a snapshot
-        through :meth:`save_snapshot`. A RuntimeError will be generated when not
-        doing so.
+        through :meth:`save_snapshot`. A RuntimeError will be generated if this
+        is not done.
 
         See also :meth:`should_save_final_snapshot` for the variant that must be
         called at the end of the reuse loop.
 
         Args:
-            timestamp: current timestamp of the submodel
+            timestamp: current timestamp of the submodel.
 
         Returns:
             True iff a snapshot should be taken by the submodel according to the
             checkpoint rules provided in the ymmsl configuration.
         """
         self._api_guard.verify_should_save_snapshot()
         result = self._trigger_manager.should_save_snapshot(timestamp)
@@ -600,20 +592,14 @@
 
         Before saving a snapshot, you should check using
         :meth:`should_save_snapshot` if a snapshot should be saved according to
         the checkpoint rules specified in the ymmsl configuration. You should
         use the same timestamp in the provided Message object as used to query
         `should_save_snapshot`.
 
-        Although it is allowed to save a snapshot even when
-        :meth:`should_save_snapshot` returns False, you should avoid this: this
-        situation is not likely to lead to a consistent snapshot over all
-        submodels of the run (and therefore it is not useful to restart from).
-        It could also lead to a lot of snapshot files clogging your file system.
-
         See also :meth:`save_final_snapshot` for the variant that must be called
         at the end of the reuse loop.
 
         Args:
             message: Message object that is saved as snapshot. The message
                 timestamp attribute should be the same as passed to
                 :meth:`should_save_snapshot`. The data attribute can be used to
@@ -624,38 +610,29 @@
             raise RuntimeError('Please specify a Message to save as snapshot.')
         self._save_snapshot(message, False)
         self._api_guard.save_snapshot_done()
 
     def should_save_final_snapshot(self) -> bool:
         """Check if a snapshot should be saved at the end of the reuse loop.
 
-        This method checks if a snapshot should be saved now.
+        This method checks if a snapshot should be saved at the end of the reuse
+        loop. All your communication on O_F ports must be finished before calling
+        this method, otherwise your simulation may deadlock.
 
         When this method returns True, the submodel must also save a snapshot
         through :meth:`save_final_snapshot`. A :class:`RuntimeError` will be
-        generated when not doing so.
+        generated if this is not done.
 
         See also :meth:`should_save_snapshot` for the variant that may be called
         inside of a time-integration loop of the submodel.
 
         .. note::
             This method will block until it can determine whether a final
-            snapshot should be taken. This means it must also determine if this
-            instance is reused. The optional keyword-only argument
-            `apply_overlay` has the same meaning as for :meth:`reuse_instance`.
-
-        Args:
-            apply_overlay: Whether to apply the received settings
-                overlay or to save it. If you're going to use
-                :meth:`receive_with_settings` on your F_INIT ports, set this to
-                False. If you don't know what that means, just call
-                :meth:`should_save_final_snapshot()` without specifying this and
-                everything will be fine. If it turns out that you did need to
-                specify False, MUSCLE3 will tell you about it in an error
-                message and you can add it still.
+            snapshot should be taken, because it must determine if this
+            instance is reused.
 
         Returns:
             True iff a final snapshot should be taken by the submodel according
             to the checkpoint rules provided in the ymmsl configuration.
         """
         self._api_guard.verify_should_save_final_snapshot()
 
@@ -669,20 +646,14 @@
     def save_final_snapshot(self, message: Message) -> None:
         """Save a snapshot at the end of the reuse loop.
 
         Before saving a snapshot, you should check using
         :meth:`should_save_final_snapshot` if a snapshot should be saved
         according to the checkpoint rules specified in the ymmsl configuration.
 
-        Although it is allowed to save a snapshot even when
-        :meth:`should_save_final_snapshot` returns False, you should avoid this:
-        this situation is not likely to lead to a consistent snapshot over all
-        submodels of the run (and therefore it is not useful to restart from).
-        It could also lead to a lot of snapshot files clogging your file system.
-
         See also :meth:`save_snapshot` for the variant that may be called after
         each S Operator of the submodel.
 
         Args:
             message: Message object that is saved as snapshot. The data
                 attribute can be used to store the internal state of the
                 submodel.
@@ -700,43 +671,85 @@
         return max(
                 (msg.timestamp for msg in self._f_init_cache.values()),
                 default=None)
 
     def _register(self) -> None:
         """Register this instance with the manager.
         """
-        register_event = self._profiler.start(ProfileEventType.REGISTER)
+        register_event = ProfileEvent(
+                ProfileEventType.REGISTER, ProfileTimestamp())
         locations = self._communicator.get_locations()
         port_list = self.__list_declared_ports()
-        self.__manager.register_instance(
-                self._instance_name(), locations, port_list)
-        register_event.stop()
+        self.__manager.register_instance(locations, port_list)
+        self._profiler.record_event(register_event)
         _logger.info('Registered with the manager')
 
     def _connect(self) -> None:
         """Connect this instance to the given peers / conduits.
         """
-        connect_event = self._profiler.start(ProfileEventType.CONNECT)
-        conduits, peer_dims, peer_locations = self.__manager.request_peers(
-                self._instance_name())
+        connect_event = ProfileEvent(
+                ProfileEventType.CONNECT, ProfileTimestamp())
+        conduits, peer_dims, peer_locations = self.__manager.request_peers()
         self._communicator.connect(conduits, peer_dims, peer_locations)
         self._settings_manager.base = self.__manager.get_settings()
-        connect_event.stop()
+        self._profiler.record_event(connect_event)
         _logger.info('Received peer locations and base settings')
 
     def _deregister(self) -> None:
         """Deregister this instance from the manager.
         """
-        deregister_event = self._profiler.start(ProfileEventType.DEREGISTER)
-        self.__manager.deregister_instance(self._instance_name())
-        deregister_event.stop()
-        # this is the last thing we'll profile, so flush messages
+        # Make sure we record this even if profiling is disabled, so
+        # that we always have register, connect and deregister at
+        # least.
+        self._profiler.set_level('all')
+
+        deregister_event = ProfileEvent(
+                ProfileEventType.DEREGISTER, ProfileTimestamp())
+        # We need to finish the event right away, because we need to
+        # submit it before deregistering, which is the last interaction
+        # with the manager we'll have.
+        self._profiler.record_event(deregister_event)
+
+        # This is the last thing we'll profile, so flush messages
         self._profiler.shutdown()
+        self.__manager.deregister_instance()
+
+        # Remove handler, the manager may be gone at this point so we
+        # cannot send it any more log messages.
+        logging.getLogger().removeHandler(self._mmp_handler)
         _logger.info('Deregistered from the manager')
 
+    def _setup_checkpointing(self) -> None:
+        """Setup checkpointing.
+        """
+        checkpoint_info = self.__manager.get_checkpoint_info()
+
+        elapsed_time, checkpoints = checkpoint_info[0:2]
+        self._trigger_manager.set_checkpoint_info(elapsed_time, checkpoints)
+
+        if checkpoints and not (self._flags & _CHECKPOINT_SUPPORT_MASK):
+            err_msg = (
+                    'The workflow has requested checkpoints, but this instance'
+                    ' does not support checkpointing. Please consult the'
+                    ' MUSCLE3 checkpointing documentation how to add'
+                    ' checkpointing support.')
+            self.__shutdown(err_msg)
+            raise RuntimeError(err_msg)
+
+        resume_snapshot, snapshot_dir = checkpoint_info[2:4]
+        saved_at = self._snapshot_manager.prepare_resume(
+                resume_snapshot, snapshot_dir)
+        # Resume settings overlay
+        overlay = self._snapshot_manager.resume_overlay
+        if overlay is not None:
+            self._settings_manager.overlay = overlay
+
+        if saved_at is not None:
+            self._trigger_manager.update_checkpoints(saved_at)
+
     @staticmethod
     def __extract_manager_location() -> str:
         """Gets the manager network location from the command line.
 
         We use a --muscle-manager=<host:port> argument to tell the
         MUSCLE library how to connect to the manager. This function
         will extract this argument from the command line arguments,
@@ -756,15 +769,15 @@
                 return arg[len(prefix):]
 
         return os.environ.get('MUSCLE_MANAGER', 'tcp:localhost:9000')
 
     def __set_up_logging(self) -> None:
         """Adds logging handlers for one or more instances.
         """
-        id_str = str(self._instance_name())
+        id_str = str(self._instance_id)
 
         logfile = extract_log_file_location('muscle3.{}.log'.format(id_str))
         if logfile is not None:
             local_handler = logging.FileHandler(str(logfile), mode='w')
             formatter = logging.Formatter(
                     '%(asctime)-15s: %(levelname)-7s %(name)s: %(message)s')
             local_handler.setFormatter(formatter)
@@ -772,16 +785,32 @@
             logging.getLogger('ymmsl').addHandler(local_handler)
 
         if self.__manager is not None:
             self._mmp_handler = MuscleManagerHandler(id_str, logging.WARNING,
                                                      self.__manager)
             logging.getLogger().addHandler(self._mmp_handler)
 
-    def _decide_reuse_instance(
-            self, apply_overlay: Optional[bool] = None) -> bool:
+    def _setup_profiling(self) -> None:
+        """Configures profiler with settings from settings.
+        """
+        try:
+            profile_level_str = self.get_setting('muscle_profile_level', 'str')
+        except KeyError:
+            profile_level_str = 'all'
+
+        if profile_level_str not in ('none', 'all'):
+            _logger.warning(
+                    'Invalid value for muscle_profile_level:'
+                    f' {profile_level_str}. Please specify "none" or "all".'
+                    ' Using default value "all".')
+            profile_level_str = 'all'
+
+        self._profiler.set_level(profile_level_str)
+
+    def _decide_reuse_instance(self) -> bool:
         """Decide whether and how to reuse the instance.
 
         This sets self._first_run, self._do_resume and self._do_init, and
         returns whether to reuse one more time. This is the real top of
         the reuse loop, and it gets called by reuse_instance and
         should_save_final_snapshot.
         """
@@ -797,15 +826,15 @@
             return True
 
         f_init_connected = self._have_f_init_connections()
 
         # resume from final
         if self._first_run and self._snapshot_manager.resuming_from_final():
             if f_init_connected:
-                got_f_init_messages = self._pre_receive(apply_overlay)
+                got_f_init_messages = self._pre_receive()
                 self._do_resume = True
                 self._do_init = True
                 return got_f_init_messages
             else:
                 self._do_resume = False     # unused
                 self._do_init = False       # unused
                 return False
@@ -815,15 +844,15 @@
 
         # simple straight single run without resuming
         if not f_init_connected:
             self._do_init = self._first_run
             return self._first_run
 
         # not resuming and f_init connected, run while we get messages
-        got_f_init_messages = self._pre_receive(apply_overlay)
+        got_f_init_messages = self._pre_receive()
         self._do_init = got_f_init_messages
         return got_f_init_messages
 
     def _save_snapshot(
             self, message: Optional[Message], final: bool,
             f_init_max_timestamp: Optional[float] = None) -> None:
         """Save a snapshot to disk and notify manager.
@@ -906,15 +935,15 @@
                          ) -> Tuple[Reference, List[int]]:
         """Returns instance name and index.
 
         This takes the argument to the --muscle-instance= command-line
         option and splits it into a component name and an index.
         """
         def split_reference(ref: Reference) -> Tuple[Reference, List[int]]:
-            index = list()     # type: List[int]
+            index: List[int] = []
             i = 0
             while i < len(ref) and isinstance(ref[i], Identifier):
                 i += 1
             name = ref[:i]
 
             while i < len(ref) and isinstance(ref[i], int):
                 index.append(cast(int, ref[i]))
@@ -954,19 +983,14 @@
             for operator, port_names in self._declared_ports.items():
                 for name in port_names:
                     if name.endswith('[]'):
                         name = name[:-2]
                     result.append(Port(Identifier(name), operator))
         return result
 
-    def _instance_name(self) -> Reference:
-        """Returns the full instance name.
-        """
-        return self._name + self._index
-
     def __check_port(self, port_name: str) -> None:
         if not self._communicator.port_exists(port_name):
             err_msg = (('Port "{}" does not exist on "{}". Please check'
                         ' the name and the list of ports you gave for'
                         ' this component.').format(port_name, self._name))
             self.__shutdown(err_msg)
             raise RuntimeError(err_msg)
@@ -978,24 +1002,24 @@
         """
         ports = self._communicator.list_ports()
         f_init_connected = any(
                 [self.is_connected(port)
                  for port in ports.get(Operator.F_INIT, [])])
         return f_init_connected or self._communicator.settings_in_connected()
 
-    def _pre_receive(self, apply_overlay: Optional[bool]) -> bool:
+    def _pre_receive(self) -> bool:
         """Pre-receives on all ports.
 
         This includes muscle_settings_in and all user-defined ports.
 
         Returns:
             True iff no ClosePort messages were received.
         """
         all_ports_open = self.__receive_settings()
-        self.__pre_receive_f_init(apply_overlay)
+        self.__pre_receive_f_init()
         for message in self._f_init_cache.values():
             if isinstance(message.data, ClosePort):
                 all_ports_open = False
         return all_ports_open
 
     def __receive_settings(self) -> bool:
         """Receives settings on muscle_settings_in.
@@ -1009,39 +1033,33 @@
         if isinstance(message.data, ClosePort):
             return False
         if not isinstance(message.data, Settings):
             err_msg = ('"{}" received a message on'
                        ' muscle_settings_in that is not a'
                        ' Settings. It seems that your'
                        ' simulation is miswired or the sending'
-                       ' instance is broken.'.format(self._instance_name()))
+                       ' instance is broken.'.format(self._instance_id))
             self.__shutdown(err_msg)
             raise RuntimeError(err_msg)
 
         settings = cast(Settings, message.settings)
         for key, value in message.data.items():
             settings[key] = value
         self._settings_manager.overlay = settings
 
         self._trigger_manager.harmonise_wall_time(saved_until)
         return True
 
-    def __pre_receive_f_init(self, apply_overlay: Optional[bool]) -> None:
+    def __pre_receive_f_init(self) -> None:
         """Receives on all ports connected to F_INIT.
 
         This receives all incoming messages on F_INIT and stores them
         in self._f_init_cache.
         """
-        if apply_overlay is not None:
-            warnings.warn(
-                    'Explicitly providing apply_overlay in reuse_instance is'
-                    ' deprecated. Use InstanceFlags.DONT_APPLY_OVERLAY when'
-                    ' creating the instance instead.', DeprecationWarning)
-        else:
-            apply_overlay = InstanceFlags.DONT_APPLY_OVERLAY not in self._flags
+        apply_overlay = InstanceFlags.DONT_APPLY_OVERLAY not in self._flags
 
         def pre_receive(port_name: str, slot: Optional[int]) -> None:
             msg, saved_until = self._communicator.receive_message(
                     port_name, slot)
             self._f_init_cache[(port_name, slot)] = msg
             if apply_overlay:
                 self.__apply_overlay(msg)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/logging.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/logging.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/logging_handler.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/logging_handler.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,9 +23,9 @@
         super().__init__(level)
         self._instance_id = instance_id
         self._manager = mmp_client
 
     def emit(self, record: logging.LogRecord) -> None:
         message = LogMessage(self._instance_id, Timestamp(record.created),
                              LogLevel.from_python_level(record.levelno),
-                             record.msg)
+                             self.format(record))
         self._manager.submit_log_message(message)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/instance_manager.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/instance_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import logging
+from textwrap import indent
 from threading import Thread
-from typing import Union
+from typing import Dict, Optional, Union
 from multiprocessing import Queue
 import queue
 
-from ymmsl import Configuration
+from ymmsl import Configuration, Reference
 
+from libmuscle.manager.instance_registry import InstanceRegistry
 from libmuscle.manager.instantiator import (
         CancelAllRequest, CrashedResult, InstantiatorRequest,
         InstantiationRequest, ProcessStatus, ShutdownRequest)
+from libmuscle.manager.logger import last_lines
 from libmuscle.manager.qcgpj_instantiator import Process, QCGPJInstantiator
 from libmuscle.manager.run_dir import RunDir
 from libmuscle.planner.planner import Planner, Resources
 
 
 _logger = logging.getLogger(__name__)
 
@@ -51,37 +54,41 @@
 
 _ResultType = Union[Process, CrashedResult]
 
 
 class InstanceManager:
     """Instantiates and manages running instances"""
     def __init__(
-            self, configuration: Configuration, run_dir: RunDir) -> None:
+            self, configuration: Configuration, run_dir: RunDir,
+            instance_registry: InstanceRegistry) -> None:
         """Create a ProcessManager.
 
         Args:
             configuration: The global configuration
             run_dir: Directory to run in
+            instance_registry: The InstanceRegistry to use
         """
         self._configuration = configuration
         self._run_dir = run_dir
+        self._instance_registry = instance_registry
 
-        self._resources_in = Queue()    # type: Queue[Resources]
-        self._requests_out = Queue()    # type: Queue[InstantiatorRequest]
-        self._results_in = Queue()      # type: Queue[_ResultType]
-        self._log_records_in = Queue()  # type: Queue[logging.LogRecord]
+        self._resources_in: Queue[Resources] = Queue()
+        self._requests_out: Queue[InstantiatorRequest] = Queue()
+        self._results_in: Queue[_ResultType] = Queue()
+        self._log_records_in: Queue[logging.LogRecord] = Queue()
 
         self._instantiator = QCGPJInstantiator(
                 self._resources_in, self._requests_out, self._results_in,
                 self._log_records_in, self._run_dir.path)
         self._instantiator.start()
 
         self._log_handler = LogHandlingThread(self._log_records_in)
         self._log_handler.start()
 
+        self._allocations: Optional[Dict[Reference, Resources]] = None
         self._planner = Planner(self._resources_in.get())
         self._num_running = 0
 
     def set_manager_location(self, location: str) -> None:
         """Sets the network location of the manager.
 
         Call this before starting any instances so that the location
@@ -90,20 +97,20 @@
         Args:
             location: The network location (e.g. localhost:5000)
         """
         self._manager_location = location
 
     def start_all(self) -> None:
         """Starts all the instances of the model."""
-        allocations = self._planner.allocate_all(self._configuration)
-        for instance, resources in allocations.items():
+        self._allocations = self._planner.allocate_all(self._configuration)
+        for instance, resources in self._allocations.items():
             _logger.info(f'Planned {instance} on {resources}')
 
         components = {c.name: c for c in self._configuration.model.components}
-        for instance, resources in allocations.items():
+        for instance, resources in self._allocations.items():
             component = components[instance.without_trailing_ints()]
             if component.implementation is None:
                 _logger.warning(
                         f'No implementation specified for {component.name}'
                         ', not starting it.')
                 continue
             implementation = self._configuration.implementations[
@@ -119,17 +126,40 @@
                     instance, implementation,
                     self._configuration.resources[component.name],
                     resources, idir, workdir, stdout_path, stderr_path)
             _logger.info(f'Instantiating {instance} on {resources}')
             self._requests_out.put(request)
             self._num_running += 1
 
+    def get_resources(self) -> Dict[Reference, Resources]:
+        """Returns the resources allocated to each instance.
+
+        Only call this after start_all() has been called, or it will raise
+        an exception because the information is not available.
+
+        Return:
+            The resources for each instance instantiated by start_all()
+        """
+        if self._allocations is None:
+            raise RuntimeError(
+                    'Tried to get resources but we are running without'
+                    ' --start-all')
+
+        return self._allocations
+
     def wait(self) -> bool:
         """Waits for all instances to be done."""
         all_seemingly_okay = True
+
+        def cancel_all() -> None:
+            nonlocal all_seemingly_okay
+            if all_seemingly_okay:
+                self._requests_out.put(CancelAllRequest())
+                all_seemingly_okay = False
+
         while self._num_running > 0:
             result = self._results_in.get()
 
             if isinstance(result, CrashedResult):
                 _logger.error(
                     'Instantiator crashed. This should not happen, please file'
                     ' a bug report.')
@@ -140,20 +170,35 @@
                     _logger.info(
                             f'Instance {result.instance} was shut down by'
                             f' MUSCLE3 because an error occurred elsewhere')
                 else:
                     _logger.error(
                             f'Instance {result.instance} quit with error'
                             f' {result.exit_code}')
+
+                    stderr_file = (
+                            self._run_dir.instance_dir(result.instance) /
+                            'stderr.txt')
+                    _logger.error(
+                            'The last error output of this instance was:')
                     _logger.error(
-                            'Output may be found in'
-                            f' {self._run_dir.instance_dir(result.instance)}')
-                    if all_seemingly_okay:
-                        self._requests_out.put(CancelAllRequest())
-                        all_seemingly_okay = False
+                            '\n' + indent(last_lines(stderr_file, 20), '    '))
+                    _logger.error(
+                            'More output may be found in'
+                            f' {self._run_dir.instance_dir(result.instance)}\n'
+                            )
+                    cancel_all()
+
+            elif not self._instance_registry.did_register(result.instance):
+                _logger.error(
+                        f'Instance {result.instance} quit with no error'
+                        ' (exit code 0), but it never registered with the'
+                        ' manager. Maybe it never created an Instance'
+                        ' object?')
+                cancel_all()
             else:
                 if result.status == ProcessStatus.CANCELED:
                     _logger.info(
                             f'Instance {result.instance} was not started'
                             f' because of an error elsewhere')
                 else:
                     _logger.debug(f'Instance {result.instance} finished')
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/instance_registry.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/instance_registry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from threading import Condition
-from typing import Dict  # noqa
-from typing import List
+from typing import Dict, List, Set
 
 from ymmsl import Port, Reference
 
 
 class AlreadyRegistered(RuntimeError):
     pass
 
@@ -14,16 +13,17 @@
 
     The InstanceRegistry is a simple in-memory database that stores
     information about running instances of simulation components.
     """
     def __init__(self) -> None:
         """Construct an empty InstanceRegistry"""
         self._deregistered_one = Condition()    # doubles as lock
-        self._locations = dict()  # type: Dict[Reference, List[str]]
-        self._ports = dict()  # type: Dict[Reference, List[Port]]
+        self._locations: Dict[Reference, List[str]] = {}
+        self._ports: Dict[Reference, List[Port]] = {}
+        self._seen: Set[Reference] = set()
         self._startup = True
 
     def add(self, name: Reference, locations: List[str], ports: List[Port]
             ) -> None:
         """Add an instance to the registry.
 
         Args:
@@ -38,14 +38,15 @@
         with self._deregistered_one:
             if name in self._locations:
                 raise AlreadyRegistered(
                         'Instance {} tried to register twice'.format(name))
 
             self._locations[name] = locations
             self._ports[name] = ports
+            self._seen.add(name)
             self._startup = False
 
     def get_locations(self, name: Reference) -> List[str]:
         """Retrieves the locations of a registered instance.
 
         Args:
             name: The name of the instance to get the location of.
@@ -78,14 +79,26 @@
             KeyError: If the instance does not exist.
         """
         with self._deregistered_one:
             del self._locations[name]
             del self._ports[name]
             self._deregistered_one.notify()
 
+    def did_register(self, name: Reference) -> bool:
+        """Check whether the instance has registered at some point.
+
+        This returns True iff the instance registered at some point
+        before the function was called. If it was subsequently
+        deregistered, this will still return True.
+
+        Args:
+            name: Name of the instance to check.
+        """
+        return name in self._seen
+
     def wait(self) -> None:
         """Waits until all instances are deregistered.
 
         This function blocks, and returns after each instance has been
         registered and deregistered again, signally the end of the
         simulation run.
         """
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/instantiator.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/instantiator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import enum
 import logging
 import multiprocessing as mp
 from pathlib import Path
+import traceback
 from typing import Optional
 
 from ymmsl import Implementation, Reference, ResourceRequirements
 
 from libmuscle.planner.planner import Resources
 
 
@@ -43,16 +44,16 @@
 
         Args:
             resources: Resources allocated to this process.
         """
         self.instance = instance
         self.resources = resources
         self.status = ProcessStatus.STARTED
-        self.exit_code = None   # type: Optional[int]
-        self.error_msg = None   # type: Optional[str]
+        self.exit_code: Optional[int] = None
+        self.error_msg: Optional[str] = None
 
 
 class InstantiatorRequest:
     """Base class for requests to an instantiator."""
     pass
 
 
@@ -122,8 +123,13 @@
 
     def emit(self, record: logging.LogRecord) -> None:
         """Emit the record by enqueueing it.
 
         Args:
             record: A log record to enqueue.
         """
+        if record.exc_info:
+            record.msg += '\n' + ''.join(
+                    traceback.format_exception(*record.exc_info))
+            record.exc_info = None
+
         self._queue.put(record)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/logger.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pathlib import Path
-from typing import Optional
+from typing import List, Optional
 
 from libmuscle.logging import LogLevel, Timestamp
 from libmuscle.util import extract_log_file_location
 
 
 class Formatter(logging.Formatter):
     """A custom formatter that can format remote messages."""
@@ -121,7 +121,40 @@
         logger = logging.getLogger(instance_id)
         logger.log(
                 level.as_python_level(),
                 text,
                 extra={
                     'instance': instance_id,
                     'iasctime': timestamp.to_asctime()})
+
+
+def last_lines(file: Path, count: int) -> str:
+    """Utility function that returns the last lines of a text file.
+
+    This opens the file and returns the final `count` lines. It reads
+    at most 10000 bytes, to avoid memory problems if the file contains
+    e.g. a large amount of binary data.
+
+    Args:
+        file: The file to read
+        count: Number of lines to read
+
+    Return:
+        A string of at most 10000 bytes, containing at most `count`
+        newlines.
+    """
+    if not file.exists():
+        return ''
+
+    file_size = file.stat().st_size
+    start_point = max(file_size - 10000, 0)
+
+    lines: List[str] = []
+    with file.open('r') as f:
+        f.seek(start_point)
+        f.readline()    # skip partial line
+        line = f.readline()
+        while line:
+            lines.append(line)
+            line = f.readline()
+
+    return '\n' + ''.join(lines[-count:])
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/manager.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from pathlib import Path
 import logging
 import sys
 import traceback
 from typing import Optional
 
-from ymmsl import PartialConfiguration, save as save_ymmsl
+from ymmsl import Model, PartialConfiguration, save as save_ymmsl
 
 from libmuscle.manager.instance_registry import InstanceRegistry
 from libmuscle.manager.logger import Logger
 from libmuscle.manager.mmp_server import MMPServer
 from libmuscle.manager.instance_manager import InstanceManager
+from libmuscle.manager.profile_store import ProfileStore
 from libmuscle.manager.run_dir import RunDir
 from libmuscle.manager.snapshot_registry import SnapshotRegistry
 from libmuscle.manager.topology_store import TopologyStore
 
 
 _logger = logging.getLogger(__name__)
 
@@ -37,14 +38,15 @@
             configuration: The simulation configuration.
             run_dir: Main working directory.
         """
         self._configuration = configuration
         self._run_dir = run_dir
         log_dir = self._run_dir.path if self._run_dir else Path.cwd()
         self._logger = Logger(log_dir, log_level)
+        self._profile_store = ProfileStore(log_dir)
         self._topology_store = TopologyStore(configuration)
         self._instance_registry = InstanceRegistry()
         if run_dir is not None:
             snapshot_dir = run_dir.snapshot_dir()
         else:
             snapshot_dir = Path.cwd()
             if self._configuration.checkpoints:
@@ -53,66 +55,80 @@
                                 ' stored in the current working directory.')
 
         if self._run_dir:
             save_ymmsl(
                     self._configuration,
                     self._run_dir.path / 'configuration.ymmsl')
 
-        self._instance_manager = None    # type: Optional[InstanceManager]
+        if isinstance(self._configuration.model, Model):
+            self._profile_store.store_instances([
+                instance_name
+                for c in self._configuration.model.components
+                for instance_name in c.instances()])
+
+        self._instance_manager: Optional[InstanceManager] = None
         try:
             configuration = self._configuration.as_configuration()
             if self._run_dir is not None:
                 self._instance_manager = InstanceManager(
-                        configuration, self._run_dir)
+                        configuration, self._run_dir, self._instance_registry)
         except ValueError:
             pass
 
         # SnapshotRegistry creates a worker thread, must be created after
         # instance_manager which forks the process
         self._snapshot_registry = SnapshotRegistry(
                 configuration, snapshot_dir, self._topology_store)
         self._snapshot_registry.start()
 
         self._server = MMPServer(
-                self._logger, self._configuration,
+                self._logger, self._profile_store, self._configuration,
                 self._instance_registry, self._topology_store,
                 self._snapshot_registry, run_dir)
 
         if self._instance_manager:
             self._instance_manager.set_manager_location(
                     self.get_server_location())
 
     def get_server_location(self) -> str:
         """Returns the network location of the server."""
         return self._server.get_location()
 
     def start_instances(self) -> None:
         """Starts all required component instances."""
         if self._run_dir is None:
-            raise RuntimeError('No run dir specified')
+            message = 'No run dir specified'
+            _logger.error(message)
+            raise RuntimeError(message)
         if not self._instance_manager:
-            raise RuntimeError(
+            message = (
                     'For MUSCLE3 to be able to start instances, the'
                     ' configuration must contain a model, implementations,'
                     ' and resources. Please make sure they are all there.')
+            _logger.error(message)
+            raise RuntimeError(message)
         try:
             self._instance_manager.start_all()
+            self._profile_store.store_resources(
+                    self._instance_manager.get_resources())
         except:     # noqa
             _logger.error('An error occurred while starting the components:')
             for line in traceback.format_exception(*sys.exc_info()):
                 _logger.error(line)
             self._instance_manager.shutdown()
             raise
 
     def stop(self) -> None:
         """Shuts down the manager."""
-        # self._server.stop()
+        if self._instance_manager:
+            self._instance_manager.shutdown()
         self._server.stop()
         self._snapshot_registry.shutdown()
         self._snapshot_registry.join()
+        self._profile_store.shutdown()
         self._logger.close()
 
     def wait(self) -> bool:
         """Blocks until the simulation is done, then shuts down.
 
         Returns:
             True if success, False if an error occurred.
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/mmp_server.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/mmp_server.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,30 @@
 import logging
 import time
 from typing import Any, Dict, cast, List, Optional
 
 import msgpack
 from ymmsl import (
         Conduit, Identifier, Operator, Port, Reference, PartialConfiguration,
-        Checkpoints)
+        Checkpoints, CheckpointRule, CheckpointAtRule, CheckpointRangeRule)
 
 import libmuscle
 from libmuscle.logging import LogLevel
 from libmuscle.manager.instance_registry import (
         AlreadyRegistered, InstanceRegistry)
 from libmuscle.manager.logger import Logger
 from libmuscle.manager.run_dir import RunDir
 from libmuscle.manager.snapshot_registry import SnapshotRegistry
 from libmuscle.manager.topology_store import TopologyStore
 from libmuscle.mcp.protocol import RequestType, ResponseType
 from libmuscle.mcp.tcp_transport_server import TcpTransportServer
 from libmuscle.mcp.transport_server import RequestHandler
+from libmuscle.manager.profile_store import ProfileStore
+from libmuscle.profiling import (
+        ProfileEvent, ProfileEventType, ProfileTimestamp)
 from libmuscle.snapshot import SnapshotMetadata
 from libmuscle.timestamp import Timestamp
 
 
 _logger = logging.getLogger(__name__)
 
 
@@ -37,28 +40,43 @@
 
 
 def encode_conduit(conduit: Conduit) -> List[str]:
     """Convert a Conduit to a MsgPack-compatible value."""
     return [str(conduit.sender), str(conduit.receiver)]
 
 
+def encode_checkpoint_rule(rule: CheckpointRule) -> Dict[str, Any]:
+    """Convert a CheckpointRule to a MsgPack-compatible value."""
+    if isinstance(rule, CheckpointAtRule):
+        return {'at': list(map(float, rule.at))}
+    if isinstance(rule, CheckpointRangeRule):
+        return {
+            'start': None if rule.start is None else float(rule.start),
+            'stop': None if rule.stop is None else float(rule.stop),
+            'every': float(rule.every)}
+    raise TypeError(f"Unknown checkpoint rule type: {type(rule)}.")
+
+
 def encode_checkpoints(checkpoints: Checkpoints) -> Dict[str, Any]:
     """Convert a Checkpoins to a MsgPack-compatible value."""
     return {
         "at_end": checkpoints.at_end,
-        "wallclock_time": [vars(rule) for rule in checkpoints.wallclock_time],
-        "simulation_time": [vars(rule) for rule in checkpoints.simulation_time]
+        "wallclock_time":
+            list(map(encode_checkpoint_rule, checkpoints.wallclock_time)),
+        "simulation_time":
+            list(map(encode_checkpoint_rule, checkpoints.simulation_time)),
     }
 
 
 class MMPRequestHandler(RequestHandler):
     """Handles Manager requests."""
     def __init__(
             self,
             logger: Logger,
+            profile_store: ProfileStore,
             configuration: PartialConfiguration,
             instance_registry: InstanceRegistry,
             topology_store: TopologyStore,
             snapshot_registry: SnapshotRegistry,
             run_dir: Optional[RunDir]
             ) -> None:
         """Create an MMPRequestHandler.
@@ -66,14 +84,15 @@
         Args:
             logger: The Logger component to log messages to.
             settings: The global settings to serve to instances.
             instance_registry: The database for instances.
             topology_store: Keeps track of how to connect things.
         """
         self._logger = logger
+        self._profile_store = profile_store
         self._configuration = configuration
         self._instance_registry = instance_registry
         self._topology_store = topology_store
         self._snapshot_registry = snapshot_registry
         self._run_dir = run_dir
         self._reference_time = time.monotonic()
 
@@ -104,14 +123,22 @@
         elif req_type == RequestType.SUBMIT_SNAPSHOT.value:
             response = self._submit_snapshot(*req_args)
         elif req_type == RequestType.GET_CHECKPOINT_INFO.value:
             response = self._get_checkpoint_info(*req_args)
 
         return cast(bytes, msgpack.packb(response, use_bin_type=True))
 
+    def close(self) -> None:
+        """Free per-thread resources.
+
+        On shutdown of the server, this will be called by each server
+        thread before it shuts down.
+        """
+        self._profile_store.close()
+
     def _register_instance(
             self, instance_id: str, locations: List[str],
             ports: List[List[str]], version: str = '') -> Any:
         """Handle a register instance request.
 
         Args:
             instance_id: ID of the instance to register
@@ -256,24 +283,36 @@
 
             status (ResponseType): SUCCESS
         """
         self._logger.log_message(
                 instance_id, Timestamp(timestamp), LogLevel(level), text)
         return [ResponseType.SUCCESS.value]
 
-    def _submit_profile_events(self, events: List[List[Any]]) -> Any:
+    def _submit_profile_events(
+            self, instance_id: str, events: List[List[Any]]) -> Any:
         """Handle a submit profile events request.
 
-        Not implemented yet.
+        Args:
+            instance_id: Instance that sent these events
+            events: Profiling events to store
 
         Returns:
             A list containing the following values on success:
 
             status (ResponseType): SUCCESS
         """
+        ev = [
+                ProfileEvent(
+                    ProfileEventType(e[0]), ProfileTimestamp(e[1]),
+                    ProfileTimestamp(e[2]),
+                    Port(e[3][0], Operator[e[3][1]]) if e[3] else None,
+                    e[4], e[5], e[6], e[7], e[8])
+                for e in events]
+
+        self._profile_store.add_events(Reference(instance_id), ev)
         return [ResponseType.SUCCESS.value]
 
     def _submit_snapshot(
             self, instance_id: str, snapshot: Dict[str, Any]) -> Any:
         """Handle a submit snapshot request.
 
         Returns:
@@ -325,14 +364,15 @@
     This class accepts connections from the instances comprising
     the multiscale model to be executed, and services them using an
     MMPRequestHandler.
     """
     def __init__(
             self,
             logger: Logger,
+            profile_store: ProfileStore,
             configuration: PartialConfiguration,
             instance_registry: InstanceRegistry,
             topology_store: TopologyStore,
             snapshot_registry: SnapshotRegistry,
             run_dir: Optional[RunDir]
             ) -> None:
         """Create an MMPServer.
@@ -340,23 +380,26 @@
         This starts a TCP Transport server and connects it to an
         MMPRequestHandler, which uses the given components to service
         the requests. By default, we listen on port 9000, unless it's
         not available in which case we use a random other one.
 
         Args:
             logger: Logger to send log messages to
+            profile_store: ProfileStore to store profile data in
             configuration: Configuration component to get settings, checkpoints
                 and resumes from
             instance_registry: To register instances with and get
                 peer locations from
             topology_store: To get peers and conduits from
+            snapshot_registry: To register snapshots with
+            run_dir: To save snapshots to
         """
         self._handler = MMPRequestHandler(
-                logger, configuration, instance_registry, topology_store,
-                snapshot_registry, run_dir)
+                logger, profile_store, configuration, instance_registry,
+                topology_store, snapshot_registry, run_dir)
         try:
             self._server = TcpTransportServer(self._handler, 9000)
         except OSError as e:
             if e.errno != errno.EADDRINUSE:
                 raise
             self._server = TcpTransportServer(self._handler)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/qcgpj_instantiator.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/qcgpj_instantiator.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     and updates the list accordingly.
 
     Attributes:
         processes: Dict mapping instance names to Process objects.
     """
     def __init__(self) -> None:
         """Create a StateTracker."""
-        self.processes = dict()     # type: Dict[Reference, Process]
+        self.processes: Dict[Reference, Process] = {}
 
         # These are for communicating with QCG-PJ
         self.queued_to_execute = 0
         self.stop_processing = False
         self.zmq_address = ''
 
     # QCG-PJ callbacks
@@ -118,16 +118,15 @@
         qcgpj_dir = self._run_dir / 'qcgpj'
         qcgpj_dir.mkdir(exist_ok=True)
         os.chdir(qcgpj_dir)
 
         self._reconfigure_logging()
 
         # Executor needs to be instantiated before we go async
-        qcg_config = {
-                qcg_Config.AUX_DIR: str(qcgpj_dir)}     # type: Dict[str, str]
+        qcg_config: Dict[str, str] = {qcg_Config.AUX_DIR: str(qcgpj_dir)}
         self._qcg_resources = qcg_get_resources(qcg_config)
         self._state_tracker = StateTracker()
         self._executor = qcg_Executor(
                 self._state_tracker, qcg_config, self._qcg_resources)
 
         self._send_resources()
 
@@ -142,15 +141,15 @@
     async def _main(self) -> None:
         """Main function for the background process.
 
         This sets up QCG-PJ and then accepts requests for instantiating
         jobs, stopping them, or shutting down. Results of finished jobs
         are returned via the results queue.
         """
-        qcg_iters = dict()  # type: Dict[Reference, qcg_SchedulingIteration]
+        qcg_iters: Dict[Reference, qcg_SchedulingIteration] = {}
 
         await asyncio.sleep(0.01)  # allow requests_in queue to be populated
 
         shutting_down = False
         done = False
         while not done:
             while not shutting_down:
@@ -265,15 +264,15 @@
         qcg_allocation = qcg_Allocation()
         for node_name, cores in request.resources.cores.items():
             qcg_cores = [str(i) for i in cores]
             qcg_allocation.add_node(
                     qcg_NodeAllocation(qcg_Node(node_name), qcg_cores, {}))
 
         sjob = qcg_SchedulingJob(self._state_tracker, qcg_job)
-        qcg_iteration = qcg_SchedulingIteration(sjob, None, None, None, [])
+        qcg_iteration = qcg_SchedulingIteration(sjob, None, None, resources, [])
         return qcg_allocation, qcg_iteration
 
     def _create_env(
             self, instance: Reference, overlay: Dict[str, str]
             ) -> Dict[str, str]:
         """Updates the environment with the implementation's env.
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/run_dir.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/run_dir.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/snapshot_registry.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/snapshot_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,18 +196,18 @@
                              ' contain a (complete) model section, so there'
                              ' is nothing to run!')
         self._configuration = config
         self._model = config.model
         self._snapshot_folder = snapshot_folder
         self._topology_store = topology_store
 
-        self._queue = Queue()               # type: Queue[_QueueItemType]
-        self._snapshots = {}                # type: _SnapshotDictType
+        self._queue: Queue[_QueueItemType] = Queue()
+        self._snapshots: _SnapshotDictType = {}
 
-        self._instances = set()             # type: Set[Reference]
+        self._instances: Set[Reference] = set()
         for component in config.model.components:
             self._instances.update(component.instances())
 
         # Create snapshot nodes for starting from scratch
         for instance in self._instances:
             self.register_snapshot(instance, _NULL_SNAPSHOT)
 
@@ -290,15 +290,15 @@
 
         # Instances that don't have a snapshot node chosen yet:
         instances_to_cover = list(self._instances - {snapshot.instance})
         # Allowed snapshots per instance. This is updated during the heuristic
         # to further restrict the sets of snapshots as peer snapshots are
         # selected.
         # First restriction is that the snapshots have to be locally consistent.
-        allowed_snapshots = {}  # type: Dict[Reference, FrozenSet[SnapshotNode]]
+        allowed_snapshots: Dict[Reference, FrozenSet[SnapshotNode]] = {}
         for instance in instances_to_cover:
             allowed_snapshots[instance] = frozenset(
                     i_snapshot
                     for i_snapshot in self._snapshots.get(instance, [])
                     if i_snapshot.consistent)
             if not allowed_snapshots[instance]:
                 # there cannot be a workflow snapshot if this instance has no
@@ -317,15 +317,15 @@
 
         # Do a full, depth-first search for all workflow snapshots
         # ========================================================
 
         workflow_snapshots = []
         selected_snapshots = [snapshot]
         # This stack stores history of allowed_snapshots and enables roll back
-        stack = []  # type: List[Dict[Reference, FrozenSet[SnapshotNode]]]
+        stack: List[Dict[Reference, FrozenSet[SnapshotNode]]] = []
 
         # Update allowed_snapshots for peers of the selected snapshot
         for peer, snapshots in snapshot.consistent_peers.items():
             intersection = allowed_snapshots[peer].intersection(snapshots)
             if not intersection:
                 return []
             allowed_snapshots[peer] = intersection
@@ -426,15 +426,15 @@
         description = self._generate_description(selected_snapshots, now)
         return PartialConfiguration(resume=resume, description=description)
 
     def _generate_description(
             self, selected_snapshots: List[SnapshotNode], now: datetime) -> str:
         """Generate a human-readable description of the workflow snapshot.
         """
-        triggers = {}   # type: Dict[str, List[str]]
+        triggers: Dict[str, List[str]] = {}
         component_info = []
         max_instance_len = len('Instance ')
         for node in selected_snapshots:
             for trigger in node.snapshot.triggers:
                 triggers.setdefault(trigger, []).append(str(node.instance))
             component_info.append((
                     str(node.instance),
@@ -473,15 +473,15 @@
                             for snapshot in workflow_snapshots[0]}
         for workflow_snapshot in workflow_snapshots[1:]:
             for snapshot in workflow_snapshot:
                 if newest_snapshots[snapshot.instance].num < snapshot.num:
                     newest_snapshots[snapshot.instance] = snapshot
 
         # Remove all snapshots that are older than the newest snapshots
-        removed_snapshots = set()  # type: Set[SnapshotNode]
+        removed_snapshots: Set[SnapshotNode] = set()
         for snapshot in newest_snapshots.values():
             all_snapshots = self._snapshots[snapshot.instance]
             idx = all_snapshots.index(snapshot)
             self._snapshots[snapshot.instance] = all_snapshots[idx:]
             removed_snapshots.update(all_snapshots[:idx])
 
         # Remove all references in SnapshotNode.peer_snapshot to the snapshots
@@ -534,15 +534,15 @@
                     situation the flag ``_ConnectionInfo.PEER_IS_VECTOR`` is
                     set. When both ports are vector or non-vector, neither flag
                     is set.
         """
         instance_kernel = instance.without_trailing_ints()
         peer_kernel = peer.without_trailing_ints()
 
-        connected_ports = []  # type: List[_ConnectionType]
+        connected_ports: List[_ConnectionType] = []
         for conduit in self._model.conduits:
             if (conduit.sending_component() == instance_kernel and
                     conduit.receiving_component() == peer_kernel):
                 conn_type = _ConnectionInfo.SELF_IS_SENDING
             elif (conduit.receiving_component() == instance_kernel and
                     conduit.sending_component() == peer_kernel):
                 conn_type = _ConnectionInfo(0)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/conftest.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-from pathlib import Path
-
 import pytest
 from ymmsl import Component, Conduit, Configuration, Model, Reference
 
 from libmuscle.manager.instance_registry import InstanceRegistry
 from libmuscle.manager.logger import Logger
 from libmuscle.manager.mmp_server import MMPRequestHandler
 from libmuscle.manager.run_dir import RunDir
 from libmuscle.manager.snapshot_registry import SnapshotRegistry
 from libmuscle.manager.topology_store import TopologyStore
+from libmuscle.manager.profile_store import ProfileStore
 
 
 @pytest.fixture
-def logger(tmpdir):
-    test_logger = Logger(Path(str(tmpdir)))
+def logger(tmp_path):
+    test_logger = Logger(tmp_path)
     yield test_logger
     test_logger.close()
 
 
 @pytest.fixture
 def mmp_configuration():
     return Configuration(
@@ -30,14 +29,21 @@
                 [
                     Conduit('macro.out', 'micro.in'),
                     Conduit('micro.out', 'macro.in')
                 ]))
 
 
 @pytest.fixture
+def profile_store(tmp_path):
+    test_profile_store = ProfileStore(tmp_path)
+    yield test_profile_store
+    test_profile_store.close()
+
+
+@pytest.fixture
 def instance_registry():
     return InstanceRegistry()
 
 
 @pytest.fixture
 def topology_store(mmp_configuration) -> TopologyStore:
     return TopologyStore(mmp_configuration)
@@ -46,19 +52,19 @@
 @pytest.fixture
 def snapshot_registry(mmp_configuration, topology_store) -> SnapshotRegistry:
     return SnapshotRegistry(mmp_configuration, None, topology_store)
 
 
 @pytest.fixture
 def mmp_request_handler(
-        logger, mmp_configuration, instance_registry, topology_store,
-        snapshot_registry):
+        logger, profile_store, mmp_configuration, instance_registry,
+        topology_store, snapshot_registry):
     return MMPRequestHandler(
-            logger, mmp_configuration, instance_registry, topology_store,
-            snapshot_registry, None)
+            logger, profile_store, mmp_configuration, instance_registry,
+            topology_store, snapshot_registry, None)
 
 
 @pytest.fixture
 def loaded_instance_registry(instance_registry):
     instance_registry.add(Reference('macro'), ['direct:macro'], [])
     for j in range(10):
         for i in range(10):
@@ -66,19 +72,19 @@
             location = 'direct:{}'.format(name)
             instance_registry.add(name, [location], [])
     return instance_registry
 
 
 @pytest.fixture
 def registered_mmp_request_handler(
-        logger, mmp_configuration, loaded_instance_registry, topology_store,
-        snapshot_registry):
+        logger, profile_store, mmp_configuration, loaded_instance_registry,
+        topology_store, snapshot_registry):
     return MMPRequestHandler(
-            logger, mmp_configuration, loaded_instance_registry, topology_store,
-            snapshot_registry, None)
+            logger, profile_store, mmp_configuration, loaded_instance_registry,
+            topology_store, snapshot_registry, None)
 
 
 @pytest.fixture
 def mmp_configuration2():
     return Configuration(
             Model(
                 'test_model',
@@ -122,13 +128,13 @@
             location = 'direct:{}'.format(name)
             instance_registry.add(name, [location], [])
     return instance_registry
 
 
 @pytest.fixture
 def registered_mmp_request_handler2(
-        logger, mmp_configuration, loaded_instance_registry2, topology_store2,
-        snapshot_registry2, tmp_path):
+        logger, profile_store, mmp_configuration, loaded_instance_registry2,
+        topology_store2, snapshot_registry2, tmp_path):
     return MMPRequestHandler(
-            logger, mmp_configuration,
+            logger, profile_store, mmp_configuration,
             loaded_instance_registry2, topology_store2, snapshot_registry2,
             RunDir(tmp_path))
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_instance_registry.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_instance_registry.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_logger.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_mmp_request_handler.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_mmp_request_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 import libmuscle
 from libmuscle.logging import LogLevel
 from libmuscle.manager.mmp_server import MMPRequestHandler
 from libmuscle.mcp.protocol import RequestType, ResponseType
 from libmuscle.snapshot import SnapshotMetadata
 
 
-def test_create_servicer(logger, mmp_configuration, instance_registry,
-                         topology_store, snapshot_registry):
+def test_create_servicer(
+        logger, profile_store, mmp_configuration, instance_registry,
+        topology_store, snapshot_registry):
     MMPRequestHandler(
-            logger, mmp_configuration, instance_registry, topology_store,
-            snapshot_registry, None)
+            logger, profile_store, mmp_configuration, instance_registry,
+            topology_store, snapshot_registry, None)
 
 
 def test_log_message(mmp_request_handler, caplog):
     request = [
             RequestType.SUBMIT_LOG_MESSAGE.value,
             'test_instance_id', 0.0, LogLevel.WARNING.value,
             'Testing log message']
@@ -148,15 +149,19 @@
     assert isinstance(checkpoints, dict)
     assert checkpoints.keys() == {'at_end', 'wallclock_time', 'simulation_time'}
     assert checkpoints['at_end'] is True
     assert checkpoints['simulation_time'] == []
     wallclock_time = checkpoints['wallclock_time']
     assert len(wallclock_time) == 2
     assert wallclock_time[0] == {'start': None, 'stop': None, 'every': 10}
+    assert all(isinstance(obj, (type(None), float))
+               for obj in wallclock_time[0].values())
     assert wallclock_time[1] == {'at': [1, 2, 3.0]}
+    assert all(isinstance(obj, (type(None), float))
+               for obj in wallclock_time[1]['at'])
 
     assert resume is not None
     assert Path(resume) == resume_path
 
     assert snapshot_directory is None
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_snapshot_registry.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_snapshot_registry.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/test/test_topology_store.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/test/test_topology_store.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/manager/topology_store.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/manager/topology_store.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mcp/protocol.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mcp/protocol.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mcp/tcp_transport_client.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mcp/tcp_transport_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from errno import ENOTCONN
 import socket
-from typing import Optional
+from typing import Optional, Tuple
 
-from libmuscle.mcp.transport_client import TransportClient
+from libmuscle.mcp.transport_client import ProfileData, TransportClient
 from libmuscle.mcp.tcp_util import recv_all, recv_int64, send_int64
+from libmuscle.profiling import ProfileTimestamp
 
 
 class TcpTransportClient(TransportClient):
     """A client that connects to a TCPTransport server.
     """
     @staticmethod
     def can_connect_to(location: str) -> bool:
@@ -27,15 +29,15 @@
         messages from any instance and port represented by it.
 
         Args:
             location: A location string for the peer.
         """
         addresses = location[4:].split(',')
 
-        sock = None     # type: Optional[socket.SocketType]
+        sock: Optional[socket.SocketType] = None
         for address in addresses:
             try:
                 sock = self._connect(address)
                 break
             except RuntimeError:
                 pass
 
@@ -45,39 +47,50 @@
         else:
             if hasattr(socket, "TCP_NODELAY"):
                 sock.setsockopt(socket.SOL_TCP, socket.TCP_NODELAY, 1)
             if hasattr(socket, "TCP_QUICKACK"):
                 sock.setsockopt(socket.SOL_TCP, socket.TCP_QUICKACK, 1)
             self._socket = sock
 
-    def call(self, request: bytes) -> bytes:
+    def call(self, request: bytes) -> Tuple[bytes, ProfileData]:
         """Send a request to the server and receive the response.
 
         This is a blocking call.
 
         Args:
             request: The request to send
 
         Returns:
             The received response
         """
+        start_wait = ProfileTimestamp()
         send_int64(self._socket, len(request))
         self._socket.sendall(request)
 
         length = recv_int64(self._socket)
-        return recv_all(self._socket, length)
+        start_transfer = ProfileTimestamp()
+
+        response = recv_all(self._socket, length)
+        stop_transfer = ProfileTimestamp()
+        return response, (start_wait, start_transfer, stop_transfer)
 
     def close(self) -> None:
         """Closes this client.
 
         This closes any connections this client has and/or performs
         other shutdown activities.
         """
-        self._socket.shutdown(socket.SHUT_RDWR)
-        self._socket.close()
+        try:
+            self._socket.shutdown(socket.SHUT_RDWR)
+            self._socket.close()
+        except OSError as e:
+            # This can happen if the peer has shut down already when we
+            # close our connection to it, which is fine.
+            if e.errno != ENOTCONN:
+                raise
 
     def _connect(self, address: str) -> socket.SocketType:
         loc_parts = address.rsplit(':', 1)
         host = loc_parts[0]
         if host.startswith('['):
             if host.endswith(']'):
                 host = host[1:-1]
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mcp/tcp_transport_server.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mcp/tcp_transport_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,19 @@
         try:
             length = recv_int64(self.request)
             reqbuf = recv_all(self.request, length)
             return reqbuf
         except SocketClosed:
             return None
 
+    def finish(self) -> None:
+        """Called when shutting down the thread?"""
+        server = cast(TcpTransportServerImpl, self.server).transport_server
+        server._handler.close()
+
 
 class TcpTransportServer(TransportServer):
     """A TransportServer that uses TCP to communicate."""
     def __init__(self, handler: RequestHandler, port: int = 0) -> None:
         """Create a TCPServer.
 
         Args:
@@ -83,15 +88,15 @@
         """Returns the location this server listens on.
 
         Returns:
             A string containing the location.
         """
         host, port = self._server.server_address
 
-        locs = list()   # type: List[str]
+        locs: List[str] = []
         for address in self._get_if_addresses():
             locs.append('{}:{}'.format(address, port))
         return 'tcp:{}'.format(','.join(locs))
 
     def close(self) -> None:
         """Closes this server.
 
@@ -99,15 +104,15 @@
         disconnect, then frees any other resources.
         """
         self._server.shutdown()
         self._server_thread.join()
         self._server.server_close()
 
     def _get_if_addresses(self) -> List[str]:
-        all_addresses = list()  # type: List[str]
+        all_addresses: List[str] = []
         ifs = netifaces.interfaces()
         for interface in ifs:
             addrs = netifaces.ifaddresses(interface)
             for props in addrs.get(netifaces.AF_INET, []):
                 if not props['addr'].startswith('127.'):
                     all_addresses.append(props['addr'])
             for props in addrs.get(netifaces.AF_INET6, []):
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mcp/tcp_util.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mcp/tcp_util.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mcp/test/conftest.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mcp/test/conftest.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mcp/test/test_tcp_transport.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mcp/test/test_tcp_transport.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,12 +19,12 @@
     server = TcpTransportServer(handler)
 
     # create client
     server_location = server.get_location()
     assert TcpTransportClient.can_connect_to(server_location)
     client = TcpTransportClient(server_location)
 
-    response2 = client.call(request)
+    response2, _ = client.call(request)
     assert response == response2
 
     client.close()
     server.close()
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mcp/test/test_tcp_transport_server.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mcp/test/test_tcp_transport_server.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mcp/transport_client.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mcp/transport_server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,62 @@
-class TransportClient:
-    """A client that connects to an MCP server.
+class RequestHandler:
+    """Handles requests sent to a TransportServer.
 
-    This is a base class for MCP Transport Clients. An MCP Transport
-    Client connects to an MCP Transport Server over some communication
-    protocol, requests messages from it, and returns responses.
+    TransportServers operate in terms of chunks of bytes received and
+    sent in return. RequestHandlers interpret received chunks of bytes,
+    handle the request, and return a chunk of bytes containing an
+    encoded response.
     """
-    @staticmethod
-    def can_connect_to(location: str) -> bool:
-        """Whether this client class can connect to the given location.
+    def handle_request(self, request: bytes) -> bytes:
+        """Handle a request.
 
         Args:
-            location: The location to potentially connect to.
+            request: A received request
 
         Returns:
-            True iff this class can connect to this location.
+            An encoded response
         """
         raise NotImplementedError()     # pragma: no cover
 
-    def call(self, request: bytes) -> bytes:
-        """Send a request to the server and receive the response.
+    def close(self) -> None:
+        """Free per-thread resources.
+
+        On shutdown of the server, this will be called by each server
+        thread before it shuts down.
+        """
+        pass
+
+
+class ServerNotSupported(RuntimeError):
+    pass
+
 
-        This is a blocking call.
+class TransportServer:
+    """A server that accepts MCP connections.
+
+    This is a base class for MCP Servers. An MCP Server accepts
+    connections over some lower-level communication protocol, receives
+    requests and returns responses from a RequestHandler.
+    """
+    def __init__(self, handler: RequestHandler) -> None:
+        """Create a TransportServer.
 
         Args:
-            request: The request to send
+            handler: A handler to handle requests.
+        """
+        self._handler = handler
+
+    def get_location(self) -> str:
+        """Returns the location this server listens on.
 
         Returns:
-            The received response
+            A string containing the location.
         """
-        raise NotImplementedError()     # pragma: no cover
+        raise NotImplementedError()  # pragma: no cover
 
     def close(self) -> None:
-        """Closes this client.
+        """Closes this server.
 
-        This closes any connections this client has and/or performs
-        other shutdown activities as needed.
+        Stops the server listening, waits for existing clients to
+        disconnect, then frees any other resources.
         """
-        raise NotImplementedError()     # pragma: no cover
+        raise NotImplementedError()  # pragma: no cover
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mmp_client.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mmp_client.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,21 +41,25 @@
 
     Args:
         event: A profile event
 
     Returns:
         A list with its attributes, for MMP serialisation.
     """
+    if event.start_time is None or event.stop_time is None:
+        raise RuntimeError(
+                'Incomplete ProfileEvent sent. This is a bug, please'
+                ' report it.')
+
     encoded_port = encode_port(event.port) if event.port else None
     return [
-            str(event.instance_id),
-            event.start_time.seconds, event.stop_time.seconds,
             event.event_type.value,
+            event.start_time.nanoseconds, event.stop_time.nanoseconds,
             encoded_port, event.port_length, event.slot,
-            event.message_size]
+            event.message_number, event.message_size, event.message_timestamp]
 
 
 def decode_checkpoint_rule(rule: Dict[str, Any]) -> CheckpointRule:
     """Decode a checkpoint rule from a MsgPack-compatible value."""
     if rule.keys() == {'at'}:
         return CheckpointAtRule(**rule)
     if rule.keys() == {'start', 'stop', 'every'}:
@@ -99,20 +103,21 @@
 
     This class connects to the Manager and communicates with it on
     behalf of the rest of libmuscle.
 
     It manages the connection, and converts between our native types
     and the gRPC generated types.
     """
-    def __init__(self, location: str) -> None:
+    def __init__(self, instance_id: Reference, location: str) -> None:
         """Create an MMPClient
 
         Args:
             location: A connection string of the form hostname:port
         """
+        self._instance_id = instance_id
         self._transport_client = TcpTransportClient(location)
 
     def close(self) -> None:
         """Close the connection
 
         This closes the connection. After this no other member
         functions can be called.
@@ -135,103 +140,97 @@
         """Sends profiling events to the manager.
 
         Args:
             events: The events to send.
         """
         request = [
                 RequestType.SUBMIT_PROFILE_EVENTS.value,
+                str(self._instance_id),
                 [encode_profile_event(e) for e in events]]
         self._call_manager(request)
 
     def submit_snapshot_metadata(
-                self, name: Reference, snapshot_metadata: SnapshotMetadata
-                ) -> None:
+            self, snapshot_metadata: SnapshotMetadata) -> None:
         """Send snapshot metadata to the manager.
 
         Args:
-            name: Name of the instance in the simulation.
             snapshot_metadata: Snapshot metadata to supply to the manager.
         """
         request = [
                 RequestType.SUBMIT_SNAPSHOT.value,
-                str(name),
+                str(self._instance_id),
                 dataclasses.asdict(snapshot_metadata)]
         self._call_manager(request)
 
     def get_settings(self) -> Settings:
         """Get the central settings from the manager.
 
         Returns:
             The requested settings.
         """
         request = [RequestType.GET_SETTINGS.value]
         response = self._call_manager(request)
         return Settings(response[1])
 
-    def get_checkpoint_info(self, name: Reference) -> _CheckpointInfoType:
+    def get_checkpoint_info(self) -> _CheckpointInfoType:
         """Get the checkpoint info from the manager.
 
         Returns:
             elapsed_time: current elapsed time
             checkpoints: checkpoint configuration
             resume: path to the resume snapshot
             snapshot_directory: path to store snapshots
         """
-        request = [RequestType.GET_CHECKPOINT_INFO.value, str(name)]
+        request = [RequestType.GET_CHECKPOINT_INFO.value, str(self._instance_id)]
         response = self._call_manager(request)
         return decode_checkpoint_info(*response[1:])
 
-    def register_instance(self, name: Reference, locations: List[str],
-                          ports: List[Port]) -> None:
+    def register_instance(
+            self, locations: List[str], ports: List[Port]) -> None:
         """Register a component instance with the manager.
 
         Args:
-            name: Name of the instance in the simulation.
             locations: List of places where the instance can be
                     reached.
             ports: List of ports of this instance.
         """
         request = [
                 RequestType.REGISTER_INSTANCE.value,
-                str(name), locations,
+                str(self._instance_id), locations,
                 [encode_port(p) for p in ports],
                 libmuscle.__version__]
         response = self._call_manager(request)
         if response[0] == ResponseType.ERROR.value:
             raise RuntimeError(
                     f'Error registering instance: {response[1]}')
 
-    def request_peers(
-            self, name: Reference) -> Tuple[
-                    List[Conduit],
-                    Dict[Reference, List[int]],
-                    Dict[Reference, List[str]]]:
+    def request_peers(self) -> Tuple[
+            List[Conduit],
+            Dict[Reference, List[int]],
+            Dict[Reference, List[str]]]:
         """Request connection information about peers.
 
         This will repeat the request at an exponentially increasing
         query interval at first, until it reaches the interval
         specified by PEER_INTERVAL_MIN and PEER_INTERVAL_MAX. From
         there on, intervals are drawn randomly from that range.
 
-        Args:
-            name: Name of the current instance.
-
         Returns:
             A tuple containing a list of conduits that this instance is
             attached to, a dictionary of peer dimensions, which is
             indexed by Reference to the peer kernel, and specifies how
             many instances of that kernel there are, and a dictionary
             of peer instance locations, indexed by Reference to a peer
             instance, and containing for each peer instance a list of
             network location strings at which it can be reached.
         """
         sleep_time = 0.1
         start_time = perf_counter()
 
-        request = [RequestType.GET_PEERS.value, str(name)]
+        request = [RequestType.GET_PEERS.value, str(self._instance_id)]
         response = self._call_manager(request)
 
         while (response[0] == ResponseType.PENDING.value and
                perf_counter() < start_time + PEER_TIMEOUT and
                sleep_time < PEER_INTERVAL_MIN):
             sleep(sleep_time)
             response = self._call_manager(request)
@@ -257,21 +256,19 @@
 
         peer_locations = {
                 Reference(instance): locs
                 for instance, locs in response[3].items()}
 
         return conduits, peer_dimensions, peer_locations
 
-    def deregister_instance(self, name: Reference) -> None:
+    def deregister_instance(self) -> None:
         """Deregister a component instance with the manager.
-
-        Args:
-            name: Name of the instance in the simulation.
         """
-        request = [RequestType.DEREGISTER_INSTANCE.value, str(name)]
+        request = [
+                RequestType.DEREGISTER_INSTANCE.value, str(self._instance_id)]
         response = self._call_manager(request)
 
         if response[0] == ResponseType.ERROR.value:
             raise RuntimeError('Error deregistering instance: {}'.format(
                     response[1]))
 
     def _call_manager(self, request: Any) -> Any:
@@ -280,9 +277,9 @@
         Args:
             request: The request to encode and send
 
         Returns:
             The decoded response
         """
         encoded_request = msgpack.packb(request, use_bin_type=True)
-        response = self._transport_client.call(encoded_request)
+        response, _ = self._transport_client.call(encoded_request)
         return msgpack.unpackb(response, raw=False)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mpp_client.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mpp_client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from typing import List, Optional
+from typing import List, Optional, Tuple
 
 import msgpack
 from ymmsl import Reference
 
 from libmuscle.mcp.protocol import RequestType
-from libmuscle.mcp.transport_client import TransportClient
+from libmuscle.mcp.transport_client import ProfileData, TransportClient
 from libmuscle.mcp.type_registry import transport_client_types
 
 
 class MPPClient:
     """A client that connects to an MPP server.
 
     This client connects to a peer to retrieve messages. It uses an MCP
@@ -20,15 +20,15 @@
         The client will connect to the peer on one of its locations. It
         tries the most efficient protocol first. Once connected, it can
         request messages from any component and port represented by it.
 
         Args:
             locations: The peer's location strings
         """
-        client = None       # type: Optional[TransportClient]
+        client: Optional[TransportClient] = None
         for ClientType in transport_client_types:
             for location in locations:
                 if ClientType.can_connect_to(location):
                     try:
                         client = ClientType(location)
                         break
                     except Exception:
@@ -36,22 +36,22 @@
             if client:
                 break
         else:
             raise RuntimeError('Failed to connect')
 
         self._transport_client = client
 
-    def receive(self, receiver: Reference) -> bytes:
+    def receive(self, receiver: Reference) -> Tuple[bytes, ProfileData]:
         """Receive a message from a port this client connects to.
 
         Args:
             receiver: The receiving (local) port.
 
         Returns:
-            The received message.
+            The received message, and profiling data
         """
         request = [RequestType.GET_NEXT_MESSAGE.value, str(receiver)]
         encoded_request = msgpack.packb(request, use_bin_type=True)
         return self._transport_client.call(encoded_request)
 
     def close(self) -> None:
         """Closes this client.
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/mpp_message.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/mpp_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,16 +99,15 @@
             'fa': 'F',
             'la': 'C'}
 
     grid_dict = msgpack.unpackb(data, raw=False)
     order = order_map[grid_dict['order']]
     shape = tuple(grid_dict['shape'])
     dtype = type_map[ExtTypeId(code)]
-    array = np.ndarray(     # type: ignore
-            shape, dtype, grid_dict['data'], order=order)   # type: ignore
+    array = np.ndarray(shape, dtype, grid_dict['data'], order=order)  # type: ignore
     indexes = grid_dict['indexes']
     if indexes == []:
         indexes = None
     return Grid(array, indexes)
 
 
 def _data_encoder(obj: Any) -> Any:
@@ -138,15 +137,15 @@
         return Settings(plain_dict)
     elif code in _grid_types:
         return _decode_grid(code, data)
     return msgpack.ExtType(code, data)
 
 
 class MPPMessage:
-    """A MUSCLE Communication Protocol message.
+    """A MUSCLE Peer Protocol message.
 
     Messages carry the identity of their sender and receiver, so that
     they can be routed by a MUSCLE Transport Overlay when we get to
     multi-site running in the future.
     """
     def __init__(self, sender: Reference, receiver: Reference,
                  port_length: Optional[int],
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/outbox.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/outbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     An Outbox is a queue of messages, which may be deposited and
     then retrieved in the same order.
     """
     def __init__(self) -> None:
         """Create an empty Outbox.
         """
-        self.__queue = Queue()  # type: Queue[bytes]
+        self.__queue: Queue[bytes] = Queue()
 
     def is_empty(self) -> bool:
         """Returns True iff the outbox is empty.
         """
         return self.__queue.empty()
 
     def deposit(self, message: bytes) -> None:
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/peer_manager.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/peer_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             peer_locations: A list of locations for each peer instance
                     we share a conduit with.
         """
         self.__kernel = kernel
         self.__index = index
 
         # peer port ids, indexed by local kernel.port id
-        self.__peers = dict()  # type: Dict[Reference, List[Reference]]
+        self.__peers: Dict[Reference, List[Reference]] = {}
 
         for conduit in conduits:
             if str(conduit.sending_component()) == str(kernel):
                 # we send on the port this conduit attaches to
                 self.__peers.setdefault(
                         conduit.sender, []).append(conduit.receiver)
             if str(conduit.receiving_component()) == str(kernel):
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/planner/planner.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/planner/planner.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from copy import copy, deepcopy
 import logging
-from typing import Dict, Iterable, List, Mapping, Optional, Set
+from typing import Dict, Iterable, List, Mapping, Optional, Set, Tuple
 
 from ymmsl import (
         Component, Configuration, Model, MPICoresResReq, MPINodesResReq,
         Operator, Reference, ResourceRequirements, ThreadedResReq)
 
+from libmuscle.util import instance_indices
+
 
 _logger = logging.getLogger(__name__)
 
 
-_PredSuccType = Dict[Component, Set[Component]]
+_PredSuccType = Dict[Component, Set[Tuple[Component, int]]]
 
 
 class ModelGraph:
     """Represents a yMMSL model as a graph."""
     def __init__(self, model: Model) -> None:
         """Create a ModelGraph.
 
@@ -22,29 +24,29 @@
         analyse a yMMSL model definition.
 
         Args:
             model: The model to represent.
         """
         self._model = model
 
-        self._direct_superpreds = dict()    # type: _PredSuccType
-        self._direct_predecessors = dict()  # type: _PredSuccType
-        self._direct_subpreds = dict()      # type: _PredSuccType
-
-        self._direct_supersuccs = dict()    # type: _PredSuccType
-        self._direct_successors = dict()    # type: _PredSuccType
-        self._direct_subsuccs = dict()      # type: _PredSuccType
-
-        self._superpreds = dict()           # type: _PredSuccType
-        self._predecessors = dict()         # type: _PredSuccType
-        self._subpreds = dict()             # type: _PredSuccType
-
-        self._supersuccs = dict()           # type: _PredSuccType
-        self._successors = dict()           # type: _PredSuccType
-        self._subsuccs = dict()             # type: _PredSuccType
+        self._direct_superpreds: _PredSuccType = {}
+        self._direct_predecessors: _PredSuccType = {}
+        self._direct_subpreds: _PredSuccType = {}
+
+        self._direct_supersuccs: _PredSuccType = {}
+        self._direct_successors: _PredSuccType = {}
+        self._direct_subsuccs: _PredSuccType = {}
+
+        self._superpreds: _PredSuccType = {}
+        self._predecessors: _PredSuccType = {}
+        self._subpreds: _PredSuccType = {}
+
+        self._supersuccs: _PredSuccType = {}
+        self._successors: _PredSuccType = {}
+        self._subsuccs: _PredSuccType = {}
 
         self._calc_direct_succs_preds()
         self._calc_predecessors()
         self._calc_successors()
 
     def components(self) -> Iterable[Component]:
         """Return the components of the model (nodes)."""
@@ -63,15 +65,15 @@
             KeyError: If no component could be found
         """
         for component in self._model.components:
             if component.name == name:
                 return component
         raise KeyError('Component {} not found'.format(name))
 
-    def successors(self, component: Component) -> Set[Component]:
+    def successors(self, component: Component) -> Set[Tuple[Component, int]]:
         """Return the successors of the given component.
 
         Args:
             component: The reference component
 
         Returns:
             The set of components for which a path exists from
@@ -79,15 +81,15 @@
 
         Raises:
             KeyError: If the component is not in the model used to
                 construct this object.
         """
         return self._successors[component]
 
-    def predecessors(self, component: Component) -> Set[Component]:
+    def predecessors(self, component: Component) -> Set[Tuple[Component, int]]:
         """Return the predecessors of the given component.
 
         Args:
             component: The reference component
 
         Returns:
             The set of components for which a path exists from
@@ -95,44 +97,61 @@
 
         Raises:
             KeyError: If the component is not in the model used to
                 construct this object.
         """
         return self._predecessors[component]
 
-    def macros(self, component: Component) -> Set[Component]:
+    def macros(self, component: Component) -> Set[Tuple[Component, int]]:
         """Return the macros of the given component.
 
         These are components that are both before the component's
         F_INIT and after its O_F.
 
         Args:
             component: The reference component
 
         Returns:
             The set of components that are both super-predecessor
             and super-successor of component.
         """
         return self._superpreds[component] & self._supersuccs[component]
 
-    def micros(self, component: Component) -> Set[Component]:
+    def micros(self, component: Component) -> Set[Tuple[Component, int]]:
         """Return the micros of the given component.
 
         These are components that are in between the component's
         O_I and its S.
 
         Args:
             component: The reference component
 
         Returns:
             The set of components that are both sub-successor
             and sub-predecessor of component.
         """
         return self._subsuccs[component] & self._subpreds[component]
 
+    def _propagate(
+            self, from_set: Set[Tuple[Component, int]],
+            to_set: Set[Tuple[Component, int]], shared_dims: int
+            ) -> None:
+        """Propagates from_set into to_set.
+
+        Note: Modifies to_set.
+
+        Args:
+            from_set: Set to propagate components from
+            to_set: Set to propagate them into
+            shared_dims: Maximum shared dimensions to carry
+        """
+        to_set.update({
+            (cmp, min(sd, shared_dims))
+            for cmp, sd in from_set})
+
     def _calc_predecessors(self) -> None:
         """Calculates predecessors of each component in the model.
 
         This function determines for each component in the model which
         other components can be reached by following incoming conduits.
 
         Preconditions:
@@ -144,70 +163,92 @@
             with for each component in the model the corresponding set
             of components.
         """
         self._superpreds = {c: set() for c in self._model.components}
         self._predecessors = {c: set() for c in self._model.components}
         self._subpreds = {c: set() for c in self._model.components}
 
-        remaining_preds = {
+        num_remaining_preds = {
                 c: (
                     len(self._direct_predecessors[c]) +
                     len(self._direct_superpreds[c]))
                 for c in self._model.components}
-        remaining_subpreds = {
+        num_remaining_subpreds = {
                 c: len(self._direct_subpreds[c])
                 for c in self._model.components}
 
         todo = set(self._model.components)
-        started = set()     # type: Set[Component]
-        doing = set()       # type: Set[Component]
-        finished = set()    # type: Set[Component]
-        done = set()        # type: Set[Component]
+        started: Set[Component] = set()
+        doing: Set[Component] = set()
+        finished: Set[Component] = set()
+        done: Set[Component] = set()
         while todo or doing:
             started.clear()
             for component in todo:
-                if not remaining_preds[component]:
-                    for subsucc in self._direct_subsuccs[component]:
-                        self._superpreds[subsucc].add(component)
-                        self._predecessors[subsucc].update(
-                                self._predecessors[component])
-                        self._superpreds[subsucc].update(
-                                self._superpreds[component])
-                        remaining_preds[subsucc] -= 1
+                if num_remaining_preds[component] == 0:
+                    for subsucc, shared_dims in self._direct_subsuccs[component]:
+                        self._superpreds[subsucc].add((component, shared_dims))
+                        self._propagate(
+                                self._predecessors[component],
+                                self._predecessors[subsucc], shared_dims)
+
+                        self._propagate(
+                                self._superpreds[component],
+                                self._superpreds[subsucc], shared_dims)
+
+                        num_remaining_preds[subsucc] -= 1
                     started.add(component)
 
             todo -= started
             doing |= started
 
             finished.clear()
             for component in doing:
-                if not remaining_subpreds[component]:
-                    for succ in self._direct_successors[component]:
-                        self._predecessors[succ].add(component)
-                        self._predecessors[succ].update(
-                                self._subpreds[component])
-                        self._predecessors[succ].update(
-                                self._predecessors[component])
-                        self._superpreds[succ].update(
-                                self._superpreds[component])
-                        remaining_preds[succ] -= 1
-
-                    for supersucc in self._direct_supersuccs[component]:
-                        self._subpreds[supersucc].add(component)
-                        self._subpreds[supersucc].update(
-                                self._subpreds[component])
-                        self._subpreds[supersucc].update(
-                                self._predecessors[component])
-                        remaining_subpreds[supersucc] -= 1
+                if num_remaining_subpreds[component] == 0:
+                    for succ, shared_dims in self._direct_successors[component]:
+                        self._predecessors[succ].add((component, shared_dims))
+                        self._propagate(
+                                self._subpreds[component],
+                                self._predecessors[succ], shared_dims)
+
+                        self._propagate(
+                                self._predecessors[component],
+                                self._predecessors[succ], shared_dims)
+
+                        self._propagate(
+                                self._superpreds[component],
+                                self._superpreds[succ], shared_dims)
+
+                        num_remaining_preds[succ] -= 1
+
+                    for supersucc, shared_dims in self._direct_supersuccs[component]:
+                        self._subpreds[supersucc].add((component, shared_dims))
+
+                        self._propagate(
+                                self._subpreds[component],
+                                self._subpreds[supersucc], shared_dims)
+
+                        self._propagate(
+                                self._predecessors[component],
+                                self._subpreds[supersucc], shared_dims)
+
+                        num_remaining_subpreds[supersucc] -= 1
 
                     finished.add(component)
 
             doing -= finished
             done |= finished
 
+            if not started and not finished:
+                raise RuntimeError(
+                        'Could not plan resource allocation for this model.'
+                        ' Do you have a cycle of O_F -> F_INIT conduits?'
+                        ' That does not work, because the models will all be'
+                        ' waiting for each other to start.')
+
     def _calc_successors(self) -> None:
         """Calculates successors of each component in the model.
 
         This function determines for each component in the model which
         other components can be reached by following outgoing conduits.
 
         Preconditions:
@@ -219,65 +260,77 @@
             with for each component in the model the corresponding set
             of components.
         """
         self._supersuccs = {c: set() for c in self._model.components}
         self._successors = {c: set() for c in self._model.components}
         self._subsuccs = {c: set() for c in self._model.components}
 
-        remaining_succs = {
+        num_remaining_succs = {
                 c: (
                     len(self._direct_successors[c]) +
                     len(self._direct_supersuccs[c]))
                 for c in self._model.components}
 
-        remaining_subsuccs = {
+        num_remaining_subsuccs = {
                 c: len(self._direct_subsuccs[c])
                 for c in self._model.components}
 
         todo = set(self._model.components)
-        started = set()     # type: Set[Component]
-        doing = set()       # type: Set[Component]
-        finished = set()    # type: Set[Component]
-        done = set()        # type: Set[Component]
+        started: Set[Component] = set()
+        doing: Set[Component] = set()
+        finished: Set[Component] = set()
+        done: Set[Component] = set()
         while todo or doing:
             started.clear()
             for component in todo:
-                if not remaining_succs[component]:
-                    for subpred in self._direct_subpreds[component]:
-                        self._supersuccs[subpred].add(component)
-                        self._successors[subpred].update(
-                                self._successors[component])
-                        self._supersuccs[subpred].update(
-                                self._supersuccs[component])
-                        remaining_succs[subpred] -= 1
+                if num_remaining_succs[component] == 0:
+                    for subpred, shared_dims in self._direct_subpreds[component]:
+                        self._supersuccs[subpred].add((component, shared_dims))
+                        self._propagate(
+                                self._successors[component],
+                                self._successors[subpred], shared_dims)
+
+                        self._propagate(
+                                self._supersuccs[component],
+                                self._supersuccs[subpred], shared_dims)
+                        num_remaining_succs[subpred] -= 1
+
                     started.add(component)
 
             todo -= started
             doing |= started
 
             finished.clear()
             for component in doing:
-                if not remaining_subsuccs[component]:
-                    for pred in self._direct_predecessors[component]:
-                        self._successors[pred].add(component)
-                        self._successors[pred].update(
-                                self._successors[component])
-                        self._supersuccs[pred].update(
-                                self._supersuccs[component])
-                        self._successors[pred].update(
-                                self._subsuccs[component])
-                        remaining_succs[pred] -= 1
-
-                    for superpred in self._direct_superpreds[component]:
-                        self._subsuccs[superpred].add(component)
-                        self._subsuccs[superpred].update(
-                                self._successors[component])
-                        self._subsuccs[superpred].update(
-                                self._subsuccs[component])
-                        remaining_subsuccs[superpred] -= 1
+                if num_remaining_subsuccs[component] == 0:
+                    for pred, shared_dims in self._direct_predecessors[component]:
+                        self._successors[pred].add((component, shared_dims))
+                        self._propagate(
+                                self._successors[component],
+                                self._successors[pred], shared_dims)
+
+                        self._propagate(
+                                self._supersuccs[component],
+                                self._supersuccs[pred], shared_dims)
+
+                        self._propagate(
+                                self._subsuccs[component],
+                                self._successors[pred], shared_dims)
+                        num_remaining_succs[pred] -= 1
+
+                    for superpred, shared_dims in self._direct_superpreds[component]:
+                        self._subsuccs[superpred].add((component, shared_dims))
+                        self._propagate(
+                                self._successors[component],
+                                self._subsuccs[superpred], shared_dims)
+
+                        self._propagate(
+                                self._subsuccs[component],
+                                self._subsuccs[superpred], shared_dims)
+                        num_remaining_subsuccs[superpred] -= 1
                     finished.add(component)
 
             doing -= finished
             done |= finished
 
     def _calc_direct_succs_preds(self) -> None:
         """Calculates all successors and predecessors of components.
@@ -313,23 +366,25 @@
                 recv_op = Operator.F_INIT
             elif receiver.ports:
                 if conduit.receiving_port() in receiver.ports.f_init:
                     recv_op = Operator.F_INIT
                 elif conduit.receiving_port() in receiver.ports.s:
                     recv_op = Operator.S
 
+            shared_dims = min(len(sender.multiplicity), len(receiver.multiplicity))
+
             if (snd_op, recv_op) == (Operator.O_I, Operator.F_INIT):
-                self._direct_superpreds[receiver].add(sender)
-                self._direct_subsuccs[sender].add(receiver)
+                self._direct_superpreds[receiver].add((sender, shared_dims))
+                self._direct_subsuccs[sender].add((receiver, shared_dims))
             elif (snd_op, recv_op) == (Operator.O_F, Operator.F_INIT):
-                self._direct_successors[sender].add(receiver)
-                self._direct_predecessors[receiver].add(sender)
+                self._direct_successors[sender].add((receiver, shared_dims))
+                self._direct_predecessors[receiver].add((sender, shared_dims))
             elif (snd_op, recv_op) == (Operator.O_F, Operator.S):
-                self._direct_subpreds[receiver].add(sender)
-                self._direct_supersuccs[sender].add(receiver)
+                self._direct_subpreds[receiver].add((sender, shared_dims))
+                self._direct_supersuccs[sender].add((receiver, shared_dims))
 
 
 class Resources:
     """Designates a (sub)set of resources.
 
     Whether these resources are free or allocated in general or by
     something specific depends on the context, this just says which
@@ -342,22 +397,37 @@
     def __init__(self, cores: Optional[Dict[str, Set[int]]] = None) -> None:
         """Create a Resources object with the given cores.
 
         Args:
             cores: Cores to be designated by this object.
         """
         if cores is None:
-            self.cores = dict()     # type: Dict[str, Set[int]]
+            self.cores: Dict[str, Set[int]] = {}
         else:
             self.cores = cores
 
     def __copy__(self) -> 'Resources':
         """Copy the object."""
         return Resources(deepcopy(self.cores))
 
+    def __eq__(self, other: object) -> bool:
+        """Check for equality."""
+        if not isinstance(other, Resources):
+            return NotImplemented
+
+        if len(self.cores) != len(other.cores):
+            return False
+
+        for node, cores in self.cores.items():
+            if node not in other.cores:
+                return False
+            if other.cores[node] != cores:
+                return False
+        return True
+
     def __iadd__(self, other: 'Resources') -> 'Resources':
         """Add the resources in the argument to this object."""
         for node in other.cores:
             if node in self.cores:
                 self.cores[node] |= other.cores[node]
             else:
                 self.cores[node] = set(other.cores[node])
@@ -370,16 +440,36 @@
                 self.cores[node] -= other.cores[node]
                 if not self.cores[node]:
                     del self.cores[node]
         return self
 
     def __str__(self) -> str:
         """Return a human-readable string representation."""
+        def collapse_ranges(cores: Set[int]) -> str:
+            if len(cores) == 0:
+                return ''
+
+            result = list()
+            scores = sorted(cores)
+            start = 0
+            i = 1
+            while i <= len(scores):
+                if (i == len(scores)) or (scores[i-1] != scores[i] - 1):
+                    if start == i - 1:
+                        # run of one
+                        result.append(str(scores[i-1]))
+                    else:
+                        # run of at least two
+                        result.append(f'{scores[start]}-{scores[i-1]}')
+                    start = i
+                i += 1
+            return ','.join(result)
+
         return 'Resources(' + '; '.join([
-            n + ': ' + ','.join(sorted(map(str, cs)))
+            n + ': ' + collapse_ranges(cs)
             for n, cs in self.cores.items()]) + ')'
 
     def __repr__(self) -> str:
         """Return a string representation."""
         return f'Resources({self.cores})'
 
     def nodes(self) -> Iterable[str]:
@@ -425,16 +515,16 @@
         """Create a ResourceManager.
 
         Args:
             all_resources: An object describing the available resources
                     to be managed by this ResourceManager.
         """
         self._all_resources = all_resources
-        self._allocations = dict()  # type: Dict[Reference, Resources]
-        self._oversubscribed = dict()   # type: Dict[Reference, Resources]
+        self._allocations: Dict[Reference, Resources] = {}
+        self._oversubscribed: Dict[Reference, Resources] = {}
         self._next_virtual_node = 1
 
     def allocate_all(
             self, configuration: Configuration, virtual: bool = False
             ) -> Dict[Reference, Resources]:
         """Allocates resources for the given components.
 
@@ -454,39 +544,39 @@
         Args:
             configuration: Configuration to allocate all components of
             virtual: Allocate on virtual resources or not, see above
 
         Returns:
             Resources for each instance required by the model.
         """
-        result = dict()     # type: Dict[Reference, Resources]
+        result: Dict[Reference, Resources] = {}
 
         # Analyse model
         model = ModelGraph(configuration.model)
         requirements = configuration.resources
         implementations = configuration.implementations
         exclusive = {
-                c for c in model.components()
+                i for c in model.components() for i in c.instances()
                 if (c.implementation and
                     not implementations[c.implementation].can_share_resources)}
 
         # Allocate
         unallocated_instances = [
                 i for c in model.components() for i in c.instances()]
-        leftover_instances = list()     # type: List[Reference]
+        leftover_instances: List[Reference] = []
         while unallocated_instances:
             leftover_instances.clear()
 
             to_allocate = self._sort_instances(
                     unallocated_instances, requirements)
 
             for instance in to_allocate:
                 component = model.component(instance.without_trailing_ints())
                 conflicting_names = self._conflicting_names(
-                        model, exclusive, component)
+                        model, exclusive, component, instance)
 
                 done = False
                 while not done:
                     try:
                         result[instance] = self._allocate_instance(
                                 instance, component,
                                 requirements[component.name],
@@ -541,25 +631,56 @@
                 if isinstance(r, MPICoresResReq)]
         sorted_mpi = sorted(mpi, key=lambda x: x[1], reverse=True)
         sorted_mpi_instances = [x[0] for x in sorted_mpi]
 
         return sorted_threaded_instances + sorted_mpi_instances
 
     def _conflicting_names(
-            self, model: ModelGraph, exclusive: Set[Component],
-            component: Component) -> Set[Reference]:
-        """Returns names of components that cannot share resources."""
-        conflicting_comps = set(model.components())
-        conflicting_comps -= model.predecessors(component)
-        conflicting_comps -= model.successors(component)
+            self, model: ModelGraph, exclusive: Set[Reference],
+            component: Component, instance: Reference) -> Set[Reference]:
+        """Find conflicting components.
+
+        This returns the names of instances that cannot share resources
+        with the given component, so that they can be avoided when
+        assigning resources.
+
+        Args:
+            model: Model to search
+            exclusive: List of instances that cannot share resources
+            component: Component to find conflicts for
+            instance: Instance (of component) to find conflicts for
+        """
+        def indices_match(
+                instance1: Reference, instance2: Reference, dims: int) -> bool:
+            idx1 = instance_indices(instance1)
+            idx2 = instance_indices(instance2)
+            return idx1[:dims] == idx2[:dims]
+
+        def matching_instances(
+                others: Set[Tuple[Component, int]]) -> Set[Reference]:
+            return {
+                    i for c, d in others for i in c.instances()
+                    if indices_match(i, instance, d)}
+
+        conflicting_instances = {
+                i for c in model.components() for i in c.instances()}
+
+        if instance in exclusive:
+            return conflicting_instances
+
+        conflicting_instances -= matching_instances(model.predecessors(component))
+        conflicting_instances -= matching_instances(model.successors(component))
+
         if component not in exclusive:
-            mms = model.micros(component) | model.macros(component)
-            nonconflicting_mms = mms - exclusive
-            conflicting_comps -= nonconflicting_mms
-        return {c.name for c in conflicting_comps}
+            micros = matching_instances(model.micros(component))
+            macros = matching_instances(model.macros(component))
+            nonconflicting_mms = (micros | macros) - exclusive
+            conflicting_instances -= nonconflicting_mms
+
+        return conflicting_instances
 
     def _expand_resources(
             self, name: Reference, req: ResourceRequirements) -> None:
         """Adds an extra virtual node to the available resources."""
         taken = True
         while taken:
             new_node = 'node{:06d}'.format(self._next_virtual_node)
@@ -581,40 +702,40 @@
                         f' which is impossible with {num_cores} cores per'
                         ' node.')
         self._all_resources.cores[new_node] = set(range(num_cores))
 
     def _allocate_instance(
             self, instance: Reference, component: Component,
             requirements: ResourceRequirements,
-            simultaneous_components: Set[Reference], virtual: bool
+            simultaneous_instances: Set[Reference], virtual: bool
             ) -> Resources:
         """Allocates resources for the given instance.
 
         If we are on real resources, and the instance requires more
         threads than our nodes have cores, then we'll just give it all
         cores on a node and hope for the best. If we are on virtual
         resources, this will raise InsufficientResourcesAvailable.
 
         Args:
             instance: The instance to allocate for
             component: The component it is an instance of
             requirements: Its resource requirements
-            simultaneous_components: Components which may execute
+            simultaneous_instances: Instances which may execute
                     simultaneously and whose resources we therefore
                     cannot overlap with
             virtual: Whether we are on virtual resources
 
         Returns:
             A Resources object describing the resources allocated
         """
         allocation = Resources({})
         free_resources = copy(self._all_resources)
 
         for other in self._allocations:
-            if other.without_trailing_ints() in simultaneous_components:
+            if other in simultaneous_instances:
                 free_resources -= self._allocations[other]
 
         try:
             if isinstance(requirements, ThreadedResReq):
                 allocation = self._allocate_thread_block(
                         free_resources, requirements.threads)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/port.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/port.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         """
         super().__init__(Identifier(name), operator)
 
         self._is_connected = is_connected
 
         if is_vector:
             if our_ndims == len(peer_dims):
-                self._length = 0    # type: Optional[int]
+                self._length: Optional[int] = 0
             elif our_ndims + 1 == len(peer_dims):
                 self._length = peer_dims[-1]
             elif our_ndims > len(peer_dims):
                 raise RuntimeError(('Vector port "{}" is connected to an'
                                     ' instance set with fewer dimensions.'
                                     ' It should be connected to a scalar'
                                     ' port on a set with one more dimension,'
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/post_office.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/post_office.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
     A PostOffice holds outboxes with messages for receivers. It also
     acts as a request handler for incoming requests for messages.
     """
     def __init__(self) -> None:
         """Create a PostOffice.
         """
-        self._outboxes = dict()  # type: Dict[Reference, Outbox]
+        self._outboxes: Dict[Reference, Outbox] = {}
 
         self._outbox_lock = Lock()
 
     def handle_request(self, request: bytes) -> bytes:
         """Handle a request.
 
         This receives an MCP request and handles it by blocking until
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/profiling.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/profiling.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,109 @@
 from enum import Enum
-import time
+from time import perf_counter_ns, time_ns
 from typing import Optional
 
-from ymmsl import Port, Reference
-
-from libmuscle.timestamp import Timestamp
+from ymmsl import Port
 
 
 class ProfileEventType(Enum):
-    """Profiling event types for MUSCLE3.
-
-    These match the types in the MUSCLE Manager Protocol, and should \
-    be kept identical to those.
-    """
+    """Profiling event types for MUSCLE3."""
     REGISTER = 0
     CONNECT = 4
     DEREGISTER = 1
     SEND = 2
     RECEIVE = 3
+    RECEIVE_WAIT = 5
+    RECEIVE_TRANSFER = 6
+    RECEIVE_DECODE = 7
+
+
+class ProfileTimestamp:
+    """A timestamp for profiling.
+
+    This has higher resolution than Timestamp, storing a number of
+    nanoseconds since the UNIX epoch in an int.
+
+    Attributes:
+        nanoseconds: Nanoseconds since the UNIX epoch.
+    """
+    _time_ref = time_ns() - perf_counter_ns()
+
+    def __init__(self, nanoseconds: Optional[int] = None) -> None:
+        """Create a timestamp representing now.
+
+        Args:
+            nanoseconds: Time to set. If None, use the current time.
+        """
+        if nanoseconds is None:
+            nanoseconds = perf_counter_ns() + self._time_ref
+        self.nanoseconds = nanoseconds
 
 
 class ProfileEvent:
     """A profile event as used by MUSCLE3.
 
     This represents a single measurement of the timing of some event
     that occurred while executing the simulation.
 
     Args:
-        instance_id: The identifier of the instance that generated \
-                this message.
-        start_time: When the event started (real-world, not \
+        event_type: Type of event that was measured.
+        start_time: When the event started (real-world, not
                 simulation time).
-        stop_time: When the event ended (real-world, not simulation \
+        stop_time: When the event ended (real-world, not simulation
                 time).
-        event_type: Type of event that was measured.
         port: Port used for sending or receiving, if applicable.
         port_length: Length of that port, if a vector.
         slot: Slot that was sent or received on, if applicable.
+        message_number: Number of message on this port, if applicable.
+                Starts at 0 for the first message sent or received.
         message_size: Size of the message involved, if applicable.
+        message_timestamp: Timestamp sent with the message, if
+                applicable.
 
     Attributes:
-        instance_id: The identifier of the instance that generated \
-                this message.
-        start_time: When the event started (real-world, not \
+        event_type: Type of event that was measured.
+        start_time: When the event started (real-world, not
                 simulation time).
-        stop_time: When the event ended (real-world, not simulation \
+        stop_time: When the event ended (real-world, not simulation
                 time).
-        event_type: Type of event that was measured.
         port: Port used for sending or receiving, if applicable.
         port_length: Length of that port, if a vector.
         slot: Slot that was sent or received on, if applicable.
+        message_number: Number of message on this port, if applicable.
+                Starts at 0 for the first message sent or received.
         message_size: Size of the message involved, if applicable.
+        message_timestamp: Timestamp sent with the message, if
+                applicable.
     """
     def __init__(
             self,
-            instance_id: Reference,
-            start_time: Timestamp,
-            stop_time: Timestamp,
             event_type: ProfileEventType,
+            start_time: Optional[ProfileTimestamp] = None,
+            stop_time: Optional[ProfileTimestamp] = None,
             port: Optional[Port] = None,
             port_length: Optional[int] = None,
             slot: Optional[int] = None,
-            message_size: Optional[int] = None
+            message_number: Optional[int] = None,
+            message_size: Optional[int] = None,
+            message_timestamp: Optional[float] = None
             ) -> None:
 
-        self.instance_id = instance_id
+        self.event_type = event_type
         self.start_time = start_time
         self.stop_time = stop_time
-        self.event_type = event_type
         self.port = port
         self.port_length = port_length
         self.slot = slot
+        self.message_number = message_number
         self.message_size = message_size
+        self.message_timestamp = message_timestamp
+
+    def start(self) -> None:
+        """Sets start_time to the current time.
+        """
+        self.start_time = ProfileTimestamp()
 
     def stop(self) -> None:
         """Sets stop_time to the current time.
         """
-        self.stop_time = Timestamp(time.time())
+        self.stop_time = ProfileTimestamp()
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/runner.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 Starting instances is out of scope for MUSCLE3, but is also very
 useful for testing and prototyping. So we have a little bit of
 support for it in this module.
 """
 import logging
 import multiprocessing as mp
 import multiprocessing.connection as mpc
+from pathlib import Path
 import sys
-from typing import Callable, Dict, List, Tuple, cast
+from time import sleep
+import traceback
+from typing import Callable, Dict, List, Set, Tuple, cast
 
 from ymmsl import Configuration, Identifier, Model, Reference
 
 from libmuscle.util import generate_indices
+from libmuscle.manager.logger import last_lines
 from libmuscle.manager.manager import Manager
 
 
 __all__ = ['run_simulation']
 
 
 _logger = logging.getLogger(__name__)
@@ -92,15 +96,15 @@
 
 
 def implementation_process(
         instance_id: str, manager_location: str,
         implementation: Callable) -> None:
     prefix_tag = '--muscle-prefix='
     name_prefix = str()
-    index_prefix = list()   # type: List[int]
+    index_prefix: List[int] = []
 
     instance = Reference(instance_id)
 
     for i, arg in enumerate(sys.argv):
         if arg.startswith(prefix_tag):
             prefix_str = arg[len(prefix_tag):]
             name_prefix, index_prefix = _parse_prefix(prefix_str)
@@ -141,18 +145,19 @@
         sys.stderr = log_file
         sys.stdout = log_file
 
         # chain call
         try:
             implementation()
         except Exception:
-            _logger.exception(
+            traceback.print_exc()
+            _logger.error(
                     f'Component {instance} crashed, please check the log file'
                     ' for error messages')
-            raise
+            exit(1)
 
 
 def _parse_prefix(prefix: str) -> Tuple[str, List[int]]:
     """Parse a --muscle-prefix argument.
 
     This is like a Reference, but not quite, because the
     initial identifier may be omitted. That is, [1][2] is
@@ -178,15 +183,15 @@
         number = str()
         while i < len(prefix) and prefix[i] in '0123456789':
             number += prefix[i]
             i += 1
         return int(number), i
 
     name = str()
-    index = list()  # type: List[int]
+    index: List[int] = []
     i = 0
 
     if i == len(prefix):
         return name, index
 
     idt, i = parse_identifier(prefix, i)
     name += idt
@@ -208,15 +213,15 @@
         raise ValueError(('Found invalid extra character {} in'
                           ' --muscle-prefix.').format(prefix[i]))
 
     return name, index
 
 
 def _split_reference(ref: Reference) -> Tuple[Reference, List[int]]:
-    index = list()     # type: List[int]
+    index: List[int] = []
     i = 0
     while i < len(ref) and isinstance(ref[i], Identifier):
         i += 1
     name = ref[:i]
 
     while i < len(ref) and isinstance(ref[i], int):
         index.append(cast(int, ref[i]))
@@ -234,35 +239,58 @@
     a function to run as the corresponding value. Each instance
     will be run in a separate process.
 
     Args:
         instances: A dictionary of instances to run
         manager_location: Network location of the manager
     """
+    # start processes
     instance_processes = list()
     for instance_id_str, implementation in instances.items():
         instance_id = Reference(instance_id_str)
         process = mp.Process(
                 target=implementation_process,
                 args=(instance_id_str, manager_location, implementation),
-                name='Instance-{}'.format(instance_id))
+                name=str(instance_id))
         process.start()
         instance_processes.append(process)
 
-    failed_processes = list()
-    for instance_process in instance_processes:
-        instance_process.join()
-        if instance_process.exitcode != 0:
-            failed_processes.append(instance_process)
-
-    if len(failed_processes) > 0:
-        failed_names = map(lambda x: x.name, failed_processes)
-        raise RuntimeError('Instances {} failed to shut down cleanly, please'
-                           ' check the logs to see what went wrong.'.format(
-                               ', '.join(failed_names)))
+    # wait for them to finish or one to fail
+    failed_processes: List[mp.Process] = list()
+    done_processes: Set[mp.Process] = set()
+    while len(done_processes) < len(instance_processes) and not failed_processes:
+        sleep(0.5)
+        for instance_process in instance_processes:
+            if instance_process not in done_processes:
+                if not instance_process.is_alive():
+                    done_processes.add(instance_process)
+                    if instance_process.exitcode != 0:
+                        failed_processes.append(instance_process)
+
+    # if one failed, shut down the rest
+    if failed_processes:
+        for process in instance_processes:
+            if process not in done_processes:
+                process.terminate()
+            process.join(1.0)
+            if process.is_alive():
+                process.kill()
+
+        failed_names = [proc.name for proc in failed_processes]
+        log_files = [Path(f'muscle3.{name}.log') for name in failed_names]
+        outputs = [last_lines(log_file, 20) for log_file in log_files]
+        msg = (
+                'Instance(s) {} failed to shut down cleanly. Here is the final'
+                ' bit of the output:').format(', '.join(failed_names))
+        for name, output in zip(failed_names, outputs):
+            msg += '\n ---------- ' + name + ' ----------\n'
+            msg += output + '\n'
+            msg += f'See muscle3.{name}.log for the complete output\n'
+
+        raise RuntimeError(msg)
 
 
 def run_simulation(
         configuration: Configuration, implementations: Dict[str, Callable]
         ) -> None:
     """Runs a simulation with the given configuration and instances.
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/snapshot.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/snapshot.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/snapshot_manager.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/snapshot_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,15 @@
         'Invalid message provided to `{}`. Please create a Message object to'
         ' store the state of the instance in a snapshot.')
 
 
 class SnapshotManager:
     """Manages information on snapshots for the Instance
 
-    Implements the public checkpointing API with handoffs to
-    :class:`TriggerManager` for checkpoint triggers.
+    Implements the saving and loading of snapshots in the checkpointing API.
     """
 
     def __init__(self,
                  instance_id: Reference,
                  manager: MMPClient,
                  communicator: Communicator) -> None:
         """Create a new snapshot manager
@@ -39,16 +38,16 @@
         self._instance_id = instance_id
         # replace identifier[i] by identifier-i to use in snapshot file name
         # using a dash (-) because that is not allowed in Identifiers
         self._safe_id = str(instance_id).replace("[", "-").replace("]", "")
         self._communicator = communicator
         self._manager = manager
 
-        self._resume_from_snapshot = None   # type: Optional[Snapshot]
-        self._resume_overlay = Settings()
+        self._resume_from_snapshot: Optional[Snapshot] = None
+        self.resume_overlay = Settings()
         self._next_snapshot_num = 1
 
     def prepare_resume(
             self, resume_snapshot: Optional[Path],
             snapshot_directory: Optional[Path]) -> Optional[float]:
         """Apply checkpoint info received from the manager.
 
@@ -61,31 +60,31 @@
             resume_snapshot: Snapshot to resume from (or None if not
                 resuming)
             snapshot_directory: directory to save snapshots in
 
         Returns:
             Time at which the initial snapshot was saved, if resuming.
         """
-        result = None       # type: Optional[float]
+        result: Optional[float] = None
         self._snapshot_directory = snapshot_directory or Path.cwd()
         if resume_snapshot is not None:
             snapshot = self.load_snapshot_from_file(resume_snapshot)
 
             if snapshot.message is not None:
                 # snapshot.message is None for implicit snapshots
                 self._resume_from_snapshot = snapshot
                 result = snapshot.message.timestamp
-            self._resume_overlay = snapshot.settings_overlay
+            self.resume_overlay = snapshot.settings_overlay
 
             self._communicator.restore_message_counts(
                 snapshot.port_message_counts)
             # Store a copy of the snapshot in the current run directory
             path = self.__store_snapshot(snapshot)
             metadata = SnapshotMetadata.from_snapshot(snapshot, str(path))
-            self._manager.submit_snapshot_metadata(self._instance_id, metadata)
+            self._manager.submit_snapshot_metadata(metadata)
 
         return result
 
     def resuming_from_intermediate(self) -> bool:
         """Check whether we have an intermediate snapshot.
 
         Doesn't say whether we should resume now, just that we were
@@ -121,17 +120,18 @@
 
         Args:
             msg: Message object representing the snapshot.
             final: True iff called from save_final_snapshot.
             triggers: Description of checkpoints that triggered this.
             wallclock_time: Wallclock time when saving.
             f_init_max_timestamp: Timestamp for final snapshots.
+            settings_overlay: Current settings overlay.
 
         Returns:
-            Simulation time at which the snapshot was made
+            Simulation time at which the snapshot was made.
         """
         port_message_counts = self._communicator.get_message_counts()
         if final:
             # Decrease F_INIT port counts by one: F_INIT messages are already
             # pre-received, but not yet processed by the user code. Therefore,
             # the snapshot state should treat these as not-received.
             all_ports = self._communicator.list_ports()
@@ -144,29 +144,29 @@
 
         snapshot = MsgPackSnapshot(
                 triggers, wallclock_time, port_message_counts, final, msg,
                 settings_overlay)
 
         path = self.__store_snapshot(snapshot)
         metadata = SnapshotMetadata.from_snapshot(snapshot, str(path))
-        self._manager.submit_snapshot_metadata(self._instance_id, metadata)
+        self._manager.submit_snapshot_metadata(metadata)
 
         timestamp = msg.timestamp if msg is not None else float('-inf')
         if final and f_init_max_timestamp is not None:
             # For final snapshots f_init_max_snapshot is the reference time (see
             # should_save_final_snapshot).
             timestamp = f_init_max_timestamp
         return timestamp
 
     @staticmethod
     def load_snapshot_from_file(snapshot_location: Path) -> Snapshot:
-        """Load a previously stored snapshot from the filesystem
+        """Load a previously stored snapshot from the filesystem.
 
         Args:
-            snapshot_location: path where the snapshot is stored
+            snapshot_location: path where the snapshot is stored.
         """
         _logger.debug(f'Loading snapshot from {snapshot_location}')
         if not snapshot_location.is_file():
             raise RuntimeError(f'Unable to load snapshot: {snapshot_location}'
                                ' is not a file. Please ensure this path exists'
                                ' and can be read.')
 
@@ -180,21 +180,21 @@
             raise RuntimeError('Unable to load snapshot from'
                                f' {snapshot_location}: unknown version of'
                                ' snapshot file. Was the file saved with a'
                                ' different version of libmuscle or'
                                ' edited?')
 
     def __store_snapshot(self, snapshot: Snapshot) -> Path:
-        """Store a snapshot on the filesystem
+        """Store a snapshot on the filesystem.
 
         Args:
-            snapshot: snapshot to store
+            snapshot: Snapshot to store.
 
         Returns:
-            Path where the snapshot is stored
+            Path where the snapshot is stored.
         """
         _logger.debug(f'Saving snapshot to {self._snapshot_directory}')
         for _ in range(_MAX_FILE_EXISTS_CHECK):
             # Expectation is that muscle_snapshot_directory is empty initially
             # and we succeed in the first loop. Still wrapping in a for-loop
             # such that an existing filename doesn't immediately raise an error
             fname = f"{self._safe_id}_{self._next_snapshot_num}.pack"
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_api_guard.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_api_guard.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_checkpoint_triggers.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_checkpoint_triggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from libmuscle.checkpoint_triggers import (
     CombinedCheckpointTriggers, AtCheckpointTrigger, RangeCheckpointTrigger,
     TriggerManager)
 
 
 def test_at_checkpoint_trigger():
-    trigger = AtCheckpointTrigger([CheckpointAtRule([1, 3, 4, 4.5, 9])])
+    trigger = AtCheckpointTrigger([CheckpointAtRule([1.0, 3.0, 4.0, 4.5, 9.0])])
 
     assert trigger.next_checkpoint(0) == 1
     assert trigger.previous_checkpoint(0) is None
 
     assert trigger.next_checkpoint(1) == 3
     assert trigger.previous_checkpoint(1) == 1
 
@@ -33,15 +33,15 @@
     assert trigger.previous_checkpoint(9) == 9
 
     assert trigger.next_checkpoint(11) is None
     assert trigger.previous_checkpoint(11) == 9
 
 
 def test_range_checkpoint_trigger():
-    range = CheckpointRangeRule(start=0, stop=20, every=1.2)
+    range = CheckpointRangeRule(start=0.0, stop=20.0, every=1.2)
     trigger = RangeCheckpointTrigger(range)
 
     assert trigger.next_checkpoint(-1) == 0
     assert trigger.previous_checkpoint(-1) is None
 
     assert trigger.next_checkpoint(0) == pytest.approx(1.2)
     assert trigger.previous_checkpoint(0) == 0
@@ -53,43 +53,43 @@
     assert trigger.previous_checkpoint(18.2) == pytest.approx(18)
 
     assert trigger.next_checkpoint(20) is None
     assert trigger.previous_checkpoint(20) == pytest.approx(19.2)
 
 
 def test_range_checkpoint_trigger_default_stop():
-    range = CheckpointRangeRule(start=1, every=1.2)
+    range = CheckpointRangeRule(start=1.0, every=1.2)
     trigger = RangeCheckpointTrigger(range)
 
     assert trigger.next_checkpoint(-1.) == 1
     assert trigger.previous_checkpoint(-1.) is None
 
     assert trigger.next_checkpoint(148148.) == pytest.approx(148148.2)
     assert trigger.previous_checkpoint(148148.) == pytest.approx(148147)
 
     assert trigger.next_checkpoint(148148148.) == pytest.approx(148148149)
     assert trigger.previous_checkpoint(148148148.) == pytest.approx(148148147.8)
 
 
 def test_range_checkpoint_trigger_default_start():
-    range = CheckpointRangeRule(every=1.2, stop=10)
+    range = CheckpointRangeRule(every=1.2, stop=10.0)
     trigger = RangeCheckpointTrigger(range)
 
     assert trigger.next_checkpoint(10) is None
     assert trigger.previous_checkpoint(10) == pytest.approx(9.6)
 
     assert trigger.next_checkpoint(0.0) == pytest.approx(1.2)
     assert trigger.previous_checkpoint(0.0) == pytest.approx(0.0)
 
     assert trigger.next_checkpoint(-148148.) == pytest.approx(-148147.2)
     assert trigger.previous_checkpoint(-148148.) == pytest.approx(-148148.4)
 
 
 def test_combined_checkpoint_trigger_every_at():
-    rules = [CheckpointRangeRule(every=10), CheckpointAtRule([3, 7, 13, 17])]
+    rules = [CheckpointRangeRule(every=10.0), CheckpointAtRule([3.0, 7.0, 13.0, 17.0])]
     trigger = CombinedCheckpointTriggers(rules)
 
     assert trigger.next_checkpoint(-11.) == pytest.approx(-10)
     assert trigger.previous_checkpoint(-11) == pytest.approx(-20)
 
     assert trigger.next_checkpoint(0.) == pytest.approx(3)
     assert trigger.previous_checkpoint(0.) == pytest.approx(0)
@@ -101,17 +101,17 @@
     assert trigger.previous_checkpoint(14.2) == pytest.approx(13)
 
     assert trigger.next_checkpoint(25.2) == pytest.approx(30)
     assert trigger.previous_checkpoint(25.2) == pytest.approx(20)
 
 
 def test_combined_checkpoint_trigger_at_ranges():
-    rules = [CheckpointAtRule([3, 7, 13, 17]),
-             CheckpointRangeRule(start=0, every=5, stop=20),
-             CheckpointRangeRule(start=20, every=20, stop=100)]
+    rules = [CheckpointAtRule([3.0, 7.0, 13.0, 17.0]),
+             CheckpointRangeRule(start=0.0, every=5.0, stop=20.0),
+             CheckpointRangeRule(start=20.0, every=20.0, stop=100.0)]
     trigger = CombinedCheckpointTriggers(rules)
 
     assert trigger.next_checkpoint(-11.) == pytest.approx(0)
     assert trigger.previous_checkpoint(-11) is None
 
     assert trigger.next_checkpoint(0.) == pytest.approx(3)
     assert trigger.previous_checkpoint(0.) == pytest.approx(0)
@@ -138,24 +138,24 @@
 def test_trigger_manager_reference_time():
     monotonic_start = time.monotonic()
     ref_elapsed = 15.0
     trigger_manager = TriggerManager()
     trigger_manager.set_checkpoint_info(ref_elapsed, Checkpoints(at_end=True))
     elapsed_walltime = trigger_manager.elapsed_walltime()
     duration = time.monotonic() - monotonic_start
-    assert ref_elapsed < elapsed_walltime <= (ref_elapsed + duration)
+    assert ref_elapsed < elapsed_walltime < (ref_elapsed + duration)
 
 
 def test_trigger_manager():
     ref_elapsed = 0.0
     trigger_manager = TriggerManager()
     trigger_manager.set_checkpoint_info(ref_elapsed, Checkpoints(
             at_end=True,
             wallclock_time=[CheckpointAtRule([1e-12])],
-            simulation_time=[CheckpointAtRule([1, 3, 5])]))
+            simulation_time=[CheckpointAtRule([1.0, 3.0, 5.0])]))
 
     assert trigger_manager.should_save_snapshot(0.1)
     triggers = trigger_manager.get_triggers()
     assert len(triggers) == 1
     assert "wallclock_time" in triggers[0]
     trigger_manager.update_checkpoints(0.1)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_communicator.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_communicator.py`

 * *Files 4% similar despite different names*

```diff
@@ -389,20 +389,20 @@
     assert msg.timestamp == float('inf')
     assert msg.next_timestamp is None
     assert msg.settings_overlay == Settings()
     assert msg.message_number == 0
     assert isinstance(msg.data, ClosePort)
 
 
-def test_receive_message(communicator) -> None:
+def test_receive_message(communicator, profile_data) -> None:
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('other.out[13]'), Reference('kernel[13].in'),
             None, 0.0, None, Settings({'test1': 12}), 0, 2.0,
-            b'test').encoded()
+            b'test').encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator._Communicator__get_client = get_client_mock
     communicator._profiler = MagicMock()
 
     msg, last_saved = communicator.receive_message('in')
 
     get_client_mock.assert_called_with(Reference('other'))
@@ -431,132 +431,134 @@
 
 
 def test_receive_on_invalid_port(communicator) -> None:
     with pytest.raises(ValueError):
         communicator.receive_message('@$Invalid_id')
 
 
-def test_receive_msgpack(communicator) -> None:
+def test_receive_msgpack(communicator, profile_data) -> None:
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('other.out[13]'), Reference('kernel[13].in'),
             None, 0.0, None, Settings({'test1': 12}), 0, 1.0,
-            {'test': 13}).encoded()
+            {'test': 13}).encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator._Communicator__get_client = get_client_mock
     communicator._profiler = MagicMock()
 
     msg, last_saved = communicator.receive_message('in')
 
     get_client_mock.assert_called_with(Reference('other'))
     client_mock.receive.assert_called_with(Reference('kernel[13].in'))
     assert msg.data == {'test': 13}
     assert last_saved == 1.0
 
 
-def test_receive_with_slot(communicator2) -> None:
+def test_receive_with_slot(communicator2, profile_data) -> None:
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('kernel[13].out'), Reference('other.in[13]'),
             None, 0.0, None, Settings({'test': 'testing'}), 0, 3.0,
-            b'test').encoded()
+            b'test').encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator2._Communicator__get_client = get_client_mock
     communicator2._profiler = MagicMock()
 
     msg, last_saved = communicator2.receive_message('in', 13)
 
     get_client_mock.assert_called_with(Reference('kernel[13]'))
     client_mock.receive.assert_called_with(Reference('other.in[13]'))
     assert msg.data == b'test'
     assert msg.settings['test'] == 'testing'
     assert last_saved == 3.0
 
 
-def test_receive_message_resizable(communicator3) -> None:
+def test_receive_message_resizable(communicator3, profile_data) -> None:
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('other.out[13]'), Reference('kernel.in[13]'),
             20, 0.0, None, Settings({'test': 'testing'}), 0, 12.3,
-            b'test').encoded()
+            b'test').encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator3._Communicator__get_client = get_client_mock
     communicator3._profiler = MagicMock()
 
     msg, last_saved = communicator3.receive_message('in', 13)
 
     get_client_mock.assert_called_with(Reference('other'))
     client_mock.receive.assert_called_with(Reference('kernel.in[13]'))
     assert msg.data == b'test'
     assert communicator3.get_port('in').get_length() == 20
     assert last_saved == 12.3
 
 
-def test_receive_with_settings(communicator) -> None:
+def test_receive_with_settings(communicator, profile_data) -> None:
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('other.out[13]'), Reference('kernel[13].in'),
             None, 0.0, None, Settings({'test2': 3.1}), 0, 0.1,
-            b'test').encoded()
+            b'test').encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator._Communicator__get_client = get_client_mock
     communicator._profiler = MagicMock()
 
     msg, last_saved = communicator.receive_message('in')
 
     get_client_mock.assert_called_with(Reference('other'))
     client_mock.receive.assert_called_with(Reference('kernel[13].in'))
     assert msg.data == b'test'
     assert msg.settings['test2'] == 3.1
     assert last_saved == 0.1
 
 
-def test_receive_msgpack_with_slot_and_settings(communicator2) -> None:
+def test_receive_msgpack_with_slot_and_settings(
+        communicator2, profile_data) -> None:
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('kernel[13].out'), Reference('other.in[13]'),
-            None, 0.0, 1.0,
-            Settings({'test': 'testing'}), 0, 1.0, 'test').encoded()
+            None, 0.0, 1.0, Settings({'test': 'testing'}), 0, 1.0,
+            'test').encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator2._Communicator__get_client = get_client_mock
     communicator2._profiler = MagicMock()
 
     msg, last_saved = communicator2.receive_message('in', 13)
 
     get_client_mock.assert_called_with(Reference('kernel[13]'))
     client_mock.receive.assert_called_with(Reference('other.in[13]'))
     assert msg.data == 'test'
     assert msg.settings['test'] == 'testing'
     assert last_saved == 1.0
 
 
-def test_receive_settings(communicator) -> None:
+def test_receive_settings(communicator, profile_data) -> None:
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('other.out[13]'), Reference('kernel[13].in'),
             None, 0.0, None, Settings({'test1': 12}), 0, 1.0,
-            Settings({'test': 13})).encoded()
+            Settings({'test': 13})).encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator._Communicator__get_client = get_client_mock
     communicator._profiler = MagicMock()
 
     msg, last_saved = communicator.receive_message('in')
 
     get_client_mock.assert_called_with(Reference('other'))
     client_mock.receive.assert_called_with(Reference('kernel[13].in'))
     assert isinstance(msg.data, Settings)
     assert msg.data['test'] == 13
     assert last_saved == 1.0
 
 
-def test_receive_close_port(communicator) -> None:
+def test_receive_close_port(communicator, profile_data) -> None:
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('other.out[13]'), Reference('kernel[13].in'),
-            None, 0.0, None, Settings(), 0, 0.1, ClosePort()).encoded()
+            None, 0.0, None, Settings(), 0, 0.1, ClosePort()
+            ).encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator._Communicator__get_client = get_client_mock
     communicator._profiler = MagicMock()
 
     msg, _ = communicator.receive_message('in')
 
     assert isinstance(msg.data, ClosePort)
@@ -617,38 +619,38 @@
                           'muscle_settings_in': [4]}
 
     # empty post office
     communicator2._post_office.get_message('kernel[13].in')
     communicator2._post_office.get_message('kernel[13].in')
 
 
-def test_port_count_validation(communicator):
+def test_port_count_validation(communicator, profile_data):
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('other.out[13]'), Reference('kernel[13].in'),
             None, 0.0, None, Settings({'test1': 12}), 0, 7.6,
-            b'test').encoded()
+            b'test').encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator._Communicator__get_client = get_client_mock
     communicator._profiler = MagicMock()
 
     communicator.receive_message('in')
     assert communicator.get_message_counts()['in'] == [1]
 
     with pytest.raises(RuntimeError):
         # the message received has message_number = 0 again
         communicator.receive_message('in')
 
 
-def test_port_discard_error_on_resume(caplog, communicator):
+def test_port_discard_error_on_resume(caplog, communicator, profile_data):
     client_mock = MagicMock()
     client_mock.receive.return_value = MPPMessage(
             Reference('other.out[13]'), Reference('kernel[13].in'),
             None, 0.0, None, Settings({'test1': 12}), 1, 2.3,
-            b'test').encoded()
+            b'test').encoded(), profile_data
     get_client_mock = MagicMock(return_value=client_mock)
     communicator._Communicator__get_client = get_client_mock
     communicator._profiler = MagicMock()
 
     communicator.restore_message_counts({'out': [0],
                                          'in': [2],
                                          'muscle_settings_in': [0]})
@@ -662,20 +664,20 @@
     with caplog.at_level(logging.DEBUG, 'libmuscle.communicator'):
         with pytest.raises(RuntimeError):
             communicator.receive_message('in')
         # records 0, 2 and 3 are debug logs for starting/receiving on port
         assert 'Discarding received message' in caplog.records[1].message
 
 
-def test_port_discard_success_on_resume(caplog, communicator):
+def test_port_discard_success_on_resume(caplog, communicator, profile_data):
     client_mock = MagicMock()
-    client_mock.receive.side_effect = [MPPMessage(
+    client_mock.receive.side_effect = [(MPPMessage(
             Reference('other.out[13]'), Reference('kernel[13].in'),
             None, 0.0, None, Settings({'test1': 12}), message_number, 1.0,
-            {'this is message': message_number}).encoded()
+            {'this is message': message_number}).encoded(), profile_data)
             for message_number in [1, 2]]
     get_client_mock = MagicMock(return_value=client_mock)
     communicator._Communicator__get_client = get_client_mock
     communicator._profiler = MagicMock()
 
     communicator.restore_message_counts({'out': [0],
                                          'in': [2],
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_instance.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,16 @@
         instance = Instance(ports)
         assert instance._name == Reference('test_instance')
         assert instance._index == [13, 42]
         assert instance._declared_ports == ports
         assert isinstance(instance._settings_manager, SettingsManager)
         assert len(instance._settings_manager.base) == 0
         assert len(instance._settings_manager.overlay) == 0
-        mmp_client.assert_called_once_with('localhost:9000')
+        mmp_client.assert_called_once_with(
+                Reference('test_instance[13][42]'), 'localhost:9000')
         assert mmp_client_object._register.called_with()
         assert mmp_client_object._connect.called_with()
         comm_type.assert_called_with(Reference('test_instance'), [13, 42],
                                      ports, instance._profiler)
         assert instance._communicator == comm_type.return_value
         assert isinstance(instance._settings_manager, SettingsManager)
         assert len(instance._settings_manager.base) == 0
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_mmp_client.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_mmp_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 from libmuscle.mcp.protocol import RequestType, ResponseType
 from libmuscle.mmp_client import MMPClient
 
 
 def test_init() -> None:
     with patch('libmuscle.mmp_client.TcpTransportClient') as mock_ttc:
         stub = mock_ttc.return_value
-        client = MMPClient('')
+        client = MMPClient(Reference([]), '')
         assert client._transport_client == stub     # type: ignore
 
 
 def test_connection_fail() -> None:
     with patch('libmuscle.mmp_client.CONNECTION_TIMEOUT', 1):
         with pytest.raises(RuntimeError):
             # Port 255 is reserved and privileged, so there's probably
             # nothing there.
-            MMPClient('tcp:localhost:255')
+            MMPClient(Reference([]), 'tcp:localhost:255')
 
 
-def test_submit_log_message(mocked_mmp_client) -> None:
+def test_submit_log_message(mocked_mmp_client, profile_data) -> None:
     client, stub = mocked_mmp_client
     result = [ResponseType.SUCCESS.value]
-    stub.call.return_value = msgpack.packb(result, use_bin_type=True)
+    stub.call.return_value = (
+            msgpack.packb(result, use_bin_type=True), profile_data)
 
     message = LogMessage(
             'test_mmp_client',
             Timestamp(1.0),
             LogLevel.WARNING,
             'Testing the MMPClient')
 
@@ -44,126 +45,132 @@
 
     assert decoded_request == [
             RequestType.SUBMIT_LOG_MESSAGE.value,
             'test_mmp_client', 1.0, LogLevel.WARNING.value,
             'Testing the MMPClient']
 
 
-def test_get_settings(mocked_mmp_client) -> None:
+def test_get_settings(mocked_mmp_client, profile_data) -> None:
     client, stub = mocked_mmp_client
 
     settings_msg = {
             'test1': 'test',
             'test2': 12,
             'test3': 3.14,
             'test4': True,
             'test5': [1.2, 3.4],
             'test6': [[1.2, 3.4], [5.6, 7.8]]}
     transport_result = [ResponseType.SUCCESS.value, settings_msg]
-    stub.call.return_value = msgpack.packb(transport_result, use_bin_type=True)
+    stub.call.return_value = (
+            msgpack.packb(transport_result, use_bin_type=True), profile_data)
 
     settings = client.get_settings()
     assert len(settings) == 6
     assert settings['test1'] == 'test'
     assert settings['test2'] == 12
     assert settings['test3'] == 3.14
     assert settings['test4'] is True
     assert settings['test5'] == [1.2, 3.4]
     assert settings['test6'] == [[1.2, 3.4], [5.6, 7.8]]
 
 
-def test_register_instance(mocked_mmp_client) -> None:
+def test_register_instance(mocked_mmp_client, profile_data) -> None:
     client, stub = mocked_mmp_client
 
     result = [ResponseType.SUCCESS.value]
-    stub.call.return_value = msgpack.packb(result, use_bin_type=True)
+    stub.call.return_value = (
+            msgpack.packb(result, use_bin_type=True), profile_data)
 
     client.register_instance(
-            Reference('kernel[13]'),
             ['direct:test', 'tcp:test'],
             [Port('out', Operator.O_I), Port('in', Operator.S)])
 
     assert stub.call.called
     sent_msg = msgpack.unpackb(stub.call.call_args[0][0], raw=False)
     assert sent_msg == [
-            RequestType.REGISTER_INSTANCE.value, 'kernel[13]',
+            RequestType.REGISTER_INSTANCE.value, 'component[13]',
             ['direct:test', 'tcp:test'], [['out', 'O_I'], ['in', 'S']],
             libmuscle.__version__]
 
 
-def test_request_peers(mocked_mmp_client) -> None:
+def test_request_peers(mocked_mmp_client, profile_data) -> None:
     client, stub = mocked_mmp_client
 
     result_msg = [
             ResponseType.SUCCESS.value,
             [['kernel.out', 'other.in']],
             {'other': [20]},
             {'other': ['direct:test', 'tcp:test']}]
-    stub.call.return_value = msgpack.packb(result_msg, use_bin_type=True)
+    stub.call.return_value = (
+            msgpack.packb(result_msg, use_bin_type=True), profile_data)
 
-    result = client.request_peers(Reference('kernel[13]'))
+    result = client.request_peers()
 
     assert stub.call.called
     sent_msg = msgpack.unpackb(stub.call.call_args[0][0], raw=False)
     assert sent_msg[0] == RequestType.GET_PEERS.value
-    assert sent_msg[1] == 'kernel[13]'
+    assert sent_msg[1] == 'component[13]'
 
     assert len(result[0]) == 1
     assert isinstance(result[0][0], Conduit)
     assert result[0][0].sender == 'kernel.out'
     assert result[0][0].receiver == 'other.in'
 
     assert isinstance(result[1], dict)
     assert result[1]['other'] == [20]
 
     assert isinstance(result[2], dict)
     assert result[2]['other'] == ['direct:test', 'tcp:test']
 
 
-def test_request_peers_error(mocked_mmp_client) -> None:
+def test_request_peers_error(mocked_mmp_client, profile_data) -> None:
     client, stub = mocked_mmp_client
 
     result_msg = [ResponseType.ERROR.value, 'test_error_message']
-    stub.call.return_value = msgpack.packb(result_msg, use_bin_type=True)
+    stub.call.return_value = (
+            msgpack.packb(result_msg, use_bin_type=True), profile_data)
 
     with pytest.raises(RuntimeError):
-        client.request_peers(Reference('kernel[13]'))
+        client.request_peers()
 
 
-def test_request_peers_timeout(mocked_mmp_client) -> None:
+def test_request_peers_timeout(mocked_mmp_client, profile_data) -> None:
     client, stub = mocked_mmp_client
 
     result_msg = [ResponseType.PENDING.value, 'test_status_message']
-    stub.call.return_value = msgpack.packb(result_msg, use_bin_type=True)
+    stub.call.return_value = (
+            msgpack.packb(result_msg, use_bin_type=True), profile_data)
 
     with patch('libmuscle.mmp_client.PEER_TIMEOUT', 1), \
             patch('libmuscle.mmp_client.PEER_INTERVAL_MIN', 0.1), \
             patch('libmuscle.mmp_client.PEER_INTERVAL_MAX', 1.0):
         with pytest.raises(RuntimeError):
-            client.request_peers(Reference('kernel[13]'))
+            client.request_peers()
 
 
-def test_deregister_instance(mocked_mmp_client) -> None:
+def test_deregister_instance(mocked_mmp_client, profile_data) -> None:
     client, stub = mocked_mmp_client
 
     result = [ResponseType.SUCCESS.value]
-    stub.call.return_value = msgpack.packb(result, use_bin_type=True)
+    stub.call.return_value = (
+            msgpack.packb(result, use_bin_type=True), profile_data)
 
-    client.deregister_instance(Reference('kernel[13]'))
+    client.deregister_instance()
 
     assert stub.call.called
     sent_msg = msgpack.unpackb(stub.call.call_args[0][0], raw=False)
-    assert sent_msg == [RequestType.DEREGISTER_INSTANCE.value, 'kernel[13]']
+    assert sent_msg == [RequestType.DEREGISTER_INSTANCE.value, 'component[13]']
 
 
-def test_deregister_instance_error(mocked_mmp_client) -> None:
+def test_deregister_instance_error(mocked_mmp_client, profile_data) -> None:
     client, stub = mocked_mmp_client
 
-    result = [ResponseType.ERROR.value, 'Instance kernel[13] unknown']
-    stub.call.return_value = msgpack.packb(result, use_bin_type=True)
+    result = [ResponseType.ERROR.value, 'Instance component[13] unknown']
+    stub.call.return_value = (
+            msgpack.packb(result, use_bin_type=True), profile_data)
 
     with pytest.raises(RuntimeError):
-        client.deregister_instance(Reference('kernel[13]'))
+        client.deregister_instance()
 
     assert stub.call.called
     sent_msg = msgpack.unpackb(stub.call.call_args[0][0], raw=False)
-    assert sent_msg == [RequestType.DEREGISTER_INSTANCE.value, 'kernel[13]']
+    assert sent_msg == [RequestType.DEREGISTER_INSTANCE.value, 'component[13]']
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_mpp_message.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_mpp_message.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_outbox.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_outbox.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_port.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_port.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_snapshot.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_snapshot.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_snapshot_manager.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_snapshot_manager.py`

 * *Files 13% similar despite different names*

```diff
@@ -34,16 +34,15 @@
 
     snapshot_manager.save_snapshot(
             Message(0.2, None, 'test data'), False, ['test'], 13.0, None,
             Settings())
 
     communicator.get_message_counts.assert_called_with()
     manager.submit_snapshot_metadata.assert_called()
-    instance, metadata = manager.submit_snapshot_metadata.call_args[0]
-    assert instance == instance_id
+    metadata, = manager.submit_snapshot_metadata.call_args[0]
     assert isinstance(metadata, SnapshotMetadata)
     assert metadata.triggers == ['test']
     assert metadata.wallclock_time == 13.0
     assert metadata.timestamp == 0.2
     assert metadata.next_timestamp is None
     assert metadata.port_message_counts == port_message_counts
     assert not metadata.is_final_snapshot
@@ -63,33 +62,26 @@
     assert msg.next_timestamp is None
     assert msg.data == 'test data'
 
     snapshot_manager2.save_snapshot(
             Message(0.6, None, 'test data2'), True, ['test'], 42.2, 1.2,
             Settings())
 
-    instance, metadata = manager.submit_snapshot_metadata.call_args[0]
-    assert instance == instance_id
+    metadata, = manager.submit_snapshot_metadata.call_args[0]
     assert isinstance(metadata, SnapshotMetadata)
     assert metadata.triggers == ['test']
     assert metadata.wallclock_time == 42.2
     assert metadata.timestamp == 0.6
     assert metadata.next_timestamp is None
     assert metadata.port_message_counts == port_message_counts
     assert metadata.is_final_snapshot
     snapshot_path = Path(metadata.snapshot_filename)
     assert snapshot_path.parent == tmp_path
     assert snapshot_path.name == 'test-1_3.pack'
 
-    assert snapshot_manager2.resuming_from_intermediate()
-    assert not snapshot_manager2.resuming_from_final()
-    snapshot_manager2.load_snapshot()
-    assert snapshot_manager2.resuming_from_intermediate()
-    assert not snapshot_manager2.resuming_from_final()
-
 
 def test_save_load_implicit_snapshot(tmp_path: Path) -> None:
     manager = MagicMock()
     communicator = MagicMock()
     port_message_counts = {'in': [1], 'out': [2], 'muscle_settings_in': [0]}
     communicator.get_message_counts.return_value = port_message_counts
 
@@ -101,16 +93,15 @@
     assert not snapshot_manager.resuming_from_intermediate()
     assert not snapshot_manager.resuming_from_final()
     # save implicit snapshot
     snapshot_manager.save_snapshot(
             None, True, ['implicit'], 1.0, 1.5, Settings())
 
     manager.submit_snapshot_metadata.assert_called_once()
-    instance, metadata = manager.submit_snapshot_metadata.call_args[0]
-    assert instance == instance_id
+    metadata, = manager.submit_snapshot_metadata.call_args[0]
     assert isinstance(metadata, SnapshotMetadata)
     snapshot_path = Path(metadata.snapshot_filename)
     manager.submit_snapshot_metadata.reset_mock()
 
     snapshot_manager2 = SnapshotManager(instance_id, manager, communicator)
 
     snapshot_manager2.prepare_resume(snapshot_path, tmp_path)
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/test/test_util.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/test/test_util.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/timestamp.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/timestamp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import datetime
+import time
+from typing import Optional
 
 
 class Timestamp:
     """A timestamp, as the number of seconds since the UNIX epoch.
 
     Args:
         seconds: The number of seconds since the start of 1970.
     """
-    def __init__(self, seconds: float) -> None:
+    def __init__(self, seconds: Optional[float] = None) -> None:
+        """Create a Timestamp representing the given time, or now.
+
+        If seconds is None, the current time is used.
+        """
+        if seconds is None:
+            seconds = time.time()
         self.seconds = seconds
 
     def to_asctime(self) -> str:
         """Converts a Timestamp to a LogRecord asctime.
 
         Returns:
             The timestamp as a string in the format used by default
```

### Comparing `muscle3-0.6.0/libmuscle/python/libmuscle/util.py` & `muscle3-0.7.0/libmuscle/python/libmuscle/util.py`

 * *Files identical despite different names*

### Comparing `muscle3-0.6.0/muscle3/muscle3.py` & `muscle3-0.7.0/muscle3/muscle3.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import ymmsl
 from ymmsl import PartialConfiguration
 
 
 from libmuscle.planner.planner import (
         Planner, Resources, InsufficientResourcesAvailable)
 from libmuscle.snapshot_manager import SnapshotManager
+from muscle3.profiling import (
+        plot_instances, plot_resources, plot_timeline, show_plots)
 
 
 _RESOURCES_INCOMPLETE_MODEL = """
 A model, implementations and resources must be given to be able to calculate
 resources for a model. Please ensure that you have specified all of them in
 your yMMSL file(s).
 """
@@ -28,14 +30,69 @@
     using MUSCLE3.
 
     Use muscle3 <command> --help for help with individual commands.
     """
     pass
 
 
+@muscle3.command(short_help='Visualise profiling information')
+@click.argument(
+        'performance_file', nargs=1, type=click.Path(
+            exists=True, file_okay=True, dir_okay=False, readable=True,
+            allow_dash=True, resolve_path=True))
+@click.option('-i', '--instances', is_flag=True, help='Show per-instance statistics')
+@click.option('-r', '--resources', is_flag=True, help='Show per-resource statistics')
+@click.option('-t', '--timeline', is_flag=True, help='Show a timeline of events')
+def profile(
+        performance_file: str, instances: bool, resources: bool, timeline: bool
+        ) -> None:
+    """Visualise profiling information.
+
+    Takes data from a performance.sqlite file written by the manager,
+    and produces one or more plots on the screen.
+
+    Profiling functionality is still somewhat experimental, so this
+    command may be changed and extended in the coming releases. Please
+    let us know if there are any changes or additional features you
+    would like to have by making an issue on GitHub, or through your
+    usual support channel.
+
+    Result:
+        With -i, shows a chart depicting for each instance how much time
+        it spend running, waiting and communicating.
+
+        With -r, shows a chart depicting for each resource (CPU core)
+        which instances ran on it for how long.
+
+        With -t, shows a timeline of the different instances, depicting
+        when they were sending, waiting, receiving and running.
+    """
+    if instances:
+        plot_instances(Path(performance_file))
+
+    if resources:
+        plot_resources(Path(performance_file))
+
+    if timeline:
+        plot_timeline(Path(performance_file))
+        click.echo(
+                'Hint: To inspect the timeline in more detail, use the'
+                ' pan and zoom buttons at the bottom of the window.')
+
+    if instances or resources or timeline:
+        show_plots()
+    else:
+        click.echo(
+                'Please specify -i, -r or -t to choose which data'
+                ' you would like to see.')
+        sys.exit(1)
+
+    sys.exit(0)
+
+
 @muscle3.command(short_help='Calculate resources needed for a simulation')
 @click.argument(
         'ymmsl_files', nargs=-1, required=True, type=click.Path(
             exists=True, file_okay=True, dir_okay=False, readable=True,
             allow_dash=True, resolve_path=True))
 @click.option(
         '-c', '--cores-per-node', nargs=1, type=int, required=True,
```

### Comparing `muscle3-0.6.0/muscle3.egg-info/PKG-INFO` & `muscle3-0.7.0/muscle3.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muscle3
-Version: 0.6.0
+Version: 0.7.0
 Summary: Version 3 of the MUltiScale Coupling Library and Environment
 Home-page: https://github.com/multiscale/muscle3
 Author: Lourens Veen
 Author-email: l.veen@esciencecenter.nl
 License: Apache License 2.0
 Keywords: multiscale,coupling,MUSCLE
 Platform: UNKNOWN
@@ -20,30 +20,22 @@
 Provides-Extra: dev
 License-File: LICENSE
 License-File: NOTICE
 
 .. image:: https://github.com/multiscale/muscle3/raw/develop/docs/source/muscle3_logo_readme.png
     :alt: MUSCLE3
 
-.. image:: https://readthedocs.org/projects/muscle3/badge/?version=master
-    :target: https://muscle3.readthedocs.io/en/develop/?badge=master
+.. image:: https://readthedocs.org/projects/muscle3/badge/?version=latest
+    :target: https://muscle3.readthedocs.io/en/develop/?badge=latest
     :alt: Documentation Build Status
 
 .. image:: https://github.com/multiscale/muscle3/workflows/continuous_integration/badge.svg?branch=master
     :target: https://github.com/multiscale/muscle3/actions
     :alt: Build Status
 
-.. image:: https://app.codacy.com/project/badge/Coverage/4542a84edcd947ee982a0bfabe617089
-    :target: https://www.codacy.com/gh/multiscale/muscle3/dashboard
-    :alt: Code Coverage
-
-.. image:: https://app.codacy.com/project/badge/Grade/4542a84edcd947ee982a0bfabe617089
-    :target: https://www.codacy.com/gh/multiscale/muscle3/dashboard
-    :alt: Codacy Grade
-
 .. image:: https://zenodo.org/badge/122876985.svg
    :target: https://zenodo.org/badge/latestdoi/122876985
 
 .. image:: https://img.shields.io/badge/rsd-muscle3-00a3e3.svg
    :target: https://www.research-software.nl/software/muscle3
 
 |
```

### Comparing `muscle3-0.6.0/muscle3.egg-info/SOURCES.txt` & `muscle3-0.7.0/muscle3.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,14 @@
 LICENSE
 MANIFEST.in
 NOTICE
 README.rst
 VERSION
 setup.cfg
 setup.py
-integration_test/__init__.py
-integration_test/conftest.py
-integration_test/include_libmuscle.py
-integration_test/test_all.py
-integration_test/test_cpp_macro_micro.py
-integration_test/test_cpp_mmp_client.py
-integration_test/test_cpp_tcp_server.py
-integration_test/test_duplication_mapper.py
-integration_test/test_fortran_macro_micro.py
-integration_test/test_logging.py
-integration_test/test_mpi_macro_micro.py
-integration_test/test_parameter_overlays.py
-integration_test/test_registration.py
-integration_test/test_version.py
 libmuscle/python/libmuscle/__init__.py
 libmuscle/python/libmuscle/api_guard.py
 libmuscle/python/libmuscle/checkpoint_triggers.py
 libmuscle/python/libmuscle/communicator.py
 libmuscle/python/libmuscle/endpoint.py
 libmuscle/python/libmuscle/grid.py
 libmuscle/python/libmuscle/instance.py
@@ -47,23 +33,27 @@
 libmuscle/python/libmuscle/manager/__init__.py
 libmuscle/python/libmuscle/manager/instance_manager.py
 libmuscle/python/libmuscle/manager/instance_registry.py
 libmuscle/python/libmuscle/manager/instantiator.py
 libmuscle/python/libmuscle/manager/logger.py
 libmuscle/python/libmuscle/manager/manager.py
 libmuscle/python/libmuscle/manager/mmp_server.py
+libmuscle/python/libmuscle/manager/profile_database.py
+libmuscle/python/libmuscle/manager/profile_store.py
 libmuscle/python/libmuscle/manager/qcgpj_instantiator.py
 libmuscle/python/libmuscle/manager/run_dir.py
 libmuscle/python/libmuscle/manager/snapshot_registry.py
 libmuscle/python/libmuscle/manager/topology_store.py
 libmuscle/python/libmuscle/manager/test/__init__.py
 libmuscle/python/libmuscle/manager/test/conftest.py
 libmuscle/python/libmuscle/manager/test/test_instance_registry.py
 libmuscle/python/libmuscle/manager/test/test_logger.py
 libmuscle/python/libmuscle/manager/test/test_mmp_request_handler.py
+libmuscle/python/libmuscle/manager/test/test_profile_database.py
+libmuscle/python/libmuscle/manager/test/test_profile_store.py
 libmuscle/python/libmuscle/manager/test/test_snapshot_registry.py
 libmuscle/python/libmuscle/manager/test/test_topology_store.py
 libmuscle/python/libmuscle/mcp/__init__.py
 libmuscle/python/libmuscle/mcp/protocol.py
 libmuscle/python/libmuscle/mcp/tcp_transport_client.py
 libmuscle/python/libmuscle/mcp/tcp_transport_server.py
 libmuscle/python/libmuscle/mcp/tcp_util.py
@@ -83,22 +73,24 @@
 libmuscle/python/libmuscle/test/test_communicator.py
 libmuscle/python/libmuscle/test/test_grid.py
 libmuscle/python/libmuscle/test/test_instance.py
 libmuscle/python/libmuscle/test/test_mmp_client.py
 libmuscle/python/libmuscle/test/test_mpp_message.py
 libmuscle/python/libmuscle/test/test_outbox.py
 libmuscle/python/libmuscle/test/test_port.py
+libmuscle/python/libmuscle/test/test_profiler.py
 libmuscle/python/libmuscle/test/test_settings_manager.py
 libmuscle/python/libmuscle/test/test_snapshot.py
 libmuscle/python/libmuscle/test/test_snapshot_manager.py
 libmuscle/python/libmuscle/test/test_test.py
 libmuscle/python/libmuscle/test/test_util.py
 muscle3/__init__.py
 muscle3/conftest.py
 muscle3/muscle3.py
 muscle3/muscle_manager.py
+muscle3/profiling.py
 muscle3.egg-info/PKG-INFO
 muscle3.egg-info/SOURCES.txt
 muscle3.egg-info/dependency_links.txt
 muscle3.egg-info/entry_points.txt
 muscle3.egg-info/requires.txt
 muscle3.egg-info/top_level.txt
```

### Comparing `muscle3-0.6.0/setup.cfg` & `muscle3-0.7.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool:pytest]
 testpaths = libmuscle/python integration_test
 addopts = --cov --cov-report xml --cov-report term-missing -s
 
 [mypy]
-files = libmuscle/python/**/*.py
+files = libmuscle/python/**/*.py, scripts/*.py
 mypy_path = libmuscle/python
 warn_unused_configs = True
 disallow_subclassing_any = True
 disallow_untyped_calls = True
 disallow_untyped_defs = True
 disallow_incomplete_defs = True
 check_untyped_defs = True
@@ -41,16 +41,16 @@
 [mypy-numpy.*]
 ignore_missing_imports = True
 
 [mypy-qcg.*]
 ignore_missing_imports = True
 
 [flake8]
-ignore = 
+per-file-ignores = 
 	setup.py: E501
-	libmuscle/manager_protocol/*.py: ALL
 	*.py: E123 E126 W504
+max-line-length = 88
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `muscle3-0.6.0/setup.py` & `muscle3-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,20 +47,21 @@
         'console_scripts': [
             'muscle_manager=muscle3.muscle_manager:manage_simulation',
             'muscle3=muscle3.muscle3:muscle3']
     },
     python_requires='>=3.7, <4',
     install_requires=[
         'click>=7.1,<9',
+        'matplotlib>=3,<4',
         'msgpack>=1,<2',
         'netifaces==0.11.0',
         "numpy<1.22; python_version=='3.7'",
         "numpy>=1.22,<=1.25; python_version>='3.8'",
         'qcg-pilotjob==0.13.1',
-        'typing_extensions<4',
+        'typing_extensions>=4.4.0,<5',
         'ymmsl>=0.13.0,<0.14'          # Also in CI, update there as well
     ],
     extras_require={
         'dev': [
             'sphinx<3.2',
             'sphinx_rtd_theme',
             'sphinx-fortran',
```

