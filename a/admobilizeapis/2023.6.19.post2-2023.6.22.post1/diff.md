# Comparing `tmp/admobilizeapis-2023.6.19.post2.tar.gz` & `tmp/admobilizeapis-2023.6.22.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/admobilizeapis-2023.6.19.post2.tar", last modified: Mon Jun 19 19:20:54 2023, max compression
+gzip compressed data, was "dist/admobilizeapis-2023.6.22.post1.tar", last modified: Thu Jun 22 05:58:54 2023, max compression
```

## Comparing `admobilizeapis-2023.6.19.post2.tar` & `admobilizeapis-2023.6.22.post1.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/google/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/google/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/google/longrunning/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/google/longrunning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8090 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/google/longrunning/operations_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10932 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/google/longrunning/operations_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/wifi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/wifi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/wifi/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/wifi/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2457 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/wifi/v1/wifi_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/datagateway/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/datagateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/datagateway/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/datagateway/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8861 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8708 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/iam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/iam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    25837 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4250 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    35932 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/notification/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/notification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6645 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10396 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/notification_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14597 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/model_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     2515 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/vision_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/vision_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4194 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/model_pb2.py
--rw-r--r--   0 root         (0) root         (0)    25636 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/vision_pb2.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/mlmodel/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/mlmodel/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/mlmodel/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)     6478 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/mlmodel/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/salestool/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/salestool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/salestool/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/salestool/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4784 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     5528 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15461 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    39106 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28693 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10609 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    28083 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    18992 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    20392 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    99455 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    76701 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    13543 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    41623 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29786 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9576 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14877 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15271 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6954 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    22477 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     8758 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/malos/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/malos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/malos/v1/
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/malos/v1/driver_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/malos/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4590 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/malos/v1/driver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6136 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/malos/v1/maloseye_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/query/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/query/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    14646 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    31149 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28346 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/query_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    15801 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21203 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18378 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    24106 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3240 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/common/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/common/job_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/common/admobilize_types_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     4485 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/common/entity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/common/admobilize_types_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2897 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/common/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/common/entity_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/billing/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/billing/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/billing/v1alpha1/billing_pb2.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)    22301 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16652 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/__init__.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    29481 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10026 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    24348 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21841 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3174 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16356 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/
--rw-r--r--   0 root         (0) root         (0)       76 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)     6814 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      849 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1201 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/README.md
--rw-r--r--   0 root         (0) root         (0)     1293 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 19:20:54.000000 admobilizeapis-2023.6.19.post2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8090 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/operations_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10932 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/operations_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/wifi_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/wifi_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8861 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8708 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    25837 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4250 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    35932 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6645 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    10396 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14597 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/model_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4194 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/model_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    25636 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_pb2.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)     6478 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4784 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     5528 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15461 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    39106 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28693 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10609 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    28083 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    18992 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    20392 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    99455 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    76701 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    13543 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    41623 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29786 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     9576 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    14877 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15271 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     6954 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    22477 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     8758 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/driver_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4590 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/driver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6136 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/maloseye_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/maloseye_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    14646 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    31149 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    28346 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    15801 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21203 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18378 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    24106 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3240 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/job_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/admobilize_types_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     4485 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/entity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/admobilize_types_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2897 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/common/entity_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/billing_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)    22301 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16652 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    29481 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)    10026 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    24348 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21841 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2_grpc.py
+-rw-r--r--   0 root         (0) root         (0)     3174 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    16356 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)     6814 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      849 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1201 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1293 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 05:58:54.000000 admobilizeapis-2023.6.22.post1/setup.cfg
```

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/google/longrunning/operations_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/google/longrunning/operations_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/google/longrunning/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/wifi/v1/wifi_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/wifi/v1/wifi_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/datagateway/v1alpha1/datagateway_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/iam_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/iam/v1alpha1/iam_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/notification_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/notification_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/notification/v1beta1/notification_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/vision_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/vision_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/model_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/model_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/vision/v1/vision_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/vision/v1/vision_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/mlmodel/v1alpha1/mlmodel_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/salestool/v1alpha1/salestool_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1/device_manager_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v2/device_manager_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v2/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha3/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/devicemanagement/v1alpha1/device_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/admprovider/v1alpha1/admprovider_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/malos/v1/driver_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/malos/v1/maloseye_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/malos/v1/maloseye_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/resources_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf import field_mask_pb2 as google_dot_protobuf_dot_field__mask__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)admobilize/query/v1alpha1/resources.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"B\n\x07Project\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x12\n\ncreated_at\x18\x02 \x01(\t\x12\x12\n\nupdated_at\x18\x03 \x01(\t\"\x80\x01\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x66ield\x18\x02 \x01(\t\x12\x11\n\toperation\x18\x03 \x01(\t\x12\x0e\n\x06\x66ilter\x18\x04 \x03(\t\x12\r\n\x05order\x18\x05 \x01(\t\x12\x19\n\x11\x63onversion_factor\x18\x06 \x01(\x01\x12\x0c\n\x04\x63\x61st\x18\x07 \x01(\t\"@\n\x0f\x41ggregateResult\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\n\n\x02\x61s\x18\x03 \x01(\t\"\xbb\x01\n\x0fQueryFromResult\x12\x0e\n\x06select\x18\x01 \x03(\t\x12\x0b\n\x03sum\x18\x02 \x03(\t\x12\x0b\n\x03\x61vg\x18\x03 \x03(\t\x12\x0f\n\x07groupBy\x18\x04 \x03(\t\x12\x43\n\x07orderBy\x18\x05 \x03(\x0b\x32\x32.admobilize.query.v1alpha1.QueryFromResult.OrderBy\x1a(\n\x07OrderBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"4\n\rEncoderParams\x12\x0f\n\x07metrics\x18\x01 \x03(\t\x12\x12\n\ndimensions\x18\x02 \x03(\t\"?\n\x07\x44\x61taset\x12\r\n\x05label\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value\")\n\x0bSchemaField\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x80\x01\n\nClassifier\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\r\n\x05\x66ield\x18\x03 \x01(\t\x12\x42\n\nconditions\x18\x04 \x03(\x0b\x32..admobilize.query.v1alpha1.ClassifierCondition\"+\n\nOrderField\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"M\n\x13\x43lassifierCondition\x12\x0c\n\x04when\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x03\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x03\x12\x0c\n\x04then\x18\x04 \x01(\t\"5\n\x06Status\x12\x13\n\x0bstatus_code\x18\x01 \x01(\t\x12\x16\n\x0estatus_message\x18\x02 \x01(\t\"3\n\tDeviceMap\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\"\xc0\x01\n\x03Job\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.admobilize.query.v1alpha1.Job.Status\x12\x0e\n\x06\x64\x65tail\x18\x03 \x01(\t\x12\x16\n\x0estatus_message\x18\x04 \x01(\t\x12\x11\n\tself_link\x18\x05 \x01(\t\"7\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x08\n\x04\x44ONE\x10\x03\x12\t\n\x05\x45RROR\x10\x04\"\xc9\x04\n\x06Report\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x02 \x03(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x64\x61ys_to_send\x18\x04 \x03(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\r\n\x05\x65mail\x18\x06 \x03(\t\x12\x0e\n\x06\x66ields\x18\x07 \x03(\t\x12\x0e\n\x06\x66ormat\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x10\n\x08interval\x18\n \x01(\t\x12-\n\tlast_sent\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flast_report_url\x18\x0c \x01(\t\x12\r\n\x05media\x18\r \x03(\t\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x12\n\nproject_id\x18\x0f \x01(\t\x12.\n\nstart_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_date\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11\x66ilter_by_weekday\x18\x16 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x17 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06status\x18\x11 \x01(\t\x12\r\n\x05table\x18\x12 \x01(\t\x12\x10\n\x08timezone\x18\x13 \x01(\t\x12\x0c\n\x04type\x18\x14 \x01(\t\"*\n\x0c\x46ilterByTime\x12\r\n\x05start\x18\x01 \x01(\t\x12\x0b\n\x03\x65nd\x18\x02 \x01(\t\")\n\x08\x46ilterBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0c\x43MSDimension\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02\x61s\x18\x02 \x01(\t\"~\n\rCMSDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x15\n\rplaylog_table\x18\x03 \x01(\t\x12\x39\n\x07\x63olumns\x18\x04 \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSColumnsMap\"V\n\rCMSColumnsMap\x12\x13\n\x0b\x61\x64vertisers\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x01(\t\x12\x0e\n\x06medias\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\tB\x93\x01\n\x1d\x63om.admobilize.query.v1alpha1B\nQueryProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)admobilize/query/v1alpha1/resources.proto\x12\x19\x61\x64mobilize.query.v1alpha1\x1a\x1cgoogle/api/annotations.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"B\n\x07Project\x12\x0f\n\x07project\x18\x01 \x01(\t\x12\x12\n\ncreated_at\x18\x02 \x01(\t\x12\x12\n\nupdated_at\x18\x03 \x01(\t\"\x80\x01\n\x06Metric\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05\x66ield\x18\x02 \x01(\t\x12\x11\n\toperation\x18\x03 \x01(\t\x12\x0e\n\x06\x66ilter\x18\x04 \x03(\t\x12\r\n\x05order\x18\x05 \x01(\t\x12\x19\n\x11\x63onversion_factor\x18\x06 \x01(\x01\x12\x0c\n\x04\x63\x61st\x18\x07 \x01(\t\"@\n\x0f\x41ggregateResult\x12\x0e\n\x06metric\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\n\n\x02\x61s\x18\x03 \x01(\t\"\xbb\x01\n\x0fQueryFromResult\x12\x0e\n\x06select\x18\x01 \x03(\t\x12\x0b\n\x03sum\x18\x02 \x03(\t\x12\x0b\n\x03\x61vg\x18\x03 \x03(\t\x12\x0f\n\x07groupBy\x18\x04 \x03(\t\x12\x43\n\x07orderBy\x18\x05 \x03(\x0b\x32\x32.admobilize.query.v1alpha1.QueryFromResult.OrderBy\x1a(\n\x07OrderBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"4\n\rEncoderParams\x12\x0f\n\x07metrics\x18\x01 \x03(\t\x12\x12\n\ndimensions\x18\x02 \x03(\t\"?\n\x07\x44\x61taset\x12\r\n\x05label\x18\x01 \x01(\t\x12%\n\x05value\x18\x02 \x01(\x0b\x32\x16.google.protobuf.Value\")\n\x0bSchemaField\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\"\x80\x01\n\nClassifier\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\x12\r\n\x05\x66ield\x18\x03 \x01(\t\x12\x42\n\nconditions\x18\x04 \x03(\x0b\x32..admobilize.query.v1alpha1.ClassifierCondition\"+\n\nOrderField\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05order\x18\x02 \x01(\t\"M\n\x13\x43lassifierCondition\x12\x0c\n\x04when\x18\x01 \x01(\t\x12\r\n\x05start\x18\x02 \x01(\x02\x12\x0b\n\x03\x65nd\x18\x03 \x01(\x02\x12\x0c\n\x04then\x18\x04 \x01(\t\"5\n\x06Status\x12\x13\n\x0bstatus_code\x18\x01 \x01(\t\x12\x16\n\x0estatus_message\x18\x02 \x01(\t\"3\n\tDeviceMap\x12\x11\n\tdevice_id\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65vice_name\x18\x02 \x01(\t\"\xc0\x01\n\x03Job\x12\x0e\n\x06job_id\x18\x01 \x01(\t\x12\x35\n\x06status\x18\x02 \x01(\x0e\x32%.admobilize.query.v1alpha1.Job.Status\x12\x0e\n\x06\x64\x65tail\x18\x03 \x01(\t\x12\x16\n\x0estatus_message\x18\x04 \x01(\t\x12\x11\n\tself_link\x18\x05 \x01(\t\"7\n\x06Status\x12\x0b\n\x07PENDING\x10\x00\x12\x0b\n\x07RUNNING\x10\x01\x12\x08\n\x04\x44ONE\x10\x03\x12\t\n\x05\x45RROR\x10\x04\"\xc9\x04\n\x06Report\x12\n\n\x02id\x18\x01 \x01(\t\x12\x13\n\x0b\x61\x64vertisers\x18\x02 \x03(\t\x12.\n\ncreated_on\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x64\x61ys_to_send\x18\x04 \x03(\t\x12\x12\n\ndevice_ids\x18\x05 \x03(\t\x12\r\n\x05\x65mail\x18\x06 \x03(\t\x12\x0e\n\x06\x66ields\x18\x07 \x03(\t\x12\x0e\n\x06\x66ormat\x18\x08 \x01(\t\x12\x11\n\tfrequency\x18\t \x01(\t\x12\x10\n\x08interval\x18\n \x01(\t\x12-\n\tlast_sent\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x17\n\x0flast_report_url\x18\x0c \x01(\t\x12\r\n\x05media\x18\r \x03(\t\x12\x0c\n\x04name\x18\x0e \x01(\t\x12\x12\n\nproject_id\x18\x0f \x01(\t\x12.\n\nstart_date\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_date\x18\x15 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x19\n\x11\x66ilter_by_weekday\x18\x16 \x03(\r\x12?\n\x0e\x66ilter_by_time\x18\x17 \x01(\x0b\x32\'.admobilize.query.v1alpha1.FilterByTime\x12\x0e\n\x06status\x18\x11 \x01(\t\x12\r\n\x05table\x18\x12 \x01(\t\x12\x10\n\x08timezone\x18\x13 \x01(\t\x12\x0c\n\x04type\x18\x14 \x01(\t\"*\n\x0c\x46ilterByTime\x12\r\n\x05start\x18\x01 \x01(\t\x12\x0b\n\x03\x65nd\x18\x02 \x01(\t\")\n\x08\x46ilterBy\x12\x0e\n\x06\x63olumn\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t\"(\n\x0c\x43MSDimension\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\n\n\x02\x61s\x18\x02 \x01(\t\"~\n\rCMSDescriptor\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05table\x18\x02 \x01(\t\x12\x15\n\rplaylog_table\x18\x03 \x01(\t\x12\x39\n\x07\x63olumns\x18\x04 \x01(\x0b\x32(.admobilize.query.v1alpha1.CMSColumnsMap\"V\n\rCMSColumnsMap\x12\x13\n\x0b\x61\x64vertisers\x18\x01 \x01(\t\x12\r\n\x05sites\x18\x02 \x01(\t\x12\x0e\n\x06medias\x18\x03 \x01(\t\x12\x11\n\ttimestamp\x18\x04 \x01(\tB\x93\x01\n\x1d\x63om.admobilize.query.v1alpha1B\nQueryProtoP\x01Z@bitbucket.org/admobilize/admobilizeapis-go/pkg/queryapi/v1alpha1\xa2\x02\x05\x41\x44MQY\xaa\x02\x19\x41\x64Mobilize.Query.V1Alpha1b\x06proto3')
 
 
 
 _PROJECT = DESCRIPTOR.message_types_by_name['Project']
 _METRIC = DESCRIPTOR.message_types_by_name['Metric']
 _AGGREGATERESULT = DESCRIPTOR.message_types_by_name['AggregateResult']
 _QUERYFROMRESULT = DESCRIPTOR.message_types_by_name['QueryFromResult']
```

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/query_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/query/v1alpha1/query_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/query/v1alpha1/query_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/ayuda_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/ayuda/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/ayuda/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/signagelive_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/signagelive/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/signagelive/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/common/entity_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/common/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/common/admobilize_types_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/common/admobilize_types_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/common/job_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/common/job_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/billing/v1alpha1/billing_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/billing/v1alpha1/billing_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/brightauthor/v1alpha1/brightauthor_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/cmsintegrations/v1/cmsintegrations_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/resources_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py` & `admobilizeapis-2023.6.22.post1/admobilize/proto/broadsign/v1alpha1/broadsign_service_pb2.py`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/PKG-INFO` & `admobilizeapis-2023.6.22.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.6.19.post2
+Version: 2023.6.22.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/SOURCES.txt` & `admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/admobilizeapis.egg-info/PKG-INFO` & `admobilizeapis-2023.6.22.post1/admobilizeapis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: admobilizeapis
-Version: 2023.6.19.post2
+Version: 2023.6.22.post1
 Summary: Protobufs used in AdMobilize Ecosystem
 Home-page: https://www.bitbucket.org/admobilize/admobilizeapis
 Author: AdMobilize Team
 Author-email: devel@admobilize.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `admobilizeapis-2023.6.19.post2/README.md` & `admobilizeapis-2023.6.22.post1/README.md`

 * *Files identical despite different names*

### Comparing `admobilizeapis-2023.6.19.post2/setup.py` & `admobilizeapis-2023.6.22.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 install_requires = ["google-api-core >= 1.6.0, < 2.0.0dev", "protobuf >= 3.6.0, < 4.0"]
 
 extras_require = {"grpc": ["grpcio>=1.2.0"]}
 
 setup(
     name="admobilizeapis",
-    version='2023.06.19r2',
+    version='2023.06.22r1',
     author="AdMobilize Team",
     author_email="devel@admobilize.com",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Programming Language :: Python",
```

