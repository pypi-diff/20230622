# Comparing `tmp/lightning-fabric-2.0.3.tar.gz` & `tmp/lightning-fabric-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-fabric-2.0.3.tar", last modified: Wed Jun  7 17:11:24 2023, max compression
+gzip compressed data, was "lightning-fabric-2.0.4.tar", last modified: Thu Jun 22 18:25:15 2023, max compression
```

## Comparing `lightning-fabric-2.0.3.tar` & `lightning-fabric-2.0.4.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.029971 lightning-fabric-2.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.017971 lightning-fabric-2.0.3/.actions/
--rw-r--r--   0 runner    (1001) docker     (123)    17470 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-07 17:11:24.029971 lightning-fabric-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.013971 lightning-fabric-2.0.3/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.017971 lightning-fabric-2.0.3/requirements/fabric/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/examples.txt
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/strategies.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/requirements/fabric/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 17:11:24.029971 lightning-fabric-2.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.017971 lightning-fabric-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/
--rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/mps.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/accelerators/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    27286 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    40477 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/fabric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/loggers/csv_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/torch_collective.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/cluster_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/kubeflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/lightning.py
--rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/torchelastic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/torch_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/double.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/fsdp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/tpu_bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/dp.py
--rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/fsdp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.025971 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/subprocess_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/xla.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/single_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/single_tpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/strategies/xla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.029971 lightning-fabric-2.0.3/src/lightning_fabric/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/apply_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/device_dtype_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/device_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    13054 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/rank_zero.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/lightning_fabric/version.info
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 17:11:24.021971 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 17:11:23.000000 lightning-fabric-2.0.3/src/lightning_fabric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 17:11:12.000000 lightning-fabric-2.0.3/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.352394 lightning-fabric-2.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-22 18:25:15.352394 lightning-fabric-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22069 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10146 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.336394 lightning-fabric-2.0.4/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/requirements/fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/examples.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/strategies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/requirements/fabric/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 18:25:15.352394 lightning-fabric-2.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/src/lightning_fabric/
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-06-22 18:25:14.000000 lightning-fabric-2.0.4/src/lightning_fabric/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10135 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-22 18:25:14.000000 lightning-fabric-2.0.4/src/lightning_fabric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/mps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/accelerators/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-06-22 18:25:14.000000 lightning-fabric-2.0.4/src/lightning_fabric/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27286 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40477 2023-06-22 18:25:14.000000 lightning-fabric-2.0.4/src/lightning_fabric/fabric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/loggers/csv_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12810 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/torch_collective.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/cluster_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/kubeflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/lightning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7571 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/torchelastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.344394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/torch_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.348394 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/double.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/tpu_bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.348394 lightning-fabric-2.0.4/src/lightning_fabric/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36789 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/dp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/fsdp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.348394 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/subprocess_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/xla.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/single_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/single_tpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14964 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/strategies/xla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.352394 lightning-fabric-2.0.4/src/lightning_fabric/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/apply_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/device_dtype_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7302 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/device_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12928 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/rank_zero.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/lightning_fabric/version.info
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 18:25:15.340394 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 18:25:15.000000 lightning-fabric-2.0.4/src/lightning_fabric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 18:25:04.000000 lightning-fabric-2.0.4/src/version.info
```

### Comparing `lightning-fabric-2.0.3/.actions/assistant.py` & `lightning-fabric-2.0.4/.actions/assistant.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import glob
+import logging
 import os
 import pathlib
 import re
 import shutil
 import tarfile
 import tempfile
 import urllib.request
@@ -138,15 +139,15 @@
 
 
 def load_requirements(path_dir: str, file_name: str = "base.txt", unfreeze: str = "all") -> List[str]:
     """Loading requirements from a file.
 
     >>> path_req = os.path.join(_PROJECT_ROOT, "requirements")
     >>> load_requirements(path_req, "docs.txt", unfreeze="major")  # doctest: +ELLIPSIS +NORMALIZE_WHITESPACE
-    ['sphinx<6.0,>=4.0', ...]
+    ['sphinx<...]
     """
     assert unfreeze in {"none", "major", "all"}
     path = Path(path_dir) / file_name
     assert path.exists(), (path_dir, file_name, path)
     text = path.read_text()
     return [req.adjust(unfreeze) for req in _parse_requirements(text)]
 
@@ -417,12 +418,48 @@
         """Copy package content with import adjustments."""
         source_imports = source_import.strip().split(",")
         target_imports = target_import.strip().split(",")
         copy_replace_imports(
             source_dir, source_imports, target_imports, target_dir=target_dir, lightning_by=lightning_by
         )
 
+    @staticmethod
+    def pull_docs_files(
+        gh_user_repo: str,
+        target_dir: str = "docs/source-pytorch/XXX",
+        checkout: str = "tags/1.0.0",
+        source_dir: str = "docs/source",
+    ) -> None:
+        """Pull docs pages from external source and append to local docs."""
+        import zipfile
+
+        zip_url = f"https://github.com/{gh_user_repo}/archive/refs/{checkout}.zip"
+
+        with tempfile.TemporaryDirectory() as tmp:
+            zip_file = os.path.join(tmp, "repo.zip")
+            urllib.request.urlretrieve(zip_url, zip_file)
+
+            with zipfile.ZipFile(zip_file, "r") as zip_ref:
+                zip_ref.extractall(tmp)
+
+            zip_dirs = [d for d in glob.glob(os.path.join(tmp, "*")) if os.path.isdir(d)]
+            # check that the extracted archive has only repo folder
+            assert len(zip_dirs) == 1
+            repo_dir = zip_dirs[0]
+
+            ls_pages = glob.glob(os.path.join(repo_dir, source_dir, "*.rst"))
+            ls_pages += glob.glob(os.path.join(repo_dir, source_dir, "**", "*.rst"))
+            for rst in ls_pages:
+                rel_rst = rst.replace(os.path.join(repo_dir, source_dir) + os.path.sep, "")
+                rel_dir = os.path.dirname(rel_rst)
+                os.makedirs(os.path.join(_PROJECT_ROOT, target_dir, rel_dir), exist_ok=True)
+                new_rst = os.path.join(_PROJECT_ROOT, target_dir, rel_rst)
+                if os.path.isfile(new_rst):
+                    logging.warning(f"Page {new_rst} already exists in the local tree so it will be skipped.")
+                    continue
+                shutil.copy(rst, new_rst)
+
 
 if __name__ == "__main__":
     import jsonargparse
 
     jsonargparse.CLI(AssistantCLI, as_positional=False)
```

### Comparing `lightning-fabric-2.0.3/LICENSE` & `lightning-fabric-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/PKG-INFO` & `lightning-fabric-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.3
+Version: 2.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,16 +21,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: strategies
 Provides-Extra: test
+Provides-Extra: strategies
 Provides-Extra: examples
 Provides-Extra: deepspeed
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `lightning-fabric-2.0.3/README.md` & `lightning-fabric-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/pyproject.toml` & `lightning-fabric-2.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/setup.py` & `lightning-fabric-2.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/CHANGELOG.md` & `lightning-fabric-2.0.4/src/lightning_fabric/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.4] - 2023-06-22
+
+### Fixed
+
+- Fixed validation of parameters of `plugins.precision.MixedPrecision` ([#17687](https://github.com/Lightning-AI/lightning/pull/17687))
+- Fixed an issue with hpu imports leading to performance degradation  ([#17788](https://github.com/Lightning-AI/lightning/pull/17788))
+
+
 ## [2.0.3] - 2023-06-07
 
 - Added support for `Callback` registration through entry points ([#17756](https://github.com/Lightning-AI/lightning/pull/17756))
 - Add Fabric internal hooks ([#17759](https://github.com/Lightning-AI/lightning/pull/17759))
 
 ### Changed
```

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/README.md` & `lightning-fabric-2.0.4/src/lightning_fabric/README.md`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/__setup__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/accelerator.py` & `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/accelerator.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/cpu.py` & `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/cpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/cuda.py` & `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/cuda.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/mps.py` & `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/mps.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/registry.py` & `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/accelerators/tpu.py` & `lightning-fabric-2.0.4/src/lightning_fabric/accelerators/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/cli.py` & `lightning-fabric-2.0.4/src/lightning_fabric/cli.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/connector.py` & `lightning-fabric-2.0.4/src/lightning_fabric/connector.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/fabric.py` & `lightning-fabric-2.0.4/src/lightning_fabric/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/loggers/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/loggers/csv_logs.py` & `lightning-fabric-2.0.4/src/lightning_fabric/loggers/csv_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/loggers/logger.py` & `lightning-fabric-2.0.4/src/lightning_fabric/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/loggers/tensorboard.py` & `lightning-fabric-2.0.4/src/lightning_fabric/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/collective.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/single_device.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/collectives/torch_collective.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/collectives/torch_collective.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/cluster_environment.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/cluster_environment.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/kubeflow.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/kubeflow.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/lightning.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/lightning.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/lsf.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/lsf.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/mpi.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/mpi.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/slurm.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/slurm.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/torchelastic.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/torchelastic.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/environments/xla.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/environments/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/checkpoint_io.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/torch_io.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/torch_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/io/xla.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/io/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/amp.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/amp.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,20 @@
 
     def __init__(
         self,
         precision: Literal["16-mixed", "bf16-mixed"],
         device: str,
         scaler: Optional[torch.cuda.amp.GradScaler] = None,
     ) -> None:
+        if precision not in ("16-mixed", "bf16-mixed"):
+            raise ValueError(
+                f"Passed `{type(self).__name__}(precision={precision!r})`."
+                " Precision must be '16-mixed' or 'bf16-mixed'."
+            )
+
         self.precision = cast(Literal["16-mixed", "bf16-mixed"], str(precision))
         if scaler is None and self.precision == "16-mixed":
             with _patch_cuda_is_available():
                 # if possible, we defer CUDA initialization to support strategies that will attempt forks
                 scaler = torch.cuda.amp.GradScaler()
         if scaler is not None and self.precision == "bf16-mixed":
             raise ValueError(f"`precision='bf16-mixed'` does not use a scaler, found {scaler}.")
```

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/deepspeed.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/double.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/double.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/fsdp.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/precision.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/precision.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/tpu.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/tpu_bf16.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/tpu_bf16.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/plugins/precision/utils.py` & `lightning-fabric-2.0.4/src/lightning_fabric/plugins/precision/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/ddp.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/ddp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/deepspeed.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/deepspeed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/dp.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/dp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/fsdp.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/fsdp.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/base.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/base.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/launcher.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/launcher.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/multiprocessing.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/subprocess_script.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/subprocess_script.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/launchers/xla.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/launchers/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/parallel.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/parallel.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/registry.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/single_device.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/single_device.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/single_tpu.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/single_tpu.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/strategy.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/strategies/xla.py` & `lightning-fabric-2.0.4/src/lightning_fabric/strategies/xla.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/__init__.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/apply_func.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/apply_func.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/cloud_io.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/cloud_io.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/data.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/data.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/device_dtype_mixin.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/device_dtype_mixin.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/device_parser.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/device_parser.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/distributed.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/distributed.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import sys
 from contextlib import nullcontext
 from typing import Any, Iterable, Iterator, List, Optional, Sized, Tuple, Union
 
 import torch
 import torch.nn.functional as F
-from lightning_utilities.core.imports import module_available
+from lightning_utilities.core.imports import package_available
 from torch import Tensor
 from torch.utils.data import Dataset, DistributedSampler, Sampler
 
 from lightning_fabric.plugins.environments.cluster_environment import ClusterEnvironment
 from lightning_fabric.utilities.imports import _TORCH_GREATER_EQUAL_1_12
 from lightning_fabric.utilities.rank_zero import rank_zero_info
 from lightning_fabric.utilities.types import ReduceOp
@@ -134,24 +134,25 @@
             divide_by_world_size = True
         else:
             op = getattr(ReduceOp, reduce_op.upper())
     else:
         op = reduce_op
 
     # WA for HPU. HPU doesn't support Long types, forcefully set it to float
-    if module_available("habana_frameworks.torch.utils.library_loader"):
-        from habana_frameworks.torch.utils.library_loader import is_habana_avaialble
-
-        if (
-            is_habana_avaialble()
-            and os.environ.get("HCCL_DISTRIBUTED_BACKEND") == "1"
-            and result.type() in ("torch.LongTensor", "torch.hpu.LongTensor")
-        ):
-            rank_zero_info("Long tensor unsupported on HPU, casting to float")
-            result = result.float()
+    if (
+        package_available("habana_frameworks")
+        and os.environ.get("HCCL_DISTRIBUTED_BACKEND") == "1"
+        and result.type()
+        in (
+            "torch.LongTensor",
+            "torch.hpu.LongTensor",
+        )
+    ):
+        rank_zero_info("Long tensor unsupported on HPU, casting to float")
+        result = result.float()
 
     # Sync all processes before reduction
     torch.distributed.barrier(group=group)
     torch.distributed.all_reduce(result, op=op, group=group, async_op=False)
 
     if divide_by_world_size:
         result = result / torch.distributed.get_world_size(group)
```

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/enums.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/enums.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/exceptions.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/imports.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/logger.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/optimizer.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/optimizer.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/rank_zero.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/rank_zero.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/registry.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/registry.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/seed.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/seed.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/types.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/utilities/warnings.py` & `lightning-fabric-2.0.4/src/lightning_fabric/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric/wrappers.py` & `lightning-fabric-2.0.4/src/lightning_fabric/wrappers.py`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric.egg-info/PKG-INFO` & `lightning-fabric-2.0.4/src/lightning_fabric.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-fabric
-Version: 2.0.3
+Version: 2.0.4
 Summary: UNKNOWN
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
@@ -21,16 +21,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: strategies
 Provides-Extra: test
+Provides-Extra: strategies
 Provides-Extra: examples
 Provides-Extra: deepspeed
 Provides-Extra: all
 Provides-Extra: dev
 License-File: LICENSE
 
 <div align="center">
```

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric.egg-info/SOURCES.txt` & `lightning-fabric-2.0.4/src/lightning_fabric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-fabric-2.0.3/src/lightning_fabric.egg-info/requires.txt` & `lightning-fabric-2.0.4/src/lightning_fabric.egg-info/requires.txt`

 * *Files identical despite different names*

