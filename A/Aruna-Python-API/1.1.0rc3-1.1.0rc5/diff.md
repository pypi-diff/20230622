# Comparing `tmp/Aruna-Python-API-1.1.0rc3.tar.gz` & `tmp/Aruna-Python-API-1.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Aruna-Python-API-1.1.0rc3.tar", last modified: Wed Jun 21 11:10:47 2023, max compression
+gzip compressed data, was "Aruna-Python-API-1.1.0rc5.tar", last modified: Thu Jun 22 18:53:03 2023, max compression
```

## Comparing `Aruna-Python-API-1.1.0rc3.tar` & `Aruna-Python-API-1.1.0rc5.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.694933 Aruna-Python-API-1.1.0rc3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.682932 Aruna-Python-API-1.1.0rc3/Aruna_Python_API.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-21 11:10:47.000000 Aruna-Python-API-1.1.0rc3/Aruna_Python_API.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-21 11:10:47.000000 Aruna-Python-API-1.1.0rc3/Aruna_Python_API.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 11:10:47.000000 Aruna-Python-API-1.1.0rc3/Aruna_Python_API.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-21 11:10:47.000000 Aruna-Python-API-1.1.0rc3/Aruna_Python_API.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 11:10:47.000000 Aruna-Python-API-1.1.0rc3/Aruna_Python_API.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-21 11:10:47.694933 Aruna-Python-API-1.1.0rc3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/api/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/authorize_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/authorize_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/authorize_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/bundler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/bundler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/bundler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/notification_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/notification_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/notification_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/proxy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/proxy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/proxy_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/api/notification/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/notification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/v1/notification_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/v1/notification_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/api/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.686933 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.690933 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/auth_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/auth_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/auth_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14500 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/models_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/models_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/models_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/query_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/query_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/query_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.690933 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:47.694933 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 11:10:26.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/collection_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/collection_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23861 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/endpoint_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/info_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/info_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/info_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31693 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/object_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/object_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    57329 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/object_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/objectgroup_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/project_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/project_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/project_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/service_account_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/service_account_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/user_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/user_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/user_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-21 11:10:47.694933 Aruna-Python-API-1.1.0rc3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-21 11:10:38.000000 Aruna-Python-API-1.1.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.386815 Aruna-Python-API-1.1.0rc5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.378815 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:53:03.000000 Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-22 18:53:03.386815 Aruna-Python-API-1.1.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.378815 Aruna-Python-API-1.1.0rc5/aruna/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.378815 Aruna-Python-API-1.1.0rc5/aruna/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.378815 Aruna-Python-API-1.1.0rc5/aruna/api/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6592 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11854 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/notification/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15269 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21174 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.382815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:53:03.386815 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:52:40.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    26046 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11442 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31693 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25274 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    57329 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12477 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21104 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11519 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22176 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11655 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    22042 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14076 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29274 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 18:53:03.386815 Aruna-Python-API-1.1.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-06-22 18:52:53.000000 Aruna-Python-API-1.1.0rc5/setup.py
```

### Comparing `Aruna-Python-API-1.1.0rc3/Aruna_Python_API.egg-info/PKG-INFO` & `Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc3
+Version: 1.1.0rc5
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc3/Aruna_Python_API.egg-info/SOURCES.txt` & `Aruna-Python-API-1.1.0rc5/Aruna_Python_API.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/LICENSE` & `Aruna-Python-API-1.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/PKG-INFO` & `Aruna-Python-API-1.1.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Aruna-Python-API
-Version: 1.1.0rc3
+Version: 1.1.0rc5
 Summary: Aruna Object Storage Python API builds
 Home-page: https://github.com/ArunaStorage/python-api
 Author: Marius Dieckmann, Jannis Hochmuth
 Author-email: marius.dieckmann@computational.bio.uni-giessen.de, jannis.hochmuth@computational.bio.uni-giessen.de
 License: Apache 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `Aruna-Python-API-1.1.0rc3/README.md` & `Aruna-Python-API-1.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/authorize_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/authorize_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/authorize_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/authorize_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/bundler_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,46 +9,48 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.api import visibility_pb2 as google_dot_api_dot_visibility__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
+from aruna.api.internal.v1 import proxy_pb2 as aruna_dot_api_dot_internal_dot_v1_dot_proxy__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#aruna/api/internal/v1/bundler.proto\x12\x15\x61runa.api.internal.v1\x1a\x1bgoogle/api/visibility.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"3\n\x14PrepareBundleRequest\x12\x1b\n\tbundle_id\x18\x01 \x01(\tR\x08\x62undleId\"\x17\n\x15PrepareBundleResponse\"|\n\tObjectRef\x12\'\n\x0fobject_location\x18\x01 \x01(\tR\x0eobjectLocation\x12%\n\x0e\x65ncryption_key\x18\x02 \x01(\tR\rencryptionKey\x12\x1f\n\x0bobject_path\x18\x03 \x01(\tR\nobjectPath\"\xa3\x01\n\x06\x42undle\x12\x1b\n\tbundle_id\x18\x01 \x01(\tR\x08\x62undleId\x12\x41\n\x0bobject_refs\x18\x02 \x03(\x0b\x32 .aruna.api.internal.v1.ObjectRefR\nobjectRefs\x12\x39\n\nexpires_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\"L\n\x13\x45nableBundleRequest\x12\x35\n\x06\x62undle\x18\x01 \x01(\x0b\x32\x1d.aruna.api.internal.v1.BundleR\x06\x62undle\"\x16\n\x14\x45nableBundleResponse\"\x13\n\x11GetBundlesRequest\"M\n\x12GetBundlesResponse\x12\x37\n\x07\x62undles\x18\x01 \x03(\x0b\x32\x1d.aruna.api.internal.v1.BundleR\x07\x62undles\"6\n\x17InvalidateBundleRequest\x12\x1b\n\tbundle_id\x18\x01 \x01(\tR\x08\x62undleId\"\x1a\n\x18InvalidateBundleResponse2\xfa\x02\n\x16InternalBundlerService\x12l\n\rPrepareBundle\x12+.aruna.api.internal.v1.PrepareBundleRequest\x1a,.aruna.api.internal.v1.PrepareBundleResponse\"\x00\x12i\n\x0c\x45nableBundle\x12*.aruna.api.internal.v1.EnableBundleRequest\x1a+.aruna.api.internal.v1.EnableBundleResponse\"\x00\x12u\n\x10InvalidateBundle\x12..aruna.api.internal.v1.InvalidateBundleRequest\x1a/.aruna.api.internal.v1.InvalidateBundleResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL2\x9a\x01\n!InternalBundlerBackchannelService\x12\x63\n\nGetBundles\x12(.aruna.api.internal.v1.GetBundlesRequest\x1a).aruna.api.internal.v1.GetBundlesResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#aruna/api/internal/v1/bundler.proto\x12\x15\x61runa.api.internal.v1\x1a\x1bgoogle/api/visibility.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a(aruna/api/storage/models/v1/models.proto\x1a!aruna/api/internal/v1/proxy.proto\"3\n\x14PrepareBundleRequest\x12\x1b\n\tbundle_id\x18\x01 \x01(\tR\x08\x62undleId\"\x17\n\x15PrepareBundleResponse\"\xb6\x01\n\tObjectRef\x12H\n\x0fobject_location\x18\x01 \x01(\x0b\x32\x1f.aruna.api.internal.v1.LocationR\x0eobjectLocation\x12\x44\n\x0bobject_info\x18\x02 \x01(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\nobjectInfo\x12\x19\n\x08sub_path\x18\x03 \x01(\tR\x07subPath\"\xa3\x01\n\x06\x42undle\x12\x1b\n\tbundle_id\x18\x01 \x01(\tR\x08\x62undleId\x12\x41\n\x0bobject_refs\x18\x02 \x03(\x0b\x32 .aruna.api.internal.v1.ObjectRefR\nobjectRefs\x12\x39\n\nexpires_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\texpiresAt\"L\n\x13\x45nableBundleRequest\x12\x35\n\x06\x62undle\x18\x01 \x01(\x0b\x32\x1d.aruna.api.internal.v1.BundleR\x06\x62undle\"\x16\n\x14\x45nableBundleResponse\"4\n\x11GetBundlesRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId\"M\n\x12GetBundlesResponse\x12\x37\n\x07\x62undles\x18\x01 \x03(\x0b\x32\x1d.aruna.api.internal.v1.BundleR\x07\x62undles\"6\n\x17InvalidateBundleRequest\x12\x1b\n\tbundle_id\x18\x01 \x01(\tR\x08\x62undleId\"\x1a\n\x18InvalidateBundleResponse2\xfa\x02\n\x16InternalBundlerService\x12l\n\rPrepareBundle\x12+.aruna.api.internal.v1.PrepareBundleRequest\x1a,.aruna.api.internal.v1.PrepareBundleResponse\"\x00\x12i\n\x0c\x45nableBundle\x12*.aruna.api.internal.v1.EnableBundleRequest\x1a+.aruna.api.internal.v1.EnableBundleResponse\"\x00\x12u\n\x10InvalidateBundle\x12..aruna.api.internal.v1.InvalidateBundleRequest\x1a/.aruna.api.internal.v1.InvalidateBundleResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNAL2\x9a\x01\n!InternalBundlerBackchannelService\x12\x63\n\nGetBundles\x12(.aruna.api.internal.v1.GetBundlesRequest\x1a).aruna.api.internal.v1.GetBundlesResponse\"\x00\x1a\x10\xfa\xd2\xe4\x93\x02\n\x12\x08INTERNALB6Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.internal.v1.bundler_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z4github.com/ArunaStorage/go-api/aruna/api/internal/v1'
   _INTERNALBUNDLERSERVICE._options = None
   _INTERNALBUNDLERSERVICE._serialized_options = b'\372\322\344\223\002\n\022\010INTERNAL'
   _INTERNALBUNDLERBACKCHANNELSERVICE._options = None
   _INTERNALBUNDLERBACKCHANNELSERVICE._serialized_options = b'\372\322\344\223\002\n\022\010INTERNAL'
-  _PREPAREBUNDLEREQUEST._serialized_start=124
-  _PREPAREBUNDLEREQUEST._serialized_end=175
-  _PREPAREBUNDLERESPONSE._serialized_start=177
-  _PREPAREBUNDLERESPONSE._serialized_end=200
-  _OBJECTREF._serialized_start=202
-  _OBJECTREF._serialized_end=326
-  _BUNDLE._serialized_start=329
-  _BUNDLE._serialized_end=492
-  _ENABLEBUNDLEREQUEST._serialized_start=494
-  _ENABLEBUNDLEREQUEST._serialized_end=570
-  _ENABLEBUNDLERESPONSE._serialized_start=572
-  _ENABLEBUNDLERESPONSE._serialized_end=594
-  _GETBUNDLESREQUEST._serialized_start=596
-  _GETBUNDLESREQUEST._serialized_end=615
-  _GETBUNDLESRESPONSE._serialized_start=617
-  _GETBUNDLESRESPONSE._serialized_end=694
-  _INVALIDATEBUNDLEREQUEST._serialized_start=696
-  _INVALIDATEBUNDLEREQUEST._serialized_end=750
-  _INVALIDATEBUNDLERESPONSE._serialized_start=752
-  _INVALIDATEBUNDLERESPONSE._serialized_end=778
-  _INTERNALBUNDLERSERVICE._serialized_start=781
-  _INTERNALBUNDLERSERVICE._serialized_end=1159
-  _INTERNALBUNDLERBACKCHANNELSERVICE._serialized_start=1162
-  _INTERNALBUNDLERBACKCHANNELSERVICE._serialized_end=1316
+  _PREPAREBUNDLEREQUEST._serialized_start=201
+  _PREPAREBUNDLEREQUEST._serialized_end=252
+  _PREPAREBUNDLERESPONSE._serialized_start=254
+  _PREPAREBUNDLERESPONSE._serialized_end=277
+  _OBJECTREF._serialized_start=280
+  _OBJECTREF._serialized_end=462
+  _BUNDLE._serialized_start=465
+  _BUNDLE._serialized_end=628
+  _ENABLEBUNDLEREQUEST._serialized_start=630
+  _ENABLEBUNDLEREQUEST._serialized_end=706
+  _ENABLEBUNDLERESPONSE._serialized_start=708
+  _ENABLEBUNDLERESPONSE._serialized_end=730
+  _GETBUNDLESREQUEST._serialized_start=732
+  _GETBUNDLESREQUEST._serialized_end=784
+  _GETBUNDLESRESPONSE._serialized_start=786
+  _GETBUNDLESRESPONSE._serialized_end=863
+  _INVALIDATEBUNDLEREQUEST._serialized_start=865
+  _INVALIDATEBUNDLEREQUEST._serialized_end=919
+  _INVALIDATEBUNDLERESPONSE._serialized_start=921
+  _INVALIDATEBUNDLERESPONSE._serialized_end=947
+  _INTERNALBUNDLERSERVICE._serialized_start=950
+  _INTERNALBUNDLERSERVICE._serialized_end=1328
+  _INTERNALBUNDLERBACKCHANNELSERVICE._serialized_start=1331
+  _INTERNALBUNDLERBACKCHANNELSERVICE._serialized_end=1485
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/bundler_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from google.api import visibility_pb2 as _visibility_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from aruna.api.storage.models.v1 import models_pb2 as _models_pb2
+from aruna.api.internal.v1 import proxy_pb2 as _proxy_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
@@ -24,16 +26,18 @@
     def __init__(self, bundle: _Optional[_Union[Bundle, _Mapping]] = ...) -> None: ...
 
 class EnableBundleResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class GetBundlesRequest(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
+    __slots__ = ["endpoint_id"]
+    ENDPOINT_ID_FIELD_NUMBER: _ClassVar[int]
+    endpoint_id: str
+    def __init__(self, endpoint_id: _Optional[str] = ...) -> None: ...
 
 class GetBundlesResponse(_message.Message):
     __slots__ = ["bundles"]
     BUNDLES_FIELD_NUMBER: _ClassVar[int]
     bundles: _containers.RepeatedCompositeFieldContainer[Bundle]
     def __init__(self, bundles: _Optional[_Iterable[_Union[Bundle, _Mapping]]] = ...) -> None: ...
 
@@ -44,22 +48,22 @@
     def __init__(self, bundle_id: _Optional[str] = ...) -> None: ...
 
 class InvalidateBundleResponse(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class ObjectRef(_message.Message):
-    __slots__ = ["encryption_key", "object_location", "object_path"]
-    ENCRYPTION_KEY_FIELD_NUMBER: _ClassVar[int]
+    __slots__ = ["object_info", "object_location", "sub_path"]
+    OBJECT_INFO_FIELD_NUMBER: _ClassVar[int]
     OBJECT_LOCATION_FIELD_NUMBER: _ClassVar[int]
-    OBJECT_PATH_FIELD_NUMBER: _ClassVar[int]
-    encryption_key: str
-    object_location: str
-    object_path: str
-    def __init__(self, object_location: _Optional[str] = ..., encryption_key: _Optional[str] = ..., object_path: _Optional[str] = ...) -> None: ...
+    SUB_PATH_FIELD_NUMBER: _ClassVar[int]
+    object_info: _models_pb2.Object
+    object_location: _proxy_pb2.Location
+    sub_path: str
+    def __init__(self, object_location: _Optional[_Union[_proxy_pb2.Location, _Mapping]] = ..., object_info: _Optional[_Union[_models_pb2.Object, _Mapping]] = ..., sub_path: _Optional[str] = ...) -> None: ...
 
 class PrepareBundleRequest(_message.Message):
     __slots__ = ["bundle_id"]
     BUNDLE_ID_FIELD_NUMBER: _ClassVar[int]
     bundle_id: str
     def __init__(self, bundle_id: _Optional[str] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/bundler_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/bundler_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/notification_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/notification_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/notification_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/notification_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/proxy_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/proxy_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/internal/v1/proxy_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/internal/v1/proxy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/v1/notification_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/v1/notification_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/notification/services/v1/notification_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/notification/services/v1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/auth_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/auth_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/models_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,38 +10,40 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(aruna/api/storage/models/v1/models.proto\x12\x1b\x61runa.api.storage.models.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"2\n\x08KeyValue\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"?\n\rLabelOntology\x12.\n\x13required_label_keys\x18\x01 \x03(\tR\x11requiredLabelKeys\"8\n\x05Stats\x12\x14\n\x05\x63ount\x18\x01 \x01(\x03R\x05\x63ount\x12\x19\n\x08\x61\x63\x63_size\x18\x02 \x01(\x03R\x07\x61\x63\x63Size\"\xc5\x01\n\x0f\x43ollectionStats\x12\x45\n\x0cobject_stats\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.StatsR\x0bobjectStats\x12,\n\x12object_group_count\x18\x02 \x01(\x03R\x10objectGroupCount\x12=\n\x0clast_updated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"\x98\x01\n\x10ObjectGroupStats\x12\x45\n\x0cobject_stats\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.StatsR\x0bobjectStats\x12=\n\x0clast_updated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"K\n\x07Version\x12\x14\n\x05major\x18\x01 \x01(\x05R\x05major\x12\x14\n\x05minor\x18\x02 \x01(\x05R\x05minor\x12\x14\n\x05patch\x18\x03 \x01(\x05R\x05patch\"X\n\x04Hash\x12<\n\x03\x61lg\x18\x01 \x01(\x0e\x32*.aruna.api.storage.models.v1.HashalgorithmR\x03\x61lg\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\"\x1e\n\x06Origin\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02idJ\x04\x08\x01\x10\x02\"r\n\x06Source\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\x12H\n\x0bsource_type\x18\x02 \x01(\x0e\x32\'.aruna.api.storage.models.v1.SourceTypeR\nsourceType\"\xf6\x02\n\x08\x45ndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x42\n\x07\x65p_type\x18\x02 \x01(\x0e\x32).aruna.api.storage.models.v1.EndpointTypeR\x06\x65pType\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12%\n\x0eproxy_hostname\x18\x04 \x01(\tR\rproxyHostname\x12+\n\x11internal_hostname\x18\x05 \x01(\tR\x10internalHostname\x12-\n\x12\x64ocumentation_path\x18\x06 \x01(\tR\x11\x64ocumentationPath\x12\x1b\n\tis_public\x18\x07 \x01(\x08R\x08isPublic\x12\x1d\n\nis_default\x18\x08 \x01(\x08R\tisDefault\x12\x43\n\x06status\x18\t \x01(\x0e\x32+.aruna.api.storage.models.v1.EndpointStatusR\x06status\"\x9e\x05\n\x06Object\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1a\n\x08\x66ilename\x18\x02 \x01(\tR\x08\x66ilename\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x34\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x1f\n\x0b\x63ontent_len\x18\x07 \x01(\x03R\ncontentLen\x12;\n\x06status\x18\x08 \x01(\x0e\x32#.aruna.api.storage.models.v1.StatusR\x06status\x12;\n\x06origin\x18\t \x01(\x0b\x32#.aruna.api.storage.models.v1.OriginR\x06origin\x12\x45\n\ndata_class\x18\n \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataClass\x12\x39\n\x06hashes\x18\x10 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12\x1d\n\nrev_number\x18\x0c \x01(\x03R\trevNumber\x12;\n\x06source\x18\r \x01(\x0b\x32#.aruna.api.storage.models.v1.SourceR\x06source\x12\x16\n\x06latest\x18\x0e \x01(\x08R\x06latest\x12\x1f\n\x0b\x61uto_update\x18\x0f \x01(\x08R\nautoUpdateJ\x04\x08\x0b\x10\x0c\"H\n\x07Objects\x12=\n\x07objects\x18\x01 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\"\xba\x03\n\x0bObjectGroup\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12=\n\x07objects\x18\x08 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\x12\x46\n\x0cmeta_objects\x18\t \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x0bmetaObjects\x12\x43\n\x05stats\x18\n \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\x0b \x01(\x03R\trevNumber\"]\n\x0cObjectGroups\x12M\n\robject_groups\x18\x01 \x03(\x0b\x32(.aruna.api.storage.models.v1.ObjectGroupR\x0cobjectGroups\"\xbb\x02\n\x13ObjectGroupOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x43\n\x05stats\x18\x08 \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\t \x01(\x03R\trevNumber\"~\n\x14ObjectGroupOverviews\x12\x66\n\x16object_group_overviews\x18\x01 \x03(\x0b\x32\x30.aruna.api.storage.models.v1.ObjectGroupOverviewR\x14objectGroupOverviews\"\x80\x03\n\x11ObjectGroupWithID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x1d\n\nobject_ids\x18\x08 \x03(\tR\tobjectIds\x12&\n\x0fmeta_object_ids\x18\t \x03(\tR\rmetaObjectIds\x12\x43\n\x05stats\x18\n \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\x0b \x01(\x03R\trevNumber\"w\n\x12ObjectGroupWithIDs\x12\x61\n\x15object_group_with_ids\x18\x01 \x03(\x0b\x32..aruna.api.storage.models.v1.ObjectGroupWithIDR\x12objectGroupWithIds\"\x8b\x06\n\nCollection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12=\n\x07objects\x18\x08 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\x12K\n\x0especifications\x18\t \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x0especifications\x12M\n\robject_groups\x18\n \x03(\x0b\x32(.aruna.api.storage.models.v1.ObjectGroupR\x0cobjectGroups\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"X\n\x0b\x43ollections\x12I\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\'.aruna.api.storage.models.v1.CollectionR\x0b\x63ollections\"\xb8\x04\n\x12\x43ollectionOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"y\n\x13\x43ollectionOverviews\x12\x62\n\x14\x63ollection_overviews\x18\x01 \x03(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\x13\x63ollectionOverviews\"\x9d\x05\n\x10\x43ollectionWithID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x18\n\x07objects\x18\x08 \x03(\tR\x07objects\x12&\n\x0especifications\x18\t \x03(\tR\x0especifications\x12#\n\robject_groups\x18\n \x03(\tR\x0cobjectGroups\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"r\n\x11\x43ollectionWithIDs\x12]\n\x13\x63ollection_with_ids\x18\x01 \x03(\x0b\x32-.aruna.api.storage.models.v1.CollectionWithIDR\x11\x63ollectionWithIds*\xb7\x01\n\x0cResourceType\x12\x1d\n\x19RESOURCE_TYPE_UNSPECIFIED\x10\x00\x12\x19\n\x15RESOURCE_TYPE_PROJECT\x10\x01\x12\x1c\n\x18RESOURCE_TYPE_COLLECTION\x10\x02\x12\x1e\n\x1aRESOURCE_TYPE_OBJECT_GROUP\x10\x03\x12\x18\n\x14RESOURCE_TYPE_OBJECT\x10\x04\x12\x15\n\x11RESOURCE_TYPE_ALL\x10\x05*\xbb\x01\n\x0eResourceAction\x12\x1f\n\x1bRESOURCE_ACTION_UNSPECIFIED\x10\x00\x12\x1a\n\x16RESOURCE_ACTION_CREATE\x10\x01\x12\x1a\n\x16RESOURCE_ACTION_APPEND\x10\x02\x12\x1a\n\x16RESOURCE_ACTION_UPDATE\x10\x03\x12\x18\n\x14RESOURCE_ACTION_READ\x10\x04\x12\x1a\n\x16RESOURCE_ACTION_DELETE\x10\x05*\xa2\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x17\n\x13STATUS_INITIALIZING\x10\x01\x12\x14\n\x10STATUS_AVAILABLE\x10\x02\x12\x16\n\x12STATUS_UNAVAILABLE\x10\x03\x12\x10\n\x0cSTATUS_ERROR\x10\x04\x12\x10\n\x0cSTATUS_TRASH\x10\x05\x12\x15\n\x11STATUS_FINALIZING\x10\x06*\xd2\x01\n\x0e\x45ndpointStatus\x12\x1f\n\x1b\x45NDPOINT_STATUS_UNSPECIFIED\x10\x00\x12 \n\x1c\x45NDPOINT_STATUS_INITIALIZING\x10\x01\x12\x1d\n\x19\x45NDPOINT_STATUS_AVAILABLE\x10\x02\x12\x1c\n\x18\x45NDPOINT_STATUS_DEGRADED\x10\x03\x12\x1f\n\x1b\x45NDPOINT_STATUS_UNAVAILABLE\x10\x04\x12\x1f\n\x1b\x45NDPOINT_STATUS_MAINTENANCE\x10\x05*k\n\rHashalgorithm\x12\x1d\n\x19HASHALGORITHM_UNSPECIFIED\x10\x00\x12\x15\n\x11HASHALGORITHM_MD5\x10\x01\x12\x18\n\x14HASHALGORITHM_SHA256\x10\x03\"\x04\x08\x02\x10\x02\"\x04\x08\x04\x10\x07*\x8d\x01\n\tDataClass\x12\x1a\n\x16\x44\x41TA_CLASS_UNSPECIFIED\x10\x00\x12\x15\n\x11\x44\x41TA_CLASS_PUBLIC\x10\x01\x12\x16\n\x12\x44\x41TA_CLASS_PRIVATE\x10\x02\x12\x1b\n\x17\x44\x41TA_CLASS_CONFIDENTIAL\x10\x03\x12\x18\n\x14\x44\x41TA_CLASS_PROTECTED\x10\x04*S\n\nSourceType\x12\x1b\n\x17SOURCE_TYPE_UNSPECIFIED\x10\x00\x12\x13\n\x0fSOURCE_TYPE_URL\x10\x01\x12\x13\n\x0fSOURCE_TYPE_DOI\x10\x02*[\n\x0c\x45ndpointType\x12\x1d\n\x19\x45NDPOINT_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10\x45NDPOINT_TYPE_S3\x10\x01\x12\x16\n\x12\x45NDPOINT_TYPE_FILE\x10\x02\x42<Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(aruna/api/storage/models/v1/models.proto\x12\x1b\x61runa.api.storage.models.v1\x1a\x1fgoogle/protobuf/timestamp.proto\"2\n\x08KeyValue\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"?\n\rLabelOntology\x12.\n\x13required_label_keys\x18\x01 \x03(\tR\x11requiredLabelKeys\"8\n\x05Stats\x12\x14\n\x05\x63ount\x18\x01 \x01(\x03R\x05\x63ount\x12\x19\n\x08\x61\x63\x63_size\x18\x02 \x01(\x03R\x07\x61\x63\x63Size\"\xc5\x01\n\x0f\x43ollectionStats\x12\x45\n\x0cobject_stats\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.StatsR\x0bobjectStats\x12,\n\x12object_group_count\x18\x02 \x01(\x03R\x10objectGroupCount\x12=\n\x0clast_updated\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"\x98\x01\n\x10ObjectGroupStats\x12\x45\n\x0cobject_stats\x18\x01 \x01(\x0b\x32\".aruna.api.storage.models.v1.StatsR\x0bobjectStats\x12=\n\x0clast_updated\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0blastUpdated\"K\n\x07Version\x12\x14\n\x05major\x18\x01 \x01(\x05R\x05major\x12\x14\n\x05minor\x18\x02 \x01(\x05R\x05minor\x12\x14\n\x05patch\x18\x03 \x01(\x05R\x05patch\"X\n\x04Hash\x12<\n\x03\x61lg\x18\x01 \x01(\x0e\x32*.aruna.api.storage.models.v1.HashalgorithmR\x03\x61lg\x12\x12\n\x04hash\x18\x02 \x01(\tR\x04hash\"\x1e\n\x06Origin\x12\x0e\n\x02id\x18\x02 \x01(\tR\x02idJ\x04\x08\x01\x10\x02\"r\n\x06Source\x12\x1e\n\nidentifier\x18\x01 \x01(\tR\nidentifier\x12H\n\x0bsource_type\x18\x02 \x01(\x0e\x32\'.aruna.api.storage.models.v1.SourceTypeR\nsourceType\"\xbb\x01\n\x12\x45ndpointHostConfig\x12\x10\n\x03url\x18\x01 \x01(\tR\x03url\x12\x1d\n\nis_primary\x18\x02 \x01(\x08R\tisPrimary\x12\x10\n\x03ssl\x18\x03 \x01(\x08R\x03ssl\x12\x16\n\x06public\x18\x04 \x01(\x08R\x06public\x12J\n\thost_type\x18\x05 \x01(\x0e\x32-.aruna.api.storage.models.v1.EndpointHostTypeR\x08hostType\"\x95\x03\n\x08\x45ndpoint\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x42\n\x07\x65p_type\x18\x02 \x01(\x0e\x32).aruna.api.storage.models.v1.EndpointTypeR\x06\x65pType\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12-\n\x12\x64ocumentation_path\x18\x06 \x01(\tR\x11\x64ocumentationPath\x12\x1b\n\tis_public\x18\x07 \x01(\x08R\x08isPublic\x12\x1d\n\nis_default\x18\x08 \x01(\x08R\tisDefault\x12\x43\n\x06status\x18\t \x01(\x0e\x32+.aruna.api.storage.models.v1.EndpointStatusR\x06status\x12\x1d\n\nis_bundler\x18\n \x01(\x08R\tisBundler\x12R\n\x0chost_configs\x18\x0b \x03(\x0b\x32/.aruna.api.storage.models.v1.EndpointHostConfigR\x0bhostConfigs\"\x9e\x05\n\x06Object\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1a\n\x08\x66ilename\x18\x02 \x01(\tR\x08\x66ilename\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x34\n\x07\x63reated\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x1f\n\x0b\x63ontent_len\x18\x07 \x01(\x03R\ncontentLen\x12;\n\x06status\x18\x08 \x01(\x0e\x32#.aruna.api.storage.models.v1.StatusR\x06status\x12;\n\x06origin\x18\t \x01(\x0b\x32#.aruna.api.storage.models.v1.OriginR\x06origin\x12\x45\n\ndata_class\x18\n \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataClass\x12\x39\n\x06hashes\x18\x10 \x03(\x0b\x32!.aruna.api.storage.models.v1.HashR\x06hashes\x12\x1d\n\nrev_number\x18\x0c \x01(\x03R\trevNumber\x12;\n\x06source\x18\r \x01(\x0b\x32#.aruna.api.storage.models.v1.SourceR\x06source\x12\x16\n\x06latest\x18\x0e \x01(\x08R\x06latest\x12\x1f\n\x0b\x61uto_update\x18\x0f \x01(\x08R\nautoUpdateJ\x04\x08\x0b\x10\x0c\"H\n\x07Objects\x12=\n\x07objects\x18\x01 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\"\xba\x03\n\x0bObjectGroup\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12=\n\x07objects\x18\x08 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\x12\x46\n\x0cmeta_objects\x18\t \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x0bmetaObjects\x12\x43\n\x05stats\x18\n \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\x0b \x01(\x03R\trevNumber\"]\n\x0cObjectGroups\x12M\n\robject_groups\x18\x01 \x03(\x0b\x32(.aruna.api.storage.models.v1.ObjectGroupR\x0cobjectGroups\"\xbb\x02\n\x13ObjectGroupOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x43\n\x05stats\x18\x08 \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\t \x01(\x03R\trevNumber\"~\n\x14ObjectGroupOverviews\x12\x66\n\x16object_group_overviews\x18\x01 \x03(\x0b\x32\x30.aruna.api.storage.models.v1.ObjectGroupOverviewR\x14objectGroupOverviews\"\x80\x03\n\x11ObjectGroupWithID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x07 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12\x1d\n\nobject_ids\x18\x08 \x03(\tR\tobjectIds\x12&\n\x0fmeta_object_ids\x18\t \x03(\tR\rmetaObjectIds\x12\x43\n\x05stats\x18\n \x01(\x0b\x32-.aruna.api.storage.models.v1.ObjectGroupStatsR\x05stats\x12\x1d\n\nrev_number\x18\x0b \x01(\x03R\trevNumber\"w\n\x12ObjectGroupWithIDs\x12\x61\n\x15object_group_with_ids\x18\x01 \x03(\x0b\x32..aruna.api.storage.models.v1.ObjectGroupWithIDR\x12objectGroupWithIds\"\x8b\x06\n\nCollection\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12=\n\x07objects\x18\x08 \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x07objects\x12K\n\x0especifications\x18\t \x03(\x0b\x32#.aruna.api.storage.models.v1.ObjectR\x0especifications\x12M\n\robject_groups\x18\n \x03(\x0b\x32(.aruna.api.storage.models.v1.ObjectGroupR\x0cobjectGroups\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"X\n\x0b\x43ollections\x12I\n\x0b\x63ollections\x18\x01 \x03(\x0b\x32\'.aruna.api.storage.models.v1.CollectionR\x0b\x63ollections\"\xb8\x04\n\x12\x43ollectionOverview\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"y\n\x13\x43ollectionOverviews\x12\x62\n\x14\x63ollection_overviews\x18\x01 \x03(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\x13\x63ollectionOverviews\"\x9d\x05\n\x10\x43ollectionWithID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x34\n\x07\x63reated\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x63reated\x12\x18\n\x07objects\x18\x08 \x03(\tR\x07objects\x12&\n\x0especifications\x18\t \x03(\tR\x0especifications\x12#\n\robject_groups\x18\n \x03(\tR\x0cobjectGroups\x12Q\n\x10semantic_version\x18\x0c \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionH\x00R\x0fsemanticVersion\x12\x18\n\x06latest\x18\r \x01(\x08H\x00R\x06latest\x12\x42\n\x05stats\x18\x0e \x01(\x0b\x32,.aruna.api.storage.models.v1.CollectionStatsR\x05stats\x12\x1b\n\tis_public\x18\x0f \x01(\x08R\x08isPublicB\t\n\x07version\"r\n\x11\x43ollectionWithIDs\x12]\n\x13\x63ollection_with_ids\x18\x01 \x03(\x0b\x32-.aruna.api.storage.models.v1.CollectionWithIDR\x11\x63ollectionWithIds*\xb7\x01\n\x0cResourceType\x12\x1d\n\x19RESOURCE_TYPE_UNSPECIFIED\x10\x00\x12\x19\n\x15RESOURCE_TYPE_PROJECT\x10\x01\x12\x1c\n\x18RESOURCE_TYPE_COLLECTION\x10\x02\x12\x1e\n\x1aRESOURCE_TYPE_OBJECT_GROUP\x10\x03\x12\x18\n\x14RESOURCE_TYPE_OBJECT\x10\x04\x12\x15\n\x11RESOURCE_TYPE_ALL\x10\x05*\xbb\x01\n\x0eResourceAction\x12\x1f\n\x1bRESOURCE_ACTION_UNSPECIFIED\x10\x00\x12\x1a\n\x16RESOURCE_ACTION_CREATE\x10\x01\x12\x1a\n\x16RESOURCE_ACTION_APPEND\x10\x02\x12\x1a\n\x16RESOURCE_ACTION_UPDATE\x10\x03\x12\x18\n\x14RESOURCE_ACTION_READ\x10\x04\x12\x1a\n\x16RESOURCE_ACTION_DELETE\x10\x05*\xa2\x01\n\x06Status\x12\x16\n\x12STATUS_UNSPECIFIED\x10\x00\x12\x17\n\x13STATUS_INITIALIZING\x10\x01\x12\x14\n\x10STATUS_AVAILABLE\x10\x02\x12\x16\n\x12STATUS_UNAVAILABLE\x10\x03\x12\x10\n\x0cSTATUS_ERROR\x10\x04\x12\x10\n\x0cSTATUS_TRASH\x10\x05\x12\x15\n\x11STATUS_FINALIZING\x10\x06*\xd2\x01\n\x0e\x45ndpointStatus\x12\x1f\n\x1b\x45NDPOINT_STATUS_UNSPECIFIED\x10\x00\x12 \n\x1c\x45NDPOINT_STATUS_INITIALIZING\x10\x01\x12\x1d\n\x19\x45NDPOINT_STATUS_AVAILABLE\x10\x02\x12\x1c\n\x18\x45NDPOINT_STATUS_DEGRADED\x10\x03\x12\x1f\n\x1b\x45NDPOINT_STATUS_UNAVAILABLE\x10\x04\x12\x1f\n\x1b\x45NDPOINT_STATUS_MAINTENANCE\x10\x05*k\n\rHashalgorithm\x12\x1d\n\x19HASHALGORITHM_UNSPECIFIED\x10\x00\x12\x15\n\x11HASHALGORITHM_MD5\x10\x01\x12\x18\n\x14HASHALGORITHM_SHA256\x10\x03\"\x04\x08\x02\x10\x02\"\x04\x08\x04\x10\x07*\x8d\x01\n\tDataClass\x12\x1a\n\x16\x44\x41TA_CLASS_UNSPECIFIED\x10\x00\x12\x15\n\x11\x44\x41TA_CLASS_PUBLIC\x10\x01\x12\x16\n\x12\x44\x41TA_CLASS_PRIVATE\x10\x02\x12\x1b\n\x17\x44\x41TA_CLASS_CONFIDENTIAL\x10\x03\x12\x18\n\x14\x44\x41TA_CLASS_PROTECTED\x10\x04*S\n\nSourceType\x12\x1b\n\x17SOURCE_TYPE_UNSPECIFIED\x10\x00\x12\x13\n\x0fSOURCE_TYPE_URL\x10\x01\x12\x13\n\x0fSOURCE_TYPE_DOI\x10\x02*[\n\x0c\x45ndpointType\x12\x1d\n\x19\x45NDPOINT_TYPE_UNSPECIFIED\x10\x00\x12\x14\n\x10\x45NDPOINT_TYPE_S3\x10\x01\x12\x16\n\x12\x45NDPOINT_TYPE_FILE\x10\x02*\x95\x01\n\x10\x45ndpointHostType\x12\"\n\x1e\x45NDPOINT_HOST_TYPE_UNSPECIFIED\x10\x00\x12\x1c\n\x18\x45NDPOINT_HOST_TYPE_PROXY\x10\x01\x12\x1f\n\x1b\x45NDPOINT_HOST_TYPE_INTERNAL\x10\x02\x12\x1e\n\x1a\x45NDPOINT_HOST_TYPE_BUNDLER\x10\x03\x42<Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.models.v1.models_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z:github.com/ArunaStorage/go-api/aruna/api/storage/models/v1'
-  _RESOURCETYPE._serialized_start=5924
-  _RESOURCETYPE._serialized_end=6107
-  _RESOURCEACTION._serialized_start=6110
-  _RESOURCEACTION._serialized_end=6297
-  _STATUS._serialized_start=6300
-  _STATUS._serialized_end=6462
-  _ENDPOINTSTATUS._serialized_start=6465
-  _ENDPOINTSTATUS._serialized_end=6675
-  _HASHALGORITHM._serialized_start=6677
-  _HASHALGORITHM._serialized_end=6784
-  _DATACLASS._serialized_start=6787
-  _DATACLASS._serialized_end=6928
-  _SOURCETYPE._serialized_start=6930
-  _SOURCETYPE._serialized_end=7013
-  _ENDPOINTTYPE._serialized_start=7015
-  _ENDPOINTTYPE._serialized_end=7106
+  _RESOURCETYPE._serialized_start=6145
+  _RESOURCETYPE._serialized_end=6328
+  _RESOURCEACTION._serialized_start=6331
+  _RESOURCEACTION._serialized_end=6518
+  _STATUS._serialized_start=6521
+  _STATUS._serialized_end=6683
+  _ENDPOINTSTATUS._serialized_start=6686
+  _ENDPOINTSTATUS._serialized_end=6896
+  _HASHALGORITHM._serialized_start=6898
+  _HASHALGORITHM._serialized_end=7005
+  _DATACLASS._serialized_start=7008
+  _DATACLASS._serialized_end=7149
+  _SOURCETYPE._serialized_start=7151
+  _SOURCETYPE._serialized_end=7234
+  _ENDPOINTTYPE._serialized_start=7236
+  _ENDPOINTTYPE._serialized_end=7327
+  _ENDPOINTHOSTTYPE._serialized_start=7330
+  _ENDPOINTHOSTTYPE._serialized_end=7479
   _KEYVALUE._serialized_start=106
   _KEYVALUE._serialized_end=156
   _LABELONTOLOGY._serialized_start=158
   _LABELONTOLOGY._serialized_end=221
   _STATS._serialized_start=223
   _STATS._serialized_end=279
   _COLLECTIONSTATS._serialized_start=282
@@ -52,38 +54,40 @@
   _VERSION._serialized_end=711
   _HASH._serialized_start=713
   _HASH._serialized_end=801
   _ORIGIN._serialized_start=803
   _ORIGIN._serialized_end=833
   _SOURCE._serialized_start=835
   _SOURCE._serialized_end=949
-  _ENDPOINT._serialized_start=952
-  _ENDPOINT._serialized_end=1326
-  _OBJECT._serialized_start=1329
-  _OBJECT._serialized_end=1999
-  _OBJECTS._serialized_start=2001
-  _OBJECTS._serialized_end=2073
-  _OBJECTGROUP._serialized_start=2076
-  _OBJECTGROUP._serialized_end=2518
-  _OBJECTGROUPS._serialized_start=2520
-  _OBJECTGROUPS._serialized_end=2613
-  _OBJECTGROUPOVERVIEW._serialized_start=2616
-  _OBJECTGROUPOVERVIEW._serialized_end=2931
-  _OBJECTGROUPOVERVIEWS._serialized_start=2933
-  _OBJECTGROUPOVERVIEWS._serialized_end=3059
-  _OBJECTGROUPWITHID._serialized_start=3062
-  _OBJECTGROUPWITHID._serialized_end=3446
-  _OBJECTGROUPWITHIDS._serialized_start=3448
-  _OBJECTGROUPWITHIDS._serialized_end=3567
-  _COLLECTION._serialized_start=3570
-  _COLLECTION._serialized_end=4349
-  _COLLECTIONS._serialized_start=4351
-  _COLLECTIONS._serialized_end=4439
-  _COLLECTIONOVERVIEW._serialized_start=4442
-  _COLLECTIONOVERVIEW._serialized_end=5010
-  _COLLECTIONOVERVIEWS._serialized_start=5012
-  _COLLECTIONOVERVIEWS._serialized_end=5133
-  _COLLECTIONWITHID._serialized_start=5136
-  _COLLECTIONWITHID._serialized_end=5805
-  _COLLECTIONWITHIDS._serialized_start=5807
-  _COLLECTIONWITHIDS._serialized_end=5921
+  _ENDPOINTHOSTCONFIG._serialized_start=952
+  _ENDPOINTHOSTCONFIG._serialized_end=1139
+  _ENDPOINT._serialized_start=1142
+  _ENDPOINT._serialized_end=1547
+  _OBJECT._serialized_start=1550
+  _OBJECT._serialized_end=2220
+  _OBJECTS._serialized_start=2222
+  _OBJECTS._serialized_end=2294
+  _OBJECTGROUP._serialized_start=2297
+  _OBJECTGROUP._serialized_end=2739
+  _OBJECTGROUPS._serialized_start=2741
+  _OBJECTGROUPS._serialized_end=2834
+  _OBJECTGROUPOVERVIEW._serialized_start=2837
+  _OBJECTGROUPOVERVIEW._serialized_end=3152
+  _OBJECTGROUPOVERVIEWS._serialized_start=3154
+  _OBJECTGROUPOVERVIEWS._serialized_end=3280
+  _OBJECTGROUPWITHID._serialized_start=3283
+  _OBJECTGROUPWITHID._serialized_end=3667
+  _OBJECTGROUPWITHIDS._serialized_start=3669
+  _OBJECTGROUPWITHIDS._serialized_end=3788
+  _COLLECTION._serialized_start=3791
+  _COLLECTION._serialized_end=4570
+  _COLLECTIONS._serialized_start=4572
+  _COLLECTIONS._serialized_end=4660
+  _COLLECTIONOVERVIEW._serialized_start=4663
+  _COLLECTIONOVERVIEW._serialized_end=5231
+  _COLLECTIONOVERVIEWS._serialized_start=5233
+  _COLLECTIONOVERVIEWS._serialized_end=5354
+  _COLLECTIONWITHID._serialized_start=5357
+  _COLLECTIONWITHID._serialized_end=6026
+  _COLLECTIONWITHIDS._serialized_start=6028
+  _COLLECTIONWITHIDS._serialized_end=6142
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/models_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/models_pb2.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -7,14 +7,18 @@
 
 DATA_CLASS_CONFIDENTIAL: DataClass
 DATA_CLASS_PRIVATE: DataClass
 DATA_CLASS_PROTECTED: DataClass
 DATA_CLASS_PUBLIC: DataClass
 DATA_CLASS_UNSPECIFIED: DataClass
 DESCRIPTOR: _descriptor.FileDescriptor
+ENDPOINT_HOST_TYPE_BUNDLER: EndpointHostType
+ENDPOINT_HOST_TYPE_INTERNAL: EndpointHostType
+ENDPOINT_HOST_TYPE_PROXY: EndpointHostType
+ENDPOINT_HOST_TYPE_UNSPECIFIED: EndpointHostType
 ENDPOINT_STATUS_AVAILABLE: EndpointStatus
 ENDPOINT_STATUS_DEGRADED: EndpointStatus
 ENDPOINT_STATUS_INITIALIZING: EndpointStatus
 ENDPOINT_STATUS_MAINTENANCE: EndpointStatus
 ENDPOINT_STATUS_UNAVAILABLE: EndpointStatus
 ENDPOINT_STATUS_UNSPECIFIED: EndpointStatus
 ENDPOINT_TYPE_FILE: EndpointType
@@ -161,34 +165,48 @@
 class Collections(_message.Message):
     __slots__ = ["collections"]
     COLLECTIONS_FIELD_NUMBER: _ClassVar[int]
     collections: _containers.RepeatedCompositeFieldContainer[Collection]
     def __init__(self, collections: _Optional[_Iterable[_Union[Collection, _Mapping]]] = ...) -> None: ...
 
 class Endpoint(_message.Message):
-    __slots__ = ["documentation_path", "ep_type", "id", "internal_hostname", "is_default", "is_public", "name", "proxy_hostname", "status"]
+    __slots__ = ["documentation_path", "ep_type", "host_configs", "id", "is_bundler", "is_default", "is_public", "name", "status"]
     DOCUMENTATION_PATH_FIELD_NUMBER: _ClassVar[int]
     EP_TYPE_FIELD_NUMBER: _ClassVar[int]
+    HOST_CONFIGS_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
-    INTERNAL_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
+    IS_BUNDLER_FIELD_NUMBER: _ClassVar[int]
     IS_DEFAULT_FIELD_NUMBER: _ClassVar[int]
     IS_PUBLIC_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    PROXY_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     documentation_path: str
     ep_type: EndpointType
+    host_configs: _containers.RepeatedCompositeFieldContainer[EndpointHostConfig]
     id: str
-    internal_hostname: str
+    is_bundler: bool
     is_default: bool
     is_public: bool
     name: str
-    proxy_hostname: str
     status: EndpointStatus
-    def __init__(self, id: _Optional[str] = ..., ep_type: _Optional[_Union[EndpointType, str]] = ..., name: _Optional[str] = ..., proxy_hostname: _Optional[str] = ..., internal_hostname: _Optional[str] = ..., documentation_path: _Optional[str] = ..., is_public: bool = ..., is_default: bool = ..., status: _Optional[_Union[EndpointStatus, str]] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., ep_type: _Optional[_Union[EndpointType, str]] = ..., name: _Optional[str] = ..., documentation_path: _Optional[str] = ..., is_public: bool = ..., is_default: bool = ..., status: _Optional[_Union[EndpointStatus, str]] = ..., is_bundler: bool = ..., host_configs: _Optional[_Iterable[_Union[EndpointHostConfig, _Mapping]]] = ...) -> None: ...
+
+class EndpointHostConfig(_message.Message):
+    __slots__ = ["host_type", "is_primary", "public", "ssl", "url"]
+    HOST_TYPE_FIELD_NUMBER: _ClassVar[int]
+    IS_PRIMARY_FIELD_NUMBER: _ClassVar[int]
+    PUBLIC_FIELD_NUMBER: _ClassVar[int]
+    SSL_FIELD_NUMBER: _ClassVar[int]
+    URL_FIELD_NUMBER: _ClassVar[int]
+    host_type: EndpointHostType
+    is_primary: bool
+    public: bool
+    ssl: bool
+    url: str
+    def __init__(self, url: _Optional[str] = ..., is_primary: bool = ..., ssl: bool = ..., public: bool = ..., host_type: _Optional[_Union[EndpointHostType, str]] = ...) -> None: ...
 
 class Hash(_message.Message):
     __slots__ = ["alg", "hash"]
     ALG_FIELD_NUMBER: _ClassVar[int]
     HASH_FIELD_NUMBER: _ClassVar[int]
     alg: Hashalgorithm
     hash: str
@@ -385,7 +403,10 @@
     __slots__ = []
 
 class SourceType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
 
 class EndpointType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
     __slots__ = []
+
+class EndpointHostType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+    __slots__ = []
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/query_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/models/v1/query_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/models/v1/query_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/collection_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
 from aruna.api.storage.models.v1 import query_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_query__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n6aruna/api/storage/services/v1/collection_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\'aruna/api/storage/models/v1/query.proto\x1a\x1cgoogle/api/annotations.proto\";\n\x16\x43reateWorkspaceRequest\x12!\n\x0cproject_name\x18\x01 \x01(\tR\x0bprojectName\"\x90\x01\n\x17\x43reateWorkspaceResponse\x12!\n\x0cworkspace_id\x18\x01 \x01(\tR\x0bworkspaceId\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\x12\x1d\n\naccess_key\x18\x03 \x01(\tR\taccessKey\x12\x1d\n\nsecret_key\x18\x04 \x01(\tR\tsecretKey\";\n\x16\x44\x65leteWorkspaceRequest\x12!\n\x0cworkspace_id\x18\x01 \x01(\tR\x0bworkspaceId\"\x19\n\x17\x44\x65leteWorkspaceResponse\"P\n\x15\x43laimWorkspaceRequest\x12!\n\x0cworkspace_id\x18\x01 \x01(\tR\x0bworkspaceId\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\x18\n\x16\x43laimWorkspaceResponse\"b\n\x18MoveWorkspaceDataRequest\x12!\n\x0cworkspace_id\x18\x01 \x01(\tR\x0bworkspaceId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\"\x1b\n\x19MoveWorkspaceDataResponse\"\x86\x03\n\x1a\x43reateNewCollectionRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\nproject_id\x18\x03 \x01(\tR\tprojectId\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x44\n\tdataclass\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\"B\n\x1b\x43reateNewCollectionResponse\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\"?\n\x18GetCollectionByIDRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\"l\n\x19GetCollectionByIDResponse\x12O\n\ncollection\x18\x01 \x01(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\ncollection\"\xdd\x01\n\x15GetCollectionsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12X\n\x12label_or_id_filter\x18\x02 \x01(\x0b\x32+.aruna.api.storage.models.v1.LabelOrIDQueryR\x0flabelOrIdFilter\x12K\n\x0cpage_request\x18\x03 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\"l\n\x16GetCollectionsResponse\x12R\n\x0b\x63ollections\x18\x01 \x01(\x0b\x32\x30.aruna.api.storage.models.v1.CollectionOverviewsR\x0b\x63ollections\"\xc9\x03\n\x17UpdateCollectionRequest\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x04 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x07 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x44\n\tdataclass\x18\x08 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12>\n\x07version\x18\t \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionR\x07version\"k\n\x18UpdateCollectionResponse\x12O\n\ncollection\x18\x01 \x01(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\ncollection\"\x82\x01\n\x1bPinCollectionVersionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12>\n\x07version\x18\x02 \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionR\x07version\"o\n\x1cPinCollectionVersionResponse\x12O\n\ncollection\x18\x01 \x01(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\ncollection\"T\n\x17\x44\x65leteCollectionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x14\n\x05\x66orce\x18\x03 \x01(\x08R\x05\x66orce\"\x1a\n\x18\x44\x65leteCollectionResponse2\xb7\x08\n\x11\x43ollectionService\x12\xa7\x01\n\x13\x43reateNewCollection\x12\x39.aruna.api.storage.services.v1.CreateNewCollectionRequest\x1a:.aruna.api.storage.services.v1.CreateNewCollectionResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/v1/collection\x12\xae\x01\n\x11GetCollectionByID\x12\x37.aruna.api.storage.services.v1.GetCollectionByIDRequest\x1a\x38.aruna.api.storage.services.v1.GetCollectionByIDResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v1/collection/{collection_id}\x12\xa3\x01\n\x0eGetCollections\x12\x34.aruna.api.storage.services.v1.GetCollectionsRequest\x1a\x35.aruna.api.storage.services.v1.GetCollectionsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/collections/{project_id}\x12\xae\x01\n\x10UpdateCollection\x12\x36.aruna.api.storage.services.v1.UpdateCollectionRequest\x1a\x37.aruna.api.storage.services.v1.UpdateCollectionResponse\")\x82\xd3\xe4\x93\x02#:\x01*\x1a\x1e/v1/collection/{collection_id}\x12\xbe\x01\n\x14PinCollectionVersion\x12:.aruna.api.storage.services.v1.PinCollectionVersionRequest\x1a;.aruna.api.storage.services.v1.PinCollectionVersionResponse\"-\x82\xd3\xe4\x93\x02\':\x01*\"\"/v1/collection/{collection_id}/pin\x12\xae\x01\n\x10\x44\x65leteCollection\x12\x36.aruna.api.storage.services.v1.DeleteCollectionRequest\x1a\x37.aruna.api.storage.services.v1.DeleteCollectionResponse\")\x82\xd3\xe4\x93\x02#:\x01**\x1e/v1/collection/{collection_id}2\xd1\x05\n\x10WorkspaceService\x12\x9a\x01\n\x0f\x43reateWorkspace\x12\x35.aruna.api.storage.services.v1.CreateWorkspaceRequest\x1a\x36.aruna.api.storage.services.v1.CreateWorkspaceResponse\"\x18\x82\xd3\xe4\x93\x02\x12:\x01*\"\r/v1/workspace\x12\xa9\x01\n\x0f\x44\x65leteWorkspace\x12\x35.aruna.api.storage.services.v1.DeleteWorkspaceRequest\x1a\x36.aruna.api.storage.services.v1.DeleteWorkspaceResponse\"\'\x82\xd3\xe4\x93\x02!:\x01**\x1c/v1/workspace/{workspace_id}\x12\xac\x01\n\x0e\x43laimWorkspace\x12\x34.aruna.api.storage.services.v1.ClaimWorkspaceRequest\x1a\x35.aruna.api.storage.services.v1.ClaimWorkspaceResponse\"-\x82\xd3\xe4\x93\x02\':\x01*\"\"/v1/workspace/{workspace_id}/claim\x12\xc4\x01\n\x11MoveWorkspaceData\x12\x37.aruna.api.storage.services.v1.MoveWorkspaceDataRequest\x1a\x38.aruna.api.storage.services.v1.MoveWorkspaceDataResponse\"<\x82\xd3\xe4\x93\x02\x36:\x01*\"1/v1/workspace/{workspace_id}/move/{collection_id}B\x93\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x11\x43ollectionServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n6aruna/api/storage/services/v1/collection_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\'aruna/api/storage/models/v1/query.proto\x1a\x1cgoogle/api/annotations.proto\";\n\x16\x43reateWorkspaceRequest\x12!\n\x0cproject_name\x18\x01 \x01(\tR\x0bprojectName\"\x90\x01\n\x17\x43reateWorkspaceResponse\x12!\n\x0cworkspace_id\x18\x01 \x01(\tR\x0bworkspaceId\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\x12\x1d\n\naccess_key\x18\x03 \x01(\tR\taccessKey\x12\x1d\n\nsecret_key\x18\x04 \x01(\tR\tsecretKey\";\n\x16\x44\x65leteWorkspaceRequest\x12!\n\x0cworkspace_id\x18\x01 \x01(\tR\x0bworkspaceId\"\x19\n\x17\x44\x65leteWorkspaceResponse\"P\n\x15\x43laimWorkspaceRequest\x12!\n\x0cworkspace_id\x18\x01 \x01(\tR\x0bworkspaceId\x12\x14\n\x05token\x18\x02 \x01(\tR\x05token\"\x18\n\x16\x43laimWorkspaceResponse\"b\n\x18MoveWorkspaceDataRequest\x12!\n\x0cworkspace_id\x18\x01 \x01(\tR\x0bworkspaceId\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\"\x1b\n\x19MoveWorkspaceDataResponse\"\x86\x03\n\x1a\x43reateNewCollectionRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\nproject_id\x18\x03 \x01(\tR\tprojectId\x12=\n\x06labels\x18\x04 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x06 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x44\n\tdataclass\x18\x07 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\"B\n\x1b\x43reateNewCollectionResponse\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\"?\n\x18GetCollectionByIDRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\"l\n\x19GetCollectionByIDResponse\x12O\n\ncollection\x18\x01 \x01(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\ncollection\"\xdd\x01\n\x15GetCollectionsRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12X\n\x12label_or_id_filter\x18\x02 \x01(\x0b\x32+.aruna.api.storage.models.v1.LabelOrIDQueryR\x0flabelOrIdFilter\x12K\n\x0cpage_request\x18\x03 \x01(\x0b\x32(.aruna.api.storage.models.v1.PageRequestR\x0bpageRequest\"l\n\x16GetCollectionsResponse\x12R\n\x0b\x63ollections\x18\x01 \x01(\x0b\x32\x30.aruna.api.storage.models.v1.CollectionOverviewsR\x0b\x63ollections\"\xc9\x03\n\x17UpdateCollectionRequest\x12#\n\rcollection_id\x18\x02 \x01(\tR\x0c\x63ollectionId\x12\x12\n\x04name\x18\x03 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x04 \x01(\tR\x0b\x64\x65scription\x12=\n\x06labels\x18\x05 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x06 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\x12Q\n\x0elabel_ontology\x18\x07 \x01(\x0b\x32*.aruna.api.storage.models.v1.LabelOntologyR\rlabelOntology\x12\x44\n\tdataclass\x18\x08 \x01(\x0e\x32&.aruna.api.storage.models.v1.DataClassR\tdataclass\x12>\n\x07version\x18\t \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionR\x07version\"k\n\x18UpdateCollectionResponse\x12O\n\ncollection\x18\x01 \x01(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\ncollection\"\x82\x01\n\x1bPinCollectionVersionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12>\n\x07version\x18\x02 \x01(\x0b\x32$.aruna.api.storage.models.v1.VersionR\x07version\"o\n\x1cPinCollectionVersionResponse\x12O\n\ncollection\x18\x01 \x01(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\ncollection\"T\n\x17\x44\x65leteCollectionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12\x14\n\x05\x66orce\x18\x03 \x01(\x08R\x05\x66orce\"\x1a\n\x18\x44\x65leteCollectionResponse\"\xc2\x01\n\x1f\x41\x64\x64KeyValuesToCollectionRequest\x12#\n\rcollection_id\x18\x01 \x01(\tR\x0c\x63ollectionId\x12=\n\x06labels\x18\x02 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x06labels\x12;\n\x05hooks\x18\x03 \x03(\x0b\x32%.aruna.api.storage.models.v1.KeyValueR\x05hooks\"s\n AddKeyValuesToCollectionResponse\x12O\n\ncollection\x18\x01 \x01(\x0b\x32/.aruna.api.storage.models.v1.CollectionOverviewR\ncollection2\x8e\n\n\x11\x43ollectionService\x12\xa7\x01\n\x13\x43reateNewCollection\x12\x39.aruna.api.storage.services.v1.CreateNewCollectionRequest\x1a:.aruna.api.storage.services.v1.CreateNewCollectionResponse\"\x19\x82\xd3\xe4\x93\x02\x13:\x01*\"\x0e/v1/collection\x12\xae\x01\n\x11GetCollectionByID\x12\x37.aruna.api.storage.services.v1.GetCollectionByIDRequest\x1a\x38.aruna.api.storage.services.v1.GetCollectionByIDResponse\"&\x82\xd3\xe4\x93\x02 \x12\x1e/v1/collection/{collection_id}\x12\xa3\x01\n\x0eGetCollections\x12\x34.aruna.api.storage.services.v1.GetCollectionsRequest\x1a\x35.aruna.api.storage.services.v1.GetCollectionsResponse\"$\x82\xd3\xe4\x93\x02\x1e\x12\x1c/v1/collections/{project_id}\x12\xae\x01\n\x10UpdateCollection\x12\x36.aruna.api.storage.services.v1.UpdateCollectionRequest\x1a\x37.aruna.api.storage.services.v1.UpdateCollectionResponse\")\x82\xd3\xe4\x93\x02#:\x01*\x1a\x1e/v1/collection/{collection_id}\x12\xbe\x01\n\x14PinCollectionVersion\x12:.aruna.api.storage.services.v1.PinCollectionVersionRequest\x1a;.aruna.api.storage.services.v1.PinCollectionVersionResponse\"-\x82\xd3\xe4\x93\x02\':\x01*\"\"/v1/collection/{collection_id}/pin\x12\xae\x01\n\x10\x44\x65leteCollection\x12\x36.aruna.api.storage.services.v1.DeleteCollectionRequest\x1a\x37.aruna.api.storage.services.v1.DeleteCollectionResponse\")\x82\xd3\xe4\x93\x02#:\x01**\x1e/v1/collection/{collection_id}\x12\xd4\x01\n\x18\x41\x64\x64KeyValuesToCollection\x12>.aruna.api.storage.services.v1.AddKeyValuesToCollectionRequest\x1a?.aruna.api.storage.services.v1.AddKeyValuesToCollectionResponse\"7\x82\xd3\xe4\x93\x02\x31:\x01*2,/v1/collection/{collection_id}/add_key_value2\xd1\x05\n\x10WorkspaceService\x12\x9a\x01\n\x0f\x43reateWorkspace\x12\x35.aruna.api.storage.services.v1.CreateWorkspaceRequest\x1a\x36.aruna.api.storage.services.v1.CreateWorkspaceResponse\"\x18\x82\xd3\xe4\x93\x02\x12:\x01*\"\r/v1/workspace\x12\xa9\x01\n\x0f\x44\x65leteWorkspace\x12\x35.aruna.api.storage.services.v1.DeleteWorkspaceRequest\x1a\x36.aruna.api.storage.services.v1.DeleteWorkspaceResponse\"\'\x82\xd3\xe4\x93\x02!:\x01**\x1c/v1/workspace/{workspace_id}\x12\xac\x01\n\x0e\x43laimWorkspace\x12\x34.aruna.api.storage.services.v1.ClaimWorkspaceRequest\x1a\x35.aruna.api.storage.services.v1.ClaimWorkspaceResponse\"-\x82\xd3\xe4\x93\x02\':\x01*\"\"/v1/workspace/{workspace_id}/claim\x12\xc4\x01\n\x11MoveWorkspaceData\x12\x37.aruna.api.storage.services.v1.MoveWorkspaceDataRequest\x1a\x38.aruna.api.storage.services.v1.MoveWorkspaceDataResponse\"<\x82\xd3\xe4\x93\x02\x36:\x01*\"1/v1/workspace/{workspace_id}/move/{collection_id}B\x93\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x11\x43ollectionServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.collection_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\021CollectionServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1'
@@ -32,14 +32,16 @@
   _COLLECTIONSERVICE.methods_by_name['GetCollections']._serialized_options = b'\202\323\344\223\002\036\022\034/v1/collections/{project_id}'
   _COLLECTIONSERVICE.methods_by_name['UpdateCollection']._options = None
   _COLLECTIONSERVICE.methods_by_name['UpdateCollection']._serialized_options = b'\202\323\344\223\002#:\001*\032\036/v1/collection/{collection_id}'
   _COLLECTIONSERVICE.methods_by_name['PinCollectionVersion']._options = None
   _COLLECTIONSERVICE.methods_by_name['PinCollectionVersion']._serialized_options = b'\202\323\344\223\002\':\001*\"\"/v1/collection/{collection_id}/pin'
   _COLLECTIONSERVICE.methods_by_name['DeleteCollection']._options = None
   _COLLECTIONSERVICE.methods_by_name['DeleteCollection']._serialized_options = b'\202\323\344\223\002#:\001**\036/v1/collection/{collection_id}'
+  _COLLECTIONSERVICE.methods_by_name['AddKeyValuesToCollection']._options = None
+  _COLLECTIONSERVICE.methods_by_name['AddKeyValuesToCollection']._serialized_options = b'\202\323\344\223\0021:\001*2,/v1/collection/{collection_id}/add_key_value'
   _WORKSPACESERVICE.methods_by_name['CreateWorkspace']._options = None
   _WORKSPACESERVICE.methods_by_name['CreateWorkspace']._serialized_options = b'\202\323\344\223\002\022:\001*\"\r/v1/workspace'
   _WORKSPACESERVICE.methods_by_name['DeleteWorkspace']._options = None
   _WORKSPACESERVICE.methods_by_name['DeleteWorkspace']._serialized_options = b'\202\323\344\223\002!:\001**\034/v1/workspace/{workspace_id}'
   _WORKSPACESERVICE.methods_by_name['ClaimWorkspace']._options = None
   _WORKSPACESERVICE.methods_by_name['ClaimWorkspace']._serialized_options = b'\202\323\344\223\002\':\001*\"\"/v1/workspace/{workspace_id}/claim'
   _WORKSPACESERVICE.methods_by_name['MoveWorkspaceData']._options = None
@@ -80,12 +82,16 @@
   _PINCOLLECTIONVERSIONREQUEST._serialized_end=2405
   _PINCOLLECTIONVERSIONRESPONSE._serialized_start=2407
   _PINCOLLECTIONVERSIONRESPONSE._serialized_end=2518
   _DELETECOLLECTIONREQUEST._serialized_start=2520
   _DELETECOLLECTIONREQUEST._serialized_end=2604
   _DELETECOLLECTIONRESPONSE._serialized_start=2606
   _DELETECOLLECTIONRESPONSE._serialized_end=2632
-  _COLLECTIONSERVICE._serialized_start=2635
-  _COLLECTIONSERVICE._serialized_end=3714
-  _WORKSPACESERVICE._serialized_start=3717
-  _WORKSPACESERVICE._serialized_end=4438
+  _ADDKEYVALUESTOCOLLECTIONREQUEST._serialized_start=2635
+  _ADDKEYVALUESTOCOLLECTIONREQUEST._serialized_end=2829
+  _ADDKEYVALUESTOCOLLECTIONRESPONSE._serialized_start=2831
+  _ADDKEYVALUESTOCOLLECTIONRESPONSE._serialized_end=2946
+  _COLLECTIONSERVICE._serialized_start=2949
+  _COLLECTIONSERVICE._serialized_end=4243
+  _WORKSPACESERVICE._serialized_start=4246
+  _WORKSPACESERVICE._serialized_end=4967
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/collection_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
+class AddKeyValuesToCollectionRequest(_message.Message):
+    __slots__ = ["collection_id", "hooks", "labels"]
+    COLLECTION_ID_FIELD_NUMBER: _ClassVar[int]
+    HOOKS_FIELD_NUMBER: _ClassVar[int]
+    LABELS_FIELD_NUMBER: _ClassVar[int]
+    collection_id: str
+    hooks: _containers.RepeatedCompositeFieldContainer[_models_pb2.KeyValue]
+    labels: _containers.RepeatedCompositeFieldContainer[_models_pb2.KeyValue]
+    def __init__(self, collection_id: _Optional[str] = ..., labels: _Optional[_Iterable[_Union[_models_pb2.KeyValue, _Mapping]]] = ..., hooks: _Optional[_Iterable[_Union[_models_pb2.KeyValue, _Mapping]]] = ...) -> None: ...
+
+class AddKeyValuesToCollectionResponse(_message.Message):
+    __slots__ = ["collection"]
+    COLLECTION_FIELD_NUMBER: _ClassVar[int]
+    collection: _models_pb2.CollectionOverview
+    def __init__(self, collection: _Optional[_Union[_models_pb2.CollectionOverview, _Mapping]] = ...) -> None: ...
+
 class ClaimWorkspaceRequest(_message.Message):
     __slots__ = ["token", "workspace_id"]
     TOKEN_FIELD_NUMBER: _ClassVar[int]
     WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
     token: str
     workspace_id: str
     def __init__(self, workspace_id: _Optional[str] = ..., token: _Optional[str] = ...) -> None: ...
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/collection_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/collection_service_pb2_grpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,19 @@
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.PinCollectionVersionResponse.FromString,
                 )
         self.DeleteCollection = channel.unary_unary(
                 '/aruna.api.storage.services.v1.CollectionService/DeleteCollection',
                 request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.DeleteCollectionRequest.SerializeToString,
                 response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.DeleteCollectionResponse.FromString,
                 )
+        self.AddKeyValuesToCollection = channel.unary_unary(
+                '/aruna.api.storage.services.v1.CollectionService/AddKeyValuesToCollection',
+                request_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.AddKeyValuesToCollectionRequest.SerializeToString,
+                response_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.AddKeyValuesToCollectionResponse.FromString,
+                )
 
 
 class CollectionServiceServicer(object):
     """CollectionService
 
     Contains all methods that get/create or update Collection and associated resources
     """
@@ -134,14 +139,25 @@
         If cascade is true, all objects that are owned by the collection will also
         deleted. This should be avoided
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def AddKeyValuesToCollection(self, request, context):
+        """AddKeyValueToCollection
+
+        Status: BETA
+
+        Adds key values (labels / hooks) to a collection
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_CollectionServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'CreateNewCollection': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateNewCollection,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.CreateNewCollectionRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.CreateNewCollectionResponse.SerializeToString,
@@ -167,14 +183,19 @@
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.PinCollectionVersionResponse.SerializeToString,
             ),
             'DeleteCollection': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteCollection,
                     request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.DeleteCollectionRequest.FromString,
                     response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.DeleteCollectionResponse.SerializeToString,
             ),
+            'AddKeyValuesToCollection': grpc.unary_unary_rpc_method_handler(
+                    servicer.AddKeyValuesToCollection,
+                    request_deserializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.AddKeyValuesToCollectionRequest.FromString,
+                    response_serializer=aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.AddKeyValuesToCollectionResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'aruna.api.storage.services.v1.CollectionService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -282,14 +303,31 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.CollectionService/DeleteCollection',
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.DeleteCollectionRequest.SerializeToString,
             aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.DeleteCollectionResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
+    @staticmethod
+    def AddKeyValuesToCollection(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/aruna.api.storage.services.v1.CollectionService/AddKeyValuesToCollection',
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.AddKeyValuesToCollectionRequest.SerializeToString,
+            aruna_dot_api_dot_storage_dot_services_dot_v1_dot_collection__service__pb2.AddKeyValuesToCollectionResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
 
 class WorkspaceServiceStub(object):
     """WorkspaceService
 
     Service to manage "special" anonymous collections / workspaces 
     """
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/endpoint_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from aruna.api.storage.models.v1 import models_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_models__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n4aruna/api/storage/services/v1/endpoint_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\x1cgoogle/api/annotations.proto\"\xa4\x02\n\x12\x41\x64\x64\x45ndpointRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x42\n\x07\x65p_type\x18\x02 \x01(\x0e\x32).aruna.api.storage.models.v1.EndpointTypeR\x06\x65pType\x12%\n\x0eproxy_hostname\x18\x03 \x01(\tR\rproxyHostname\x12+\n\x11internal_hostname\x18\x04 \x01(\tR\x10internalHostname\x12-\n\x12\x64ocumentation_path\x18\x05 \x01(\tR\x11\x64ocumentationPath\x12\x1b\n\tis_public\x18\x06 \x01(\x08R\x08isPublic\x12\x16\n\x06pubkey\x18\x07 \x01(\tR\x06pubkey\"}\n\x13\x41\x64\x64\x45ndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\x08\x65ndpoint\x12#\n\rpubkey_serial\x18\x02 \x01(\x03R\x0cpubkeySerial\"j\n\x12GetEndpointRequest\x12%\n\rendpoint_name\x18\x01 \x01(\tH\x00R\x0c\x65ndpointName\x12!\n\x0b\x65ndpoint_id\x18\x02 \x01(\tH\x00R\nendpointIdB\n\n\x08\x65ndpoint\"X\n\x13GetEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\x08\x65ndpoint\"\x15\n\x13GetEndpointsRequest\"[\n\x14GetEndpointsResponse\x12\x43\n\tendpoints\x18\x01 \x03(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\tendpoints\"8\n\x15\x44\x65leteEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId\"\x18\n\x16\x44\x65leteEndpointResponse\"\x1b\n\x19GetDefaultEndpointRequest\"_\n\x1aGetDefaultEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\x08\x65ndpoint2\x8d\x06\n\x0f\x45ndpointService\x12\x8d\x01\n\x0b\x41\x64\x64\x45ndpoint\x12\x31.aruna.api.storage.services.v1.AddEndpointRequest\x1a\x32.aruna.api.storage.services.v1.AddEndpointResponse\"\x17\x82\xd3\xe4\x93\x02\x11:\x01*\"\x0c/v1/endpoint\x12\x8a\x01\n\x0bGetEndpoint\x12\x31.aruna.api.storage.services.v1.GetEndpointRequest\x1a\x32.aruna.api.storage.services.v1.GetEndpointResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/endpoint\x12\x8e\x01\n\x0cGetEndpoints\x12\x32.aruna.api.storage.services.v1.GetEndpointsRequest\x1a\x33.aruna.api.storage.services.v1.GetEndpointsResponse\"\x15\x82\xd3\xe4\x93\x02\x0f\x12\r/v1/endpoints\x12\xa1\x01\n\x0e\x44\x65leteEndpoint\x12\x34.aruna.api.storage.services.v1.DeleteEndpointRequest\x1a\x35.aruna.api.storage.services.v1.DeleteEndpointResponse\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/v1/endpoint/{endpoint_id}\x12\xa7\x01\n\x12GetDefaultEndpoint\x12\x38.aruna.api.storage.services.v1.GetDefaultEndpointRequest\x1a\x39.aruna.api.storage.services.v1.GetDefaultEndpointResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/endpoint/defaultB\x91\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0f\x45ndpointServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n4aruna/api/storage/services/v1/endpoint_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a(aruna/api/storage/models/v1/models.proto\x1a\x1cgoogle/api/annotations.proto\"\xc3\x02\n\x12\x41\x64\x64\x45ndpointRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x42\n\x07\x65p_type\x18\x02 \x01(\x0e\x32).aruna.api.storage.models.v1.EndpointTypeR\x06\x65pType\x12-\n\x12\x64ocumentation_path\x18\x05 \x01(\tR\x11\x64ocumentationPath\x12\x1b\n\tis_public\x18\x06 \x01(\x08R\x08isPublic\x12\x16\n\x06pubkey\x18\x07 \x01(\tR\x06pubkey\x12\x1d\n\nis_bundler\x18\x08 \x01(\x08R\tisBundler\x12R\n\x0chost_configs\x18\t \x03(\x0b\x32/.aruna.api.storage.models.v1.EndpointHostConfigR\x0bhostConfigs\"}\n\x13\x41\x64\x64\x45ndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\x08\x65ndpoint\x12#\n\rpubkey_serial\x18\x02 \x01(\x03R\x0cpubkeySerial\"j\n\x12GetEndpointRequest\x12%\n\rendpoint_name\x18\x01 \x01(\tH\x00R\x0c\x65ndpointName\x12!\n\x0b\x65ndpoint_id\x18\x02 \x01(\tH\x00R\nendpointIdB\n\n\x08\x65ndpoint\"X\n\x13GetEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\x08\x65ndpoint\"\x15\n\x13GetEndpointsRequest\"[\n\x14GetEndpointsResponse\x12\x43\n\tendpoints\x18\x01 \x03(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\tendpoints\"8\n\x15\x44\x65leteEndpointRequest\x12\x1f\n\x0b\x65ndpoint_id\x18\x01 \x01(\tR\nendpointId\"\x18\n\x16\x44\x65leteEndpointResponse\"\x1b\n\x19GetDefaultEndpointRequest\"_\n\x1aGetDefaultEndpointResponse\x12\x41\n\x08\x65ndpoint\x18\x01 \x01(\x0b\x32%.aruna.api.storage.models.v1.EndpointR\x08\x65ndpoint2\x8d\x06\n\x0f\x45ndpointService\x12\x8d\x01\n\x0b\x41\x64\x64\x45ndpoint\x12\x31.aruna.api.storage.services.v1.AddEndpointRequest\x1a\x32.aruna.api.storage.services.v1.AddEndpointResponse\"\x17\x82\xd3\xe4\x93\x02\x11:\x01*\"\x0c/v1/endpoint\x12\x8a\x01\n\x0bGetEndpoint\x12\x31.aruna.api.storage.services.v1.GetEndpointRequest\x1a\x32.aruna.api.storage.services.v1.GetEndpointResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/endpoint\x12\x8e\x01\n\x0cGetEndpoints\x12\x32.aruna.api.storage.services.v1.GetEndpointsRequest\x1a\x33.aruna.api.storage.services.v1.GetEndpointsResponse\"\x15\x82\xd3\xe4\x93\x02\x0f\x12\r/v1/endpoints\x12\xa1\x01\n\x0e\x44\x65leteEndpoint\x12\x34.aruna.api.storage.services.v1.DeleteEndpointRequest\x1a\x35.aruna.api.storage.services.v1.DeleteEndpointResponse\"\"\x82\xd3\xe4\x93\x02\x1c*\x1a/v1/endpoint/{endpoint_id}\x12\xa7\x01\n\x12GetDefaultEndpoint\x12\x38.aruna.api.storage.services.v1.GetDefaultEndpointRequest\x1a\x39.aruna.api.storage.services.v1.GetDefaultEndpointResponse\"\x1c\x82\xd3\xe4\x93\x02\x16\x12\x14/v1/endpoint/defaultB\x91\x01\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0f\x45ndpointServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.endpoint_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\017EndpointServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1'
@@ -30,29 +30,29 @@
   _ENDPOINTSERVICE.methods_by_name['GetEndpoints']._options = None
   _ENDPOINTSERVICE.methods_by_name['GetEndpoints']._serialized_options = b'\202\323\344\223\002\017\022\r/v1/endpoints'
   _ENDPOINTSERVICE.methods_by_name['DeleteEndpoint']._options = None
   _ENDPOINTSERVICE.methods_by_name['DeleteEndpoint']._serialized_options = b'\202\323\344\223\002\034*\032/v1/endpoint/{endpoint_id}'
   _ENDPOINTSERVICE.methods_by_name['GetDefaultEndpoint']._options = None
   _ENDPOINTSERVICE.methods_by_name['GetDefaultEndpoint']._serialized_options = b'\202\323\344\223\002\026\022\024/v1/endpoint/default'
   _ADDENDPOINTREQUEST._serialized_start=160
-  _ADDENDPOINTREQUEST._serialized_end=452
-  _ADDENDPOINTRESPONSE._serialized_start=454
-  _ADDENDPOINTRESPONSE._serialized_end=579
-  _GETENDPOINTREQUEST._serialized_start=581
-  _GETENDPOINTREQUEST._serialized_end=687
-  _GETENDPOINTRESPONSE._serialized_start=689
-  _GETENDPOINTRESPONSE._serialized_end=777
-  _GETENDPOINTSREQUEST._serialized_start=779
-  _GETENDPOINTSREQUEST._serialized_end=800
-  _GETENDPOINTSRESPONSE._serialized_start=802
-  _GETENDPOINTSRESPONSE._serialized_end=893
-  _DELETEENDPOINTREQUEST._serialized_start=895
-  _DELETEENDPOINTREQUEST._serialized_end=951
-  _DELETEENDPOINTRESPONSE._serialized_start=953
-  _DELETEENDPOINTRESPONSE._serialized_end=977
-  _GETDEFAULTENDPOINTREQUEST._serialized_start=979
-  _GETDEFAULTENDPOINTREQUEST._serialized_end=1006
-  _GETDEFAULTENDPOINTRESPONSE._serialized_start=1008
-  _GETDEFAULTENDPOINTRESPONSE._serialized_end=1103
-  _ENDPOINTSERVICE._serialized_start=1106
-  _ENDPOINTSERVICE._serialized_end=1887
+  _ADDENDPOINTREQUEST._serialized_end=483
+  _ADDENDPOINTRESPONSE._serialized_start=485
+  _ADDENDPOINTRESPONSE._serialized_end=610
+  _GETENDPOINTREQUEST._serialized_start=612
+  _GETENDPOINTREQUEST._serialized_end=718
+  _GETENDPOINTRESPONSE._serialized_start=720
+  _GETENDPOINTRESPONSE._serialized_end=808
+  _GETENDPOINTSREQUEST._serialized_start=810
+  _GETENDPOINTSREQUEST._serialized_end=831
+  _GETENDPOINTSRESPONSE._serialized_start=833
+  _GETENDPOINTSRESPONSE._serialized_end=924
+  _DELETEENDPOINTREQUEST._serialized_start=926
+  _DELETEENDPOINTREQUEST._serialized_end=982
+  _DELETEENDPOINTRESPONSE._serialized_start=984
+  _DELETEENDPOINTRESPONSE._serialized_end=1008
+  _GETDEFAULTENDPOINTREQUEST._serialized_start=1010
+  _GETDEFAULTENDPOINTREQUEST._serialized_end=1037
+  _GETDEFAULTENDPOINTRESPONSE._serialized_start=1039
+  _GETDEFAULTENDPOINTRESPONSE._serialized_end=1134
+  _ENDPOINTSERVICE._serialized_start=1137
+  _ENDPOINTSERVICE._serialized_end=1918
 # @@protoc_insertion_point(module_scope)
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/endpoint_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class AddEndpointRequest(_message.Message):
-    __slots__ = ["documentation_path", "ep_type", "internal_hostname", "is_public", "name", "proxy_hostname", "pubkey"]
+    __slots__ = ["documentation_path", "ep_type", "host_configs", "is_bundler", "is_public", "name", "pubkey"]
     DOCUMENTATION_PATH_FIELD_NUMBER: _ClassVar[int]
     EP_TYPE_FIELD_NUMBER: _ClassVar[int]
-    INTERNAL_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
+    HOST_CONFIGS_FIELD_NUMBER: _ClassVar[int]
+    IS_BUNDLER_FIELD_NUMBER: _ClassVar[int]
     IS_PUBLIC_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    PROXY_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
     PUBKEY_FIELD_NUMBER: _ClassVar[int]
     documentation_path: str
     ep_type: _models_pb2.EndpointType
-    internal_hostname: str
+    host_configs: _containers.RepeatedCompositeFieldContainer[_models_pb2.EndpointHostConfig]
+    is_bundler: bool
     is_public: bool
     name: str
-    proxy_hostname: str
     pubkey: str
-    def __init__(self, name: _Optional[str] = ..., ep_type: _Optional[_Union[_models_pb2.EndpointType, str]] = ..., proxy_hostname: _Optional[str] = ..., internal_hostname: _Optional[str] = ..., documentation_path: _Optional[str] = ..., is_public: bool = ..., pubkey: _Optional[str] = ...) -> None: ...
+    def __init__(self, name: _Optional[str] = ..., ep_type: _Optional[_Union[_models_pb2.EndpointType, str]] = ..., documentation_path: _Optional[str] = ..., is_public: bool = ..., pubkey: _Optional[str] = ..., is_bundler: bool = ..., host_configs: _Optional[_Iterable[_Union[_models_pb2.EndpointHostConfig, _Mapping]]] = ...) -> None: ...
 
 class AddEndpointResponse(_message.Message):
     __slots__ = ["endpoint", "pubkey_serial"]
     ENDPOINT_FIELD_NUMBER: _ClassVar[int]
     PUBKEY_SERIAL_FIELD_NUMBER: _ClassVar[int]
     endpoint: _models_pb2.Endpoint
     pubkey_serial: int
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/endpoint_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/info_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/info_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/info_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/info_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/object_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/object_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/object_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/object_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/objectgroup_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/objectgroup_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/project_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 
 from aruna.api.storage.models.v1 import auth_pb2 as aruna_dot_api_dot_storage_dot_models_dot_v1_dot_auth__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from protoc_gen_openapiv2.options import annotations_pb2 as protoc__gen__openapiv2_dot_options_dot_annotations__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.3*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3aruna/api/storage/services/v1/project_service.proto\x12\x1d\x61runa.api.storage.services.v1\x1a&aruna/api/storage/models/v1/auth.proto\x1a\x1cgoogle/api/annotations.proto\x1a.protoc-gen-openapiv2/options/annotations.proto\"L\n\x14\x43reateProjectRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\"6\n\x15\x43reateProjectResponse\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x91\x01\n\x17\x41\x64\x64UserToProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x03 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\x1a\n\x18\x41\x64\x64UserToProjectResponse\"2\n\x11GetProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\\\n\x12GetProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"\x14\n\x12GetProjectsRequest\"_\n\x13GetProjectsResponse\x12H\n\x08projects\x18\x01 \x03(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x08projects\"6\n\x15\x44\x65stroyProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"\x18\n\x16\x44\x65stroyProjectResponse\"k\n\x14UpdateProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\"_\n\x15UpdateProjectResponse\x12\x46\n\x07project\x18\x01 \x01(\x0b\x32,.aruna.api.storage.models.v1.ProjectOverviewR\x07project\"V\n\x1cRemoveUserFromProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x1f\n\x1dRemoveUserFromProjectResponse\"]\n#GetUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12\x17\n\x07user_id\x18\x02 \x01(\tR\x06userId\"\x8a\x01\n$GetUserPermissionsForProjectResponse\x12\x62\n\x0fuser_permission\x18\x01 \x01(\x0b\x32\x39.aruna.api.storage.models.v1.ProjectPermissionDisplayNameR\x0euserPermission\"\x9e\x01\n$EditUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\x12W\n\x0fuser_permission\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0euserPermission\"\'\n%EditUserPermissionsForProjectResponse\"\xae\x01\n\x1aUserWithProjectPermissions\x12\x35\n\x04user\x18\x01 \x01(\x0b\x32!.aruna.api.storage.models.v1.UserR\x04user\x12Y\n\x10user_permissions\x18\x02 \x01(\x0b\x32..aruna.api.storage.models.v1.ProjectPermissionR\x0fuserPermissions\"G\n&GetAllUserPermissionsForProjectRequest\x12\x1d\n\nproject_id\x18\x01 \x01(\tR\tprojectId\"z\n\'GetAllUserPermissionsForProjectResponse\x12O\n\x05users\x18\x01 \x03(\x0b\x32\x39.aruna.api.storage.services.v1.UserWithProjectPermissionsR\x05users2\x90\x0e\n\x0eProjectService\x12\x92\x01\n\rCreateProject\x12\x33.aruna.api.storage.services.v1.CreateProjectRequest\x1a\x34.aruna.api.storage.services.v1.CreateProjectResponse\"\x16\x82\xd3\xe4\x93\x02\x10:\x01*\"\x0b/v1/project\x12\xb1\x01\n\x10\x41\x64\x64UserToProject\x12\x36.aruna.api.storage.services.v1.AddUserToProjectRequest\x1a\x37.aruna.api.storage.services.v1.AddUserToProjectResponse\",\x82\xd3\xe4\x93\x02&:\x01*\"!/v1/project/{project_id}/add_user\x12\x93\x01\n\nGetProject\x12\x30.aruna.api.storage.services.v1.GetProjectRequest\x1a\x31.aruna.api.storage.services.v1.GetProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x12\x18/v1/project/{project_id}\x12\x8a\x01\n\x0bGetProjects\x12\x31.aruna.api.storage.services.v1.GetProjectsRequest\x1a\x32.aruna.api.storage.services.v1.GetProjectsResponse\"\x14\x82\xd3\xe4\x93\x02\x0e\x12\x0c/v1/projects\x12\x9f\x01\n\x0e\x44\x65stroyProject\x12\x34.aruna.api.storage.services.v1.DestroyProjectRequest\x1a\x35.aruna.api.storage.services.v1.DestroyProjectResponse\" \x82\xd3\xe4\x93\x02\x1a*\x18/v1/project/{project_id}\x12\x9c\x01\n\rUpdateProject\x12\x33.aruna.api.storage.services.v1.UpdateProjectRequest\x1a\x34.aruna.api.storage.services.v1.UpdateProjectResponse\" \x82\xd3\xe4\x93\x02\x1a\x1a\x18/v1/project/{project_id}\x12\xc0\x01\n\x15RemoveUserFromProject\x12;.aruna.api.storage.services.v1.RemoveUserFromProjectRequest\x1a<.aruna.api.storage.services.v1.RemoveUserFromProjectResponse\",\x82\xd3\xe4\x93\x02&*$/v1/project/{project_id}/remove_user\x12\xd2\x01\n\x1cGetUserPermissionsForProject\x12\x42.aruna.api.storage.services.v1.GetUserPermissionsForProjectRequest\x1a\x43.aruna.api.storage.services.v1.GetUserPermissionsForProjectResponse\")\x82\xd3\xe4\x93\x02#\x12!/v1/project/{project_id}/get_user\x12\xdc\x01\n\x1fGetAllUserPermissionsForProject\x12\x45.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectRequest\x1a\x46.aruna.api.storage.services.v1.GetAllUserPermissionsForProjectResponse\"*\x82\xd3\xe4\x93\x02$\x12\"/v1/project/{project_id}/get_users\x12\xd9\x01\n\x1d\x45\x64itUserPermissionsForProject\x12\x43.aruna.api.storage.services.v1.EditUserPermissionsForProjectRequest\x1a\x44.aruna.api.storage.services.v1.EditUserPermissionsForProjectResponse\"-\x82\xd3\xe4\x93\x02\':\x01*2\"/v1/project/{project_id}/edit_userB\xe5\x02\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\x0eProjectServiceP\x01Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\x92\x41\xd1\x01\x12\x31\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.5*\x01\x02\x32\x10\x61pplication/json:\x10\x61pplication/jsonZ`\n^\n\rAccessKeyAuth\x12M\x08\x02\x12\x38\x41uthentication token, prefixed by Bearer: Bearer <token>\x1a\rAuthorization \x02\x62\x13\n\x11\n\rAccessKeyAuth\x12\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'aruna.api.storage.services.v1.project_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.3*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
+  DESCRIPTOR._serialized_options = b'\n>com.github.ArunaStorage.java_api.aruna.api.storage.services.v1B\016ProjectServiceP\001Z<github.com/ArunaStorage/go-api/aruna/api/storage/services/v1\222A\321\001\0221\n#Aruna Object Storage (AOS) REST API2\n1.1.0-rc.5*\001\0022\020application/json:\020application/jsonZ`\n^\n\rAccessKeyAuth\022M\010\002\0228Authentication token, prefixed by Bearer: Bearer <token>\032\rAuthorization \002b\023\n\021\n\rAccessKeyAuth\022\000'
   _PROJECTSERVICE.methods_by_name['CreateProject']._options = None
   _PROJECTSERVICE.methods_by_name['CreateProject']._serialized_options = b'\202\323\344\223\002\020:\001*\"\013/v1/project'
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._options = None
   _PROJECTSERVICE.methods_by_name['AddUserToProject']._serialized_options = b'\202\323\344\223\002&:\001*\"!/v1/project/{project_id}/add_user'
   _PROJECTSERVICE.methods_by_name['GetProject']._options = None
   _PROJECTSERVICE.methods_by_name['GetProject']._serialized_options = b'\202\323\344\223\002\032\022\030/v1/project/{project_id}'
   _PROJECTSERVICE.methods_by_name['GetProjects']._options = None
```

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/project_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/project_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/project_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/service_account_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/service_account_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/service_account_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/user_service_pb2.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/user_service_pb2.pyi` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/aruna/api/storage/services/v1/user_service_pb2_grpc.py` & `Aruna-Python-API-1.1.0rc5/aruna/api/storage/services/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `Aruna-Python-API-1.1.0rc3/setup.py` & `Aruna-Python-API-1.1.0rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(
     name='Aruna-Python-API',
-    version="1.1.0-rc.3",
+    version="1.1.0-rc.5",
     description='Aruna Object Storage Python API builds',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/ArunaStorage/python-api',
     license='Apache 2.0',
     author='Marius Dieckmann, Jannis Hochmuth',
     author_email='marius.dieckmann@computational.bio.uni-giessen.de, '
```

