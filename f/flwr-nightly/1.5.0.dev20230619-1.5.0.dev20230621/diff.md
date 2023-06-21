# Comparing `tmp/flwr_nightly-1.5.0.dev20230619.tar.gz` & `tmp/flwr_nightly-1.5.0.dev20230621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.5.0.dev20230619.tar", max compression
+gzip compressed data, was "flwr_nightly-1.5.0.dev20230621.tar", max compression
```

## Comparing `flwr_nightly-1.5.0.dev20230619.tar` & `flwr_nightly-1.5.0.dev20230621.tar`

### file list

```diff
@@ -1,113 +1,112 @@
--rw-r--r--   0        0        0    11358 2023-06-19 23:02:38.137018 flwr_nightly-1.5.0.dev20230619/LICENSE
--rw-r--r--   0        0        0    10363 2023-06-19 23:02:38.137018 flwr_nightly-1.5.0.dev20230619/README.md
--rw-r--r--   0        0        0     5031 2023-06-19 23:03:07.322816 flwr_nightly-1.5.0.dev20230619/pyproject.toml
--rw-r--r--   0        0        0      952 2023-06-19 23:02:38.433037 flwr_nightly-1.5.0.dev20230619/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1164 2023-06-19 23:02:38.433037 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    13835 2023-06-19 23:02:38.433037 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     7677 2023-06-19 23:02:38.433037 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     7209 2023-06-19 23:02:38.433037 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      728 2023-06-19 23:02:38.433037 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     4295 2023-06-19 23:02:38.433037 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      745 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     5474 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      712 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5077 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1685 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     5318 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      728 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0     8333 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     2877 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1875 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1113 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0      884 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     1791 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     1889 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     3482 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     2120 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0    16315 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7805 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     3714 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      848 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      809 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     4826 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     3906 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     4877 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/driver_client_manager.py
--rw-r--r--   0        0        0     5653 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0      676 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     4663 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     3815 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     5727 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     1617 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     4982 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     4554 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     4275 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     1495 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1188 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     8232 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0    10889 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0    18721 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1370 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    26333 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6120 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2227 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1054 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      705 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     3919 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      704 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      728 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     4467 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
--rw-r--r--   0        0        0     5686 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6408 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4650 2023-06-19 23:02:38.437038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11501 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0     6313 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
--rw-r--r--   0        0        0      751 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     1858 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      724 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2024 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      728 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     3718 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4897 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15958 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/server.py
--rw-r--r--   0        0        0      996 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     6774 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    19294 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     4833 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1647 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     1667 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0     6099 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     4654 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     6995 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5893 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6740 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7014 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11522 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9991 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8286 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2708 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5428 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     7126 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     6026 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     3519 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     7079 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6343 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10154 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7484 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      901 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5067 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4940 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1271 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0     7826 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      727 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     5535 2023-06-19 23:02:38.441038 flwr_nightly-1.5.0.dev20230619/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0    12494 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230619/setup.py
--rw-r--r--   0        0        0    12838 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230619/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-06-21 23:02:31.551122 flwr_nightly-1.5.0.dev20230621/LICENSE
+-rw-r--r--   0        0        0    10363 2023-06-21 23:02:31.551122 flwr_nightly-1.5.0.dev20230621/README.md
+-rw-r--r--   0        0        0     5031 2023-06-21 23:03:00.844056 flwr_nightly-1.5.0.dev20230621/pyproject.toml
+-rw-r--r--   0        0        0      952 2023-06-21 23:02:31.859131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0     1164 2023-06-21 23:02:31.859131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    13835 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     7677 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     7209 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      728 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     4295 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      745 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     5474 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0      712 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     5077 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1685 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     5318 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      728 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0     8333 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     2877 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1875 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     1113 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0      884 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     1791 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     1889 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     3482 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0     2120 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0    16315 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7805 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     3714 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      848 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      809 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/__init__.py
+-rw-r--r--   0        0        0     4826 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/app.py
+-rw-r--r--   0        0        0     3906 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/driver.py
+-rw-r--r--   0        0        0     4877 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/driver_client_manager.py
+-rw-r--r--   0        0        0     5653 2023-06-21 23:02:31.863131 flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/driver_client_proxy.py
+-rw-r--r--   0        0        0      676 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     4663 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     3815 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     5727 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     1617 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4982 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     4554 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     4275 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     1495 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1188 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8232 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0    10889 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0    18721 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1370 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    26333 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6120 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2227 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0     1054 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      705 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     3919 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/driver/driver_servicer.py
+-rw-r--r--   0        0        0      704 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/__init__.py
+-rw-r--r--   0        0        0      728 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     4467 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py
+-rw-r--r--   0        0        0     5686 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6408 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4650 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11501 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0     6313 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py
+-rw-r--r--   0        0        0      751 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     1858 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      724 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     2024 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      728 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     3718 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0     4897 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0    15958 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0      996 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/__init__.py
+-rw-r--r--   0        0        0     6774 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/in_memory_state.py
+-rw-r--r--   0        0        0    19294 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/sqlite_state.py
+-rw-r--r--   0        0        0     4833 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/state.py
+-rw-r--r--   0        0        0     1647 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/state_factory.py
+-rw-r--r--   0        0        0     1667 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0     6099 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     4654 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     6995 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5893 2023-06-21 23:02:31.867132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6740 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7014 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11522 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9991 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8286 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2708 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5428 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     7126 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     6026 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     3519 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     7079 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6343 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10154 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7484 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      901 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5067 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     4940 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0     1271 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0     7826 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     5535 2023-06-21 23:02:31.871132 flwr_nightly-1.5.0.dev20230621/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0    12538 1970-01-01 00:00:00.000000 flwr_nightly-1.5.0.dev20230621/PKG-INFO
```

### Comparing `flwr_nightly-1.5.0.dev20230619/LICENSE` & `flwr_nightly-1.5.0.dev20230621/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/README.md` & `flwr_nightly-1.5.0.dev20230621/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/pyproject.toml` & `flwr_nightly-1.5.0.dev20230621/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.5.0-dev20230619"
+version = "1.5.0-dev20230621"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.dev>"]
 readme = "README.md"
 homepage = "https://flower.dev"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.dev"
```

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/app.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/client.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/client/rest_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/address.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/constant.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/date.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/dp.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/grpc.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/logger.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/logger.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/parameter.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/serde.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/typing.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/common/version.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/app.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/driver.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/driver/driver_client_proxy.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/driver/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/app.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/criterion.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/driver/driver_servicer.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/driver_client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_bidi/ins_scheduler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/fleet/rest_rere/rest_api.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/history.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/server.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/in_memory_state.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/sqlite_state.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/state.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/state/state_factory.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/simulation/app.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.5.0.dev20230621/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.5.0.dev20230619/setup.py` & `flwr_nightly-1.5.0.dev20230621/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,205 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flwr-nightly
+Version: 1.5.0.dev20230621
+Summary: Flower: A Friendly Federated Learning Framework
+Home-page: https://flower.dev
+License: Apache-2.0
+Author: The Flower Authors
+Author-email: hello@flower.dev
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
+Provides-Extra: rest
+Provides-Extra: simulation
+Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra == "rest"
+Requires-Dist: grpcio (>=1.48.2,<2.0.0,!=1.52.0)
+Requires-Dist: importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8"
+Requires-Dist: iterators (>=0.0.2,<0.0.3)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: protobuf (>=3.19.0,<4.0.0)
+Requires-Dist: ray[default] (>=2.4.0,<3.0.0) ; extra == "simulation"
+Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra == "rest"
+Requires-Dist: starlette (>=0.26.1,<0.27.0) ; extra == "rest"
+Requires-Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest"
+Project-URL: Documentation, https://flower.dev
+Project-URL: Repository, https://github.com/adap/flower
+Description-Content-Type: text/markdown
+
+# Flower: A Friendly Federated Learning Framework
+
+<p align="center">
+  <a href="https://flower.dev/">
+    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />
+  </a>
+</p>
+<p align="center">
+    <a href="https://flower.dev/">Website</a> |
+    <a href="https://flower.dev/blog">Blog</a> |
+    <a href="https://flower.dev/docs/">Docs</a> |
+    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |
+    <a href="https://flower.dev/join-slack">Slack</a>
+    <br /><br />
+</p>
+
+[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)
+[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)
+![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)
+![Downloads](https://pepy.tech/badge/flwr)
+[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)
+
+Flower (`flwr`) is a framework for building federated learning systems. The
+design of Flower is based on a few guiding principles:
+
+* **Customizable**: Federated learning systems vary wildly from one use case to
+  another. Flower allows for a wide range of different configurations depending
+  on the needs of each individual use case.
+
+* **Extendable**: Flower originated from a research project at the University of
+  Oxford, so it was built with AI research in mind. Many components can be
+  extended and overridden to build new state-of-the-art systems.
+
+* **Framework-agnostic**: Different machine learning frameworks have different
+  strengths. Flower can be used with any machine learning framework, for
+  example, [PyTorch](https://pytorch.org),
+  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/
+) for federated analytics, or even raw [NumPy](https://numpy.org/)
+  for users who enjoy computing gradients by hand.
+
+* **Understandable**: Flower is written with maintainability in mind. The
+  community is encouraged to both read and contribute to the codebase.
+
+Meet the Flower community on [flower.dev](https://flower.dev)!
+
+## Federated Learning Tutorial
+
+Flower's goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.
+
+0. **What is Federated Learning?**
+
+   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))
+
+1. **An Introduction to Federated Learning**
+
+   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))
+
+2. **Using Strategies in Federated Learning**
+
+   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))
+   
+3. **Building Strategies for Federated Learning**
+
+   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))
+   
+4. **Custom Clients for Federated Learning**
+
+   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))
+
+Stay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.
+
+## Documentation
+
+[Flower Docs](https://flower.dev/docs):
+* [Installation](https://flower.dev/docs/installation.html)
+* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)
+* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)
+* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)
+* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)
+* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)
+* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)
+* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)
+* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)
+* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
+* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)
+* [Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html)
+
+## Flower Baselines
+
+Flower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:
+
+* [FedAvg](https://arxiv.org/abs/1602.05629):
+  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)
+* [FedProx](https://arxiv.org/abs/1812.06127):
+  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)
+* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):
+  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)
+* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):
+  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)
+
+Check the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)
+
+The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)
+
+## Flower Usage Examples
+
+Several code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).
+
+Quickstart examples:
+
+* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)
+* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)
+* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)
+* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)
+* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)
+* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)
+* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)
+* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)
+* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
+* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)
+
+Other [examples](https://github.com/adap/flower/tree/main/examples):
+
+* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)
+* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)
+* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)
+* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)
+* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)
+* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)
+* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))
+
+## Community
+
+Flower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.
+
+<a href="https://github.com/adap/flower/graphs/contributors">
+  <img src="https://contrib.rocks/image?repo=adap/flower" />
+</a>
+
+## Citation
+
+If you publish work that uses Flower, please cite Flower as follows: 
+
+```bibtex
+@article{beutel2020flower,
+  title={Flower: A Friendly Federated Learning Research Framework},
+  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, 
+  journal={arXiv preprint arXiv:2007.14390},
+  year={2020}
+}
+```
 
-package_dir = \
-{'': 'src/py'}
+Please also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.
 
-packages = \
-['flwr',
- 'flwr.client',
- 'flwr.client.grpc_client',
- 'flwr.client.grpc_rere_client',
- 'flwr.client.message_handler',
- 'flwr.client.rest_client',
- 'flwr.common',
- 'flwr.driver',
- 'flwr.proto',
- 'flwr.server',
- 'flwr.server.driver',
- 'flwr.server.fleet',
- 'flwr.server.fleet.grpc_bidi',
- 'flwr.server.fleet.grpc_rere',
- 'flwr.server.fleet.message_handler',
- 'flwr.server.fleet.rest_rere',
- 'flwr.server.state',
- 'flwr.server.strategy',
- 'flwr.server.utils',
- 'flwr.simulation',
- 'flwr.simulation.ray_transport']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['grpcio>=1.48.2,<2.0.0,!=1.52.0',
- 'iterators>=0.0.2,<0.0.3',
- 'numpy>=1.21.0,<2.0.0',
- 'protobuf>=3.19.0,<4.0.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
- 'rest': ['requests>=2.28.2,<3.0.0',
-          'fastapi>=0.95.0,<0.96.0',
-          'starlette>=0.26.1,<0.27.0',
-          'uvicorn[standard]>=0.21.1,<0.22.0'],
- 'simulation': ['ray[default]>=2.4.0,<3.0.0']}
-
-entry_points = \
-{'console_scripts': ['flower-client = flwr.client:run_client',
-                     'flower-driver-api = flwr.server:run_driver_api',
-                     'flower-fleet-api = flwr.server:run_fleet_api',
-                     'flower-server = flwr.server:run_server']}
-
-setup_kwargs = {
-    'name': 'flwr-nightly',
-    'version': '1.5.0.dev20230619',
-    'description': 'Flower: A Friendly Federated Learning Framework',
-    'long_description': '# Flower: A Friendly Federated Learning Framework\n\n<p align="center">\n  <a href="https://flower.dev/">\n    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />\n  </a>\n</p>\n<p align="center">\n    <a href="https://flower.dev/">Website</a> |\n    <a href="https://flower.dev/blog">Blog</a> |\n    <a href="https://flower.dev/docs/">Docs</a> |\n    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |\n    <a href="https://flower.dev/join-slack">Slack</a>\n    <br /><br />\n</p>\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated learning systems. The\ndesign of Flower is based on a few guiding principles:\n\n* **Customizable**: Federated learning systems vary wildly from one use case to\n  another. Flower allows for a wide range of different configurations depending\n  on the needs of each individual use case.\n\n* **Extendable**: Flower originated from a research project at the University of\n  Oxford, so it was built with AI research in mind. Many components can be\n  extended and overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**: Different machine learning frameworks have different\n  strengths. Flower can be used with any machine learning framework, for\n  example, [PyTorch](https://pytorch.org),\n  [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https://pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://numpy.org/)\n  for users who enjoy computing gradients by hand.\n\n* **Understandable**: Flower is written with maintainability in mind. The\n  community is encouraged to both read and contribute to the codebase.\n\nMeet the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.\n\n0. **What is Federated Learning?**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb))\n   \n3. **Building Strategies for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n   \n4. **Custom Clients for Federated Learning**\n\n   [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon. Topics include **Privacy and Security in Federated Learning**, and **Scaling Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/docs):\n* [Installation](https://flower.dev/docs/installation.html)\n* [Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n* [Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android [code example])](https://github.com/adap/flower/tree/main/examples/android)\n* [Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html)\n\n## Flower Baselines\n\nFlower Baselines is a collection of community-contributed experiments that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/1602.05629):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/1812.06127):\n  * [MNIST](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on non-IID Features via Local Batch Normalization](https://arxiv.org/abs/2102.07623):\n  * [Convergence Rate](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive Federated Optimization](https://arxiv.org/abs/2003.00295):\n  * [CIFAR-10/100](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/adaptive_federated_optimization)\n\nCheck the Flower documentation to learn more: [Using Baselines](https://flower.dev/docs/using-baselines.html)\n\nThe Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline: [Contributing Baselines](https://flower.dev/docs/contributing-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded_devices)\n* [Android & TFLite](https://github.com/adap/flower/tree/main/examples/android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.\n\n<a href="https://github.com/adap/flower/graphs/contributors">\n  <img src="https://contrib.rocks/image?repo=adap/flower" />\n</a>\n\n## Citation\n\nIf you publish work that uses Flower, please cite Flower as follows: \n\n```bibtex\n@article{beutel2020flower,\n  title={Flower: A Friendly Federated Learning Research Framework},\n  author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and Gusmão, Pedro PB de and Lane, Nicholas D}, \n  journal={arXiv preprint arXiv:2007.14390},\n  year={2020}\n}\n```\n\nPlease also consider adding your publication to the list of Flower-based publications in the docs, just open a Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n',
-    'author': 'The Flower Authors',
-    'author_email': 'hello@flower.dev',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://flower.dev',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+## Contributing to Flower
 
+We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,164 +1,162 @@
-# -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'': 'src/
-py'} packages = \ ['flwr', 'flwr.client', 'flwr.client.grpc_client',
-'flwr.client.grpc_rere_client', 'flwr.client.message_handler',
-'flwr.client.rest_client', 'flwr.common', 'flwr.driver', 'flwr.proto',
-'flwr.server', 'flwr.server.driver', 'flwr.server.fleet',
-'flwr.server.fleet.grpc_bidi', 'flwr.server.fleet.grpc_rere',
-'flwr.server.fleet.message_handler', 'flwr.server.fleet.rest_rere',
-'flwr.server.state', 'flwr.server.strategy', 'flwr.server.utils',
-'flwr.simulation', 'flwr.simulation.ray_transport'] package_data = \ {'':
-['*']} install_requires = \ ['grpcio>=1.48.2,<2.0.0,!=1.52.0',
-'iterators>=0.0.2,<0.0.3', 'numpy>=1.21.0,<2.0.0', 'protobuf>=3.19.0,<4.0.0']
-extras_require = \ {':python_version < "3.8"': ['importlib-
-metadata>=4.0.0,<5.0.0'], 'rest': ['requests>=2.28.2,<3.0.0',
-'fastapi>=0.95.0,<0.96.0', 'starlette>=0.26.1,<0.27.0', 'uvicorn
-[standard]>=0.21.1,<0.22.0'], 'simulation': ['ray[default]>=2.4.0,<3.0.0']}
-entry_points = \ {'console_scripts': ['flower-client = flwr.client:run_client',
-'flower-driver-api = flwr.server:run_driver_api', 'flower-fleet-api =
-flwr.server:run_fleet_api', 'flower-server = flwr.server:run_server']}
-setup_kwargs = { 'name': 'flwr-nightly', 'version': '1.5.0.dev20230619',
-'description': 'Flower: A Friendly Federated Learning Framework',
-'long_description': '# Flower: A Friendly Federated Learning Framework\n\n
-                          \n \n_[Flower_Website]\n\n
-\n
-           \n Website |\n Blog |\n Docs |\n Conference |\n Slack\n
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.5.0.dev20230621 Summary:
+Flower: A Friendly Federated Learning Framework Home-page: https://flower.dev
+License: Apache-2.0 Author: The Flower Authors Author-email: hello@flower.dev
+Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
+Stable Classifier: Intended Audience :: Developers Classifier: Intended
+Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Operating System :: MacOS :: MacOS X Classifier:
+Operating System :: POSIX :: Linux Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
+Language :: Python :: Implementation :: CPython Classifier: Topic ::
+Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
+Mathematics Classifier: Topic :: Software Development Classifier: Topic ::
+Software Development :: Libraries Classifier: Topic :: Software Development ::
+Libraries :: Python Modules Classifier: Typing :: Typed Provides-Extra: rest
+Provides-Extra: simulation Requires-Dist: fastapi (>=0.95.0,<0.96.0) ; extra ==
+"rest" Requires-Dist: grpcio (>=1.48.2,<2.0.0,!=1.52.0) Requires-Dist:
+importlib-metadata (>=4.0.0,<5.0.0) ; python_version < "3.8" Requires-Dist:
+iterators (>=0.0.2,<0.0.3) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-
+Dist: protobuf (>=3.19.0,<4.0.0) Requires-Dist: ray[default] (>=2.4.0,<3.0.0) ;
+extra == "simulation" Requires-Dist: requests (>=2.28.2,<3.0.0) ; extra ==
+"rest" Requires-Dist: starlette (>=0.26.1,<0.27.0) ; extra == "rest" Requires-
+Dist: uvicorn[standard] (>=0.21.1,<0.22.0) ; extra == "rest" Project-URL:
+Documentation, https://flower.dev Project-URL: Repository, https://github.com/
+adap/flower Description-Content-Type: text/markdown # Flower: A Friendly
+Federated Learning Framework
+                               [Flower_Website]
+                  Website | Blog | Docs | Conference | Slack
 
-                                      \n
-\n\n[![GitHub license](https://img.shields.io/github/license/adap/flower)]
-(https://github.com/adap/flower/blob/main/LICENSE)\n[![PRs Welcome](https://
+[![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
+github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
-flower/blob/main/CONTRIBUTING.md)\n![Build](https://github.com/adap/flower/
-actions/workflows/flower.yml/badge.svg)\n![Downloads](https://pepy.tech/badge/
-flwr)\n[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://
-flower.dev/join-slack)\n\nFlower (`flwr`) is a framework for building federated
-learning systems. The\ndesign of Flower is based on a few guiding principles:
-\n\n* **Customizable**: Federated learning systems vary wildly from one use
-case to\n another. Flower allows for a wide range of different configurations
-depending\n on the needs of each individual use case.\n\n* **Extendable**:
-Flower originated from a research project at the University of\n Oxford, so it
-was built with AI research in mind. Many components can be\n extended and
-overridden to build new state-of-the-art systems.\n\n* **Framework-agnostic**:
-Different machine learning frameworks have different\n strengths. Flower can be
-used with any machine learning framework, for\n example, [PyTorch](https://
-pytorch.org),\n [TensorFlow](https://tensorflow.org), [Hugging Face
-Transformers](https://huggingface.co/), [PyTorch Lightning](https://
-pytorchlightning.ai/), [MXNet](https://mxnet.apache.org/), [scikit-learn]
-(https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite]
-(https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [Pandas](https:
-//pandas.pydata.org/\n) for federated analytics, or even raw [NumPy](https://
-numpy.org/)\n for users who enjoy computing gradients by hand.\n\n*
-**Understandable**: Flower is written with maintainability in mind. The\n
-community is encouraged to both read and contribute to the codebase.\n\nMeet
-the Flower community on [flower.dev](https://flower.dev)!\n\n## Federated
-Learning Tutorial\n\nFlower\'s goal is to make federated learning accessible to
-everyone. This series of tutorials introduces the fundamentals of federated
-learning and how to implement them in Flower.\n\n0. **What is Federated
-Learning?**\n\n [![Open in Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/
-main/doc/source/tutorial/Flower-0-What-is-FL.ipynb) (or open the [Jupyter
-Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-
-0-What-is-FL.ipynb))\n\n1. **An Introduction to Federated Learning**\n\n [!
-[Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/adap/flower/blob/main/doc/source/
-tutorial/Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook]
-(https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-
-to-FL-PyTorch.ipynb))\n\n2. **Using Strategies in Federated Learning**\n\n [!
-[Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]
-(https://colab.research.google.com/github/adap/flower/blob/main/doc/source/
-tutorial/Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter
-Notebook](https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-
-2-Strategies-in-FL-PyTorch.ipynb))\n \n3. **Building Strategies for Federated
-Learning**\n\n [![Open in Colab](https://colab.research.google.com/assets/
-colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/
-main/doc/source/tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open
-the [Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/
-tutorial/Flower-3-Building-a-Strategy-PyTorch.ipynb))\n \n4. **Custom Clients
-for Federated Learning**\n\n [![Open in Colab](https://
+flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
+actions/workflows/flower.yml/badge.svg) ![Downloads](https://pepy.tech/badge/
+flwr) [![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://
+flower.dev/join-slack) Flower (`flwr`) is a framework for building federated
+learning systems. The design of Flower is based on a few guiding principles: *
+**Customizable**: Federated learning systems vary wildly from one use case to
+another. Flower allows for a wide range of different configurations depending
+on the needs of each individual use case. * **Extendable**: Flower originated
+from a research project at the University of Oxford, so it was built with AI
+research in mind. Many components can be extended and overridden to build new
+state-of-the-art systems. * **Framework-agnostic**: Different machine learning
+frameworks have different strengths. Flower can be used with any machine
+learning framework, for example, [PyTorch](https://pytorch.org), [TensorFlow]
+(https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/),
+[PyTorch Lightning](https://pytorchlightning.ai/), [MXNet](https://
+mxnet.apache.org/), [scikit-learn](https://scikit-learn.org/), [JAX](https://
+jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://
+www.fast.ai/), [Pandas](https://pandas.pydata.org/ ) for federated analytics,
+or even raw [NumPy](https://numpy.org/) for users who enjoy computing gradients
+by hand. * **Understandable**: Flower is written with maintainability in mind.
+The community is encouraged to both read and contribute to the codebase. Meet
+the Flower community on [flower.dev](https://flower.dev)! ## Federated Learning
+Tutorial Flower's goal is to make federated learning accessible to everyone.
+This series of tutorials introduces the fundamentals of federated learning and
+how to implement them in Flower. 0. **What is Federated Learning?** [![Open in
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
+Flower-0-What-is-FL.ipynb) (or open the [Jupyter Notebook](https://github.com/
+adap/flower/blob/main/doc/source/tutorial/Flower-0-What-is-FL.ipynb)) 1. **An
+Introduction to Federated Learning** [![Open in Colab](https://
 colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
-Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the [Jupyter Notebook]
-(https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-4-Client-
-and-NumPyClient-PyTorch.ipynb))\n\nStay tuned, more tutorials are coming soon.
-Topics include **Privacy and Security in Federated Learning**, and **Scaling
-Federated Learning**.\n\n## Documentation\n\n[Flower Docs](https://flower.dev/
-docs):\n* [Installation](https://flower.dev/docs/installation.html)\n*
-[Quickstart (TensorFlow)](https://flower.dev/docs/quickstart-
-tensorflow.html)\n* [Quickstart (PyTorch)](https://flower.dev/docs/quickstart-
-pytorch.html)\n* [Quickstart (Hugging Face [code example])](https://flower.dev/
-docs/quickstart-huggingface.html)\n* [Quickstart (PyTorch Lightning [code
-example])](https://flower.dev/docs/quickstart-pytorch-lightning.html)\n*
-[Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-
-through.html)\n* [Quickstart (Pandas)](https://flower.dev/docs/quickstart-
-pandas.html)\n* [Quickstart (fastai)](https://flower.dev/docs/quickstart-
-fastai.html)\n* [Quickstart (JAX)](https://github.com/adap/flower/tree/main/
-examples/quickstart_jax)\n* [Quickstart (scikit-learn)](https://github.com/
-adap/flower/tree/main/examples/sklearn-logreg-mnist)\n* [Quickstart (TFLite on
-Android [code example])](https://github.com/adap/flower/tree/main/examples/
-android)\n* [Quickstart (iOS)](https://flower.dev/docs/quickstart-
-ios.html)\n\n## Flower Baselines\n\nFlower Baselines is a collection of
-community-contributed experiments that reproduce the experiments performed in
-popular federated learning publications. Researchers can build on Flower
-Baselines to quickly evaluate new ideas:\n\n* [FedAvg](https://arxiv.org/abs/
-1602.05629):\n * [MNIST](https://github.com/adap/flower/tree/main/baselines/
-flwr_baselines/publications/fedavg_mnist)\n* [FedProx](https://arxiv.org/abs/
-1812.06127):\n * [MNIST](https://github.com/adap/flower/tree/main/baselines/
-flwr_baselines/publications/fedprox_mnist)\n* [FedBN: Federated Learning on
-non-IID Features via Local Batch Normalization](https://arxiv.org/abs/
-2102.07623):\n * [Convergence Rate](https://github.com/adap/flower/tree/main/
-baselines/flwr_baselines/publications/fedbn/convergence_rate)\n* [Adaptive
-Federated Optimization](https://arxiv.org/abs/2003.00295):\n * [CIFAR-10/100]
-(https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
-publications/adaptive_federated_optimization)\n\nCheck the Flower documentation
-to learn more: [Using Baselines](https://flower.dev/docs/using-
-baselines.html)\n\nThe Flower community loves contributions! Make your work
-more visible and enable others to build on it by contributing it as a baseline:
-[Contributing Baselines](https://flower.dev/docs/contributing-
-baselines.html)\n\n## Flower Usage Examples\n\nSeveral code examples show
-different usage scenarios of Flower (in combination with popular machine
-learning frameworks such as PyTorch or TensorFlow).\n\nQuickstart examples:
-\n\n* [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/
-examples/quickstart_tensorflow)\n* [Quickstart (PyTorch)](https://github.com/
-adap/flower/tree/main/examples/quickstart_pytorch)\n* [Quickstart (Hugging
-Face)](https://github.com/adap/flower/tree/main/examples/
-quickstart_huggingface)\n* [Quickstart (PyTorch Lightning)](https://github.com/
-adap/flower/tree/main/examples/quickstart_pytorch_lightning)\n* [Quickstart
-(fastai)](https://github.com/adap/flower/tree/main/examples/
-quickstart_fastai)\n* [Quickstart (Pandas)](https://github.com/adap/flower/
-tree/main/examples/quickstart_pandas)\n* [Quickstart (MXNet)](https://
-github.com/adap/flower/tree/main/examples/quickstart_mxnet)\n* [Quickstart
-(JAX)](https://github.com/adap/flower/tree/main/examples/quickstart_jax)\n*
-[Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/
-sklearn-logreg-mnist)\n* [Quickstart (TFLite on Android)](https://github.com/
-adap/flower/tree/main/examples/android)\n\nOther [examples](https://github.com/
-adap/flower/tree/main/examples):\n\n* [Raspberry Pi & Nvidia Jetson Tutorial]
-(https://github.com/adap/flower/tree/main/examples/embedded_devices)\n*
-[Android & TFLite](https://github.com/adap/flower/tree/main/examples/
-android)\n* [PyTorch: From Centralized to Federated](https://github.com/adap/
-flower/tree/main/examples/pytorch_from_centralized_to_federated)\n* [MXNet:
-From Centralized to Federated](https://github.com/adap/flower/tree/main/
-examples/mxnet_from_centralized_to_federated)\n* [Advanced Flower with
-TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/
-advanced_tensorflow)\n* [Advanced Flower with PyTorch](https://github.com/adap/
-flower/tree/main/examples/advanced_pytorch)\n* Single-Machine Simulation of
-Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/
-examples/simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/
-tree/main/examples/simulation_tensorflow))\n\n## Community\n\nFlower is built
-by a wonderful community of researchers and engineers. [Join Slack](https://
-flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower)
-are welcome.\n\n\n_[https://contrib.rocks/image?repo=adap/flower]\n\n\n##
-Citation\n\nIf you publish work that uses Flower, please cite Flower as
-follows: \n\n```bibtex\n@article{beutel2020flower,\n title={Flower: A Friendly
-Federated Learning Research Framework},\n author={Beutel, Daniel J and Topal,
-Taner and Mathur, Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao,
-Yan and Sani, Lorenzo and Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o,
-Pedro PB de and Lane, Nicholas D}, \n journal={arXiv preprint arXiv:
-2007.14390},\n year={2020}\n}\n```\n\nPlease also consider adding your
-publication to the list of Flower-based publications in the docs, just open a
-Pull Request.\n\n## Contributing to Flower\n\nWe welcome contributions. Please
-see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!\n', 'author': 'The
-Flower Authors', 'author_email': 'hello@flower.dev', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://flower.dev', 'package_dir':
-package_dir, 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'extras_require': extras_require,
-'entry_points': entry_points, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+Flower-1-Intro-to-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https://
+github.com/adap/flower/blob/main/doc/source/tutorial/Flower-1-Intro-to-FL-
+PyTorch.ipynb)) 2. **Using Strategies in Federated Learning** [![Open in Colab]
+(https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
+Flower-2-Strategies-in-FL-PyTorch.ipynb) (or open the [Jupyter Notebook](https:
+//github.com/adap/flower/blob/main/doc/source/tutorial/Flower-2-Strategies-in-
+FL-PyTorch.ipynb)) 3. **Building Strategies for Federated Learning** [![Open in
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
+colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial/
+Flower-3-Building-a-Strategy-PyTorch.ipynb) (or open the [Jupyter Notebook]
+(https://github.com/adap/flower/blob/main/doc/source/tutorial/Flower-3-
+Building-a-Strategy-PyTorch.ipynb)) 4. **Custom Clients for Federated
+Learning** [![Open in Colab](https://colab.research.google.com/assets/colab-
+badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/doc/
+source/tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb) (or open the
+[Jupyter Notebook](https://github.com/adap/flower/blob/main/doc/source/
+tutorial/Flower-4-Client-and-NumPyClient-PyTorch.ipynb)) Stay tuned, more
+tutorials are coming soon. Topics include **Privacy and Security in Federated
+Learning**, and **Scaling Federated Learning**. ## Documentation [Flower Docs]
+(https://flower.dev/docs): * [Installation](https://flower.dev/docs/
+installation.html) * [Quickstart (TensorFlow)](https://flower.dev/docs/
+quickstart-tensorflow.html) * [Quickstart (PyTorch)](https://flower.dev/docs/
+quickstart-pytorch.html) * [Quickstart (Hugging Face [code example])](https://
+flower.dev/docs/quickstart-huggingface.html) * [Quickstart (PyTorch Lightning
+[code example])](https://flower.dev/docs/quickstart-pytorch-lightning.html) *
+[Quickstart (MXNet)](https://flower.dev/docs/example-mxnet-walk-through.html) *
+[Quickstart (Pandas)](https://flower.dev/docs/quickstart-pandas.html) *
+[Quickstart (fastai)](https://flower.dev/docs/quickstart-fastai.html) *
+[Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
+quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
+tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android [code
+example])](https://github.com/adap/flower/tree/main/examples/android) *
+[Quickstart (iOS)](https://flower.dev/docs/quickstart-ios.html) ## Flower
+Baselines Flower Baselines is a collection of community-contributed experiments
+that reproduce the experiments performed in popular federated learning
+publications. Researchers can build on Flower Baselines to quickly evaluate new
+ideas: * [FedAvg](https://arxiv.org/abs/1602.05629): * [MNIST](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
+fedavg_mnist) * [FedProx](https://arxiv.org/abs/1812.06127): * [MNIST](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/
+fedprox_mnist) * [FedBN: Federated Learning on non-IID Features via Local Batch
+Normalization](https://arxiv.org/abs/2102.07623): * [Convergence Rate](https://
+github.com/adap/flower/tree/main/baselines/flwr_baselines/publications/fedbn/
+convergence_rate) * [Adaptive Federated Optimization](https://arxiv.org/abs/
+2003.00295): * [CIFAR-10/100](https://github.com/adap/flower/tree/main/
+baselines/flwr_baselines/publications/adaptive_federated_optimization) Check
+the Flower documentation to learn more: [Using Baselines](https://flower.dev/
+docs/using-baselines.html) The Flower community loves contributions! Make your
+work more visible and enable others to build on it by contributing it as a
+baseline: [Contributing Baselines](https://flower.dev/docs/contributing-
+baselines.html) ## Flower Usage Examples Several code examples show different
+usage scenarios of Flower (in combination with popular machine learning
+frameworks such as PyTorch or TensorFlow). Quickstart examples: * [Quickstart
+(TensorFlow)](https://github.com/adap/flower/tree/main/examples/
+quickstart_tensorflow) * [Quickstart (PyTorch)](https://github.com/adap/flower/
+tree/main/examples/quickstart_pytorch) * [Quickstart (Hugging Face)](https://
+github.com/adap/flower/tree/main/examples/quickstart_huggingface) * [Quickstart
+(PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/
+quickstart_pytorch_lightning) * [Quickstart (fastai)](https://github.com/adap/
+flower/tree/main/examples/quickstart_fastai) * [Quickstart (Pandas)](https://
+github.com/adap/flower/tree/main/examples/quickstart_pandas) * [Quickstart
+(MXNet)](https://github.com/adap/flower/tree/main/examples/quickstart_mxnet) *
+[Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/
+quickstart_jax) * [Quickstart (scikit-learn)](https://github.com/adap/flower/
+tree/main/examples/sklearn-logreg-mnist) * [Quickstart (TFLite on Android)]
+(https://github.com/adap/flower/tree/main/examples/android) Other [examples]
+(https://github.com/adap/flower/tree/main/examples): * [Raspberry Pi & Nvidia
+Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/
+embedded_devices) * [Android & TFLite](https://github.com/adap/flower/tree/
+main/examples/android) * [PyTorch: From Centralized to Federated](https://
+github.com/adap/flower/tree/main/examples/
+pytorch_from_centralized_to_federated) * [MXNet: From Centralized to Federated]
+(https://github.com/adap/flower/tree/main/examples/
+mxnet_from_centralized_to_federated) * [Advanced Flower with TensorFlow/Keras]
+(https://github.com/adap/flower/tree/main/examples/advanced_tensorflow) *
+[Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/
+examples/advanced_pytorch) * Single-Machine Simulation of Federated Learning
+Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/
+simulation_pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/
+examples/simulation_tensorflow)) ## Community Flower is built by a wonderful
+community of researchers and engineers. [Join Slack](https://flower.dev/join-
+slack) to meet them, [contributions](#contributing-to-flower) are welcome.
+[https://contrib.rocks/image?repo=adap/flower] ## Citation If you publish work
+that uses Flower, please cite Flower as follows: ```bibtex @article
+{beutel2020flower, title={Flower: A Friendly Federated Learning Research
+Framework}, author={Beutel, Daniel J and Topal, Taner and Mathur, Akhil and
+Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and
+Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o, Pedro PB de and Lane,
+Nicholas D}, journal={arXiv preprint arXiv:2007.14390}, year={2020} } ```
+Please also consider adding your publication to the list of Flower-based
+publications in the docs, just open a Pull Request. ## Contributing to Flower
+We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get
+started!
```

