# Comparing `tmp/strmprivacy-api-definitions-2.9.0.tar.gz` & `tmp/strmprivacy-api-definitions-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strmprivacy-api-definitions-2.9.0.tar", last modified: Tue Dec 28 09:53:36 2021, max compression
+gzip compressed data, was "strmprivacy-api-definitions-3.0.0.tar", last modified: Thu Jun 22 07:58:18 2023, max compression
```

## Comparing `strmprivacy-api-definitions-2.9.0.tar` & `strmprivacy-api-definitions-3.0.0.tar`

### file list

```diff
@@ -1,111 +1,227 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.992056 strmprivacy-api-definitions-2.9.0/
--rw-r--r--   0 root         (0) root         (0)      629 2021-12-28 09:53:36.991057 strmprivacy-api-definitions-2.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-28 09:53:36.992056 strmprivacy-api-definitions-2.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1443 2021-12-28 09:53:20.000000 strmprivacy-api-definitions-2.9.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.976055 strmprivacy-api-definitions-2.9.0/strmprivacy/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.977055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.977055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/account/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.977055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/account/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/account/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30926 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/account/v1/account_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14846 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.978055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/batch_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/batch_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.978055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/batch_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/batch_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17578 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.978055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.979055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/cli/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/cli/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8535 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/cli/v1/cli_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2753 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.979055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/consent_levels/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/consent_levels/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.980055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/consent_levels/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/consent_levels/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18529 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/consent_levels/v1/consent_levels_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9797 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/consent_levels/v1/consent_levels_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.980055 strmprivacy-api-definitions-2.9.0/strmprivacy/api/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/credentials/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.981056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/credentials/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/credentials/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16558 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8979 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.981056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.982056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/entities/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/entities/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)   124220 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.982056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/event_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/event_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.982056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/event_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/event_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39011 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11581 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.983056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_clusters/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_clusters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.983056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_clusters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_clusters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18595 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9342 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.983056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.984056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18337 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.984056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_users/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_users/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.985056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_users/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_users/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16844 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8964 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.985056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/key_streams/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/key_streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.986056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/key_streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/key_streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9591 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4941 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.986056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/metrics/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/metrics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.986056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/metrics/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/metrics/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6380 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/metrics/v1/metrics_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2909 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/metrics/v1/metrics_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.987056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.987056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/schemas/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/schemas/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32964 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10359 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.987056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/sinks/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/sinks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.988056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/sinks/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/sinks/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17030 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8223 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.988056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/streams/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.989056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17539 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8475 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.989056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/usage/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/usage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.990056 strmprivacy-api-definitions-2.9.0/strmprivacy/api/usage/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/usage/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8589 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2953 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-28 09:53:36.991057 strmprivacy-api-definitions-2.9.0/strmprivacy_api_definitions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      629 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy_api_definitions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3324 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy_api_definitions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy_api_definitions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2021-12-28 09:53:36.000000 strmprivacy-api-definitions-2.9.0/strmprivacy_api_definitions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.575838 strmprivacy-api-definitions-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-22 07:58:18.574838 strmprivacy-api-definitions-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 07:58:18.575838 strmprivacy-api-definitions-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-22 07:57:41.000000 strmprivacy-api-definitions-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.378821 strmprivacy-api-definitions-3.0.0/strmprivacy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.378821 strmprivacy-api-definitions-3.0.0/strmprivacy/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.378821 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.381821 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12198 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/account_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16789 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.382821 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.387822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.387822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.390822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/audit_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5030 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.391822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.393822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.394822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.398823 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10858 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.399823 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.403823 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/cli_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.429825 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.550836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3987 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/comments_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6740 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.551836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.552836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8979 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.552836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.552836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7497 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.552836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.553836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5978 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.553836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.554836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22863 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28488 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.554836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.555836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9865 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.555836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.556836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81835 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.556836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12164 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.556836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.557836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15658 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    20098 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.557836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.558837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/handles_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.558837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.559837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7909 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6253 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6958 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10345 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.559837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.560837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6199 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9342 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.561837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.561837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.562837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.562837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5369 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8964 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.562837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.563837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.563837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.564837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.564837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.565837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10605 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13648 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.565837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.565837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.565837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.566837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5842 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9075 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.566837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.567837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/paging_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.567837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.568838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/policies_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10449 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.568838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.568838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.568838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.569838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/projects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14509 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.569838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.570838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7407 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.570838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.571838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    17973 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.571838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.571838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5254 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.572838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.572838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10437 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.572838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.573838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4644 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.574838 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/top_level.txt
```

### Comparing `strmprivacy-api-definitions-2.9.0/PKG-INFO` & `strmprivacy-api-definitions-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 2.9.0
+Version: 3.0.0
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-2.9.0/setup.py` & `strmprivacy-api-definitions-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,45 +45,54 @@
                 response_deserializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.InitializeCustomerPortalResponse.FromString,
                 )
         self.SetCheckoutCancelled = channel.unary_unary(
                 '/strmprivacy.api.account.v1.AccountService/SetCheckoutCancelled',
                 request_serializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.SetCheckoutCancelledRequest.SerializeToString,
                 response_deserializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.SetCheckoutCancelledResponse.FromString,
                 )
+        self.UpdateOnboarding = channel.unary_unary(
+                '/strmprivacy.api.account.v1.AccountService/UpdateOnboarding',
+                request_serializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.UpdateOnboardingRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.UpdateOnboardingResponse.FromString,
+                )
 
 
 class AccountServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetAccountDetails(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Retrieve information regarding quotas, and the user context
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetLegacyBillingId(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def CreateAccountHandle(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Claim and create a handle for your user
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def InitializeCheckout(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Start a checkout to subscribe to a specific subscription
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetCheckoutStatus(self, request, context):
-        """Missing associated documentation comment in .proto file."""
+        """Get the Stripe Checkout Status for an ongoing checkout
+        """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def InitializeCustomerPortal(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
@@ -94,14 +103,20 @@
         """(-- api-linter: core::0134::synonyms=disabled
         aip.dev/not-precedent: We're not updating a Checkout here. --)
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def UpdateOnboarding(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_AccountServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetAccountDetails': grpc.unary_unary_rpc_method_handler(
                     servicer.GetAccountDetails,
                     request_deserializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.GetAccountDetailsRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.GetAccountDetailsResponse.SerializeToString,
@@ -132,14 +147,19 @@
                     response_serializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.InitializeCustomerPortalResponse.SerializeToString,
             ),
             'SetCheckoutCancelled': grpc.unary_unary_rpc_method_handler(
                     servicer.SetCheckoutCancelled,
                     request_deserializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.SetCheckoutCancelledRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.SetCheckoutCancelledResponse.SerializeToString,
             ),
+            'UpdateOnboarding': grpc.unary_unary_rpc_method_handler(
+                    servicer.UpdateOnboarding,
+                    request_deserializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.UpdateOnboardingRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.UpdateOnboardingResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'strmprivacy.api.account.v1.AccountService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -260,7 +280,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.account.v1.AccountService/SetCheckoutCancelled',
             strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.SetCheckoutCancelledRequest.SerializeToString,
             strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.SetCheckoutCancelledResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def UpdateOnboarding(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.account.v1.AccountService/UpdateOnboarding',
+            strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.UpdateOnboardingRequest.SerializeToString,
+            strmprivacy_dot_api_dot_account_dot_v1_dot_account__v1__pb2.UpdateOnboardingResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/consent_levels/v1/consent_levels_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,165 +1,165 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from strmprivacy.api.consent_levels.v1 import consent_levels_v1_pb2 as strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2
+from strmprivacy.api.credentials.v1 import credentials_v1_pb2 as strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2
 
 
-class ConsentLevelMappingsServiceStub(object):
+class CredentialsServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.ListConsentLevelMappings = channel.unary_unary(
-                '/strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService/ListConsentLevelMappings',
-                request_serializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.ListConsentLevelMappingsRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.ListConsentLevelMappingsResponse.FromString,
+        self.ListCredentials = channel.unary_unary(
+                '/strmprivacy.api.credentials.v1.CredentialsService/ListCredentials',
+                request_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsResponse.FromString,
                 )
-        self.GetConsentLevelMapping = channel.unary_unary(
-                '/strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService/GetConsentLevelMapping',
-                request_serializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.GetConsentLevelMappingRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.GetConsentLevelMappingResponse.FromString,
+        self.GetCredential = channel.unary_unary(
+                '/strmprivacy.api.credentials.v1.CredentialsService/GetCredential',
+                request_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialResponse.FromString,
                 )
-        self.DeleteConsentLevelMapping = channel.unary_unary(
-                '/strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService/DeleteConsentLevelMapping',
-                request_serializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.DeleteConsentLevelMappingRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.DeleteConsentLevelMappingResponse.FromString,
+        self.CreateCredential = channel.unary_unary(
+                '/strmprivacy.api.credentials.v1.CredentialsService/CreateCredential',
+                request_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialResponse.FromString,
                 )
-        self.CreateConsentLevelMapping = channel.unary_unary(
-                '/strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService/CreateConsentLevelMapping',
-                request_serializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.CreateConsentLevelMappingRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.CreateConsentLevelMappingResponse.FromString,
+        self.DeleteCredential = channel.unary_unary(
+                '/strmprivacy.api.credentials.v1.CredentialsService/DeleteCredential',
+                request_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialResponse.FromString,
                 )
 
 
-class ConsentLevelMappingsServiceServicer(object):
+class CredentialsServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def ListConsentLevelMappings(self, request, context):
+    def ListCredentials(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetConsentLevelMapping(self, request, context):
+    def GetCredential(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteConsentLevelMapping(self, request, context):
+    def CreateCredential(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateConsentLevelMapping(self, request, context):
+    def DeleteCredential(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_ConsentLevelMappingsServiceServicer_to_server(servicer, server):
+def add_CredentialsServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'ListConsentLevelMappings': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListConsentLevelMappings,
-                    request_deserializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.ListConsentLevelMappingsRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.ListConsentLevelMappingsResponse.SerializeToString,
+            'ListCredentials': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListCredentials,
+                    request_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsResponse.SerializeToString,
             ),
-            'GetConsentLevelMapping': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetConsentLevelMapping,
-                    request_deserializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.GetConsentLevelMappingRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.GetConsentLevelMappingResponse.SerializeToString,
+            'GetCredential': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetCredential,
+                    request_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialResponse.SerializeToString,
             ),
-            'DeleteConsentLevelMapping': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteConsentLevelMapping,
-                    request_deserializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.DeleteConsentLevelMappingRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.DeleteConsentLevelMappingResponse.SerializeToString,
+            'CreateCredential': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateCredential,
+                    request_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialResponse.SerializeToString,
             ),
-            'CreateConsentLevelMapping': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateConsentLevelMapping,
-                    request_deserializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.CreateConsentLevelMappingRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.CreateConsentLevelMappingResponse.SerializeToString,
+            'DeleteCredential': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteCredential,
+                    request_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService', rpc_method_handlers)
+            'strmprivacy.api.credentials.v1.CredentialsService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class ConsentLevelMappingsService(object):
+class CredentialsService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def ListConsentLevelMappings(request,
+    def ListCredentials(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService/ListConsentLevelMappings',
-            strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.ListConsentLevelMappingsRequest.SerializeToString,
-            strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.ListConsentLevelMappingsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.credentials.v1.CredentialsService/ListCredentials',
+            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsRequest.SerializeToString,
+            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetConsentLevelMapping(request,
+    def GetCredential(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService/GetConsentLevelMapping',
-            strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.GetConsentLevelMappingRequest.SerializeToString,
-            strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.GetConsentLevelMappingResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.credentials.v1.CredentialsService/GetCredential',
+            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialRequest.SerializeToString,
+            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteConsentLevelMapping(request,
+    def CreateCredential(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService/DeleteConsentLevelMapping',
-            strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.DeleteConsentLevelMappingRequest.SerializeToString,
-            strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.DeleteConsentLevelMappingResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.credentials.v1.CredentialsService/CreateCredential',
+            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialRequest.SerializeToString,
+            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateConsentLevelMapping(request,
+    def DeleteCredential(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.consent_levels.v1.ConsentLevelMappingsService/CreateConsentLevelMapping',
-            strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.CreateConsentLevelMappingRequest.SerializeToString,
-            strmprivacy_dot_api_dot_consent__levels_dot_v1_dot_consent__levels__v1__pb2.CreateConsentLevelMappingResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.credentials.v1.CredentialsService/DeleteCredential',
+            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialRequest.SerializeToString,
+            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,165 +1,165 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from strmprivacy.api.credentials.v1 import credentials_v1_pb2 as strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2
+from strmprivacy.api.kafka_exporters.v1 import kafka_exporters_v1_pb2 as strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2
 
 
-class CredentialsServiceStub(object):
+class KafkaExportersServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.ListCredentials = channel.unary_unary(
-                '/strmprivacy.api.credentials.v1.CredentialsService/ListCredentials',
-                request_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsResponse.FromString,
+        self.ListKafkaExporters = channel.unary_unary(
+                '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/ListKafkaExporters',
+                request_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersResponse.FromString,
                 )
-        self.GetCredential = channel.unary_unary(
-                '/strmprivacy.api.credentials.v1.CredentialsService/GetCredential',
-                request_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialResponse.FromString,
+        self.GetKafkaExporter = channel.unary_unary(
+                '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/GetKafkaExporter',
+                request_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterResponse.FromString,
                 )
-        self.CreateCredential = channel.unary_unary(
-                '/strmprivacy.api.credentials.v1.CredentialsService/CreateCredential',
-                request_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialResponse.FromString,
+        self.DeleteKafkaExporter = channel.unary_unary(
+                '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/DeleteKafkaExporter',
+                request_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterResponse.FromString,
                 )
-        self.DeleteCredential = channel.unary_unary(
-                '/strmprivacy.api.credentials.v1.CredentialsService/DeleteCredential',
-                request_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialResponse.FromString,
+        self.CreateKafkaExporter = channel.unary_unary(
+                '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/CreateKafkaExporter',
+                request_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterResponse.FromString,
                 )
 
 
-class CredentialsServiceServicer(object):
+class KafkaExportersServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def ListCredentials(self, request, context):
+    def ListKafkaExporters(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetCredential(self, request, context):
+    def GetKafkaExporter(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateCredential(self, request, context):
+    def DeleteKafkaExporter(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteCredential(self, request, context):
+    def CreateKafkaExporter(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_CredentialsServiceServicer_to_server(servicer, server):
+def add_KafkaExportersServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'ListCredentials': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListCredentials,
-                    request_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsResponse.SerializeToString,
+            'ListKafkaExporters': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListKafkaExporters,
+                    request_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersResponse.SerializeToString,
             ),
-            'GetCredential': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetCredential,
-                    request_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialResponse.SerializeToString,
+            'GetKafkaExporter': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetKafkaExporter,
+                    request_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterResponse.SerializeToString,
             ),
-            'CreateCredential': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateCredential,
-                    request_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialResponse.SerializeToString,
+            'DeleteKafkaExporter': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteKafkaExporter,
+                    request_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterResponse.SerializeToString,
             ),
-            'DeleteCredential': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteCredential,
-                    request_deserializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialResponse.SerializeToString,
+            'CreateKafkaExporter': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKafkaExporter,
+                    request_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'strmprivacy.api.credentials.v1.CredentialsService', rpc_method_handlers)
+            'strmprivacy.api.kafka_exporters.v1.KafkaExportersService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class CredentialsService(object):
+class KafkaExportersService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def ListCredentials(request,
+    def ListKafkaExporters(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.credentials.v1.CredentialsService/ListCredentials',
-            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsRequest.SerializeToString,
-            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.ListCredentialsResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/ListKafkaExporters',
+            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersRequest.SerializeToString,
+            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetCredential(request,
+    def GetKafkaExporter(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.credentials.v1.CredentialsService/GetCredential',
-            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialRequest.SerializeToString,
-            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.GetCredentialResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/GetKafkaExporter',
+            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterRequest.SerializeToString,
+            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateCredential(request,
+    def DeleteKafkaExporter(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.credentials.v1.CredentialsService/CreateCredential',
-            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialRequest.SerializeToString,
-            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.CreateCredentialResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/DeleteKafkaExporter',
+            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterRequest.SerializeToString,
+            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteCredential(request,
+    def CreateKafkaExporter(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.credentials.v1.CredentialsService/DeleteCredential',
-            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialRequest.SerializeToString,
-            strmprivacy_dot_api_dot_credentials_dot_v1_dot_credentials__v1__pb2.DeleteCredentialResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/CreateKafkaExporter',
+            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterRequest.SerializeToString,
+            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py`

 * *Files 27% similar despite different names*

```diff
@@ -30,19 +30,39 @@
                 response_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.CreateEventContractResponse.FromString,
                 )
         self.UpdateEventContract = channel.unary_unary(
                 '/strmprivacy.api.event_contracts.v1.EventContractsService/UpdateEventContract',
                 request_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.UpdateEventContractRequest.SerializeToString,
                 response_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.UpdateEventContractResponse.FromString,
                 )
+        self.ActivateEventContract = channel.unary_unary(
+                '/strmprivacy.api.event_contracts.v1.EventContractsService/ActivateEventContract',
+                request_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ActivateEventContractRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ActivateEventContractResponse.FromString,
+                )
+        self.DeleteEventContract = channel.unary_unary(
+                '/strmprivacy.api.event_contracts.v1.EventContractsService/DeleteEventContract',
+                request_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.DeleteEventContractRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.DeleteEventContractResponse.FromString,
+                )
+        self.ArchiveEventContract = channel.unary_unary(
+                '/strmprivacy.api.event_contracts.v1.EventContractsService/ArchiveEventContract',
+                request_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ArchiveEventContractRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ArchiveEventContractResponse.FromString,
+                )
         self.ValidateMaskedFields = channel.unary_unary(
                 '/strmprivacy.api.event_contracts.v1.EventContractsService/ValidateMaskedFields',
                 request_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ValidateMaskedFieldsRequest.SerializeToString,
                 response_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ValidateMaskedFieldsResponse.FromString,
                 )
+        self.GetEventContractAndSchema = channel.unary_unary(
+                '/strmprivacy.api.event_contracts.v1.EventContractsService/GetEventContractAndSchema',
+                request_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.GetEventContractAndSchemaRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.GetEventContractAndSchemaResponse.FromString,
+                )
 
 
 class EventContractsServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ListEventContracts(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -64,20 +84,44 @@
 
     def UpdateEventContract(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ActivateEventContract(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteEventContract(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ArchiveEventContract(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def ValidateMaskedFields(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def GetEventContractAndSchema(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_EventContractsServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListEventContracts': grpc.unary_unary_rpc_method_handler(
                     servicer.ListEventContracts,
                     request_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ListEventContractsRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ListEventContractsResponse.SerializeToString,
@@ -93,19 +137,39 @@
                     response_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.CreateEventContractResponse.SerializeToString,
             ),
             'UpdateEventContract': grpc.unary_unary_rpc_method_handler(
                     servicer.UpdateEventContract,
                     request_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.UpdateEventContractRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.UpdateEventContractResponse.SerializeToString,
             ),
+            'ActivateEventContract': grpc.unary_unary_rpc_method_handler(
+                    servicer.ActivateEventContract,
+                    request_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ActivateEventContractRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ActivateEventContractResponse.SerializeToString,
+            ),
+            'DeleteEventContract': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteEventContract,
+                    request_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.DeleteEventContractRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.DeleteEventContractResponse.SerializeToString,
+            ),
+            'ArchiveEventContract': grpc.unary_unary_rpc_method_handler(
+                    servicer.ArchiveEventContract,
+                    request_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ArchiveEventContractRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ArchiveEventContractResponse.SerializeToString,
+            ),
             'ValidateMaskedFields': grpc.unary_unary_rpc_method_handler(
                     servicer.ValidateMaskedFields,
                     request_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ValidateMaskedFieldsRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ValidateMaskedFieldsResponse.SerializeToString,
             ),
+            'GetEventContractAndSchema': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetEventContractAndSchema,
+                    request_deserializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.GetEventContractAndSchemaRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.GetEventContractAndSchemaResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'strmprivacy.api.event_contracts.v1.EventContractsService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -177,14 +241,65 @@
         return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.event_contracts.v1.EventContractsService/UpdateEventContract',
             strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.UpdateEventContractRequest.SerializeToString,
             strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.UpdateEventContractResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ActivateEventContract(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.event_contracts.v1.EventContractsService/ActivateEventContract',
+            strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ActivateEventContractRequest.SerializeToString,
+            strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ActivateEventContractResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteEventContract(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.event_contracts.v1.EventContractsService/DeleteEventContract',
+            strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.DeleteEventContractRequest.SerializeToString,
+            strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.DeleteEventContractResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ArchiveEventContract(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.event_contracts.v1.EventContractsService/ArchiveEventContract',
+            strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ArchiveEventContractRequest.SerializeToString,
+            strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ArchiveEventContractResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def ValidateMaskedFields(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
@@ -192,7 +307,24 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.event_contracts.v1.EventContractsService/ValidateMaskedFields',
             strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ValidateMaskedFieldsRequest.SerializeToString,
             strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.ValidateMaskedFieldsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetEventContractAndSchema(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.event_contracts.v1.EventContractsService/GetEventContractAndSchema',
+            strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.GetEventContractAndSchemaRequest.SerializeToString,
+            strmprivacy_dot_api_dot_event__contracts_dot_v1_dot_event__contracts__v1__pb2.GetEventContractAndSchemaResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,165 +1,165 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from strmprivacy.api.kafka_exporters.v1 import kafka_exporters_v1_pb2 as strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2
+from strmprivacy.api.kafka_users.v1 import kafka_users_v1_pb2 as strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2
 
 
-class KafkaExportersServiceStub(object):
+class KafkaUsersServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.ListKafkaExporters = channel.unary_unary(
-                '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/ListKafkaExporters',
-                request_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersResponse.FromString,
+        self.ListKafkaUsers = channel.unary_unary(
+                '/strmprivacy.api.kafka_users.v1.KafkaUsersService/ListKafkaUsers',
+                request_serializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.ListKafkaUsersRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.ListKafkaUsersResponse.FromString,
                 )
-        self.GetKafkaExporter = channel.unary_unary(
-                '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/GetKafkaExporter',
-                request_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterResponse.FromString,
+        self.GetKafkaUser = channel.unary_unary(
+                '/strmprivacy.api.kafka_users.v1.KafkaUsersService/GetKafkaUser',
+                request_serializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.GetKafkaUserRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.GetKafkaUserResponse.FromString,
                 )
-        self.DeleteKafkaExporter = channel.unary_unary(
-                '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/DeleteKafkaExporter',
-                request_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterResponse.FromString,
+        self.DeleteKafkaUser = channel.unary_unary(
+                '/strmprivacy.api.kafka_users.v1.KafkaUsersService/DeleteKafkaUser',
+                request_serializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.DeleteKafkaUserRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.DeleteKafkaUserResponse.FromString,
                 )
-        self.CreateKafkaExporter = channel.unary_unary(
-                '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/CreateKafkaExporter',
-                request_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterResponse.FromString,
+        self.CreateKafkaUser = channel.unary_unary(
+                '/strmprivacy.api.kafka_users.v1.KafkaUsersService/CreateKafkaUser',
+                request_serializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.CreateKafkaUserRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.CreateKafkaUserResponse.FromString,
                 )
 
 
-class KafkaExportersServiceServicer(object):
+class KafkaUsersServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
-    def ListKafkaExporters(self, request, context):
+    def ListKafkaUsers(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetKafkaExporter(self, request, context):
+    def GetKafkaUser(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def DeleteKafkaExporter(self, request, context):
+    def DeleteKafkaUser(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def CreateKafkaExporter(self, request, context):
+    def CreateKafkaUser(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_KafkaExportersServiceServicer_to_server(servicer, server):
+def add_KafkaUsersServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'ListKafkaExporters': grpc.unary_unary_rpc_method_handler(
-                    servicer.ListKafkaExporters,
-                    request_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersResponse.SerializeToString,
+            'ListKafkaUsers': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListKafkaUsers,
+                    request_deserializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.ListKafkaUsersRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.ListKafkaUsersResponse.SerializeToString,
             ),
-            'GetKafkaExporter': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetKafkaExporter,
-                    request_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterResponse.SerializeToString,
+            'GetKafkaUser': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetKafkaUser,
+                    request_deserializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.GetKafkaUserRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.GetKafkaUserResponse.SerializeToString,
             ),
-            'DeleteKafkaExporter': grpc.unary_unary_rpc_method_handler(
-                    servicer.DeleteKafkaExporter,
-                    request_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterResponse.SerializeToString,
+            'DeleteKafkaUser': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteKafkaUser,
+                    request_deserializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.DeleteKafkaUserRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.DeleteKafkaUserResponse.SerializeToString,
             ),
-            'CreateKafkaExporter': grpc.unary_unary_rpc_method_handler(
-                    servicer.CreateKafkaExporter,
-                    request_deserializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterResponse.SerializeToString,
+            'CreateKafkaUser': grpc.unary_unary_rpc_method_handler(
+                    servicer.CreateKafkaUser,
+                    request_deserializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.CreateKafkaUserRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.CreateKafkaUserResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'strmprivacy.api.kafka_exporters.v1.KafkaExportersService', rpc_method_handlers)
+            'strmprivacy.api.kafka_users.v1.KafkaUsersService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class KafkaExportersService(object):
+class KafkaUsersService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
-    def ListKafkaExporters(request,
+    def ListKafkaUsers(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/ListKafkaExporters',
-            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersRequest.SerializeToString,
-            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.ListKafkaExportersResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_users.v1.KafkaUsersService/ListKafkaUsers',
+            strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.ListKafkaUsersRequest.SerializeToString,
+            strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.ListKafkaUsersResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetKafkaExporter(request,
+    def GetKafkaUser(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/GetKafkaExporter',
-            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterRequest.SerializeToString,
-            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.GetKafkaExporterResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_users.v1.KafkaUsersService/GetKafkaUser',
+            strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.GetKafkaUserRequest.SerializeToString,
+            strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.GetKafkaUserResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def DeleteKafkaExporter(request,
+    def DeleteKafkaUser(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/DeleteKafkaExporter',
-            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterRequest.SerializeToString,
-            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.DeleteKafkaExporterResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_users.v1.KafkaUsersService/DeleteKafkaUser',
+            strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.DeleteKafkaUserRequest.SerializeToString,
+            strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.DeleteKafkaUserResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def CreateKafkaExporter(request,
+    def CreateKafkaUser(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_exporters.v1.KafkaExportersService/CreateKafkaExporter',
-            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterRequest.SerializeToString,
-            strmprivacy_dot_api_dot_kafka__exporters_dot_v1_dot_kafka__exporters__v1__pb2.CreateKafkaExporterResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.kafka_users.v1.KafkaUsersService/CreateKafkaUser',
+            strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.CreateKafkaUserRequest.SerializeToString,
+            strmprivacy_dot_api_dot_kafka__users_dot_v1_dot_kafka__users__v1__pb2.CreateKafkaUserResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py`

 * *Files 25% similar despite different names*

```diff
@@ -35,14 +35,34 @@
                 response_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.UpdateSchemaResponse.FromString,
                 )
         self.GetSchemaCode = channel.unary_unary(
                 '/strmprivacy.api.schemas.v1.SchemasService/GetSchemaCode',
                 request_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaCodeRequest.SerializeToString,
                 response_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaCodeResponse.FromString,
                 )
+        self.ActivateSchema = channel.unary_unary(
+                '/strmprivacy.api.schemas.v1.SchemasService/ActivateSchema',
+                request_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ActivateSchemaRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ActivateSchemaResponse.FromString,
+                )
+        self.DeleteSchema = channel.unary_unary(
+                '/strmprivacy.api.schemas.v1.SchemasService/DeleteSchema',
+                request_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.DeleteSchemaRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.DeleteSchemaResponse.FromString,
+                )
+        self.ArchiveSchema = channel.unary_unary(
+                '/strmprivacy.api.schemas.v1.SchemasService/ArchiveSchema',
+                request_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ArchiveSchemaRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ArchiveSchemaResponse.FromString,
+                )
+        self.GetSchemaDefinition = channel.unary_unary(
+                '/strmprivacy.api.schemas.v1.SchemasService/GetSchemaDefinition',
+                request_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaDefinitionRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaDefinitionResponse.FromString,
+                )
 
 
 class SchemasServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def ListSchemas(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -70,14 +90,38 @@
 
     def GetSchemaCode(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ActivateSchema(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def DeleteSchema(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def ArchiveSchema(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetSchemaDefinition(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_SchemasServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListSchemas': grpc.unary_unary_rpc_method_handler(
                     servicer.ListSchemas,
                     request_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ListSchemasRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ListSchemasResponse.SerializeToString,
@@ -98,14 +142,34 @@
                     response_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.UpdateSchemaResponse.SerializeToString,
             ),
             'GetSchemaCode': grpc.unary_unary_rpc_method_handler(
                     servicer.GetSchemaCode,
                     request_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaCodeRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaCodeResponse.SerializeToString,
             ),
+            'ActivateSchema': grpc.unary_unary_rpc_method_handler(
+                    servicer.ActivateSchema,
+                    request_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ActivateSchemaRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ActivateSchemaResponse.SerializeToString,
+            ),
+            'DeleteSchema': grpc.unary_unary_rpc_method_handler(
+                    servicer.DeleteSchema,
+                    request_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.DeleteSchemaRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.DeleteSchemaResponse.SerializeToString,
+            ),
+            'ArchiveSchema': grpc.unary_unary_rpc_method_handler(
+                    servicer.ArchiveSchema,
+                    request_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ArchiveSchemaRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ArchiveSchemaResponse.SerializeToString,
+            ),
+            'GetSchemaDefinition': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetSchemaDefinition,
+                    request_deserializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaDefinitionRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaDefinitionResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'strmprivacy.api.schemas.v1.SchemasService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -192,7 +256,75 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.schemas.v1.SchemasService/GetSchemaCode',
             strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaCodeRequest.SerializeToString,
             strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaCodeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ActivateSchema(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.schemas.v1.SchemasService/ActivateSchema',
+            strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ActivateSchemaRequest.SerializeToString,
+            strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ActivateSchemaResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def DeleteSchema(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.schemas.v1.SchemasService/DeleteSchema',
+            strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.DeleteSchemaRequest.SerializeToString,
+            strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.DeleteSchemaResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def ArchiveSchema(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.schemas.v1.SchemasService/ArchiveSchema',
+            strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ArchiveSchemaRequest.SerializeToString,
+            strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.ArchiveSchemaResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetSchemaDefinition(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.schemas.v1.SchemasService/GetSchemaDefinition',
+            strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaDefinitionRequest.SerializeToString,
+            strmprivacy_dot_api_dot_schemas_dot_v1_dot_schemas__v1__pb2.GetSchemaDefinitionResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,14 +15,19 @@
             channel: A grpc.Channel.
         """
         self.ListStreams = channel.unary_unary(
                 '/strmprivacy.api.streams.v1.StreamsService/ListStreams',
                 request_serializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListStreamsRequest.SerializeToString,
                 response_deserializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListStreamsResponse.FromString,
                 )
+        self.ListExtendedStreams = channel.unary_unary(
+                '/strmprivacy.api.streams.v1.StreamsService/ListExtendedStreams',
+                request_serializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListExtendedStreamsRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListExtendedStreamsResponse.FromString,
+                )
         self.GetStream = channel.unary_unary(
                 '/strmprivacy.api.streams.v1.StreamsService/GetStream',
                 request_serializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.GetStreamRequest.SerializeToString,
                 response_deserializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.GetStreamResponse.FromString,
                 )
         self.DeleteStream = channel.unary_unary(
                 '/strmprivacy.api.streams.v1.StreamsService/DeleteStream',
@@ -41,14 +46,20 @@
 
     def ListStreams(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListExtendedStreams(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetStream(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def DeleteStream(self, request, context):
@@ -67,14 +78,19 @@
 def add_StreamsServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'ListStreams': grpc.unary_unary_rpc_method_handler(
                     servicer.ListStreams,
                     request_deserializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListStreamsRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListStreamsResponse.SerializeToString,
             ),
+            'ListExtendedStreams': grpc.unary_unary_rpc_method_handler(
+                    servicer.ListExtendedStreams,
+                    request_deserializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListExtendedStreamsRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListExtendedStreamsResponse.SerializeToString,
+            ),
             'GetStream': grpc.unary_unary_rpc_method_handler(
                     servicer.GetStream,
                     request_deserializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.GetStreamRequest.FromString,
                     response_serializer=strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.GetStreamResponse.SerializeToString,
             ),
             'DeleteStream': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteStream,
@@ -110,14 +126,31 @@
         return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.streams.v1.StreamsService/ListStreams',
             strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListStreamsRequest.SerializeToString,
             strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListStreamsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ListExtendedStreams(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.streams.v1.StreamsService/ListExtendedStreams',
+            strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListExtendedStreamsRequest.SerializeToString,
+            strmprivacy_dot_api_dot_streams_dot_v1_dot_streams__v1__pb2.ListExtendedStreamsResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetStream(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,66 +1,72 @@
 # Generated by the gRPC Python protocol compiler plugin. DO NOT EDIT!
 """Client and server classes corresponding to protobuf-defined services."""
 import grpc
 
-from strmprivacy.api.usage.v1 import usage_v1_pb2 as strmprivacy_dot_api_dot_usage_dot_v1_dot_usage__v1__pb2
+from strmprivacy.api.agents.v1 import streams_agent_v1_pb2 as strmprivacy_dot_api_dot_agents_dot_v1_dot_streams__agent__v1__pb2
 
 
-class UsageServiceStub(object):
-    """Missing associated documentation comment in .proto file."""
+class StreamsAgentServiceStub(object):
+    """(-- api-linter: core::0136::prepositions=disabled
+    aip.dev/not-precedent: This is an internal API and the alternative with oneof is good either. --)
+    """
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
-        self.GetStreamEventUsage = channel.unary_unary(
-                '/strmprivacy.api.usage.v1.UsageService/GetStreamEventUsage',
-                request_serializer=strmprivacy_dot_api_dot_usage_dot_v1_dot_usage__v1__pb2.GetStreamEventUsageRequest.SerializeToString,
-                response_deserializer=strmprivacy_dot_api_dot_usage_dot_v1_dot_usage__v1__pb2.GetStreamEventUsageResponse.FromString,
+        self.GetStreams = channel.unary_unary(
+                '/strmprivacy.api.agents.v1.StreamsAgentService/GetStreams',
+                request_serializer=strmprivacy_dot_api_dot_agents_dot_v1_dot_streams__agent__v1__pb2.GetStreamsRequest.SerializeToString,
+                response_deserializer=strmprivacy_dot_api_dot_agents_dot_v1_dot_streams__agent__v1__pb2.GetStreamsResponse.FromString,
                 )
 
 
-class UsageServiceServicer(object):
-    """Missing associated documentation comment in .proto file."""
+class StreamsAgentServiceServicer(object):
+    """(-- api-linter: core::0136::prepositions=disabled
+    aip.dev/not-precedent: This is an internal API and the alternative with oneof is good either. --)
+    """
 
-    def GetStreamEventUsage(self, request, context):
+    def GetStreams(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
-def add_UsageServiceServicer_to_server(servicer, server):
+def add_StreamsAgentServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-            'GetStreamEventUsage': grpc.unary_unary_rpc_method_handler(
-                    servicer.GetStreamEventUsage,
-                    request_deserializer=strmprivacy_dot_api_dot_usage_dot_v1_dot_usage__v1__pb2.GetStreamEventUsageRequest.FromString,
-                    response_serializer=strmprivacy_dot_api_dot_usage_dot_v1_dot_usage__v1__pb2.GetStreamEventUsageResponse.SerializeToString,
+            'GetStreams': grpc.unary_unary_rpc_method_handler(
+                    servicer.GetStreams,
+                    request_deserializer=strmprivacy_dot_api_dot_agents_dot_v1_dot_streams__agent__v1__pb2.GetStreamsRequest.FromString,
+                    response_serializer=strmprivacy_dot_api_dot_agents_dot_v1_dot_streams__agent__v1__pb2.GetStreamsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-            'strmprivacy.api.usage.v1.UsageService', rpc_method_handlers)
+            'strmprivacy.api.agents.v1.StreamsAgentService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
-class UsageService(object):
-    """Missing associated documentation comment in .proto file."""
+class StreamsAgentService(object):
+    """(-- api-linter: core::0136::prepositions=disabled
+    aip.dev/not-precedent: This is an internal API and the alternative with oneof is good either. --)
+    """
 
     @staticmethod
-    def GetStreamEventUsage(request,
+    def GetStreams(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.usage.v1.UsageService/GetStreamEventUsage',
-            strmprivacy_dot_api_dot_usage_dot_v1_dot_usage__v1__pb2.GetStreamEventUsageRequest.SerializeToString,
-            strmprivacy_dot_api_dot_usage_dot_v1_dot_usage__v1__pb2.GetStreamEventUsageResponse.FromString,
+        return grpc.experimental.unary_unary(request, target, '/strmprivacy.api.agents.v1.StreamsAgentService/GetStreams',
+            strmprivacy_dot_api_dot_agents_dot_v1_dot_streams__agent__v1__pb2.GetStreamsRequest.SerializeToString,
+            strmprivacy_dot_api_dot_agents_dot_v1_dot_streams__agent__v1__pb2.GetStreamsResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `strmprivacy-api-definitions-2.9.0/strmprivacy_api_definitions.egg-info/PKG-INFO` & `strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 2.9.0
+Version: 3.0.0
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

