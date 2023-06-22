# Comparing `tmp/blickfeld_qb2-1.5.2.tar.gz` & `tmp/blickfeld_qb2-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blickfeld_qb2-1.5.2.tar", last modified: Thu Jun 15 07:03:32 2023, max compression
+gzip compressed data, was "blickfeld_qb2-1.5.3.tar", last modified: Tue Jun 20 10:20:46 2023, max compression
```

## Comparing `blickfeld_qb2-1.5.2.tar` & `blickfeld_qb2-1.5.3.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2023-06-15 07:03:28.000000 blickfeld_qb2-1.5.2/LICENSE.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/PKG-INFO
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      286 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/base/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4372 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/base/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/base/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2420 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/base/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/base/geometry/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2943 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/base/geometry/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/base/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/base/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3682 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/base/grpc/channel.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/base/grpc/device_ca_cert.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      796 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1872 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4181 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    55060 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/_types.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/_version.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/casing.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/compile/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/compile/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/compile/importing.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/compile/naming.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/grpclib_client.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/grpclib_server.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/util/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/util/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/util/async_channel.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/google/
--rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/google/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/google/protobuf/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/__init__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/__main__.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/compiler.py
--rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/main.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)    28668 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/models.py
--rw-r--r--   0 yocto     (1000) yocto     (1000)     7461 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/parser.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      944 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    12345 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    13059 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/detector/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/detector/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/detector/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     1477 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/detector/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/detector/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4015 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/detector/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/hardware/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/hardware/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/hardware/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      699 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/hardware/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/hardware/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3487 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/hardware/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/laser/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/laser/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/laser/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      635 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/laser/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/laser/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3881 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/laser/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     9203 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     3024 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    26328 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_processing/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_processing/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_processing/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     6071 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_processing/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_processing/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    16640 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_processing/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_toolkit/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_toolkit/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_toolkit/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      755 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_toolkit/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_toolkit/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10428 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/percept_toolkit/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/push/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/push/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/push/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2919 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/push/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/push/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2328 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/push/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/push/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    15032 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/push/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/system/
--rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/system/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/system/config/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    10089 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/system/config/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/system/data/
--rw-r--r--   0 yocto     (1000) yocto     (1000)     4591 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/system/data/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/blickfeld_qb2/system/services/
--rw-r--r--   0 yocto     (1000) yocto     (1000)    27697 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2/system/services/__init__.py
-drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-15 07:03:32.358439 blickfeld_qb2-1.5.2/blickfeld_qb2.egg-info/
--rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2.egg-info/PKG-INFO
--rw-r--r--   0 yocto     (1000) yocto     (1000)     2995 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2.egg-info/SOURCES.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2.egg-info/dependency_links.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2.egg-info/requires.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2023-06-15 07:03:32.000000 blickfeld_qb2-1.5.2/blickfeld_qb2.egg-info/top_level.txt
--rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2023-06-15 07:03:32.362439 blickfeld_qb2-1.5.2/setup.cfg
--rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2023-06-15 07:03:31.000000 blickfeld_qb2-1.5.2/setup.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2745 2023-06-20 10:20:23.000000 blickfeld_qb2-1.5.3/LICENSE.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/PKG-INFO
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      286 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/base/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4372 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/base/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2420 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/base/geometry/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2943 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/geometry/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3682 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/channel.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1636 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/device_ca_cert.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      796 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1872 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4181 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    55060 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      295 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/_types.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      101 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/_version.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3543 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/casing.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6337 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/importing.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      300 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/naming.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     5295 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/grpclib_client.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      910 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/grpclib_server.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/util/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/util/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6793 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/util/async_channel.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    68012 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7085 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       23 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/__init__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       32 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/__main__.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1335 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/compiler.py
+-rwxr-xr-x   0 yocto     (1000) yocto     (1000)     1513 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/main.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    28668 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/models.py
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     7461 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/parser.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      944 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    12345 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    13059 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     1477 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4015 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/detector/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       43 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      699 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3487 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      635 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3881 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/laser/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     9203 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     3024 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    26328 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     6137 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    16640 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       41 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      755 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10428 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/push/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/push/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/push/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2919 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/push/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.824401 blickfeld_qb2-1.5.3/blickfeld_qb2/push/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2328 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/push/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/push/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    15032 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/push/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/system/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       62 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/system/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/system/config/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    10089 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/system/config/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/system/data/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     4591 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/system/data/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/blickfeld_qb2/system/services/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)    27697 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/blickfeld_qb2/system/services/__init__.py
+drwxr-xr-x   0 yocto     (1000) yocto     (1000)        0 2023-06-20 10:20:46.820401 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      337 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/PKG-INFO
+-rw-r--r--   0 yocto     (1000) yocto     (1000)     2995 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/SOURCES.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)        1 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/dependency_links.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       86 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/requires.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       14 2023-06-20 10:20:46.000000 blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/top_level.txt
+-rw-r--r--   0 yocto     (1000) yocto     (1000)       38 2023-06-20 10:20:46.828401 blickfeld_qb2-1.5.3/setup.cfg
+-rw-r--r--   0 yocto     (1000) yocto     (1000)      554 2023-06-20 10:20:45.000000 blickfeld_qb2-1.5.3/setup.py
```

### Comparing `blickfeld_qb2-1.5.2/LICENSE.txt` & `blickfeld_qb2-1.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/base/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/base/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/base/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/base/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/base/geometry/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/base/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/base/grpc/channel.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/base/grpc/device_ca_cert.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/base/grpc/device_ca_cert.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/config/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/beam_deflection_control/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/beam_deflection_control/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/casing.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/casing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/compile/importing.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/grpclib_client.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/grpclib_server.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/grpclib_server.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/grpc/util/async_channel.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/lib/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/compiler.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/main.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/models.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/models.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/betterproto/plugin/parser.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/betterproto/plugin/parser.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/config/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/data/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,45 +7,14 @@
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 import numpy as np
 
 from ...base import data as __base_data__
 
 
 @dataclass(eq=False, repr=False)
-class Acceleration(betterproto.Message):
-    """A measurement of the Accelerometer"""
-
-    x: float = betterproto.float_field(1)
-    """X component of acceleration vector"""
-
-    y: float = betterproto.float_field(2)
-    """Y component of acceleration vector"""
-
-    z: float = betterproto.float_field(3)
-    """Z component of acceleration vector"""
-
-
-@dataclass(eq=False, repr=False)
-class AccelerationBuffer(betterproto.Message):
-    """Buffer for multiple Acceleration samples"""
-
-    timestamp: int = betterproto.uint64_field(1)
-    """Timestamp of the first sample in the buffer."""
-
-    sampling_period: int = betterproto.uint64_field(2)
-    """Sampling period of the acceleration samples"""
-
-    cartesian: bytes = betterproto.bytes_field(3)
-    """
-    Cartesian 3-dimensional array in row-major format with [x, y, z] tuples.
-    Type: Float32
-    """
-
-
-@dataclass(eq=False, repr=False)
 class Frame(betterproto.Message):
     """This section describes the contents of a point cloud frame."""
 
     id: int = betterproto.uint64_field(1)
     """Incremental frame ID since startup of the device."""
 
     timestamp: int = betterproto.uint64_field(2)
@@ -85,14 +54,45 @@
     """
 
     timestamp: np.ndarray = betterproto.bytes_field(6, numpy_dtype="<u8")
     """Unix timestamp of points. Type: UInt64"""
 
 
 @dataclass(eq=False, repr=False)
+class AccelerationBuffer(betterproto.Message):
+    """Buffer for multiple Acceleration samples"""
+
+    timestamp: int = betterproto.uint64_field(1)
+    """Timestamp of the first sample in the buffer."""
+
+    sampling_period: int = betterproto.uint64_field(2)
+    """Sampling period of the acceleration samples"""
+
+    cartesian: bytes = betterproto.bytes_field(3)
+    """
+    Cartesian 3-dimensional array in row-major format with [x, y, z] tuples.
+    Type: Float32
+    """
+
+
+@dataclass(eq=False, repr=False)
+class Acceleration(betterproto.Message):
+    """A measurement of the Accelerometer"""
+
+    x: float = betterproto.float_field(1)
+    """X component of acceleration vector"""
+
+    y: float = betterproto.float_field(2)
+    """Y component of acceleration vector"""
+
+    z: float = betterproto.float_field(3)
+    """Z component of acceleration vector"""
+
+
+@dataclass(eq=False, repr=False)
 class Health(betterproto.Message):
     """Message representing health"""
 
     state: "__base_data__.HealthState" = betterproto.enum_field(1)
     """High-level state of module"""
 
     state_reason: str = betterproto.string_field(2)
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/core_processing/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/core_processing/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,30 @@
     """Response to acceleration get filtered request"""
 
     acceleration: "_data__.Acceleration" = betterproto.message_field(1)
     """Single filtered acceleration"""
 
 
 @dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """Response to health get request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Stream response to health watch request"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """Health state"""
+
+
+@dataclass(eq=False, repr=False)
 class PointCloudStreamResponse(betterproto.Message):
     """Stream response to point cloud stream request"""
 
     frame: "_data__.Frame" = betterproto.message_field(1)
     """Point cloud frame"""
 
 
@@ -64,30 +80,14 @@
 class PointCloudEnableDemoRequest(betterproto.Message):
     """Response to point cloud enable demo request"""
 
     recording: "_config__.DemoRecording" = betterproto.enum_field(1)
     """Select demo recording"""
 
 
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Response to health get request"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Stream response to health watch request"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """Health state"""
-
-
 class Acceleration(betterproto.ServiceStub):
     """
     The Acceleration Service provides access to the accelerometer of the
     device.
     """
 
     async def async_stream(
@@ -179,14 +179,111 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
+class Health(betterproto.ServiceStub):
+    """
+    The health service provides methods to monitor operational status of the
+    core_processing module
+    """
+
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the core_processing module"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.core_processing.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Returns the current health status of the core_processing module"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """
+        Can be used to attach to the health monitoring status information of
+        the core_processing module
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.core_processing.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """
+        Can be used to attach to the health monitoring status information of
+        the core_processing module
+        """
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+
 class PointCloud(betterproto.ServiceStub):
     """
     Point Cloud service for core point cloud stream. It is the direct result of
     the internal processing pipeline. The output is not post-processed further.
     The post-processed output can be retrieved from the percept-processing
     PointCloud service.
     """
@@ -324,104 +421,7 @@
             self.async_enable_demo(
                 recording=recording,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
-
-
-class Health(betterproto.ServiceStub):
-    """
-    The health service provides methods to monitor operational status of the
-    core_processing module
-    """
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the core_processing module"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.core_processing.services.Health/Get",
-            request,
-            HealthGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health status of the core_processing module"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """
-        Can be used to attach to the health monitoring status information of
-        the core_processing module
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.core_processing.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """
-        Can be used to attach to the health monitoring status information of
-        the core_processing module
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/detector/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/detector/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/detector/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/detector/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/hardware/config/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/hardware/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/hardware/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,90 +27,90 @@
 class IdentificationGetResponse(betterproto.Message):
     """Response message for the identification get command"""
 
     identification: "_config__.Identification" = betterproto.message_field(1)
     """The current identification"""
 
 
-class ComputeModule(betterproto.ServiceStub):
+class Identification(betterproto.ServiceStub):
     """
-    This service is used to control & observe the state of the compute module.
+    The identification service provides methods to set and read out
+    identification data of the Qb2 device.
     """
 
-    async def async_reboot(
+    async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Reboots the CM4"""
+    ) -> "IdentificationGetResponse":
+        """Gets identification configuration"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.hardware.services.ComputeModule/Reboot",
+            "/blickfeld.hardware.services.Identification/Get",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            IdentificationGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def reboot(
+    def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Reboots the CM4"""
+    ) -> "IdentificationGetResponse":
+        """Gets identification configuration"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_reboot(
+            self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Identification(betterproto.ServiceStub):
+class ComputeModule(betterproto.ServiceStub):
     """
-    The identification service provides methods to set and read out
-    identification data of the Qb2 device.
+    This service is used to control & observe the state of the compute module.
     """
 
-    async def async_get(
+    async def async_reboot(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "IdentificationGetResponse":
-        """Gets identification configuration"""
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Reboots the CM4"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.hardware.services.Identification/Get",
+            "/blickfeld.hardware.services.ComputeModule/Reboot",
             request,
-            IdentificationGetResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def reboot(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "IdentificationGetResponse":
-        """Gets identification configuration"""
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Reboots the CM4"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_reboot(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/laser/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/laser/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/laser/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/laser/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/config/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/config/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,102 +7,14 @@
 import blickfeld_qb2.betterproto as betterproto
 import blickfeld_qb2.betterproto.lib.google.protobuf as betterproto_lib_google_protobuf
 
 from ...base import geometry as __base_geometry__
 
 
 @dataclass(eq=False, repr=False)
-class PointCloudFilter(betterproto.Message):
-    """Algorithm for filtering point clouds"""
-
-    radius_outlier: "PointCloudFilterRadiusOutlier" = betterproto.message_field(
-        1, group="point_cloud_filter_type"
-    )
-    """Use radius outlier filter for noise reduction on point clouds"""
-
-
-@dataclass(eq=False, repr=False)
-class PointCloudFilterRadiusOutlier(betterproto.Message):
-    """Filter points based on the number of neighbors in a certain radius"""
-
-    min_neighbor_points: int = betterproto.uint32_field(1)
-    """Minimum number of neighbors a point has to have to be retained"""
-
-    neighbor_radius: float = betterproto.double_field(2)
-    """All points within this radius are considered neighbors of a point"""
-
-
-@dataclass(eq=False, repr=False)
-class BackgroundSubtraction(betterproto.Message):
-    """
-    Algorithms seperating the input point cloud into foreground and background.
-    """
-
-    mixture_of_gaussians: "BackgroundSubtractionMixtureOfGaussians" = (
-        betterproto.message_field(1, group="background_subtraction_type")
-    )
-    """Use mixture of gaussians for foreground/background detection"""
-
-    octree: "BackgroundSubtractionOctree" = betterproto.message_field(
-        3, group="background_subtraction_type"
-    )
-    """Use a static octree for foreground/background detection."""
-
-
-@dataclass(eq=False, repr=False)
-class BackgroundSubtractionMixtureOfGaussians(betterproto.Message):
-    """
-    Dynamic background subtraction using a mixture of gaussians. The algorithm
-    automatically slowly updates the background model if the scene changes. The
-    update rate is controlled via 'exponential_decay'.
-    """
-
-    num_initialization_frames: int = betterproto.uint32_field(1)
-    """
-    How many frames of the first received frames are used to build the
-    background Reasonable default: 10
-    """
-
-    exponential_decay: float = betterproto.float_field(2)
-    """
-    Controls how fast objects switch between foreground and background.
-    Exponential decay factor. Reasonable default: 0.005
-    """
-
-    min_weight_threshold_for_background: float = betterproto.float_field(3)
-    """
-    Controls how much noise the background/foreground is expected to have.
-    Reasonable default: 0.25
-    """
-
-
-@dataclass(eq=False, repr=False)
-class BackgroundSubtractionOctree(betterproto.Message):
-    """
-    Uses the first received frames to build a static background map of the
-    environment. The algorithm requires the scene to only contain the static
-    parts of the scene on the start of the processing. The background model is
-    not updated automatically afterwards. The ResetBackground grpc method
-    allows to update the static map of the environment.
-    """
-
-    num_initialization_frames: int = betterproto.uint32_field(1)
-    """
-    How many frames of the first received frames are used to build the
-    background Reasonable default: 10
-    """
-
-    octree_resolution: float = betterproto.float_field(2)
-    """
-    Resolution for the octree storing a static background. Reasonable default:
-    0.15
-    """
-
-
-@dataclass(eq=False, repr=False)
 class DataSource(betterproto.Message):
     """
     The configuration storing the sources to retrieve the point cloud data for
     further processing.
     """
 
     cube1_setup: "DataSourceCube1Setup" = betterproto.message_field(
@@ -174,29 +86,14 @@
     """The configuration of a Qb2 setup of the LiDAR devices"""
 
     lidars: List["DataSourceQb2"] = betterproto.message_field(1)
     """the qb2 lidars to get the point clouds from"""
 
 
 @dataclass(eq=False, repr=False)
-class Perception(betterproto.Message):
-    """
-    The configuration of perception algorithms used to run e.g. security zones
-    """
-
-    background_subtraction: "BackgroundSubtraction" = betterproto.message_field(1)
-    """Extract the foreground point cloud of the scene"""
-
-    foreground_point_cloud_filters: List[
-        "PointCloudFilter"
-    ] = betterproto.message_field(2)
-    """Filter the foreground point cloud"""
-
-
-@dataclass(eq=False, repr=False)
 class ZoneAlgorithm(betterproto.Message):
     """An algorithm that monitors the area within and around a zone."""
 
     name: str = betterproto.string_field(1)
     """The user readable zone algorithm name"""
 
     uuid: str = betterproto.string_field(2)
@@ -249,7 +146,110 @@
     """
 
     min_points: int = betterproto.uint32_field(1)
     """
     Minimum number of (foreground) points in the security zone to trigger the
     alarm. Reasonable default: 10
     """
+
+
+@dataclass(eq=False, repr=False)
+class BackgroundSubtraction(betterproto.Message):
+    """
+    Algorithms seperating the input point cloud into foreground and background.
+    """
+
+    mixture_of_gaussians: "BackgroundSubtractionMixtureOfGaussians" = (
+        betterproto.message_field(1, group="background_subtraction_type")
+    )
+    """Use mixture of gaussians for foreground/background detection"""
+
+    octree: "BackgroundSubtractionOctree" = betterproto.message_field(
+        3, group="background_subtraction_type"
+    )
+    """Use a static octree for foreground/background detection."""
+
+
+@dataclass(eq=False, repr=False)
+class BackgroundSubtractionMixtureOfGaussians(betterproto.Message):
+    """
+    Dynamic background subtraction using a mixture of gaussians. The algorithm
+    automatically slowly updates the background model if the scene changes. The
+    update rate is controlled via 'exponential_decay'.
+    """
+
+    num_initialization_frames: int = betterproto.uint32_field(1)
+    """
+    How many frames of the first received frames are used to build the
+    background Reasonable default: 10
+    """
+
+    exponential_decay: float = betterproto.float_field(2)
+    """
+    Controls how fast objects switch between foreground and background.
+    Exponential decay factor. Reasonable default: 0.005
+    """
+
+    min_weight_threshold_for_background: float = betterproto.float_field(3)
+    """
+    Controls how much noise the background/foreground is expected to have.
+    Reasonable default: 0.25
+    """
+
+
+@dataclass(eq=False, repr=False)
+class BackgroundSubtractionOctree(betterproto.Message):
+    """
+    Uses the first received frames to build a static background map of the
+    environment. The algorithm requires the scene to only contain the static
+    parts of the scene on the start of the processing. The background model is
+    not updated automatically afterwards. The ResetBackground grpc method
+    allows to update the static map of the environment.
+    """
+
+    num_initialization_frames: int = betterproto.uint32_field(1)
+    """
+    How many frames of the first received frames are used to build the
+    background Reasonable default: 10
+    """
+
+    octree_resolution: float = betterproto.float_field(2)
+    """
+    Resolution for the octree storing a static background. Reasonable default:
+    0.15
+    """
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudFilter(betterproto.Message):
+    """Algorithm for filtering point clouds"""
+
+    radius_outlier: "PointCloudFilterRadiusOutlier" = betterproto.message_field(
+        1, group="point_cloud_filter_type"
+    )
+    """Use radius outlier filter for noise reduction on point clouds"""
+
+
+@dataclass(eq=False, repr=False)
+class PointCloudFilterRadiusOutlier(betterproto.Message):
+    """Filter points based on the number of neighbors in a certain radius"""
+
+    min_neighbor_points: int = betterproto.uint32_field(1)
+    """Minimum number of neighbors a point has to have to be retained"""
+
+    neighbor_radius: float = betterproto.double_field(2)
+    """All points within this radius are considered neighbors of a point"""
+
+
+@dataclass(eq=False, repr=False)
+class Perception(betterproto.Message):
+    """
+    The configuration of perception algorithms used to run e.g. security zones
+    """
+
+    background_subtraction: "BackgroundSubtraction" = betterproto.message_field(1)
+    """Extract the foreground point cloud of the scene"""
+
+    foreground_point_cloud_filters: List[
+        "PointCloudFilter"
+    ] = betterproto.message_field(2)
+    """Filter the foreground point cloud"""
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/data/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -43,30 +43,14 @@
     source changed.
     """
 
     STATE_IDLE = 6
     """No processing is happening in the pipeline."""
 
 
-class PointCloudType(betterproto.Enum):
-    """The type of the point cloud"""
-
-    POINT_CLOUD_TYPE_UNSPECIFIED = 0
-    """The zero value that is not accepted"""
-
-    POINT_CLOUD_TYPE_FULL = 1
-    """
-    Full point cloud (combined point cloud of all devices or unfiltered point
-    cloud coming from one device)
-    """
-
-    POINT_CLOUD_TYPE_FOREGROUND = 2
-    """Point cloud containing only foreground/points from moving objects"""
-
-
 class CoordinateSystem(betterproto.Enum):
     """Specifies the coordinates system the data is expressed in"""
 
     COORDINATE_SYSTEM_UNSPECIFIED = 0
     """
     Coordinate system not specified. Not accepted neither within a request nor
     as response
@@ -77,14 +61,30 @@
     The data is expressed in the coordiante system of the data-source/device
     """
 
     COORDINATE_SYSTEM_TRANSFORMED = 2
     """The data is expressed in a map coordinate system"""
 
 
+class PointCloudType(betterproto.Enum):
+    """The type of the point cloud"""
+
+    POINT_CLOUD_TYPE_UNSPECIFIED = 0
+    """The zero value that is not accepted"""
+
+    POINT_CLOUD_TYPE_FULL = 1
+    """
+    Full point cloud (combined point cloud of all devices or unfiltered point
+    cloud coming from one device)
+    """
+
+    POINT_CLOUD_TYPE_FOREGROUND = 2
+    """Point cloud containing only foreground/points from moving objects"""
+
+
 @dataclass(eq=False, repr=False)
 class Health(betterproto.Message):
     """
     A health message that contains information about the pipeline status and
     the module itself.
     """
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/percept_pipeline/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_pipeline/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,30 @@
     If the list is empty, the background models of all data sources are reset.
     If the background models of only specific devices should be rebuilt, the
     'fqdn' of the respective devices has to be mentioned in the 'fqdns' list.
     """
 
 
 @dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """Stream response containing health of the module"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """The module health"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """Get response containing health of the module"""
+
+    health: "_data__.Health" = betterproto.message_field(1)
+    """The module health"""
+
+
+@dataclass(eq=False, repr=False)
 class PerceptionGetResponse(betterproto.Message):
     """Response containing the current perception configuration"""
 
     perception: "_config__.Perception" = betterproto.message_field(1)
     """The current perception configuration"""
 
 
@@ -128,30 +144,14 @@
     """
     Mapping from a template name to the template itself. The template can be
     used to configure the perception algorithms for certain use-cases.
     """
 
 
 @dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """Stream response containing health of the module"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """The module health"""
-
-
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """Get response containing health of the module"""
-
-    health: "_data__.Health" = betterproto.message_field(1)
-    """The module health"""
-
-
-@dataclass(eq=False, repr=False)
 class ZoneListResponse(betterproto.Message):
     """Response containing the configured list of zones"""
 
     zones: List["_config__.ZoneAlgorithm"] = betterproto.message_field(1)
     """The currently configured zones"""
 
 
@@ -407,14 +407,108 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
+class Health(betterproto.ServiceStub):
+    """Reports the health of the pipeline module."""
+
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """
+        Streams health information on a regular cadence or if certain incidents
+        happen
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.percept_pipeline.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """
+        Streams health information on a regular cadence or if certain incidents
+        happen
+        """
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
+
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Returns the current health information"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.percept_pipeline.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Returns the current health information"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+
 class Perception(betterproto.ServiceStub):
     """
     The perception service allows getting, configuring and receiving updates of
     the perception configurations. Perception configurations specify the
     algorithms used for e.g. for background subtraction etc.
     """
 
@@ -582,108 +676,14 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Health(betterproto.ServiceStub):
-    """Reports the health of the pipeline module."""
-
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """
-        Streams health information on a regular cadence or if certain incidents
-        happen
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.percept_pipeline.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """
-        Streams health information on a regular cadence or if certain incidents
-        happen
-        """
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health information"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.percept_pipeline.services.Health/Get",
-            request,
-            HealthGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Returns the current health information"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-
 class Zone(betterproto.ServiceStub):
     """
     The zone service allows getting, configuring, deleting and receiving
     updates of the configured zones.
     """
 
     async def async_list(
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/percept_processing/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     """
 
     tiles: List["StateVolumeVolumeTile"] = betterproto.message_field(2)
     """
     The tiles of the volume map The volume of a zone is approximated by a
     'volume map' see xref:blickfeld/percept_pipeline/config/zone_algorithm.adoc
     #_blickfeld_percept_pipeline_config_ZoneAlgorithm_Volume[Volume] for more
-    details.
+    details. NOTE: For performance reasons this field is currently not filled.
     """
 
     tile_size: float = betterproto.float_field(3)
     """The tile size of the volume map"""
 
     shape: "__base_geometry__.Shape" = betterproto.message_field(4)
     """
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/percept_processing/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_processing/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,68 +25,61 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
-class PointCloudStreamRequest(betterproto.Message):
-    """
-    A request to receive a stream of point cloud messages. Different point
-    clouds can be streamed depending on the set fields: - combined point cloud
-    (the full point cloud of all the available devices combined) in the map
-    coordinate system - the foreground of the combined point cloud in the map
-    coordinate system - the complete raw point cloud coming from one device,
-    but only in map coordinate system.
-    """
+class StateListStreamRequest(betterproto.Message):
+    """A request to receive a stream of state list messages"""
 
-    point_cloud_type: "__percept_pipeline_data__.PointCloudType" = (
-        betterproto.enum_field(1)
-    )
-    """The type of point cloud to stream"""
+    pass
 
-    coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = (
-        betterproto.enum_field(2)
-    )
+
+@dataclass(eq=False, repr=False)
+class StateListStreamResponse(betterproto.Message):
     """
-    The coordinate system the point cloud should be expressed in (local or
-    transformed/map)
+    A response for getting a stream of state list messages from the running
+    pipeline
     """
 
-    fqdn: str = betterproto.string_field(3, group="point_cloud_source")
-    """fqdn of the data source to get the point cloud from"""
+    state_list: "_data__.StateList" = betterproto.message_field(1)
+    """
+    The current state list with the information detected in the zones
+    configured in the running pipeline
+    """
 
 
 @dataclass(eq=False, repr=False)
-class PointCloudStreamResponse(betterproto.Message):
-    """A response for getting a stream of point cloud messages"""
+class PipelineStartRequest(betterproto.Message):
+    """A request to start a headless pipeline."""
 
-    point_cloud: "__core_processing_data__.Frame" = betterproto.message_field(1)
-    """The required point cloud, based on the fields set in the request"""
+    pass
 
 
 @dataclass(eq=False, repr=False)
-class StateListStreamRequest(betterproto.Message):
-    """A request to receive a stream of state list messages"""
+class PipelineStartResponse(betterproto.Message):
+    """
+    A response to PipelineStartRequest that contains the list of available
+    streams for the started pipeline.
+    """
 
-    pass
+    data_types: List["_data__.DataType"] = betterproto.enum_field(1)
+    """List of available streams"""
 
 
 @dataclass(eq=False, repr=False)
-class StateListStreamResponse(betterproto.Message):
+class PipelineListAvailableDataResponse(betterproto.Message):
     """
-    A response for getting a stream of state list messages from the running
-    pipeline
+    A response containing the list of the data types available for streaming in
+    the running pipeline
     """
 
-    state_list: "_data__.StateList" = betterproto.message_field(1)
-    """
-    The current state list with the information detected in the zones
-    configured in the running pipeline
-    """
+    data_types: List["_data__.DataType"] = betterproto.enum_field(1)
+    """A list of the data types available for streaming"""
 
 
 @dataclass(eq=False, repr=False)
 class HealthWatchResponse(betterproto.Message):
     """
     A response for getting a stream of health messages about the pipeline
     """
@@ -104,104 +97,93 @@
     health: "_data__.Health" = betterproto.message_field(1)
     """
     The current health message with information about the state of the pipeline
     """
 
 
 @dataclass(eq=False, repr=False)
-class PipelineStartRequest(betterproto.Message):
-    """A request to start a headless pipeline."""
-
-    pass
+class PointCloudStreamRequest(betterproto.Message):
+    """
+    A request to receive a stream of point cloud messages. Different point
+    clouds can be streamed depending on the set fields: - combined point cloud
+    (the full point cloud of all the available devices combined) in the map
+    coordinate system - the foreground of the combined point cloud in the map
+    coordinate system - the complete raw point cloud coming from one device,
+    but only in map coordinate system.
+    """
 
+    point_cloud_type: "__percept_pipeline_data__.PointCloudType" = (
+        betterproto.enum_field(1)
+    )
+    """The type of point cloud to stream"""
 
-@dataclass(eq=False, repr=False)
-class PipelineStartResponse(betterproto.Message):
+    coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = (
+        betterproto.enum_field(2)
+    )
     """
-    A response to PipelineStartRequest that contains the list of available
-    streams for the started pipeline.
+    The coordinate system the point cloud should be expressed in (local or
+    transformed/map)
     """
 
-    data_types: List["_data__.DataType"] = betterproto.enum_field(1)
-    """List of available streams"""
+    fqdn: str = betterproto.string_field(3, group="point_cloud_source")
+    """fqdn of the data source to get the point cloud from"""
 
 
 @dataclass(eq=False, repr=False)
-class PipelineListAvailableDataResponse(betterproto.Message):
-    """
-    A response containing the list of the data types available for streaming in
-    the running pipeline
-    """
+class PointCloudStreamResponse(betterproto.Message):
+    """A response for getting a stream of point cloud messages"""
 
-    data_types: List["_data__.DataType"] = betterproto.enum_field(1)
-    """A list of the data types available for streaming"""
+    point_cloud: "__core_processing_data__.Frame" = betterproto.message_field(1)
+    """The required point cloud, based on the fields set in the request"""
 
 
-class PointCloud(betterproto.ServiceStub):
+class StateList(betterproto.ServiceStub):
     """
-    An RPC service to request a stream of point cloud messages. If a pipeline
-    is already running, it will be used to stream the data. If no pipeline is
+    An RPC service to request a stream of state list messages. If a pipeline is
+    already running, it will be used to stream the data. If no pipeline is
     running, it will be started first and then the stream will start. NOTE: in
     this second case, the pipeline will also be automatically stopped once the
     this second case, the pipeline will also be automatically stopped once
     there are no more clients requesting any stream type from the module.
     """
 
     async def async_stream(
         self,
-        *,
-        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
-        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
-        fqdn: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> AsyncIterator["PointCloudStreamResponse"]:
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["StateListStreamResponse"]:
         """
-        A method to get a stream of point cloud messages from the pipeline. It
-        is possible to stream different point clouds, depending on the fields
-        set in the request
+        A method to get a stream of state list messages from the pipeline
         """
 
-        request = PointCloudStreamRequest()
-        request.point_cloud_type = point_cloud_type
-        request.coordinate_system = coordinate_system
-        request.fqdn = fqdn
+        request = StateListStreamRequest()
 
         async for response in self._unary_stream(
-            "/blickfeld.percept_processing.services.PointCloud/Stream",
+            "/blickfeld.percept_processing.services.StateList/Stream",
             request,
-            PointCloudStreamResponse,
+            StateListStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
     def stream(
         self,
-        *,
-        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
-        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
-        fqdn: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> Iterator["PointCloudStreamResponse"]:
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["StateListStreamResponse"]:
         """
-        A method to get a stream of point cloud messages from the pipeline. It
-        is possible to stream different point clouds, depending on the fields
-        set in the request
+        A method to get a stream of state list messages from the pipeline
         """
 
         loop = asyncio.get_event_loop()
         ait = self.async_stream(
-            point_cloud_type=point_cloud_type,
-            coordinate_system=coordinate_system,
-            fqdn=fqdn,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ).__aiter__()
 
         async def get_next():
             try:
@@ -213,75 +195,149 @@
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
 
-class StateList(betterproto.ServiceStub):
+class Pipeline(betterproto.ServiceStub):
     """
-    An RPC service to request a stream of state list messages. If a pipeline is
-    already running, it will be used to stream the data. If no pipeline is
-    running, it will be started first and then the stream will start. NOTE: in
-    this second case, the pipeline will also be automatically stopped once the
-    this second case, the pipeline will also be automatically stopped once
-    there are no more clients requesting any stream type from the module.
+    An RPC service to start and stop pipelines. Note that currently it is
+    impossible to run more than one pipeline at the same time.
     """
 
-    async def async_stream(
+    async def async_start(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["StateListStreamResponse"]:
+    ) -> "PipelineStartResponse":
         """
-        A method to get a stream of state list messages from the pipeline
+        A method to start a headless pipeline. This means that a pipeline
+        started with this method will only be stopped once the Stop method is
+        explicitly called
         """
 
-        request = StateListStreamRequest()
+        request = PipelineStartRequest()
 
-        async for response in self._unary_stream(
-            "/blickfeld.percept_processing.services.StateList/Stream",
+        return await self._unary_unary(
+            "/blickfeld.percept_processing.services.Pipeline/Start",
             request,
-            StateListStreamResponse,
+            PipelineStartResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        ):
-            yield response
+        )
 
-    def stream(
+    def start(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["StateListStreamResponse"]:
+    ) -> "PipelineStartResponse":
         """
-        A method to get a stream of state list messages from the pipeline
+        A method to start a headless pipeline. This means that a pipeline
+        started with this method will only be stopped once the Stop method is
+        explicitly called
         """
 
         loop = asyncio.get_event_loop()
-        ait = self.async_stream(
+        return loop.run_until_complete(
+            self.async_start(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_stop(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        A method to stop the running pipeline. This will force-stop the
+        pipeline, no matter how the pipeline was created and no matter how many
+        clients are streaming from it.
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.percept_processing.services.Pipeline/Stop",
+            request,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        ).__aiter__()
+        )
 
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
+    def stop(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """
+        A method to stop the running pipeline. This will force-stop the
+        pipeline, no matter how the pipeline was created and no matter how many
+        clients are streaming from it.
+        """
 
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_stop(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_list_available_data(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PipelineListAvailableDataResponse":
+        """
+        A method to get the list of the data streams available for the running
+        pipeline
+        """
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        return await self._unary_unary(
+            "/blickfeld.percept_processing.services.Pipeline/ListAvailableData",
+            request,
+            PipelineListAvailableDataResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
+
+    def list_available_data(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "PipelineListAvailableDataResponse":
+        """
+        A method to get the list of the data streams available for the running
+        pipeline
+        """
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_list_available_data(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
 
 
 class Health(betterproto.ServiceStub):
     """
     An RPC service to request information about the state of the pipeline and
     of the module.
     """
@@ -379,142 +435,86 @@
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class Pipeline(betterproto.ServiceStub):
+class PointCloud(betterproto.ServiceStub):
     """
-    An RPC service to start and stop pipelines. Note that currently it is
-    impossible to run more than one pipeline at the same time.
+    An RPC service to request a stream of point cloud messages. If a pipeline
+    is already running, it will be used to stream the data. If no pipeline is
+    running, it will be started first and then the stream will start. NOTE: in
+    this second case, the pipeline will also be automatically stopped once the
+    this second case, the pipeline will also be automatically stopped once
+    there are no more clients requesting any stream type from the module.
     """
 
-    async def async_start(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PipelineStartResponse":
-        """
-        A method to start a headless pipeline. This means that a pipeline
-        started with this method will only be stopped once the Stop method is
-        explicitly called
-        """
-
-        request = PipelineStartRequest()
-
-        return await self._unary_unary(
-            "/blickfeld.percept_processing.services.Pipeline/Start",
-            request,
-            PipelineStartResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def start(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PipelineStartResponse":
-        """
-        A method to start a headless pipeline. This means that a pipeline
-        started with this method will only be stopped once the Stop method is
-        explicitly called
-        """
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_start(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_stop(
+    async def async_stream(
         self,
+        *,
+        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
+        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
+        fqdn: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
+        metadata: Optional["MetadataLike"] = None
+    ) -> AsyncIterator["PointCloudStreamResponse"]:
         """
-        A method to stop the running pipeline. This will force-stop the
-        pipeline, no matter how the pipeline was created and no matter how many
-        clients are streaming from it.
+        A method to get a stream of point cloud messages from the pipeline. It
+        is possible to stream different point clouds, depending on the fields
+        set in the request
         """
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = PointCloudStreamRequest()
+        request.point_cloud_type = point_cloud_type
+        request.coordinate_system = coordinate_system
+        request.fqdn = fqdn
 
-        return await self._unary_unary(
-            "/blickfeld.percept_processing.services.Pipeline/Stop",
+        async for response in self._unary_stream(
+            "/blickfeld.percept_processing.services.PointCloud/Stream",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            PointCloudStreamResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ):
+            yield response
 
-    def stop(
+    def stream(
         self,
+        *,
+        point_cloud_type: "__percept_pipeline_data__.PointCloudType" = 0,
+        coordinate_system: "__percept_pipeline_data__.CoordinateSystem" = 0,
+        fqdn: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "betterproto_lib_google_protobuf.Empty":
+        metadata: Optional["MetadataLike"] = None
+    ) -> Iterator["PointCloudStreamResponse"]:
         """
-        A method to stop the running pipeline. This will force-stop the
-        pipeline, no matter how the pipeline was created and no matter how many
-        clients are streaming from it.
+        A method to get a stream of point cloud messages from the pipeline. It
+        is possible to stream different point clouds, depending on the fields
+        set in the request
         """
 
         loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_stop(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_list_available_data(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PipelineListAvailableDataResponse":
-        """
-        A method to get the list of the data streams available for the running
-        pipeline
-        """
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.percept_processing.services.Pipeline/ListAvailableData",
-            request,
-            PipelineListAvailableDataResponse,
+        ait = self.async_stream(
+            point_cloud_type=point_cloud_type,
+            coordinate_system=coordinate_system,
+            fqdn=fqdn,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
-        )
+        ).__aiter__()
 
-    def list_available_data(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "PipelineListAvailableDataResponse":
-        """
-        A method to get the list of the data streams available for the running
-        pipeline
-        """
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
 
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_list_available_data(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/percept_toolkit/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/percept_toolkit/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/percept_toolkit/services/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/push/config/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/push/config/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/push/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/push/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/push/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/push/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,30 @@
 if TYPE_CHECKING:
     import grpclib.server
     from blickfeld_qb2.betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
 
 @dataclass(eq=False, repr=False)
+class HealthGetResponse(betterproto.Message):
+    """request get the health of the configured publisher"""
+
+    health: "_data__.Health" = betterproto.message_field(2)
+    """health of push configurations"""
+
+
+@dataclass(eq=False, repr=False)
+class HealthWatchResponse(betterproto.Message):
+    """request watch the health of the configured publisher"""
+
+    health: "_data__.Health" = betterproto.message_field(2)
+    """health of push configurations"""
+
+
+@dataclass(eq=False, repr=False)
 class PushStoreRequest(betterproto.Message):
     """request to add a push configuration"""
 
     uuid: str = betterproto.string_field(1)
     """the uuid of the configuration (has to be generated on client side!)"""
 
     push_config: "_config__.Push" = betterproto.message_field(2)
@@ -87,28 +103,100 @@
 class DestinationValidateRequest(betterproto.Message):
     """request to validate a configured destination"""
 
     destination: "_config__.Destination" = betterproto.message_field(1)
     """the current (possibly incomplete) configuration entered"""
 
 
-@dataclass(eq=False, repr=False)
-class HealthGetResponse(betterproto.Message):
-    """request get the health of the configured publisher"""
+class Health(betterproto.ServiceStub):
+    """An gRPC service to request the status of push configurations"""
 
-    health: "_data__.Health" = betterproto.message_field(2)
-    """health of push configurations"""
+    async def async_get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Get Status for all configured push configurations"""
 
+        request = betterproto_lib_google_protobuf.Empty()
 
-@dataclass(eq=False, repr=False)
-class HealthWatchResponse(betterproto.Message):
-    """request watch the health of the configured publisher"""
+        return await self._unary_unary(
+            "/blickfeld.push.services.Health/Get",
+            request,
+            HealthGetResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        )
 
-    health: "_data__.Health" = betterproto.message_field(2)
-    """health of push configurations"""
+    def get(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "HealthGetResponse":
+        """Get Status for all configured push configurations"""
+
+        loop = asyncio.get_event_loop()
+        return loop.run_until_complete(
+            self.async_get(
+                timeout=timeout,
+                deadline=deadline,
+                metadata=metadata,
+            )
+        )
+
+    async def async_watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> AsyncIterator["HealthWatchResponse"]:
+        """Watch status changes for configured push configurations"""
+
+        request = betterproto_lib_google_protobuf.Empty()
+
+        async for response in self._unary_stream(
+            "/blickfeld.push.services.Health/Watch",
+            request,
+            HealthWatchResponse,
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ):
+            yield response
+
+    def watch(
+        self,
+        timeout: Optional[float] = None,
+        deadline: Optional["Deadline"] = None,
+        metadata: Optional["MetadataLike"] = None,
+    ) -> Iterator["HealthWatchResponse"]:
+        """Watch status changes for configured push configurations"""
+
+        loop = asyncio.get_event_loop()
+        ait = self.async_watch(
+            timeout=timeout,
+            deadline=deadline,
+            metadata=metadata,
+        ).__aiter__()
+
+        async def get_next():
+            try:
+                obj = await ait.__anext__()
+                return False, obj
+            except StopAsyncIteration:
+                return True, None
+
+        while True:
+            done, obj = loop.run_until_complete(get_next())
+            if done:
+                break
+            yield obj
 
 
 class Push(betterproto.ServiceStub):
     """An gRPC service to configure multiple push settings"""
 
     async def async_store(
         self,
@@ -409,95 +497,7 @@
             self.async_validate(
                 destination=destination,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
-
-
-class Health(betterproto.ServiceStub):
-    """An gRPC service to request the status of push configurations"""
-
-    async def async_get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Get Status for all configured push configurations"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        return await self._unary_unary(
-            "/blickfeld.push.services.Health/Get",
-            request,
-            HealthGetResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        )
-
-    def get(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "HealthGetResponse":
-        """Get Status for all configured push configurations"""
-
-        loop = asyncio.get_event_loop()
-        return loop.run_until_complete(
-            self.async_get(
-                timeout=timeout,
-                deadline=deadline,
-                metadata=metadata,
-            )
-        )
-
-    async def async_watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> AsyncIterator["HealthWatchResponse"]:
-        """Watch status changes for configured push configurations"""
-
-        request = betterproto_lib_google_protobuf.Empty()
-
-        async for response in self._unary_stream(
-            "/blickfeld.push.services.Health/Watch",
-            request,
-            HealthWatchResponse,
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ):
-            yield response
-
-    def watch(
-        self,
-        timeout: Optional[float] = None,
-        deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> Iterator["HealthWatchResponse"]:
-        """Watch status changes for configured push configurations"""
-
-        loop = asyncio.get_event_loop()
-        ait = self.async_watch(
-            timeout=timeout,
-            deadline=deadline,
-            metadata=metadata,
-        ).__aiter__()
-
-        async def get_next():
-            try:
-                obj = await ait.__anext__()
-                return False, obj
-            except StopAsyncIteration:
-                return True, None
-
-        while True:
-            done, obj = loop.run_until_complete(get_next())
-            if done:
-                break
-            yield obj
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/system/config/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/system/config/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,37 +14,14 @@
     CLASS_UNKNOWN = 0
     CUBE = 1
     CUBE_RANGE = 2
     QB2 = 3
 
 
 @dataclass(eq=False, repr=False)
-class Device(betterproto.Message):
-    """This message describes a Blickfeld Lidar device"""
-
-    fqdn_or_ip: str = betterproto.string_field(1)
-    """Fully-qualified-domain-name / Hostname or IP address"""
-
-    name: str = betterproto.string_field(2)
-    """
-    Human-readable name of the device Optional: Is filled out by the service if
-    not given.
-    """
-
-    serial_number: str = betterproto.string_field(3)
-    """
-    Serial number of the device Optional: Is filled out by the service if not
-    given.
-    """
-
-    class_: "DeviceClass" = betterproto.enum_field(4)
-    """Device class Optional: Is filled out by the service if not given."""
-
-
-@dataclass(eq=False, repr=False)
 class Network(betterproto.Message):
     """
     * The "Network" protocol message allows to define and setup the network
     configuration of the Qb2 device which can be further applied by
     "SetConfig()" service API. The message specifies the desired network
     configuration mode: "dhcp", "link-local","static" or their combination, and
     allows custom static configuration of the device. Modes "dhcp" and "static"
@@ -262,7 +239,30 @@
     """
     Temporary container used for config storage TODO Remove when daedalus-
     config supports map type.
     """
 
     name: str = betterproto.string_field(1)
     scan_pattern: "ScanPattern" = betterproto.message_field(2)
+
+
+@dataclass(eq=False, repr=False)
+class Device(betterproto.Message):
+    """This message describes a Blickfeld Lidar device"""
+
+    fqdn_or_ip: str = betterproto.string_field(1)
+    """Fully-qualified-domain-name / Hostname or IP address"""
+
+    name: str = betterproto.string_field(2)
+    """
+    Human-readable name of the device Optional: Is filled out by the service if
+    not given.
+    """
+
+    serial_number: str = betterproto.string_field(3)
+    """
+    Serial number of the device Optional: Is filled out by the service if not
+    given.
+    """
+
+    class_: "DeviceClass" = betterproto.enum_field(4)
+    """Device class Optional: Is filled out by the service if not given."""
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/system/data/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/system/data/__init__.py`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2/system/services/__init__.py` & `blickfeld_qb2-1.5.3/blickfeld_qb2/system/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -116,41 +116,14 @@
     """Continuous response with status"""
 
     status: "_data__.FirmwareStatus" = betterproto.message_field(1)
     """Current firmware status"""
 
 
 @dataclass(eq=False, repr=False)
-class NetworkValidateRequest(betterproto.Message):
-    """Request to validate method"""
-
-    config: "_config__.Network" = betterproto.message_field(1)
-    """Configuration which should be validated"""
-
-
-@dataclass(eq=False, repr=False)
-class NetworkValidateResponse(betterproto.Message):
-    """Response to validate method"""
-
-    status: "_data__.NetworkStatus" = betterproto.message_field(1)
-    """Status message with allocated IP addresses"""
-
-
-@dataclass(eq=False, repr=False)
-class NetworkGetMacAddressesResponse(betterproto.Message):
-    """Response with mac addresses"""
-
-    ethernet: str = betterproto.string_field(1)
-    """Mac address of ethernet / LAN interface"""
-
-    wireless: str = betterproto.string_field(2)
-    """Mac address of wireless / WiFi interface"""
-
-
-@dataclass(eq=False, repr=False)
 class ScanPatternGetResponse(betterproto.Message):
     name: str = betterproto.string_field(1)
     scan_pattern: "_config__.ScanPattern" = betterproto.message_field(2)
 
 
 @dataclass(eq=False, repr=False)
 class ScanPatternSetRequest(betterproto.Message):
@@ -174,14 +147,41 @@
 
 
 @dataclass(eq=False, repr=False)
 class ScanPatternDeleteRequest(betterproto.Message):
     name: str = betterproto.string_field(1)
 
 
+@dataclass(eq=False, repr=False)
+class NetworkValidateRequest(betterproto.Message):
+    """Request to validate method"""
+
+    config: "_config__.Network" = betterproto.message_field(1)
+    """Configuration which should be validated"""
+
+
+@dataclass(eq=False, repr=False)
+class NetworkValidateResponse(betterproto.Message):
+    """Response to validate method"""
+
+    status: "_data__.NetworkStatus" = betterproto.message_field(1)
+    """Status message with allocated IP addresses"""
+
+
+@dataclass(eq=False, repr=False)
+class NetworkGetMacAddressesResponse(betterproto.Message):
+    """Response with mac addresses"""
+
+    ethernet: str = betterproto.string_field(1)
+    """Mac address of ethernet / LAN interface"""
+
+    wireless: str = betterproto.string_field(2)
+    """Mac address of wireless / WiFi interface"""
+
+
 class Firmware(betterproto.ServiceStub):
     """
     The firmware service offers methods to fetch the currently installed
     firmware, upgrade it, downgrade it and also configure auto-update
     mechanisms.
     """
 
@@ -429,453 +429,453 @@
         while True:
             done, obj = loop.run_until_complete(get_next())
             if done:
                 break
             yield obj
 
 
-class Network(betterproto.ServiceStub):
-    """
-    The network service allows to setup network configuration of Qb2 device.
-    The exact structure of configuration settings is defined by "Network"
-    protocol message. Service provides "SetConfig()" and "GetConfig()" API
-    which allow to apply and read out configuration settings at run-time. The
-    "GetStatus()" API brings configuration and statistical information about
-    currently active network connection.
-    """
-
-    async def async_get_status(
+class ScanPattern(betterproto.ServiceStub):
+    async def async_get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "_data__.NetworkStatus":
-        """Brings information about currently active connection"""
+    ) -> "ScanPatternGetResponse":
+        """Gets scan pattern configuration settings"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.system.services.Network/GetStatus",
+            "/blickfeld.system.services.ScanPattern/Get",
             request,
-            _data__.NetworkStatus,
+            ScanPatternGetResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get_status(
+    def get(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "_data__.NetworkStatus":
-        """Brings information about currently active connection"""
+    ) -> "ScanPatternGetResponse":
+        """Gets scan pattern configuration settings"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_status(
+            self.async_get(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_set_config(
+    async def async_set(
         self,
         *,
-        hostname: str = "",
-        dhcp: bool = False,
-        manual: "NetworkStatic" = None,
-        link_local: bool = False,
-        wireless: "NetworkWireless" = None,
+        name: str = "",
+        scan_pattern: "_config__.ScanPattern" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Applies specified network configuration"""
+        """Sets scan pattern cofiguration settings"""
 
-        request = _config__.Network()
-        request.hostname = hostname
-        request.dhcp = dhcp
-        if manual is not None:
-            request.manual = manual
-        request.link_local = link_local
-        if wireless is not None:
-            request.wireless = wireless
+        request = ScanPatternSetRequest()
+        request.name = name
+        if scan_pattern is not None:
+            request.scan_pattern = scan_pattern
 
         return await self._unary_unary(
-            "/blickfeld.system.services.Network/SetConfig",
+            "/blickfeld.system.services.ScanPattern/Set",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def set_config(
+    def set(
         self,
         *,
-        hostname: str = "",
-        dhcp: bool = False,
-        manual: "NetworkStatic" = None,
-        link_local: bool = False,
-        wireless: "NetworkWireless" = None,
+        name: str = "",
+        scan_pattern: "_config__.ScanPattern" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Applies specified network configuration"""
+        """Sets scan pattern cofiguration settings"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set_config(
-                hostname=hostname,
-                dhcp=dhcp,
-                manual=manual,
-                link_local=link_local,
-                wireless=wireless,
+            self.async_set(
+                name=name,
+                scan_pattern=scan_pattern,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_get_config(
+    async def async_list(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "_config__.Network":
-        """Reads out provided network configuration"""
+    ) -> "ScanPatternListResponse":
+        """Return list of named scan patterns"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.system.services.Network/GetConfig",
+            "/blickfeld.system.services.ScanPattern/List",
             request,
-            _config__.Network,
+            ScanPatternListResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get_config(
+    def list(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "_config__.Network":
-        """Reads out provided network configuration"""
+    ) -> "ScanPatternListResponse":
+        """Return list of named scan patterns"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_config(
+            self.async_list(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_validate(
+    async def async_store(
         self,
         *,
-        config: "_config__.Network" = None,
+        name: str = "",
+        scan_pattern: "_config__.ScanPattern" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "NetworkValidateResponse":
-        """
-        Validates the network configuration by applying it shortly. If DHCP is
-        configured, it checks if it can acquire an IPv4 address. For static IP
-        address, the validation only works for wireless networks. It then,
-        still cannot allocate a manual IP address if the credentials are wrong.
-        [NOTE] The validation does not yet separate error messages for
-        misconfigured wireless credentials or wrongly configured DHCP server.
-        Thus, the issue is not necessarily on the device side.
-        """
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Store scan pattern"""
 
-        request = NetworkValidateRequest()
-        if config is not None:
-            request.config = config
+        request = ScanPatternStoreRequest()
+        request.name = name
+        if scan_pattern is not None:
+            request.scan_pattern = scan_pattern
 
         return await self._unary_unary(
-            "/blickfeld.system.services.Network/Validate",
+            "/blickfeld.system.services.ScanPattern/Store",
             request,
-            NetworkValidateResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def validate(
+    def store(
         self,
         *,
-        config: "_config__.Network" = None,
+        name: str = "",
+        scan_pattern: "_config__.ScanPattern" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "NetworkValidateResponse":
-        """
-        Validates the network configuration by applying it shortly. If DHCP is
-        configured, it checks if it can acquire an IPv4 address. For static IP
-        address, the validation only works for wireless networks. It then,
-        still cannot allocate a manual IP address if the credentials are wrong.
-        [NOTE] The validation does not yet separate error messages for
-        misconfigured wireless credentials or wrongly configured DHCP server.
-        Thus, the issue is not necessarily on the device side.
-        """
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Store scan pattern"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_validate(
-                config=config,
+            self.async_store(
+                name=name,
+                scan_pattern=scan_pattern,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_get_mac_addresses(
+    async def async_delete(
         self,
+        *,
+        name: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "NetworkGetMacAddressesResponse":
-        """Get MAC addresses of the available interfaces"""
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Delete stored scan pattern"""
 
-        request = betterproto_lib_google_protobuf.Empty()
+        request = ScanPatternDeleteRequest()
+        request.name = name
 
         return await self._unary_unary(
-            "/blickfeld.system.services.Network/GetMacAddresses",
+            "/blickfeld.system.services.ScanPattern/Delete",
             request,
-            NetworkGetMacAddressesResponse,
+            betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get_mac_addresses(
+    def delete(
         self,
+        *,
+        name: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None,
-    ) -> "NetworkGetMacAddressesResponse":
-        """Get MAC addresses of the available interfaces"""
+        metadata: Optional["MetadataLike"] = None
+    ) -> "betterproto_lib_google_protobuf.Empty":
+        """Delete stored scan pattern"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get_mac_addresses(
+            self.async_delete(
+                name=name,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
 
-class ScanPattern(betterproto.ServiceStub):
-    async def async_get(
+class Network(betterproto.ServiceStub):
+    """
+    The network service allows to setup network configuration of Qb2 device.
+    The exact structure of configuration settings is defined by "Network"
+    protocol message. Service provides "SetConfig()" and "GetConfig()" API
+    which allow to apply and read out configuration settings at run-time. The
+    "GetStatus()" API brings configuration and statistical information about
+    currently active network connection.
+    """
+
+    async def async_get_status(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "ScanPatternGetResponse":
-        """Gets scan pattern configuration settings"""
+    ) -> "_data__.NetworkStatus":
+        """Brings information about currently active connection"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.system.services.ScanPattern/Get",
+            "/blickfeld.system.services.Network/GetStatus",
             request,
-            ScanPatternGetResponse,
+            _data__.NetworkStatus,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def get(
+    def get_status(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "ScanPatternGetResponse":
-        """Gets scan pattern configuration settings"""
+    ) -> "_data__.NetworkStatus":
+        """Brings information about currently active connection"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_get(
+            self.async_get_status(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_set(
+    async def async_set_config(
         self,
         *,
-        name: str = "",
-        scan_pattern: "_config__.ScanPattern" = None,
+        hostname: str = "",
+        dhcp: bool = False,
+        manual: "NetworkStatic" = None,
+        link_local: bool = False,
+        wireless: "NetworkWireless" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Sets scan pattern cofiguration settings"""
+        """Applies specified network configuration"""
 
-        request = ScanPatternSetRequest()
-        request.name = name
-        if scan_pattern is not None:
-            request.scan_pattern = scan_pattern
+        request = _config__.Network()
+        request.hostname = hostname
+        request.dhcp = dhcp
+        if manual is not None:
+            request.manual = manual
+        request.link_local = link_local
+        if wireless is not None:
+            request.wireless = wireless
 
         return await self._unary_unary(
-            "/blickfeld.system.services.ScanPattern/Set",
+            "/blickfeld.system.services.Network/SetConfig",
             request,
             betterproto_lib_google_protobuf.Empty,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def set(
+    def set_config(
         self,
         *,
-        name: str = "",
-        scan_pattern: "_config__.ScanPattern" = None,
+        hostname: str = "",
+        dhcp: bool = False,
+        manual: "NetworkStatic" = None,
+        link_local: bool = False,
+        wireless: "NetworkWireless" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
     ) -> "betterproto_lib_google_protobuf.Empty":
-        """Sets scan pattern cofiguration settings"""
+        """Applies specified network configuration"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_set(
-                name=name,
-                scan_pattern=scan_pattern,
+            self.async_set_config(
+                hostname=hostname,
+                dhcp=dhcp,
+                manual=manual,
+                link_local=link_local,
+                wireless=wireless,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_list(
+    async def async_get_config(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "ScanPatternListResponse":
-        """Return list of named scan patterns"""
+    ) -> "_config__.Network":
+        """Reads out provided network configuration"""
 
         request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.system.services.ScanPattern/List",
+            "/blickfeld.system.services.Network/GetConfig",
             request,
-            ScanPatternListResponse,
+            _config__.Network,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def list(
+    def get_config(
         self,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None,
-    ) -> "ScanPatternListResponse":
-        """Return list of named scan patterns"""
+    ) -> "_config__.Network":
+        """Reads out provided network configuration"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_list(
+            self.async_get_config(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_store(
+    async def async_validate(
         self,
         *,
-        name: str = "",
-        scan_pattern: "_config__.ScanPattern" = None,
+        config: "_config__.Network" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Store scan pattern"""
+    ) -> "NetworkValidateResponse":
+        """
+        Validates the network configuration by applying it shortly. If DHCP is
+        configured, it checks if it can acquire an IPv4 address. For static IP
+        address, the validation only works for wireless networks. It then,
+        still cannot allocate a manual IP address if the credentials are wrong.
+        [NOTE] The validation does not yet separate error messages for
+        misconfigured wireless credentials or wrongly configured DHCP server.
+        Thus, the issue is not necessarily on the device side.
+        """
 
-        request = ScanPatternStoreRequest()
-        request.name = name
-        if scan_pattern is not None:
-            request.scan_pattern = scan_pattern
+        request = NetworkValidateRequest()
+        if config is not None:
+            request.config = config
 
         return await self._unary_unary(
-            "/blickfeld.system.services.ScanPattern/Store",
+            "/blickfeld.system.services.Network/Validate",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            NetworkValidateResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def store(
+    def validate(
         self,
         *,
-        name: str = "",
-        scan_pattern: "_config__.ScanPattern" = None,
+        config: "_config__.Network" = None,
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
         metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Store scan pattern"""
+    ) -> "NetworkValidateResponse":
+        """
+        Validates the network configuration by applying it shortly. If DHCP is
+        configured, it checks if it can acquire an IPv4 address. For static IP
+        address, the validation only works for wireless networks. It then,
+        still cannot allocate a manual IP address if the credentials are wrong.
+        [NOTE] The validation does not yet separate error messages for
+        misconfigured wireless credentials or wrongly configured DHCP server.
+        Thus, the issue is not necessarily on the device side.
+        """
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_store(
-                name=name,
-                scan_pattern=scan_pattern,
+            self.async_validate(
+                config=config,
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
 
-    async def async_delete(
+    async def async_get_mac_addresses(
         self,
-        *,
-        name: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Delete stored scan pattern"""
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "NetworkGetMacAddressesResponse":
+        """Get MAC addresses of the available interfaces"""
 
-        request = ScanPatternDeleteRequest()
-        request.name = name
+        request = betterproto_lib_google_protobuf.Empty()
 
         return await self._unary_unary(
-            "/blickfeld.system.services.ScanPattern/Delete",
+            "/blickfeld.system.services.Network/GetMacAddresses",
             request,
-            betterproto_lib_google_protobuf.Empty,
+            NetworkGetMacAddressesResponse,
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
 
-    def delete(
+    def get_mac_addresses(
         self,
-        *,
-        name: str = "",
         timeout: Optional[float] = None,
         deadline: Optional["Deadline"] = None,
-        metadata: Optional["MetadataLike"] = None
-    ) -> "betterproto_lib_google_protobuf.Empty":
-        """Delete stored scan pattern"""
+        metadata: Optional["MetadataLike"] = None,
+    ) -> "NetworkGetMacAddressesResponse":
+        """Get MAC addresses of the available interfaces"""
 
         loop = asyncio.get_event_loop()
         return loop.run_until_complete(
-            self.async_delete(
-                name=name,
+            self.async_get_mac_addresses(
                 timeout=timeout,
                 deadline=deadline,
                 metadata=metadata,
             )
         )
```

### Comparing `blickfeld_qb2-1.5.2/blickfeld_qb2.egg-info/SOURCES.txt` & `blickfeld_qb2-1.5.3/blickfeld_qb2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `blickfeld_qb2-1.5.2/setup.py` & `blickfeld_qb2-1.5.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="blickfeld_qb2",
-    version="1.5.2",
+    version="1.5.3",
     author="Blickfeld GmbH",
     author_email="opensource@blickfeld.com",
     url="https://github.com/Blickfeld/blickfeld-qb2",
     description="Python package to communicate securely with Qb2 LiDAR devices of the Blickfeld GmbH",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

