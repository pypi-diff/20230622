# Comparing `tmp/kuksa_client-0.4.0a2.tar.gz` & `tmp/kuksa_client-0.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuksa_client-0.4.0a2.tar", last modified: Thu Apr 20 06:55:42 2023, max compression
+gzip compressed data, was "kuksa_client-0.4.0a3.tar", last modified: Thu Jun 22 08:59:30 2023, max compression
```

## Comparing `kuksa_client-0.4.0a2.tar` & `kuksa_client-0.4.0a3.tar`

### file list

```diff
@@ -1,66 +1,65 @@
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/
--rw-r--r--   0 erik      (1000) erik      (1000)    11357 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/LICENSE
--rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/MANIFEST.in
--rw-r--r--   0 erik      (1000) erik      (1000)     9640 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     8758 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/README.md
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.498603 kuksa_client-0.4.0a2/kuksa/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.498603 kuksa_client-0.4.0a2/kuksa/val/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa/val/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.498603 kuksa_client-0.4.0a2/kuksa/val/v1/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa/val/v1/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9374 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa/val/v1/types_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa/val/v1/types_pb2_grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3751 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa/val/v1/val_pb2.py
--rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa/val/v1/val_pb2_grpc.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.502601 kuksa_client-0.4.0a2/kuksa_certificates/
--rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a2/kuksa_certificates/CA.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/CA.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a2/kuksa_certificates/Client.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1371 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_certificates/Client.pem
--rw-r--r--   0 erik      (1000) erik      (1000)     2267 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/README.md
--rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a2/kuksa_certificates/Server.key
--rw-r--r--   0 erik      (1000) erik      (1000)     1371 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_certificates/Server.pem
--rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)     1443 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_certificates/genCerts.sh
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.502601 kuksa_client-0.4.0a2/kuksa_certificates/jwt/
--rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/all-read-write.json
--rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/all-read-write.json.token
--rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/createToken.py
--rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/jwt.key
--rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/jwt.key.pub
--rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/recreateJWTkeyPair.sh
--rw-r--r--   0 erik      (1000) erik      (1000)       34 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/requirements.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/single-read.json
--rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/single-read.json.token
--rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/super-admin.json
--rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a2/kuksa_certificates/jwt/super-admin.json.token
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.502601 kuksa_client-0.4.0a2/kuksa_client/
--rw-r--r--   0 erik      (1000) erik      (1000)     3929 2023-04-20 06:51:14.000000 kuksa_client-0.4.0a2/kuksa_client/__init__.py
--rwxr-xr-x   0 erik      (1000) erik      (1000)    23519 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_client/__main__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_client/_metadata.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/kuksa_client/cli_backend/
--rw-r--r--   0 erik      (1000) erik      (1000)     2189 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_client/cli_backend/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    11064 2023-04-20 06:51:14.000000 kuksa_client-0.4.0a2/kuksa_client/cli_backend/grpc.py
--rw-r--r--   0 erik      (1000) erik      (1000)     9397 2023-04-19 12:14:28.000000 kuksa_client-0.4.0a2/kuksa_client/cli_backend/ws.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/kuksa_client/grpc/
--rw-r--r--   0 erik      (1000) erik      (1000)    37360 2023-04-20 06:51:14.000000 kuksa_client-0.4.0a2/kuksa_client/grpc/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)    16144 2023-04-20 06:51:14.000000 kuksa_client-0.4.0a2/kuksa_client/grpc/aio.py
--rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_client/logging.ini
--rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_client/logo
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/kuksa_client/ws/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/kuksa_client/ws/__init__.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/kuksa_client.egg-info/
--rw-r--r--   0 erik      (1000) erik      (1000)     9640 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/PKG-INFO
--rw-r--r--   0 erik      (1000) erik      (1000)     1542 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/SOURCES.txt
--rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/dependency_links.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/entry_points.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      227 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/requires.txt
--rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-04-20 06:55:42.000000 kuksa_client-0.4.0a2/kuksa_client.egg-info/top_level.txt
--rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-04-12 10:04:35.000000 kuksa_client-0.4.0a2/pyproject.toml
--rw-r--r--   0 erik      (1000) erik      (1000)     1388 2023-04-20 06:55:42.518593 kuksa_client-0.4.0a2/setup.cfg
--rw-r--r--   0 erik      (1000) erik      (1000)     1168 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/setup.py
-drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-04-20 06:55:42.514595 kuksa_client-0.4.0a2/tests/
--rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/tests/__init__.py
--rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-04-05 12:40:11.000000 kuksa_client-0.4.0a2/tests/conftest.py
--rw-r--r--   0 erik      (1000) erik      (1000)    63303 2023-04-12 07:56:08.000000 kuksa_client-0.4.0a2/tests/test_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.666995 kuksa_client-0.4.0a3/
+-rw-r--r--   0 erik      (1000) erik      (1000)       35 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/MANIFEST.in
+-rw-r--r--   0 erik      (1000) erik      (1000)    13241 2023-06-22 08:59:30.666995 kuksa_client-0.4.0a3/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)    12381 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/README.md
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.655000 kuksa_client-0.4.0a3/kuksa/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.655000 kuksa_client-0.4.0a3/kuksa/val/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa/val/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.655000 kuksa_client-0.4.0a3/kuksa/val/v1/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa/val/v1/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9374 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa/val/v1/types_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      159 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa/val/v1/types_pb2_grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3751 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa/val/v1/val_pb2.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     8731 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa/val/v1/val_pb2_grpc.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.658999 kuksa_client-0.4.0a3/kuksa_certificates/
+-rw-r--r--   0 erik      (1000) erik      (1000)     1675 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a3/kuksa_certificates/CA.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1342 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_certificates/CA.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a3/kuksa_certificates/Client.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_certificates/Client.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)     3537 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_certificates/README.md
+-rw-r--r--   0 erik      (1000) erik      (1000)     1679 2022-09-02 12:03:09.000000 kuksa_client-0.4.0a3/kuksa_certificates/Server.key
+-rw-r--r--   0 erik      (1000) erik      (1000)     1704 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_certificates/Server.pem
+-rw-r--r--   0 erik      (1000) erik      (1000)      114 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_certificates/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     2023 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_certificates/genCerts.sh
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.662997 kuksa_client-0.4.0a3/kuksa_certificates/jwt/
+-rw-r--r--   0 erik      (1000) erik      (1000)      151 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/all-read-write.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      875 2022-11-01 08:41:15.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/all-read-write.json.token
+-rwxr-xr-x   0 erik      (1000) erik      (1000)     1430 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/createToken.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     3243 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/jwt.key
+-rw-r--r--   0 erik      (1000) erik      (1000)      800 2022-11-01 08:46:13.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/jwt.key.pub
+-rwxr-xr-x   0 erik      (1000) erik      (1000)      901 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/recreateJWTkeyPair.sh
+-rw-r--r--   0 erik      (1000) erik      (1000)       34 2023-05-10 08:02:45.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/requirements.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      167 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/single-read.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      895 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/single-read.json.token
+-rw-r--r--   0 erik      (1000) erik      (1000)      175 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/super-admin.json
+-rw-r--r--   0 erik      (1000) erik      (1000)      899 2022-08-17 12:23:53.000000 kuksa_client-0.4.0a3/kuksa_certificates/jwt/super-admin.json.token
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.662997 kuksa_client-0.4.0a3/kuksa_client/
+-rw-r--r--   0 erik      (1000) erik      (1000)     3929 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_client/__init__.py
+-rwxr-xr-x   0 erik      (1000) erik      (1000)    25603 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_client/__main__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     1708 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_client/_metadata.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.662997 kuksa_client-0.4.0a3/kuksa_client/cli_backend/
+-rw-r--r--   0 erik      (1000) erik      (1000)     2259 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_client/cli_backend/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    11695 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_client/cli_backend/grpc.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     9892 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_client/cli_backend/ws.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.662997 kuksa_client-0.4.0a3/kuksa_client/grpc/
+-rw-r--r--   0 erik      (1000) erik      (1000)    38987 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_client/grpc/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    16627 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/kuksa_client/grpc/aio.py
+-rw-r--r--   0 erik      (1000) erik      (1000)      385 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_client/logging.ini
+-rw-r--r--   0 erik      (1000) erik      (1000)      605 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_client/logo
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.662997 kuksa_client-0.4.0a3/kuksa_client/ws/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/kuksa_client/ws/__init__.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.662997 kuksa_client-0.4.0a3/kuksa_client.egg-info/
+-rw-r--r--   0 erik      (1000) erik      (1000)    13241 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa_client.egg-info/PKG-INFO
+-rw-r--r--   0 erik      (1000) erik      (1000)     1534 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa_client.egg-info/SOURCES.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)        1 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa_client.egg-info/dependency_links.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       60 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa_client.egg-info/entry_points.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      212 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa_client.egg-info/requires.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)       44 2023-06-22 08:59:30.000000 kuksa_client-0.4.0a3/kuksa_client.egg-info/top_level.txt
+-rw-r--r--   0 erik      (1000) erik      (1000)      625 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/pyproject.toml
+-rw-r--r--   0 erik      (1000) erik      (1000)     1370 2023-06-22 08:59:30.666995 kuksa_client-0.4.0a3/setup.cfg
+-rw-r--r--   0 erik      (1000) erik      (1000)     1168 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/setup.py
+drwxr-xr-x   0 erik      (1000) erik      (1000)        0 2023-06-22 08:59:30.666995 kuksa_client-0.4.0a3/tests/
+-rw-r--r--   0 erik      (1000) erik      (1000)        0 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/tests/__init__.py
+-rw-r--r--   0 erik      (1000) erik      (1000)     2545 2023-05-09 13:51:21.000000 kuksa_client-0.4.0a3/tests/conftest.py
+-rw-r--r--   0 erik      (1000) erik      (1000)    63305 2023-06-21 14:42:58.000000 kuksa_client-0.4.0a3/tests/test_grpc.py
```

### Comparing `kuksa_client-0.4.0a2/PKG-INFO` & `kuksa_client-0.4.0a3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa_client
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: kuksa.val python clients and SDK
 Home-page: https://github.com/eclipse/kuksa.val
 Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
 Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
@@ -13,32 +13,31 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
-License-File: LICENSE
 
-# Kuksa Client
+# KUKSA.val Client
 ![kuksa.val Logo](https://raw.githubusercontent.com/eclipse/kuksa.val/0.2.5/doc/pictures/logo.png)
 
-`kuksa.val` is a part of the opensource project [eclipse kuksa](https://www.eclipse.org/kuksa/).
+`kuksa.val` is a part of the opensource project [Eclipse Kuksa](https://www.eclipse.org/kuksa/).
 More about `kuksa.val` can be found in the [repository](https://github.com/eclipse/kuksa.val).
 
 ## Introduction
 
-`kuksa-client` provides both a command-line interface (CLI) and a standalone library to interact with either
-[KUKSA.val server](https://github.com/eclipse/kuksa.val/tree/master/kuksa-val-server) or
-[KUKSA databroker](https://github.com/eclipse/kuksa.val/tree/master/kuksa_databroker).
+KUKSA.val Client provides both a command-line interface (CLI) and a standalone library to interact with either
+[KUKSA.val Server](https://github.com/eclipse/kuksa.val/tree/master/kuksa-val-server) or
+[KUKSA.val Databroker](https://github.com/eclipse/kuksa.val/tree/master/kuksa_databroker).
 
 
 ## Installing the client and starting its CLI
 
-The fastest way to start using kuksa-client is to install a pre-built version from pypi.org:
+The fastest way to start using KUKSA.val Client is to install a pre-built version from pypi.org:
 
 ```console
 $ pip install kuksa-client
 ```
 
 If you want to install from sources instead see [Building and running a local version](#building-and-running-a-local-version).
 
@@ -48,17 +47,16 @@
 $ kuksa-client
 ```
 
 With default CLI arguments, the client will try to connect to a local VISS server e.g. `kuksa-val-server`.
 If you wish to connect to a gRPC server e.g. `kuksa-databroker`, you should instead run:
 
 ```console
-$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc --insecure
+$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc
 ```
-Note: `--insecure` is required because `kuksa-databroker` does not yet support encryption or authentication.
 
 If everything works as expected and the server can be contacted you will get an output similar to below.
 
 
 ```console
 Welcome to Kuksa Client version <some_version>
 
@@ -78,64 +76,139 @@
 Default tokens directory: /some/path/kuksa_certificates/jwt
 
 connectj to wss://127.0.0.1:8090
 Websocket connected securely.
 Test Client>
 ```
 
-The next step is to authorize against the server.
-The jwt tokens for testing can either be found under [kuksa_certificates/jwt](https://github.com/eclipse/kuksa.val/tree/0.2.5/kuksa_certificates/jwt) or you can also use following command inside `kuksa-client` to find the via `pip` installed certificate directory.
+If the connected KUKSA.val Server or KUKSA.val Databroker require authorization the next step is to authorize.
+KUKSA.val Server and KUKSA.val Databroker use different token formats.
+
+### Authorizing against KUKSA.val Server
+
+The jwt tokens for testing can either be found under [../kuksa_certificates/jwt](../kuksa_certificates/jwt)
+or you can also use following command inside `kuksa-client` to find the via `pip` installed certificate directory.
 
 ```console
 Test Client> printTokenDir
 ```
-Select one of the tokens and use the `authorize` command like below.
+Select one of the tokens and use the `authorize` command like below:
 
 ```console
 Test Client> authorize /some/path/kuksa_certificates/jwt/super-admin.json.token
 ```
 
+### Authorizing against KUKSA.val Databroker
+
+If connecting to Databroker the command `printTokenDir` is not much help as it shows the default token directories
+for KUKSA.val Server example tokens. If the KUKSA.val Databroker use default example tokens then one of the
+tokens in [../jwt](../jwt) can be used, like in the example below:
+
+```console
+Test Client> authorize /some/path/jwt/provide-all.token
+```
+
+## Using TLS
+
+KUKSA.val Client use TLS by default, it only run in insecure mode if `--insecure` is given as argument.
+
+By default the KUKSA.val example Root CA and Client keys are used, but client keys have no effect as mutual authentication is not supported by KUKSA.val Databroker or KUKSA.val Server.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc
+```
+
+This call with all parameters specified give same effect:
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc --certificate ../kuksa_certificates/Client.pem --keyfile ../kuksa_certificates/Client.key --cacertificate ./kuksa_certificates/CA.pem
+```
+
+There is actually no reason to specify client key and certificate, as mutual authentication is not supported in KUKSA.val Databroker,
+so the command can be simplified like this:
+
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc --cacertificate ./kuksa_certificates/CA.pem
+```
+
+The example server protocol list 127.0.0.1 as an alternative name, but the TLS-client currently used does not accept it,
+instead a valid server name must be given as argument.
+Currently `Server` and `localhost`are valid names from the example certificates.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc  --cacertificate ../kuksa_certificates/CA.pem --tls-server-name Server
+```
+
+### Connecting to KUKSA.val Server
+
+Connecting to KUKSA.val Server is default, and TLS is used by default by KUKSA.val Server.
+`--tls-server-name` does not need to be used when connecting to KUKSA.val Server,
+that is the only difference compared to connecting to KUKSA.val Databroker.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client
+```
+
+This corresponds to this call:
+
+```
+kuksa-client --ip 127.0.0.1 --port 8090 --protocol ws --cacertificate ./kuksa_certificates/CA.pem
+```
+
 ## Usage Instructions
 
 Refer help for further information
+
 ```console
-VSS Client> help -v
+Test Client> help -v
 
 Documented commands (use 'help -v' for verbose/'help <topic>' for details):
 
 Communication Set-up Commands
 ================================================================================
 authorize           Authorize the client to interact with the server
 connect
-disconnect          Disconnect from the VSS Server
-getServerAddress    Gets the IP Address for the VSS Server
-setServerAddress    Sets the IP Address for the VSS Server
+disconnect          Disconnect from the VISS/gRPC Server
+getServerAddress    Gets the IP Address for the VISS/gRPC Server
+setServerAddress    Sets the IP Address for the VISS/gRPC Server
 
 Info Commands
 ================================================================================
 info                Show summary info of the client
 printTokenDir       Show token directory
 version             Show version of the client
 
 Kuksa Interaction Commands
 ================================================================================
-getMetaData         Get MetaData of the path
-getValue            Get the value of a path
-setValue            Set the value of a path
-updateMetaData      Update MetaData of a given path
-updateVSSTree      Update VSS Tree Entry
+getMetaData          Get MetaData of the path
+getTargetValue       Get the value of a path
+getTargetValues      Get the value of given paths
+getValue             Get the value of a path
+getValues            Get the value of given paths
+setTargetValue       Set the target value of a path
+setTargetValues      Set the target value of given paths
+setValue             Set the value of a path
+setValues            Set the value of given paths
+subscribe            Subscribe the value of a path
+subscribeMultiple    Subscribe to updates of given paths
+unsubscribe          Unsubscribe an existing subscription
+updateMetaData       Update MetaData of a given path
+updateVSSTree        Update VSS Tree Entry
+
 ```
 
 This is an example showing how some of the commands can be used:
 
-![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/0.2.5/doc/pictures/testclient_basic.gif "test client usage")
+![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/master/doc/pictures/testclient_basic.gif "test client usage")
 
 ### Updating VSS Structure
 
-Using the testclient, it is also possible to update and extend the VSS data structure. More details can be found [here](https://github.com/eclipse/kuksa.val/blob/0.2.5/doc/liveUpdateVSSTree.md).
+Using the test client, it is also possible to update and extend the VSS data structure.
+More details can be found [here](https://github.com/eclipse/kuksa.val/blob/master/doc/KUKSA.val_server/liveUpdateVSSTree.md).
 
 **Note**: You can also use `setValue` to change the value of an array, but the value should not contains any non-quoted spaces. Consider the following examples:
 
 ```console
 Test Client> setValue Vehicle.OBD.DTCList ["dtc1","dtc2"]
 {
     "action": "set",
@@ -151,15 +224,14 @@
 }
 
 Test Client> setValue Vehicle.OBD.DTCList ["dtc1", "dtc2"]
 usage: setValue [-h] Path Value
 setValue: error: unrecognized arguments: dtc2 ]
 ```
 
-
 ## Building and running a local version
 
 For development purposes it may be necessary to customize the code for the client and run a locally built version.
 First we suggest you create a dedicated [python virtual environment](https://docs.python.org/3/library/venv.html) for kuksa-client:
 
 ```console
 $ mkdir --parents ~/.venv
@@ -188,15 +260,17 @@
 Whenever you want to exit kuksa-client's virtual environment, simply run:
 ```console
 (kuksa-client) $ deactivate
 $
 ```
 
 ## Using Docker
-You can build a docker image of the testclient using the [`Dockerfile`](./Dockerfile). Not the most effcient way to pack a small python script, but it is easy to get started. The Dockerfile needs to be executed on the parent directory (so it include the needed certificates and `pip` package configuration).
+You can build a docker image of the testclient using the [`Dockerfile`](./Dockerfile).
+Not the most effcient way to pack a small python script, but it is easy to get started.
+The Dockerfile needs to be executed on the parent directory (so it include the needed certificates and `pip` package configuration).
 
 
 ```console
 $ cd /some/dir/kuksa.val
 $ docker build -f kuksa-client/Dockerfile -t kuksa-client:latest .
 ```
 
@@ -239,14 +313,34 @@
 '<your version, e.g. 0.1.7>'
 ```
 
 This package holds different APIs depending on your application's requirements.
 For more information, see ([Documentation](https://github.com/eclipse/kuksa.val/blob/master/kuksa-client/docs/main.md)).
 
 
+### TLS configuration
+
+Clients like [KUKSA.val CAN Feeder](https://github.com/eclipse/kuksa.val.feeders/tree/main/dbc2val)
+that use KUKSA.val Client library must typically set the path to the root CA certificate.
+If the path is set the VSSClient will try to establish a secure connection.
+
+```
+# Shall TLS be used (default False for Databroker, True for KUKSA.val Server)
+# tls = False
+tls = True
+
+# TLS-related settings
+# Path to root CA, needed if using TLS
+root_ca_path=../../kuksa.val/kuksa_certificates/CA.pem
+# Server name, typically only needed if accessing server by IP address like 127.0.0.1
+# and typically only if connection to KUKSA.val Databroker
+# If using KUKSA.val example certificates the names "Server" or "localhost" can be used.
+# tls_server_name=Server
+```
+
 ## Troubleshooting
 
 1. The server/data broker is listening on its port but my client is unable to connect to it and returns an error:
 ```console
 Error: Websocket could not be connected or the gRPC channel could not be created.
 ```
 If you're running both client and server on your local host, make sure that:
```

### Comparing `kuksa_client-0.4.0a2/README.md` & `kuksa_client-0.4.0a3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Kuksa Client
+# KUKSA.val Client
 ![kuksa.val Logo](https://raw.githubusercontent.com/eclipse/kuksa.val/0.2.5/doc/pictures/logo.png)
 
-`kuksa.val` is a part of the opensource project [eclipse kuksa](https://www.eclipse.org/kuksa/).
+`kuksa.val` is a part of the opensource project [Eclipse Kuksa](https://www.eclipse.org/kuksa/).
 More about `kuksa.val` can be found in the [repository](https://github.com/eclipse/kuksa.val).
 
 ## Introduction
 
-`kuksa-client` provides both a command-line interface (CLI) and a standalone library to interact with either
-[KUKSA.val server](https://github.com/eclipse/kuksa.val/tree/master/kuksa-val-server) or
-[KUKSA databroker](https://github.com/eclipse/kuksa.val/tree/master/kuksa_databroker).
+KUKSA.val Client provides both a command-line interface (CLI) and a standalone library to interact with either
+[KUKSA.val Server](https://github.com/eclipse/kuksa.val/tree/master/kuksa-val-server) or
+[KUKSA.val Databroker](https://github.com/eclipse/kuksa.val/tree/master/kuksa_databroker).
 
 
 ## Installing the client and starting its CLI
 
-The fastest way to start using kuksa-client is to install a pre-built version from pypi.org:
+The fastest way to start using KUKSA.val Client is to install a pre-built version from pypi.org:
 
 ```console
 $ pip install kuksa-client
 ```
 
 If you want to install from sources instead see [Building and running a local version](#building-and-running-a-local-version).
 
@@ -27,17 +27,16 @@
 $ kuksa-client
 ```
 
 With default CLI arguments, the client will try to connect to a local VISS server e.g. `kuksa-val-server`.
 If you wish to connect to a gRPC server e.g. `kuksa-databroker`, you should instead run:
 
 ```console
-$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc --insecure
+$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc
 ```
-Note: `--insecure` is required because `kuksa-databroker` does not yet support encryption or authentication.
 
 If everything works as expected and the server can be contacted you will get an output similar to below.
 
 
 ```console
 Welcome to Kuksa Client version <some_version>
 
@@ -57,64 +56,139 @@
 Default tokens directory: /some/path/kuksa_certificates/jwt
 
 connectj to wss://127.0.0.1:8090
 Websocket connected securely.
 Test Client>
 ```
 
-The next step is to authorize against the server.
-The jwt tokens for testing can either be found under [kuksa_certificates/jwt](https://github.com/eclipse/kuksa.val/tree/0.2.5/kuksa_certificates/jwt) or you can also use following command inside `kuksa-client` to find the via `pip` installed certificate directory.
+If the connected KUKSA.val Server or KUKSA.val Databroker require authorization the next step is to authorize.
+KUKSA.val Server and KUKSA.val Databroker use different token formats.
+
+### Authorizing against KUKSA.val Server
+
+The jwt tokens for testing can either be found under [../kuksa_certificates/jwt](../kuksa_certificates/jwt)
+or you can also use following command inside `kuksa-client` to find the via `pip` installed certificate directory.
 
 ```console
 Test Client> printTokenDir
 ```
-Select one of the tokens and use the `authorize` command like below.
+Select one of the tokens and use the `authorize` command like below:
 
 ```console
 Test Client> authorize /some/path/kuksa_certificates/jwt/super-admin.json.token
 ```
 
+### Authorizing against KUKSA.val Databroker
+
+If connecting to Databroker the command `printTokenDir` is not much help as it shows the default token directories
+for KUKSA.val Server example tokens. If the KUKSA.val Databroker use default example tokens then one of the
+tokens in [../jwt](../jwt) can be used, like in the example below:
+
+```console
+Test Client> authorize /some/path/jwt/provide-all.token
+```
+
+## Using TLS
+
+KUKSA.val Client use TLS by default, it only run in insecure mode if `--insecure` is given as argument.
+
+By default the KUKSA.val example Root CA and Client keys are used, but client keys have no effect as mutual authentication is not supported by KUKSA.val Databroker or KUKSA.val Server.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc
+```
+
+This call with all parameters specified give same effect:
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc --certificate ../kuksa_certificates/Client.pem --keyfile ../kuksa_certificates/Client.key --cacertificate ./kuksa_certificates/CA.pem
+```
+
+There is actually no reason to specify client key and certificate, as mutual authentication is not supported in KUKSA.val Databroker,
+so the command can be simplified like this:
+
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc --cacertificate ./kuksa_certificates/CA.pem
+```
+
+The example server protocol list 127.0.0.1 as an alternative name, but the TLS-client currently used does not accept it,
+instead a valid server name must be given as argument.
+Currently `Server` and `localhost`are valid names from the example certificates.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc  --cacertificate ../kuksa_certificates/CA.pem --tls-server-name Server
+```
+
+### Connecting to KUKSA.val Server
+
+Connecting to KUKSA.val Server is default, and TLS is used by default by KUKSA.val Server.
+`--tls-server-name` does not need to be used when connecting to KUKSA.val Server,
+that is the only difference compared to connecting to KUKSA.val Databroker.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client
+```
+
+This corresponds to this call:
+
+```
+kuksa-client --ip 127.0.0.1 --port 8090 --protocol ws --cacertificate ./kuksa_certificates/CA.pem
+```
+
 ## Usage Instructions
 
 Refer help for further information
+
 ```console
-VSS Client> help -v
+Test Client> help -v
 
 Documented commands (use 'help -v' for verbose/'help <topic>' for details):
 
 Communication Set-up Commands
 ================================================================================
 authorize           Authorize the client to interact with the server
 connect
-disconnect          Disconnect from the VSS Server
-getServerAddress    Gets the IP Address for the VSS Server
-setServerAddress    Sets the IP Address for the VSS Server
+disconnect          Disconnect from the VISS/gRPC Server
+getServerAddress    Gets the IP Address for the VISS/gRPC Server
+setServerAddress    Sets the IP Address for the VISS/gRPC Server
 
 Info Commands
 ================================================================================
 info                Show summary info of the client
 printTokenDir       Show token directory
 version             Show version of the client
 
 Kuksa Interaction Commands
 ================================================================================
-getMetaData         Get MetaData of the path
-getValue            Get the value of a path
-setValue            Set the value of a path
-updateMetaData      Update MetaData of a given path
-updateVSSTree      Update VSS Tree Entry
+getMetaData          Get MetaData of the path
+getTargetValue       Get the value of a path
+getTargetValues      Get the value of given paths
+getValue             Get the value of a path
+getValues            Get the value of given paths
+setTargetValue       Set the target value of a path
+setTargetValues      Set the target value of given paths
+setValue             Set the value of a path
+setValues            Set the value of given paths
+subscribe            Subscribe the value of a path
+subscribeMultiple    Subscribe to updates of given paths
+unsubscribe          Unsubscribe an existing subscription
+updateMetaData       Update MetaData of a given path
+updateVSSTree        Update VSS Tree Entry
+
 ```
 
 This is an example showing how some of the commands can be used:
 
-![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/0.2.5/doc/pictures/testclient_basic.gif "test client usage")
+![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/master/doc/pictures/testclient_basic.gif "test client usage")
 
 ### Updating VSS Structure
 
-Using the testclient, it is also possible to update and extend the VSS data structure. More details can be found [here](https://github.com/eclipse/kuksa.val/blob/0.2.5/doc/liveUpdateVSSTree.md).
+Using the test client, it is also possible to update and extend the VSS data structure.
+More details can be found [here](https://github.com/eclipse/kuksa.val/blob/master/doc/KUKSA.val_server/liveUpdateVSSTree.md).
 
 **Note**: You can also use `setValue` to change the value of an array, but the value should not contains any non-quoted spaces. Consider the following examples:
 
 ```console
 Test Client> setValue Vehicle.OBD.DTCList ["dtc1","dtc2"]
 {
     "action": "set",
@@ -130,15 +204,14 @@
 }
 
 Test Client> setValue Vehicle.OBD.DTCList ["dtc1", "dtc2"]
 usage: setValue [-h] Path Value
 setValue: error: unrecognized arguments: dtc2 ]
 ```
 
-
 ## Building and running a local version
 
 For development purposes it may be necessary to customize the code for the client and run a locally built version.
 First we suggest you create a dedicated [python virtual environment](https://docs.python.org/3/library/venv.html) for kuksa-client:
 
 ```console
 $ mkdir --parents ~/.venv
@@ -167,15 +240,17 @@
 Whenever you want to exit kuksa-client's virtual environment, simply run:
 ```console
 (kuksa-client) $ deactivate
 $
 ```
 
 ## Using Docker
-You can build a docker image of the testclient using the [`Dockerfile`](./Dockerfile). Not the most effcient way to pack a small python script, but it is easy to get started. The Dockerfile needs to be executed on the parent directory (so it include the needed certificates and `pip` package configuration).
+You can build a docker image of the testclient using the [`Dockerfile`](./Dockerfile).
+Not the most effcient way to pack a small python script, but it is easy to get started.
+The Dockerfile needs to be executed on the parent directory (so it include the needed certificates and `pip` package configuration).
 
 
 ```console
 $ cd /some/dir/kuksa.val
 $ docker build -f kuksa-client/Dockerfile -t kuksa-client:latest .
 ```
 
@@ -218,14 +293,34 @@
 '<your version, e.g. 0.1.7>'
 ```
 
 This package holds different APIs depending on your application's requirements.
 For more information, see ([Documentation](https://github.com/eclipse/kuksa.val/blob/master/kuksa-client/docs/main.md)).
 
 
+### TLS configuration
+
+Clients like [KUKSA.val CAN Feeder](https://github.com/eclipse/kuksa.val.feeders/tree/main/dbc2val)
+that use KUKSA.val Client library must typically set the path to the root CA certificate.
+If the path is set the VSSClient will try to establish a secure connection.
+
+```
+# Shall TLS be used (default False for Databroker, True for KUKSA.val Server)
+# tls = False
+tls = True
+
+# TLS-related settings
+# Path to root CA, needed if using TLS
+root_ca_path=../../kuksa.val/kuksa_certificates/CA.pem
+# Server name, typically only needed if accessing server by IP address like 127.0.0.1
+# and typically only if connection to KUKSA.val Databroker
+# If using KUKSA.val example certificates the names "Server" or "localhost" can be used.
+# tls_server_name=Server
+```
+
 ## Troubleshooting
 
 1. The server/data broker is listening on its port but my client is unable to connect to it and returns an error:
 ```console
 Error: Websocket could not be connected or the gRPC channel could not be created.
 ```
 If you're running both client and server on your local host, make sure that:
```

### Comparing `kuksa_client-0.4.0a2/kuksa/val/v1/types_pb2.py` & `kuksa_client-0.4.0a3/kuksa/val/v1/types_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa/val/v1/val_pb2.py` & `kuksa_client-0.4.0a3/kuksa/val/v1/val_pb2.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa/val/v1/val_pb2_grpc.py` & `kuksa_client-0.4.0a3/kuksa/val/v1/val_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/CA.key` & `kuksa_client-0.4.0a3/kuksa_certificates/CA.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/CA.pem` & `kuksa_client-0.4.0a3/kuksa_certificates/CA.pem`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/Client.key` & `kuksa_client-0.4.0a3/kuksa_certificates/Client.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/Client.pem` & `kuksa_client-0.4.0a3/kuksa_certificates/Client.pem`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 00000000: 2d2d 2d2d 2d42 4547 494e 2043 4552 5449  -----BEGIN CERTI
-00000010: 4649 4341 5445 2d2d 2d2d 2d0a 4d49 4944  FICATE-----.MIID
-00000020: 787a 4343 4171 2b67 4177 4942 4167 4955  xzCCAq+gAwIBAgIU
-00000030: 5239 3564 3951 3538 4469 7468 5735 3548  R95d9Q58DithW55H
-00000040: 6470 4d79 3237 5148 3235 6f77 4451 594a  dpMy27QH25owDQYJ
+00000010: 4649 4341 5445 2d2d 2d2d 2d0a 4d49 4945  FICATE-----.MIIE
+00000020: 7644 4343 4136 5367 4177 4942 4167 4955  vDCCA6SgAwIBAgIU
+00000030: 6669 6351 7a53 442b 3152 6a77 7651 5142  ficQzSD+1RjwvQQB
+00000040: 7673 336a 4764 7672 6b53 6b77 4451 594a  vs3jGdvrkSkwDQYJ
 00000050: 4b6f 5a49 6876 634e 4151 454c 0a42 5141  KoZIhvcNAQEL.BQA
 00000060: 7767 5a51 7843 7a41 4a42 674e 5642 4159  wgZQxCzAJBgNVBAY
 00000070: 5441 6b4e 424d 5241 7744 6759 4456 5151  TAkNBMRAwDgYDVQQ
 00000080: 4944 4164 5062 6e52 6863 6d6c 764d 5138  IDAdPbnRhcmlvMQ8
 00000090: 7744 5159 4456 5151 4844 415a 500a 6448  wDQYDVQQHDAZP.dH
 000000a0: 5268 6432 4578 4a54 416a 4267 4e56 4241  Rhd2ExJTAjBgNVBA
 000000b0: 6f4d 4845 566a 6247 6c77 6332 5575 6233  oMHEVjbGlwc2Uub3
 000000c0: 4a6e 4945 5a76 6457 356b 5958 5270 6232  JnIEZvdW5kYXRpb2
 000000d0: 3473 4945 6c75 5979 3478 4654 4154 0a42  4sIEluYy4xFTAT.B
 000000e0: 674e 5642 414d 4d44 4778 7659 3246 7361  gNVBAMMDGxvY2Fsa
 000000f0: 4739 7a64 4331 6a59 5445 6b4d 4349 4743  G9zdC1jYTEkMCIGC
 00000100: 5371 4753 4962 3344 5145 4a41 5259 5661  SqGSIb3DQEJARYVa
 00000110: 3356 7263 3245 745a 4756 3251 4756 6a0a  3Vrc2EtZGV2QGVj.
 00000120: 6247 6c77 6332 5575 6233 4a6e 4d42 3458  bGlwc2Uub3JnMB4X
-00000130: 4454 497a 4d44 4d79 4e44 457a 4e44 4177  DTIzMDMyNDEzNDAw
-00000140: 4d6c 6f58 4454 4930 4d44 4d79 4d7a 457a  MloXDTI0MDMyMzEz
-00000150: 4e44 4177 4d6c 6f77 6759 3478 437a 414a  NDAwMlowgY4xCzAJ
+00000130: 4454 497a 4d44 5978 4e6a 4577 4d44 5178  DTIzMDYxNjEwMDQx
+00000140: 4e6c 6f58 4454 4930 4d44 5978 4e54 4577  NloXDTI0MDYxNTEw
+00000150: 4d44 5178 4e6c 6f77 6759 3478 437a 414a  MDQxNlowgY4xCzAJ
 00000160: 0a42 674e 5642 4159 5441 6b4e 424d 5241  .BgNVBAYTAkNBMRA
 00000170: 7744 6759 4456 5151 4944 4164 5062 6e52  wDgYDVQQIDAdPbnR
 00000180: 6863 6d6c 764d 5138 7744 5159 4456 5151  hcmlvMQ8wDQYDVQQ
 00000190: 4844 415a 5064 4852 6864 3245 784a 5441  HDAZPdHRhd2ExJTA
 000001a0: 6a0a 4267 4e56 4241 6f4d 4845 566a 6247  j.BgNVBAoMHEVjbG
 000001b0: 6c77 6332 5575 6233 4a6e 4945 5a76 6457  lwc2Uub3JnIEZvdW
 000001c0: 356b 5958 5270 6232 3473 4945 6c75 5979  5kYXRpb24sIEluYy
@@ -52,35 +52,56 @@
 00000330: 3974 444d 334d 6e34 4446 5957 556d 7078  9tDM3Mn4DFYWUmpx
 00000340: 2f36 7530 3366 4932 4547 3079 644e 4f52  /6u03fI2EG0ydNOR
 00000350: 5965 595a 5242 776c 5937 536a 574c 7432  YeYZRBwlY7SjWLt2
 00000360: 3059 3839 5465 4239 0a79 6c57 4f54 466f  0Y89TeB9.ylWOTFo
 00000370: 2b33 506c 356f 3961 4c41 5a51 5252 2f66  +3Pl5o9aLAZQRR/f
 00000380: 4d4c 6179 5841 412f 2f4e 4632 4156 516a  MLayXAA//NF2AVQj
 00000390: 6144 6272 5663 4450 6e31 6e68 3044 382f  aDbrVcDPn1nh0D8/
-000003a0: 3257 5149 4441 5141 420a 6f78 5577 457a  2WQIDAQAB.oxUwEz
-000003b0: 4152 4267 4e56 4852 4545 436a 4149 6767  ARBgNVHREECjAIgg
-000003c0: 5a44 6247 6c6c 626e 5177 4451 594a 4b6f  ZDbGllbnQwDQYJKo
-000003d0: 5a49 6876 634e 4151 454c 4251 4144 6767  ZIhvcNAQELBQADgg
-000003e0: 4542 414b 4e79 6f75 6d69 0a35 737a 3653  EBAKNyoumi.5sz6S
-000003f0: 5049 4552 7459 696a 514d 6f42 4c4c 4a6a  PIERtYijQMoBLLJj
-00000400: 6953 5049 3930 646c 436b 4150 6756 5378  iSPI90dlCkAPgVSx
-00000410: 4e4e 7930 6861 316d 2b41 496e 7667 664e  NNy0ha1m+AInvgfN
-00000420: 4b5a 4970 6e68 496c 3730 340a 5442 666b  KZIpnhIl704.TBfk
-00000430: 6a2b 7a53 535a 4332 5534 4d75 4841 7a53  j+zSSZC2U4MuHAzS
-00000440: 5655 4964 6a30 7169 6974 5a68 6233 514e  VUIdj0qiitZhb3QN
-00000450: 6548 7655 4959 6648 6b33 3944 5263 4438  eHvUIYfHk39DRcD8
-00000460: 4758 7258 5a59 656a 6c70 7251 0a79 4c6f  GXrXZYejlprQ.yLo
-00000470: 3473 6a66 7069 5747 6262 3141 4178 4f30  4sjfpiWGbb1AAxO0
-00000480: 344e 426a 4859 685a 4869 304d 744e 6b4d  4NBjHYhZHi0MtNkM
-00000490: 4253 526d 6e47 6b53 504b 6936 4d55 4349  BSRmnGkSPKi6MUCI
-000004a0: 3134 626e 7943 7979 7566 6d61 440a 492b  14bnyCyyufmaD.I+
-000004b0: 6433 3257 4643 3048 6435 6a79 4875 4b73  d32WFC0Hd5jyHuKs
-000004c0: 4577 3470 5268 6d64 7955 3033 5038 7545  Ew4pRhmdyU03P8uE
-000004d0: 6438 6766 6133 4439 2b30 6342 3754 584c  d8gfa3D9+0cB7TXL
-000004e0: 4254 756c 4536 4432 694e 3434 6d6b 0a34  BTulE6D2iN44mk.4
-000004f0: 514f 3875 6f71 2f6c 417a 7468 556b 5467  QO8uoq/lAzthUkTg
-00000500: 4f57 5848 6177 7569 4b36 6b62 4269 3137  OWXHawuiK6kbBi17
-00000510: 3436 4a2f 3467 4a5a 7a74 7839 6a44 7247  46J/4gJZztx9jDrG
-00000520: 4a33 4164 4863 756f 3266 4832 3931 610a  J3AdHcuo2fH291a.
-00000530: 3150 3252 3976 5547 4776 416f 4269 303d  1P2R9vUGGvAoBi0=
-00000540: 0a2d 2d2d 2d2d 454e 4420 4345 5254 4946  .-----END CERTIF
-00000550: 4943 4154 452d 2d2d 2d2d 0a              ICATE-----.
+000003a0: 3257 5149 4441 5141 420a 6f34 4942 4344  2WQIDAQAB.o4IBCD
+000003b0: 4343 4151 5177 4967 5944 5652 3052 4242  CCAQQwIgYDVR0RBB
+000003c0: 7377 4759 4947 5132 7870 5a57 3530 6767  swGYIGQ2xpZW50gg
+000003d0: 6c73 6232 4e68 6247 6876 6333 5348 4248  lsb2NhbGhvc3SHBH
+000003e0: 3841 4141 4577 4851 5944 0a56 5230 4f42  8AAAEwHQYD.VR0OB
+000003f0: 4259 4546 4134 6a48 6358 6e66 7135 3757  BYEFA4jHcXnfq57W
+00000400: 2b53 6f32 5a32 7638 7637 6548 6839 414d  +So2Z2v8v7eHh9AM
+00000410: 4947 2b42 674e 5648 534d 4567 6259 7767  IG+BgNVHSMEgbYwg
+00000420: 624f 6867 5a71 6b67 5a63 770a 675a 5178  bOhgZqkgZcw.gZQx
+00000430: 437a 414a 4267 4e56 4241 5954 416b 4e42  CzAJBgNVBAYTAkNB
+00000440: 4d52 4177 4467 5944 5651 5149 4441 6450  MRAwDgYDVQQIDAdP
+00000450: 626e 5268 636d 6c76 4d51 3877 4451 5944  bnRhcmlvMQ8wDQYD
+00000460: 5651 5148 4441 5a50 6448 5268 0a64 3245  VQQHDAZPdHRh.d2E
+00000470: 784a 5441 6a42 674e 5642 416f 4d48 4556  xJTAjBgNVBAoMHEV
+00000480: 6a62 476c 7763 3255 7562 334a 6e49 455a  jbGlwc2Uub3JnIEZ
+00000490: 7664 5735 6b59 5852 7062 3234 7349 456c  vdW5kYXRpb24sIEl
+000004a0: 7559 7934 7846 5441 5442 674e 560a 4241  uYy4xFTATBgNV.BA
+000004b0: 4d4d 4447 7876 5932 4673 6147 397a 6443  MMDGxvY2FsaG9zdC
+000004c0: 316a 5954 456b 4d43 4947 4353 7147 5349  1jYTEkMCIGCSqGSI
+000004d0: 6233 4451 454a 4152 5956 6133 5672 6332  b3DQEJARYVa3Vrc2
+000004e0: 4574 5a47 5632 5147 566a 6247 6c77 0a63  EtZGV2QGVjbGlw.c
+000004f0: 3255 7562 334a 6e67 6852 3932 5132 4570  2Uub3JnghR92Q2Ep
+00000500: 6b68 2b6e 4956 7365 5476 4d37 5870 787a  kh+nIVseTvM7Xpxz
+00000510: 4230 5877 6a41 4e42 676b 7168 6b69 4739  B0XwjANBgkqhkiG9
+00000520: 7730 4241 5173 4641 414f 4341 5145 410a  w0BAQsFAAOCAQEA.
+00000530: 4d67 6c45 6943 636a 3758 5759 5438 4f32  MglEiCcj7XWYT8O2
+00000540: 3153 4562 776c 5054 3942 764c 7441 7766  1SEbwlPT9BvLtAwf
+00000550: 6d37 6133 4e71 4c6f 5750 7468 4a63 4a5a  m7a3NqLoWPthJcJZ
+00000560: 6356 5054 7a75 566a 4d56 3634 4f45 7951  cVPTzuVjMV64OEyQ
+00000570: 0a50 4974 6336 4a55 5a66 7a37 2b70 4833  .PItc6JUZfz7+pH3
+00000580: 6947 436f 4530 6768 7165 7949 6b36 4341  iGCoE0ghqeyIk6CA
+00000590: 5177 5764 4b6b 3672 5571 2b53 7930 7350  QwWdKk6rUq+Sy0sP
+000005a0: 2b6a 6f76 6c53 7370 7065 6c30 4a62 5931  +jovlSsppel0JbY1
+000005b0: 4b0a 7830 4474 5149 5157 7332 5a76 6a53  K.x0DtQIQWs2ZvjS
+000005c0: 724d 4a58 6277 2b50 4c62 3466 597a 332b  rMJXbw+PLb4fYz3+
+000005d0: 7263 3356 4f33 4333 495a 6868 526c 7539  rc3VO3C3IZhhRlu9
+000005e0: 785a 2f71 715a 777a 7035 6a75 6267 3151  xZ/qqZwzp5jubg1Q
+000005f0: 4c62 0a62 336a 5a67 2f73 7552 624e 6645  Lb.b3jZg/suRbNfE
+00000600: 326c 5463 344c 3759 704f 4452 6d6b 6c67  2lTc4L7YpODRmklg
+00000610: 3279 3976 6173 314a 774d 454e 3351 5839  2y9vas1JwMEN3QX9
+00000620: 5536 6f42 7654 5177 436c 4848 5538 7455  U6oBvTQwClHHU8tU
+00000630: 3636 610a 4c4f 3938 7149 4441 6b5a 315a  66a.LO98qIDAkZ1Z
+00000640: 426a 5a6e 2b74 5963 496a 4337 4b62 5343  BjZn+tYcIjC7KbSC
+00000650: 6378 466c 4867 5761 2b37 4f62 4a70 3349  cxFlHgWa+7ObJp3I
+00000660: 564b 3248 526e 4545 4266 3558 576d 6978  VK2HRnEEBf5XWmix
+00000670: 6777 4b45 0a58 584f 5533 7351 3541 446f  gwKE.XXOU3sQ5ADo
+00000680: 4e4d 4545 554f 7a72 4b31 413d 3d0a 2d2d  NMEEUOzrK1A==.--
+00000690: 2d2d 2d45 4e44 2043 4552 5449 4649 4341  ---END CERTIFICA
+000006a0: 5445 2d2d 2d2d 2d0a                      TE-----.
```

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/Server.key` & `kuksa_client-0.4.0a3/kuksa_certificates/Server.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/jwt/all-read-write.json.token` & `kuksa_client-0.4.0a3/kuksa_certificates/jwt/all-read-write.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/jwt/createToken.py` & `kuksa_client-0.4.0a3/kuksa_certificates/jwt/createToken.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/jwt/jwt.key` & `kuksa_client-0.4.0a3/kuksa_certificates/jwt/jwt.key`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/jwt/jwt.key.pub` & `kuksa_client-0.4.0a3/kuksa_certificates/jwt/jwt.key.pub`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/jwt/recreateJWTkeyPair.sh` & `kuksa_client-0.4.0a3/kuksa_certificates/jwt/recreateJWTkeyPair.sh`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/jwt/single-read.json.token` & `kuksa_client-0.4.0a3/kuksa_certificates/jwt/single-read.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_certificates/jwt/super-admin.json.token` & `kuksa_client-0.4.0a3/kuksa_certificates/jwt/super-admin.json.token`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_client/__init__.py` & `kuksa_client-0.4.0a3/kuksa_client/__init__.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_client/__main__.py` & `kuksa_client-0.4.0a3/kuksa_client/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 # SPDX-License-Identifier: Apache-2.0
 ########################################################################
 
 import argparse
 import functools
 import json
 import logging.config
+import logging
 import os
 import pathlib
 import sys
 import threading
 import time
 
 from pygments import highlight
@@ -44,14 +45,17 @@
 DEFAULT_SERVER_PORT = 8090
 DEFAULT_SERVER_PROTOCOL = "ws"
 SUPPORTED_SERVER_PROTOCOLS = ("ws", "grpc")
 
 scriptDir = os.path.dirname(os.path.realpath(__file__))
 
 
+logger = logging.getLogger(__name__)
+
+
 def assignment_statement(arg):
     path, value = arg.split('=', maxsplit=1)
     return (path, value)
 
 
 # pylint: disable=too-many-instance-attributes
 # pylint: disable=too-many-public-methods
@@ -161,15 +165,15 @@
         help='VISS/gRPC Server Communication Protocol (ws or grpc)',
         default=DEFAULT_SERVER_PROTOCOL,
     )
 
     ap_setValue = argparse.ArgumentParser()
     ap_setValue.add_argument(
         "Path", help="Path to be set", completer_method=path_completer)
-    ap_setValue.add_argument("Value", help="Value to be set")
+    ap_setValue.add_argument("Value", nargs='+', help="Value to be set")
     ap_setValue.add_argument(
         "-a", "--attribute", help="Attribute to be set", default="value")
 
     ap_setValues = argparse.ArgumentParser()
     ap_setValues.add_argument(
         "Path=Value",
         help="Path and new value this path is to be set with",
@@ -243,16 +247,18 @@
 
     ap_updateVSSTree = argparse.ArgumentParser()
     jsonfile_completer_method = functools.partial(Cmd.path_complete,
                                                   path_filter=lambda path: (os.path.isdir(path) or path.endswith(".json")))
     ap_updateVSSTree.add_argument(
         "Json", help="Json tree to update VSS", completer_method=jsonfile_completer_method)
 
-    # Constructor
-    def __init__(self, server_ip=None, server_port=None, server_protocol=None, insecure=False, token_or_tokenfile=None):
+    # Constructor, request names after protocol to avoid errors
+    def __init__(self, server_ip=None, server_port=None, server_protocol=None, *, insecure=False, token_or_tokenfile=None,
+                 certificate=None, keyfile=None,
+                 cacertificate=None, tls_server_name=None):
         super().__init__(
             persistent_history_file=".vssclient_history", persistent_history_length=100, allow_cli_args=False,
         )
 
         self.prompt = "Test Client> "
         self.max_completion_items = 20
         self.serverIP = server_ip or DEFAULT_SERVER_ADDR
@@ -261,14 +267,18 @@
         self.supportedProtocols = SUPPORTED_SERVER_PROTOCOLS
         self.vssTree = {}
         self.pathCompletionItems = []
         self.subscribeIds = set()
         self.commThread = None
         self.token_or_tokenfile = token_or_tokenfile
         self.insecure = insecure
+        self.certificate = certificate
+        self.keyfile = keyfile
+        self.cacertificate = cacertificate
+        self.tls_server_name = tls_server_name
 
         print("Welcome to Kuksa Client version " + str(_metadata.__version__))
         print()
         with (pathlib.Path(scriptDir) / 'logo').open('r', encoding='utf-8') as f:
             print(f.read())
         print("Default tokens directory: " + self.getDefaultTokenDir())
 
@@ -287,16 +297,17 @@
                     formatters.TerminalFormatter()))
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setValue)
     def do_setValue(self, args):
         """Set the value of a path"""
         if self.checkConnection():
+            value = str(' '.join(args.Value))
             resp = self.commThread.setValue(
-                args.Path, args.Value, args.attribute)
+                args.Path, value, args.attribute)
             print(highlight(resp, lexers.JsonLexer(),
                   formatters.TerminalFormatter()))
         self.pathCompletionItems = []
 
     @with_category(VSS_COMMANDS)
     @with_argparser(ap_setValues)
     def do_setValues(self, args):
@@ -480,17 +491,29 @@
         if hasattr(self, "commThread"):
             if self.commThread is not None:
                 self.commThread.stop()
                 self.commThread = None
         config = {'ip': self.serverIP,
                   'port': self.serverPort,
                   'insecure': self.insecure,
-                  'protocol': self.serverProtocol,
-                  'token_or_tokenfile': self.token_or_tokenfile,
+                  'protocol': self.serverProtocol
                   }
+                  
+        # Configs should only be added if they actually have a value
+        if self.token_or_tokenfile:
+            config['token_or_tokenfile'] = self.token_or_tokenfile
+        if self.certificate:
+            config['certificate'] = self.certificate
+        if self.keyfile:
+            config['keyfile'] = self.keyfile
+        if self.cacertificate:
+            config['cacertificate'] = self.cacertificate
+        if self.tls_server_name:
+            config['tls_server_name'] = self.tls_server_name
+            
         self.commThread = KuksaClientThread(config)
         self.commThread.start()
 
         waitForConnection = threading.Condition()
         waitForConnection.acquire()
         waitForConnection.wait_for(self.commThread.checkConnection, timeout=1)
         waitForConnection.release()
@@ -584,19 +607,42 @@
                         action='store_true', help='Connect in insecure mode')
     parser.add_argument(
         '--logging-config', default=os.path.join(scriptDir, 'logging.ini'), help="Path to logging configuration file",
     )
     parser.add_argument(
         '--token_or_tokenfile', default=None, help="JWT token or path to a JWT token file (.token)",
     )
+    
+    # Add TLS arguments
+    # Note: Databroker does not yet support mutual authentication, so no need to use two first arguments
+    parser.add_argument(
+        '--certificate', default=None, help="Client cert file(.pem), only needed for mutual authentication",
+    )
+    parser.add_argument(
+        '--keyfile', default=None, help="Client private key file (.key), only needed for mutual authentication",
+    )
+    parser.add_argument(
+        '--cacertificate', default=None, help="Client root cert file (.pem), needed unless insecure mode used",
+    )
+    # Observations for Python
+    # Connecting to "localhost" works well, subjectAltName seems to suffice
+    # Connecting to "127.0.0.1" does not work unless server-name specified
+    # For KUKSA.val example certs default name is "Server"
+    parser.add_argument(
+        '--tls-server-name', default=None, help="CA name of server, needed in some cases where subjectAltName does not suffice",
+    )
+    
     args = parser.parse_args()
 
     logging.config.fileConfig(args.logging_config)
+    
     clientApp = TestClient(args.ip, args.port, args.protocol,
-                           args.insecure, args.token_or_tokenfile)
+                           insecure = args.insecure, token_or_tokenfile = args.token_or_tokenfile,
+                           certificate = args.certificate, keyfile = args.keyfile,
+                           cacertificate = args.cacertificate, tls_server_name = args.tls_server_name)
     try:
         # We exit the loop when the user types "quit" or hits Ctrl-D.
         clientApp.cmdloop()
     finally:
         clientApp.stop()
```

### Comparing `kuksa_client-0.4.0a2/kuksa_client/_metadata.py` & `kuksa_client-0.4.0a3/kuksa_client/_metadata.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_client/cli_backend/__init__.py` & `kuksa_client-0.4.0a3/kuksa_client/cli_backend/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,29 +17,31 @@
 ########################################################################
 
 import pathlib
 
 import kuksa_certificates
 
 
+
 class Backend:
     def __init__(self, config):
         self.serverIP = config.get('ip', "127.0.0.1")
         self.serverPort = config.get('port', 8090)
         try:
             self.insecure = config.getboolean('insecure', False)
         except AttributeError:
             self.insecure = config.get('insecure', False)
         self.default_cert_path = pathlib.Path(kuksa_certificates.__path__[0])
         self.cacertificate = config.get(
             'cacertificate', str(self.default_cert_path / 'CA.pem'))
         self.certificate = config.get('certificate', str(
             self.default_cert_path / 'Client.pem'))
-        self.keyfile = config.get('key', str(
+        self.keyfile = config.get('keyfile', str(
             self.default_cert_path / 'Client.key'))
+        self.tls_server_name = config.get('tls_server_name', "")
         self.token_or_tokenfile = config.get('token_or_tokenfile', str(
             self.default_cert_path / 'jwt/all-read-write.json.token'))
 
     @staticmethod
     def from_config(config):
         protocol = config.get('protocol', 'ws')
```

### Comparing `kuksa_client-0.4.0a2/kuksa_client/cli_backend/grpc.py` & `kuksa_client-0.4.0a3/kuksa_client/cli_backend/grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,26 +23,37 @@
 import queue
 from typing import Any
 from typing import Callable
 from typing import Dict
 from typing import Iterable
 import uuid
 import os
+import re
 
 from kuksa_client import cli_backend
 import kuksa_client.grpc
 import kuksa_client.grpc.aio
 from kuksa_client.grpc import EntryUpdate
-
+from kuksa.val.v1 import types_pb2
 
 def callback_wrapper(callback: Callable[[str], None]) -> Callable[[Iterable[EntryUpdate]], None]:
     def wrapper(updates: Iterable[EntryUpdate]) -> None:
         callback(json.dumps([update.to_dict() for update in updates]))
     return wrapper
 
+class DatabrokerEncoder(json.JSONEncoder):
+    def default(self, obj):
+        if isinstance(obj, (types_pb2.StringArray, types_pb2.BoolArray, types_pb2.Uint32Array, types_pb2.Uint64Array, types_pb2.FloatArray, types_pb2.Int32Array, types_pb2.Int64Array, types_pb2.DoubleArray)):
+            string_values = []
+            for value in obj.values:
+                value = str(value)
+                string_values.append(value)
+            return {'values': string_values}
+        return super().default(obj)
+
 
 class Backend(cli_backend.Backend):
     def __init__(self, config):
         super().__init__(config)
         self.cacertificate = pathlib.Path(self.cacertificate)
         self.keyfile = pathlib.Path(self.keyfile)
         self.certificate = pathlib.Path(self.certificate)
@@ -104,14 +115,15 @@
         return self.setValues({path: value}, attribute, timeout)
 
     def setValues(self, updates: Dict[str, Any], attribute="value", timeout=5):
         if attribute in self.AttrDict:
             field, _ = self.AttrDict[attribute]
             entry_updates = []
             for path, value in updates.items():
+
                 if field is kuksa_client.grpc.Field.VALUE:
                     entry = kuksa_client.grpc.DataEntry(
                         path=path, value=kuksa_client.grpc.Datapoint(value=value))
                 elif field is kuksa_client.grpc.Field.ACTUATOR_TARGET:
                     entry = kuksa_client.grpc.DataEntry(
                         path=path, actuator_target=kuksa_client.grpc.Datapoint(
                             value=value),
@@ -187,15 +199,15 @@
         recvQueue = queue.Queue(maxsize=1)
         self.sendMsgQueue.put((call, requestArgs, recvQueue))
         try:
             resp, error = recvQueue.get(timeout=timeout)
             if error:
                 respJson = json.dumps(error, indent=4)
             elif resp:
-                respJson = json.dumps(resp, indent=4)
+                respJson = json.dumps(resp, indent=4, cls=DatabrokerEncoder)
             else:
                 respJson = "OK"
         except queue.Empty:
             respJson = json.dumps({"error": "Timeout"})
         return respJson
 
     # Async function to handle the gRPC calls
@@ -254,11 +266,12 @@
         else:
             async with kuksa_client.grpc.aio.VSSClient(
                 self.serverIP,
                 self.serverPort,
                 root_certificates=self.cacertificate,
                 private_key=self.keyfile,
                 certificate_chain=self.certificate,
+                tls_server_name=self.tls_server_name,
                 token=self.token
             ) as vss_client:
                 print("Secure gRPC channel connected.")
                 await self._grpcHandler(vss_client)
```

### Comparing `kuksa_client-0.4.0a2/kuksa_client/cli_backend/ws.py` & `kuksa_client-0.4.0a3/kuksa_client/cli_backend/ws.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 import time
 import uuid
 
 import websockets
 
 from kuksa_client import cli_backend
 
-
 class Backend(cli_backend.Backend):
     def __init__(self, config):
         super().__init__(config)
         self.wsConnected = False
 
         self.subscriptionCallbacks = {}
         self.sendMsgQueue = queue.Queue()
@@ -231,20 +230,28 @@
 
     async def connect(self):
         if not self.insecure:
             context = ssl.create_default_context()
             context.load_cert_chain(
                 certfile=self.certificate, keyfile=self.keyfile)
             context.load_verify_locations(cafile=self.cacertificate)
-            # Certificates in ../kuksa_certificates does not contain the IP address used for
-            # connection to server so hostname check must be disabled
-            context.check_hostname = False
+            # We want host name to match
+            # For example certificates we use subjectAltName to make it match for Server, localahost and 127.0.0.1
+            # If using your own certificates make sure that name is included or use tls_server_name work-around
+            context.check_hostname = True
             try:
                 print("connect to wss://"+self.serverIP+":"+str(self.serverPort))
-                async with websockets.connect("wss://"+self.serverIP+":"+str(self.serverPort), ssl=context) as ws:
+                args = {'uri':"wss://"+self.serverIP+":"+str(self.serverPort),'ssl':context}
+                # If your certificates does not contain the name of the server 
+                # (for example during testing, in production it should match)
+                # then you can specify that checks should be against a different name
+                if self.tls_server_name:
+                    args['server_hostname'] = self.tls_server_name
+
+                async with websockets.connect(**args) as ws:
                     print("Websocket connected securely.")
                     await self._msgHandler(ws)
             except OSError as e:
                 print("Disconnected!! " + str(e))
         else:
             try:
                 print("connect to ws://"+self.serverIP+":"+str(self.serverPort))
```

### Comparing `kuksa_client-0.4.0a2/kuksa_client/grpc/__init__.py` & `kuksa_client-0.4.0a3/kuksa_client/grpc/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import contextlib
 import dataclasses
 import datetime
 import enum
 import http
 import logging
+import re
 from typing import Any
 from typing import Collection
 from typing import Dict
 from typing import Iterable
 from typing import Iterator
 from typing import List
 from typing import Optional
@@ -35,15 +36,14 @@
 import grpc
 from grpc import RpcError
 
 from kuksa.val.v1 import types_pb2
 from kuksa.val.v1 import val_pb2
 from kuksa.val.v1 import val_pb2_grpc
 
-
 logger = logging.getLogger(__name__)
 
 
 class DataType(enum.IntEnum):
     UNSPECIFIED = types_pb2.DATA_TYPE_UNSPECIFIED
     STRING = types_pb2.DATA_TYPE_STRING
     BOOLEAN = types_pb2.DATA_TYPE_BOOLEAN
@@ -320,35 +320,48 @@
 
         def set_array_attr(obj, attr, values):
             array = getattr(obj, attr)
             array.Clear()
             array.values.extend(values)
 
         def cast_array_values(cast, array):
-            for item in array:
-                yield cast(item)
+            array = array.strip('[]')
+            pattern = r'(?:\\.|[^",])*"(?:\\.|[^"])*"|[^",]+'
+            values = re.findall(pattern, array)
+            for item in values:
+                if item == '':
+                    #skip
+                    pass
+                else:
+                    if cast == str:
+                        item = item.replace('\"', '').replace('\\', '"').strip()
+                    yield cast(item)
 
         def cast_bool(value):
             if value in ('False', 'false', 'F', 'f'):
                 value = 0
             return bool(value)
+        
+        def cast_str(value):
+            return str(value).replace('\"', '').replace('\\', '"').strip()
+            
 
         field, set_field, cast_field = {
             DataType.INT8: ('int32', setattr, int),
             DataType.INT16: ('int32', setattr, int),
             DataType.INT32: ('int32', setattr, int),
             DataType.UINT8: ('uint32', setattr, int),
             DataType.UINT16: ('uint32', setattr, int),
             DataType.UINT32: ('uint32', setattr, int),
             DataType.UINT64: ('uint64', setattr, int),
             DataType.INT64: ('int64', setattr, int),
             DataType.FLOAT: ('float', setattr, float),
             DataType.DOUBLE: ('double', setattr, float),
             DataType.BOOLEAN: ('bool', setattr, cast_bool),
-            DataType.STRING: ('string', setattr, str),
+            DataType.STRING: ('string', setattr, cast_str),
             DataType.INT8_ARRAY: ('int32_array', set_array_attr, lambda array: cast_array_values(int, array)),
             DataType.INT16_ARRAY: ('int32_array', set_array_attr, lambda array: cast_array_values(int, array)),
             DataType.INT32_ARRAY: ('int32_array', set_array_attr, lambda array: cast_array_values(int, array)),
             DataType.UINT8_ARRAY: ('uint32_array', set_array_attr, lambda array: cast_array_values(int, array)),
             DataType.UINT16_ARRAY: ('uint32_array', set_array_attr, lambda array: cast_array_values(int, array)),
             DataType.UINT32_ARRAY: ('uint32_array', set_array_attr, lambda array: cast_array_values(int, array)),
             DataType.UINT64_ARRAY: ('uint64_array', set_array_attr, lambda array: cast_array_values(int, array)),
@@ -464,43 +477,55 @@
     name: str
     version: str
 
     @classmethod
     def from_message(cls, message: val_pb2.GetServerInfoResponse):
         return cls(name=message.name, version=message.version)
 
-
 class BaseVSSClient:
     def __init__(
         self,
         host: str,
         port: int,
-        token: str = None,
+        token: Optional[str] = None,
         root_certificates: Optional[Path] = None,
         private_key: Optional[Path] = None,
         certificate_chain: Optional[Path] = None,
         ensure_startup_connection: bool = True,
         connected: bool = False,
+        tls_server_name: Optional[str] = None
     ):
+    
+
         self.authorization_header = self.get_authorization_header(token)
         self.target_host = f'{host}:{port}'
         self.root_certificates = root_certificates
         self.private_key = private_key
         self.certificate_chain = certificate_chain
+        self.tls_server_name = tls_server_name
         self.ensure_startup_connection = ensure_startup_connection
         self.connected = connected
         self.client_stub = None
 
     def _load_creds(self) -> Optional[grpc.ChannelCredentials]:
-        if all((self.root_certificates, self.private_key, self.certificate_chain)):
+        if self.root_certificates:
+            logger.info(f"Using TLS with Root CA from {self.root_certificates}")
             root_certificates = self.root_certificates.read_bytes()
-            private_key = self.private_key.read_bytes()
-            certificate_chain = self.certificate_chain.read_bytes()
-            return grpc.ssl_channel_credentials(root_certificates, private_key, certificate_chain)
+            if self.private_key and self.certificate_chain:
+                private_key = self.private_key.read_bytes()
+                certificate_chain = self.certificate_chain.read_bytes()
+                logger.info(f"Using private client key {self.private_key} "
+                                 f"and chain/certificate {self.certificate_chain}")
+                return grpc.ssl_channel_credentials(root_certificates, private_key, certificate_chain)
+            else:
+                logger.info(f"No client certificates provided, mutual TLS not supported!")
+                return grpc.ssl_channel_credentials(root_certificates)
+        logger.warning(f"No Root CA present!")
         return None
+        
 
     def _prepare_get_request(self, entries: Iterable[EntryRequest]) -> val_pb2.GetRequest:
         req = val_pb2.GetRequest(entries=[])
         for entry in entries:
             entry_request = val_pb2.EntryRequest(
                 path=entry.path, view=entry.view.value, fields=[])
             for field in entry.fields:
@@ -615,18 +640,28 @@
                     "Disconnected from server! Try connect.")
         return wrapper
 
     def connect(self, target_host=None):
         creds = self._load_creds()
         if target_host is None:
             target_host = self.target_host
+            
         if creds is not None:
-            channel = grpc.secure_channel(target_host, creds)
+            logger.info("Establishing secure channel")
+            if self.tls_server_name:
+                logger.info(f"Using TLS server name {self.tls_server_name}")
+                options = [('grpc.ssl_target_name_override', self.tls_server_name)]
+                channel = grpc.secure_channel(target_host, creds, options)
+            else:
+                logger.debug(f"Not providing explicit TLS server name")
+                channel = grpc.secure_channel(target_host, creds)
         else:
+            logger.info("Establishing insecure channel")
             channel = grpc.insecure_channel(target_host)
+            
         self.channel = self.exit_stack.enter_context(channel)
         self.client_stub = val_pb2_grpc.VALStub(self.channel)
         self.connected = True
         if self.ensure_startup_connection:
             logger.debug("Connected to server: %s", self.get_server_info())
 
     def disconnect(self):
```

### Comparing `kuksa_client-0.4.0a2/kuksa_client/grpc/aio.py` & `kuksa_client-0.4.0a3/kuksa_client/grpc/aio.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,16 +64,24 @@
         await self.disconnect()
 
     async def connect(self, target_host=None):
         creds = self._load_creds()
         if target_host is None:
             target_host = self.target_host
         if creds is not None:
-            channel = grpc.aio.secure_channel(target_host, creds)
+            logger.info("Establishing secure channel")
+            if self.tls_server_name:
+                logger.info(f"Using TLS server name {self.tls_server_name}")
+                options = [('grpc.ssl_target_name_override', self.tls_server_name)]
+                channel = grpc.aio.secure_channel(target_host, creds, options)
+            else:
+                logger.debug(f"Not providing explicit TLS server name")
+                channel = grpc.aio.secure_channel(target_host, creds)
         else:
+            logger.info("Establishing insecure channel")
             channel = grpc.aio.insecure_channel(target_host)
         self.channel = await self.exit_stack.enter_async_context(channel)
         self.client_stub = val_pb2_grpc.VALStub(self.channel)
         self.connected = True
         if self.ensure_startup_connection:
             logger.debug("Connected to server: %s", await self.get_server_info())
```

### Comparing `kuksa_client-0.4.0a2/kuksa_client/logo` & `kuksa_client-0.4.0a3/kuksa_client/logo`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/kuksa_client.egg-info/PKG-INFO` & `kuksa_client-0.4.0a3/kuksa_client.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kuksa-client
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: kuksa.val python clients and SDK
 Home-page: https://github.com/eclipse/kuksa.val
 Author: Sebastian Schildt, Naresh Nayak, Wenwen Chen
 Author-email: sebastian.schildt@de.bosch.com, naresh.nayak@de.bosch.com, wenwen.chen@de.bosch.com
 Project-URL: Source, https://github.com/eclipse/kuksa.val/tree/master/kuksa-client
 Project-URL: Bug Tracker, https://github.com/eclipse/kuksa.val/issues
 Classifier: Intended Audience :: Developers
@@ -13,32 +13,31 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
-License-File: LICENSE
 
-# Kuksa Client
+# KUKSA.val Client
 ![kuksa.val Logo](https://raw.githubusercontent.com/eclipse/kuksa.val/0.2.5/doc/pictures/logo.png)
 
-`kuksa.val` is a part of the opensource project [eclipse kuksa](https://www.eclipse.org/kuksa/).
+`kuksa.val` is a part of the opensource project [Eclipse Kuksa](https://www.eclipse.org/kuksa/).
 More about `kuksa.val` can be found in the [repository](https://github.com/eclipse/kuksa.val).
 
 ## Introduction
 
-`kuksa-client` provides both a command-line interface (CLI) and a standalone library to interact with either
-[KUKSA.val server](https://github.com/eclipse/kuksa.val/tree/master/kuksa-val-server) or
-[KUKSA databroker](https://github.com/eclipse/kuksa.val/tree/master/kuksa_databroker).
+KUKSA.val Client provides both a command-line interface (CLI) and a standalone library to interact with either
+[KUKSA.val Server](https://github.com/eclipse/kuksa.val/tree/master/kuksa-val-server) or
+[KUKSA.val Databroker](https://github.com/eclipse/kuksa.val/tree/master/kuksa_databroker).
 
 
 ## Installing the client and starting its CLI
 
-The fastest way to start using kuksa-client is to install a pre-built version from pypi.org:
+The fastest way to start using KUKSA.val Client is to install a pre-built version from pypi.org:
 
 ```console
 $ pip install kuksa-client
 ```
 
 If you want to install from sources instead see [Building and running a local version](#building-and-running-a-local-version).
 
@@ -48,17 +47,16 @@
 $ kuksa-client
 ```
 
 With default CLI arguments, the client will try to connect to a local VISS server e.g. `kuksa-val-server`.
 If you wish to connect to a gRPC server e.g. `kuksa-databroker`, you should instead run:
 
 ```console
-$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc --insecure
+$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc
 ```
-Note: `--insecure` is required because `kuksa-databroker` does not yet support encryption or authentication.
 
 If everything works as expected and the server can be contacted you will get an output similar to below.
 
 
 ```console
 Welcome to Kuksa Client version <some_version>
 
@@ -78,64 +76,139 @@
 Default tokens directory: /some/path/kuksa_certificates/jwt
 
 connectj to wss://127.0.0.1:8090
 Websocket connected securely.
 Test Client>
 ```
 
-The next step is to authorize against the server.
-The jwt tokens for testing can either be found under [kuksa_certificates/jwt](https://github.com/eclipse/kuksa.val/tree/0.2.5/kuksa_certificates/jwt) or you can also use following command inside `kuksa-client` to find the via `pip` installed certificate directory.
+If the connected KUKSA.val Server or KUKSA.val Databroker require authorization the next step is to authorize.
+KUKSA.val Server and KUKSA.val Databroker use different token formats.
+
+### Authorizing against KUKSA.val Server
+
+The jwt tokens for testing can either be found under [../kuksa_certificates/jwt](../kuksa_certificates/jwt)
+or you can also use following command inside `kuksa-client` to find the via `pip` installed certificate directory.
 
 ```console
 Test Client> printTokenDir
 ```
-Select one of the tokens and use the `authorize` command like below.
+Select one of the tokens and use the `authorize` command like below:
 
 ```console
 Test Client> authorize /some/path/kuksa_certificates/jwt/super-admin.json.token
 ```
 
+### Authorizing against KUKSA.val Databroker
+
+If connecting to Databroker the command `printTokenDir` is not much help as it shows the default token directories
+for KUKSA.val Server example tokens. If the KUKSA.val Databroker use default example tokens then one of the
+tokens in [../jwt](../jwt) can be used, like in the example below:
+
+```console
+Test Client> authorize /some/path/jwt/provide-all.token
+```
+
+## Using TLS
+
+KUKSA.val Client use TLS by default, it only run in insecure mode if `--insecure` is given as argument.
+
+By default the KUKSA.val example Root CA and Client keys are used, but client keys have no effect as mutual authentication is not supported by KUKSA.val Databroker or KUKSA.val Server.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc
+```
+
+This call with all parameters specified give same effect:
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc --certificate ../kuksa_certificates/Client.pem --keyfile ../kuksa_certificates/Client.key --cacertificate ./kuksa_certificates/CA.pem
+```
+
+There is actually no reason to specify client key and certificate, as mutual authentication is not supported in KUKSA.val Databroker,
+so the command can be simplified like this:
+
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip localhost --port 55555 --protocol grpc --cacertificate ./kuksa_certificates/CA.pem
+```
+
+The example server protocol list 127.0.0.1 as an alternative name, but the TLS-client currently used does not accept it,
+instead a valid server name must be given as argument.
+Currently `Server` and `localhost`are valid names from the example certificates.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client --ip 127.0.0.1 --port 55555 --protocol grpc  --cacertificate ../kuksa_certificates/CA.pem --tls-server-name Server
+```
+
+### Connecting to KUKSA.val Server
+
+Connecting to KUKSA.val Server is default, and TLS is used by default by KUKSA.val Server.
+`--tls-server-name` does not need to be used when connecting to KUKSA.val Server,
+that is the only difference compared to connecting to KUKSA.val Databroker.
+
+```
+~/kuksa.val/kuksa-client$ kuksa-client
+```
+
+This corresponds to this call:
+
+```
+kuksa-client --ip 127.0.0.1 --port 8090 --protocol ws --cacertificate ./kuksa_certificates/CA.pem
+```
+
 ## Usage Instructions
 
 Refer help for further information
+
 ```console
-VSS Client> help -v
+Test Client> help -v
 
 Documented commands (use 'help -v' for verbose/'help <topic>' for details):
 
 Communication Set-up Commands
 ================================================================================
 authorize           Authorize the client to interact with the server
 connect
-disconnect          Disconnect from the VSS Server
-getServerAddress    Gets the IP Address for the VSS Server
-setServerAddress    Sets the IP Address for the VSS Server
+disconnect          Disconnect from the VISS/gRPC Server
+getServerAddress    Gets the IP Address for the VISS/gRPC Server
+setServerAddress    Sets the IP Address for the VISS/gRPC Server
 
 Info Commands
 ================================================================================
 info                Show summary info of the client
 printTokenDir       Show token directory
 version             Show version of the client
 
 Kuksa Interaction Commands
 ================================================================================
-getMetaData         Get MetaData of the path
-getValue            Get the value of a path
-setValue            Set the value of a path
-updateMetaData      Update MetaData of a given path
-updateVSSTree      Update VSS Tree Entry
+getMetaData          Get MetaData of the path
+getTargetValue       Get the value of a path
+getTargetValues      Get the value of given paths
+getValue             Get the value of a path
+getValues            Get the value of given paths
+setTargetValue       Set the target value of a path
+setTargetValues      Set the target value of given paths
+setValue             Set the value of a path
+setValues            Set the value of given paths
+subscribe            Subscribe the value of a path
+subscribeMultiple    Subscribe to updates of given paths
+unsubscribe          Unsubscribe an existing subscription
+updateMetaData       Update MetaData of a given path
+updateVSSTree        Update VSS Tree Entry
+
 ```
 
 This is an example showing how some of the commands can be used:
 
-![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/0.2.5/doc/pictures/testclient_basic.gif "test client usage")
+![try kuksa-client out](https://raw.githubusercontent.com/eclipse/kuksa.val/master/doc/pictures/testclient_basic.gif "test client usage")
 
 ### Updating VSS Structure
 
-Using the testclient, it is also possible to update and extend the VSS data structure. More details can be found [here](https://github.com/eclipse/kuksa.val/blob/0.2.5/doc/liveUpdateVSSTree.md).
+Using the test client, it is also possible to update and extend the VSS data structure.
+More details can be found [here](https://github.com/eclipse/kuksa.val/blob/master/doc/KUKSA.val_server/liveUpdateVSSTree.md).
 
 **Note**: You can also use `setValue` to change the value of an array, but the value should not contains any non-quoted spaces. Consider the following examples:
 
 ```console
 Test Client> setValue Vehicle.OBD.DTCList ["dtc1","dtc2"]
 {
     "action": "set",
@@ -151,15 +224,14 @@
 }
 
 Test Client> setValue Vehicle.OBD.DTCList ["dtc1", "dtc2"]
 usage: setValue [-h] Path Value
 setValue: error: unrecognized arguments: dtc2 ]
 ```
 
-
 ## Building and running a local version
 
 For development purposes it may be necessary to customize the code for the client and run a locally built version.
 First we suggest you create a dedicated [python virtual environment](https://docs.python.org/3/library/venv.html) for kuksa-client:
 
 ```console
 $ mkdir --parents ~/.venv
@@ -188,15 +260,17 @@
 Whenever you want to exit kuksa-client's virtual environment, simply run:
 ```console
 (kuksa-client) $ deactivate
 $
 ```
 
 ## Using Docker
-You can build a docker image of the testclient using the [`Dockerfile`](./Dockerfile). Not the most effcient way to pack a small python script, but it is easy to get started. The Dockerfile needs to be executed on the parent directory (so it include the needed certificates and `pip` package configuration).
+You can build a docker image of the testclient using the [`Dockerfile`](./Dockerfile).
+Not the most effcient way to pack a small python script, but it is easy to get started.
+The Dockerfile needs to be executed on the parent directory (so it include the needed certificates and `pip` package configuration).
 
 
 ```console
 $ cd /some/dir/kuksa.val
 $ docker build -f kuksa-client/Dockerfile -t kuksa-client:latest .
 ```
 
@@ -239,14 +313,34 @@
 '<your version, e.g. 0.1.7>'
 ```
 
 This package holds different APIs depending on your application's requirements.
 For more information, see ([Documentation](https://github.com/eclipse/kuksa.val/blob/master/kuksa-client/docs/main.md)).
 
 
+### TLS configuration
+
+Clients like [KUKSA.val CAN Feeder](https://github.com/eclipse/kuksa.val.feeders/tree/main/dbc2val)
+that use KUKSA.val Client library must typically set the path to the root CA certificate.
+If the path is set the VSSClient will try to establish a secure connection.
+
+```
+# Shall TLS be used (default False for Databroker, True for KUKSA.val Server)
+# tls = False
+tls = True
+
+# TLS-related settings
+# Path to root CA, needed if using TLS
+root_ca_path=../../kuksa.val/kuksa_certificates/CA.pem
+# Server name, typically only needed if accessing server by IP address like 127.0.0.1
+# and typically only if connection to KUKSA.val Databroker
+# If using KUKSA.val example certificates the names "Server" or "localhost" can be used.
+# tls_server_name=Server
+```
+
 ## Troubleshooting
 
 1. The server/data broker is listening on its port but my client is unable to connect to it and returns an error:
 ```console
 Error: Websocket could not be connected or the gRPC channel could not be created.
 ```
 If you're running both client and server on your local host, make sure that:
```

### Comparing `kuksa_client-0.4.0a2/kuksa_client.egg-info/SOURCES.txt` & `kuksa_client-0.4.0a3/kuksa_client.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 ./README.md
 kuksa/__init__.py
```

### Comparing `kuksa_client-0.4.0a2/pyproject.toml` & `kuksa_client-0.4.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/setup.cfg` & `kuksa_client-0.4.0a3/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -23,16 +23,15 @@
 [options]
 python_requires = >=3.8
 install_requires = 
 	websockets >= 10.1
 	cmd2 >= 1.4, <2.0
 	pygments >= 2.5
 	importlib_metadata >= 3.6 ; python_version < "3.8"
-	grpcio >= 1.46.0
-	grpcio-tools >= 1.46.0
+	grpcio-tools >= 1.54.2
 	jsonpath-ng >= 1.5.3
 packages = find:
 
 [options.extras_require]
 test = 
 	pylint
 	pytest
```

### Comparing `kuksa_client-0.4.0a2/setup.py` & `kuksa_client-0.4.0a3/setup.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/tests/conftest.py` & `kuksa_client-0.4.0a3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kuksa_client-0.4.0a2/tests/test_grpc.py` & `kuksa_client-0.4.0a3/tests/test_grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         (DataType.BOOLEAN, ('False',), types_pb2.Datapoint(bool=False)),
         (DataType.BOOLEAN, ('false',), types_pb2.Datapoint(bool=False)),
         (DataType.BOOLEAN, ('F',), types_pb2.Datapoint(bool=False)),
         (DataType.BOOLEAN, ('f',), types_pb2.Datapoint(bool=False)),
         (DataType.BOOLEAN, (True, datetime.datetime(2022, 11, 16, tzinfo=datetime.timezone.utc)), types_pb2.Datapoint(
             bool=True, timestamp=timestamp_pb2.Timestamp(seconds=1668556800),
         )),
-        (DataType.INT8_ARRAY, ([-128, 127],), types_pb2.Datapoint(
+        (DataType.INT8_ARRAY, ('[-128, 127]',), types_pb2.Datapoint(
             int32_array=types_pb2.Int32Array(values=[-128, 127]))),
     ])
     def test_to_message(self, value_type, init_args, message):
         assert Datapoint(*init_args).to_message(value_type) == message
 
     @pytest.mark.parametrize('value_type', [DataType.UNSPECIFIED, DataType.TIMESTAMP, DataType.TIMESTAMP_ARRAY])
     def test_to_message_unsupported_value_type(self, value_type):
```

