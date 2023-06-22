# Comparing `tmp/strmprivacy-api-definitions-3.0.0.tar.gz` & `tmp/strmprivacy-api-definitions-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strmprivacy-api-definitions-3.0.0.tar", last modified: Thu Jun 22 07:58:18 2023, max compression
+gzip compressed data, was "strmprivacy-api-definitions-3.0.1.tar", last modified: Thu Jun 22 14:05:07 2023, max compression
```

## Comparing `strmprivacy-api-definitions-3.0.0.tar` & `strmprivacy-api-definitions-3.0.1.tar`

### file list

```diff
@@ -1,227 +1,227 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.575838 strmprivacy-api-definitions-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      629 2023-06-22 07:58:18.574838 strmprivacy-api-definitions-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 07:58:18.575838 strmprivacy-api-definitions-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1443 2023-06-22 07:57:41.000000 strmprivacy-api-definitions-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.378821 strmprivacy-api-definitions-3.0.0/strmprivacy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.378821 strmprivacy-api-definitions-3.0.0/strmprivacy/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.378821 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.381821 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12198 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/account_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16789 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.382821 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.387822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2356 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2300 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3129 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2369 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3261 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2161 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3267 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.387822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.390822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3449 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/audit_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5030 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.391822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.393822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5338 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.394822 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.398823 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7665 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10858 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.399823 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.403823 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3799 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/cli_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2753 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.429825 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.550836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3987 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/comments_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6740 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.551836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.552836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5049 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8979 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.552836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.552836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7497 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10288 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.552836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.553836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5978 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.553836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.554836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22863 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28488 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.554836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.555836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9865 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.555836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.556836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81835 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.556836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12164 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.556836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.557836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15658 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    20098 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.557836 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.558837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/handles_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3057 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.558837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.559837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7909 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/entities_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6253 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installations_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9499 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6958 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10345 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.559837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.560837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6199 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9342 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.561837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.561837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5362 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.562837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.562837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5369 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8964 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.562837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.563837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4941 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.563837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.564837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6738 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7722 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.564837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.565837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10605 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13648 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.565837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.565837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.565837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.566837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5842 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9075 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.566837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.567837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1340 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/paging_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.567837 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.568838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5782 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/policies_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10449 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.568838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.568838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4442 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7409 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.568838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.569838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7458 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/projects_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14509 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.569838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.570838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4483 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7407 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.570838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.571838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    17973 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.571838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.571838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5254 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8223 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.572838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.572838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5689 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/streams_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10437 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.572838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.573838 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 07:58:16.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4644 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/usage_v1_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4831 2023-06-22 07:56:56.000000 strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 07:58:18.574838 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/
--rw-r--r--   0 root         (0) root         (0)      629 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7436 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-22 07:58:17.000000 strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.462262 strmprivacy-api-definitions-3.0.1/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-22 14:05:07.462262 strmprivacy-api-definitions-3.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:05:07.462262 strmprivacy-api-definitions-3.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-06-22 14:04:32.000000 strmprivacy-api-definitions-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.417258 strmprivacy-api-definitions-3.0.1/strmprivacy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.417258 strmprivacy-api-definitions-3.0.1/strmprivacy/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.417258 strmprivacy-api-definitions-3.0.1/strmprivacy/api/account/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/account/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.419259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/account/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/account/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12198 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/account/v1/account_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16789 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/account/v1/account_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.419259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.423259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2300 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3129 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2369 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3267 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.424259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.425259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/audit/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/audit/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/audit/v1/audit_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5030 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.425259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.427259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5338 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.427259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_jobs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_jobs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.428259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_jobs/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_jobs/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7665 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10858 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.429259 strmprivacy-api-definitions-3.0.1/strmprivacy/api/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.430260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/cli/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/cli/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3799 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/cli/v1/cli_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2753 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/cli/v1/cli_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.430260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/comments/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/comments/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.431260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/comments/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/comments/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3987 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/comments/v1/comments_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6740 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.431260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/credentials/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/credentials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.432260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/credentials/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/credentials/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5049 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/credentials/v1/credentials_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8979 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.433260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/customer_entity_versions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/customer_entity_versions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.434260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/customer_entity_versions/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/customer_entity_versions/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7497 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10288 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.434260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_connectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_connectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.435260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_connectors/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_connectors/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5978 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.435260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.436260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22863 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28488 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.437260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_subjects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_subjects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.438260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_subjects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_subjects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9865 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.438260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.439260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81835 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1/entities_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.440261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12164 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.440261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/event_contracts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/event_contracts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.441260 strmprivacy-api-definitions-3.0.1/strmprivacy/api/event_contracts/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/event_contracts/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15658 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    20098 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.442261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/handles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/handles/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.443261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/handles/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/handles/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/handles/v1/handles_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3057 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.443261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.445261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7909 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/entities_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/entities_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6253 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/installations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9499 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6958 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/installed_components_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10345 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.445261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_clusters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_clusters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.445261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_clusters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_clusters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6199 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9342 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.446261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_exporters/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_exporters/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.446261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_exporters/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_exporters/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5362 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9468 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.446261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_users/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_users/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.447261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_users/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_users/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5369 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8964 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.447261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/key_streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/key_streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.448261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/key_streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/key_streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/key_streams/v1/key_streams_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.448261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/monitoring/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/monitoring/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.449261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/monitoring/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/monitoring/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6738 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/monitoring/v1/monitoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7722 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.449261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/notifications/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/notifications/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.450261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/notifications/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/notifications/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10605 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/notifications/v1/notifications_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13648 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.450261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/onboarding/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/onboarding/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.450261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/onboarding/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/onboarding/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.451261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/organizations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/organizations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.451261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/organizations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/organizations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5842 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/organizations/v1/organizations_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9075 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.451261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/paging/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/paging/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.452262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/paging/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/paging/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1340 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/paging/v1/paging_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/paging/v1/paging_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.453261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/policies/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.453261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/policies/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/policies/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5782 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/policies/v1/policies_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10449 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.453261 strmprivacy-api-definitions-3.0.1/strmprivacy/api/project_plans/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/project_plans/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.454262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/project_plans/v1alpha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/project_plans/v1alpha/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7409 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.454262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/projects/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/projects/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.455262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/projects/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/projects/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/projects/v1/projects_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14509 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.456262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/purpose_mapping/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/purpose_mapping/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.456262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/purpose_mapping/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/purpose_mapping/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4483 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7407 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.457262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/schemas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.457262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/schemas/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/schemas/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/schemas/v1/schemas_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    17973 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.457262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/sinks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/sinks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.458262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/sinks/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/sinks/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5254 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/sinks/v1/sinks_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8223 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.458262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/streams/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/streams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.459262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/streams/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/streams/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5689 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/streams/v1/streams_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10437 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.459262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/usage/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/usage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.460262 strmprivacy-api-definitions-3.0.1/strmprivacy/api/usage/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 14:05:06.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/usage/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4644 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/usage/v1/usage_v1_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4831 2023-06-22 14:03:48.000000 strmprivacy-api-definitions-3.0.1/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:05:07.461262 strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      629 2023-06-22 14:05:07.000000 strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7436 2023-06-22 14:05:07.000000 strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:05:07.000000 strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:05:07.000000 strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-22 14:05:07.000000 strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-22 14:05:07.000000 strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/top_level.txt
```

### Comparing `strmprivacy-api-definitions-3.0.0/PKG-INFO` & `strmprivacy-api-definitions-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 3.0.0
+Version: 3.0.1
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-3.0.0/setup.py` & `strmprivacy-api-definitions-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/account_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/account/v1/account_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/account/v1/account_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/account/v1/account_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/batch_exporters_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/batch_jobs_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/data_connector_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/streams_agent_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/agents/v1/streams_agent_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/audit_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/audit/v1/audit_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/audit/v1/audit_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_exporters/v1/batch_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/batch_jobs/v1/batch_jobs_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/cli_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/cli/v1/cli_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/cli/v1/cli_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/cli/v1/cli_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/comments_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/comments/v1/comments_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/comments/v1/comments_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/credentials_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/credentials/v1/credentials_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/credentials/v1/credentials_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/customer_entity_versions/v1/customer_entity_versions_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_connectors/v1/data_connectors_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_contracts/v1/data_contracts_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/data_subjects/v1/data_subjects_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1/entities_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1/entities_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/entities/v1alpha/entities_v1alpha_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/event_contracts/v1/event_contracts_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/handles_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/handles/v1/handles_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/handles/v1/handles_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/entities_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/entities_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installations_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/installations_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/installations_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installed_components_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/installed_components_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/installations/v1/installed_components_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_clusters/v1/kafka_clusters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_exporters/v1/kafka_exporters_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/kafka_users/v1/kafka_users_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/key_streams_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/key_streams/v1/key_streams_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/key_streams/v1/key_streams_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/monitoring_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/monitoring/v1/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/monitoring/v1/monitoring_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/notifications_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/notifications/v1/notifications_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/notifications/v1/notifications_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/onboarding/v1/onboarding_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/onboarding/v1/onboarding_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/organizations_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/organizations/v1/organizations_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/organizations/v1/organizations_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/paging/v1/paging_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/paging/v1/paging_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/policies_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/policies/v1/policies_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/policies/v1/policies_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/project_plans/v1alpha/project_plans_v1alpha_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/projects_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/projects/v1/projects_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/projects/v1/projects_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/purpose_mapping/v1/purpose_mapping_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/schemas_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/schemas/v1/schemas_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/schemas/v1/schemas_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/sinks_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/sinks/v1/sinks_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/sinks/v1/sinks_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/streams_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/streams/v1/streams_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/streams/v1/streams_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/usage_v1_pb2.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/usage/v1/usage_v1_pb2.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py` & `strmprivacy-api-definitions-3.0.1/strmprivacy/api/usage/v1/usage_v1_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/PKG-INFO` & `strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strmprivacy-api-definitions
-Version: 3.0.0
+Version: 3.0.1
 Summary: STRM Privacy API definitions
 Home-page: UNKNOWN
 Author: Stream Machine B.V.
 Author-email: apis@strmprivacy.io
 License: UNKNOWN
 Keywords: strmprivacy api definitions
 Platform: UNKNOWN
```

### Comparing `strmprivacy-api-definitions-3.0.0/strmprivacy_api_definitions.egg-info/SOURCES.txt` & `strmprivacy-api-definitions-3.0.1/strmprivacy_api_definitions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

