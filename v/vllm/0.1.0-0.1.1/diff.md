# Comparing `tmp/vllm-0.1.0.tar.gz` & `tmp/vllm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vllm-0.1.0.tar", last modified: Tue Jun 20 06:21:30 2023, max compression
+gzip compressed data, was "vllm-0.1.1.tar", last modified: Thu Jun 22 07:39:10 2023, max compression
```

## Comparing `vllm-0.1.0.tar` & `vllm-0.1.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.432776 vllm-0.1.0/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    11357 2023-05-23 02:52:42.000000 vllm-0.1.0/LICENSE
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)       67 2023-06-06 03:03:42.000000 vllm-0.1.0/MANIFEST.in
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4975 2023-06-20 06:21:30.432776 vllm-0.1.0/PKG-INFO
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4257 2023-06-20 06:13:44.000000 vllm-0.1.0/README.md
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.412774 vllm-0.1.0/csrc/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      234 2023-04-26 10:55:08.000000 vllm-0.1.0/csrc/activation.cpp
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1359 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/activation_kernels.cu
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.416774 vllm-0.1.0/csrc/attention/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      135 2023-06-03 23:33:23.000000 vllm-0.1.0/csrc/attention/attention_dtypes.h
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1721 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/attention_generic.cuh
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    19900 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/attention_kernels.cu
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1850 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/attention_utils.cuh
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    10962 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/dtype_bfloat16.cuh
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    10793 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/dtype_float16.cuh
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     5559 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/attention/dtype_float32.cuh
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      512 2023-04-26 10:55:08.000000 vllm-0.1.0/csrc/attention.cpp
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1151 2023-04-26 18:32:38.000000 vllm-0.1.0/csrc/cache.cpp
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    14699 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/cache_kernels.cu
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      292 2023-04-26 10:55:08.000000 vllm-0.1.0/csrc/layernorm.cpp
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1904 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/layernorm_kernels.cu
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      357 2023-05-23 02:52:42.000000 vllm-0.1.0/csrc/pos_encoding.cpp
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2901 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/pos_encoding_kernels.cu
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1592 2023-06-17 10:11:46.000000 vllm-0.1.0/csrc/reduction_utils.cuh
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      153 2023-06-06 03:03:42.000000 vllm-0.1.0/pyproject.toml
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      228 2023-05-28 17:19:12.000000 vllm-0.1.0/requirements.txt
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)       38 2023-06-20 06:21:30.432776 vllm-0.1.0/setup.cfg
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     6082 2023-06-20 06:13:44.000000 vllm-0.1.0/setup.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.420775 vllm-0.1.0/vllm/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      580 2023-06-20 06:07:35.000000 vllm-0.1.0/vllm/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1831 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/block.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     8486 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/config.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.420775 vllm-0.1.0/vllm/core/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/core/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    10341 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/core/block_manager.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      896 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/core/policy.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    17867 2023-06-18 19:39:38.000000 vllm-0.1.0/vllm/core/scheduler.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.424775 vllm-0.1.0/vllm/engine/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/engine/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     6546 2023-06-18 19:39:38.000000 vllm-0.1.0/vllm/engine/arg_utils.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     8929 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/engine/async_llm_engine.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    13352 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/engine/llm_engine.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4233 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/engine/ray_utils.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     3788 2023-06-20 06:20:08.000000 vllm-0.1.0/vllm/engine/tokenizer_utils.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.424775 vllm-0.1.0/vllm/entrypoints/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2970 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/api_server.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     5728 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/llm.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.424775 vllm-0.1.0/vllm/entrypoints/openai/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/openai/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    12233 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/openai/api_server.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     3895 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/entrypoints/openai/protocol.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1577 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/logger.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.424775 vllm-0.1.0/vllm/model_executor/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      247 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2194 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/input_metadata.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.428775 vllm-0.1.0/vllm/model_executor/layers/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1190 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/activation.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     9322 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/attention.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      773 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/layernorm.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    16062 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/layers/sampler.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1836 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/model_loader.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.428775 vllm-0.1.0/vllm/model_executor/models/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      358 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    12118 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/gpt2.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    10979 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/gpt_neox.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    11763 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/llama.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    12958 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/models/opt.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.428775 vllm-0.1.0/vllm/model_executor/parallel_utils/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      244 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    22861 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/parallel_state.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.428775 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     1418 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    18207 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/layers.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     8586 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     6056 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/random.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2460 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/utils.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      546 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/utils.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4304 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/model_executor/weight_utils.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     3959 2023-06-20 06:13:44.000000 vllm-0.1.0/vllm/outputs.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     6521 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/sampling_params.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     7767 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/sequence.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      730 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/utils.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.432776 vllm-0.1.0/vllm/worker/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/worker/__init__.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     5503 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/worker/cache_engine.py
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)    12283 2023-06-17 10:11:46.000000 vllm-0.1.0/vllm/worker/worker.py
-drwxr-xr-x   0 gcpuser   (1004) gcpuser   (1005)        0 2023-06-20 06:21:30.420775 vllm-0.1.0/vllm.egg-info/
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     4975 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/PKG-INFO
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)     2290 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/SOURCES.txt
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        1 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/dependency_links.txt
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)      113 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/requires.txt
--rw-r--r--   0 gcpuser   (1004) gcpuser   (1005)        5 2023-06-20 06:21:30.000000 vllm-0.1.0/vllm.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.312857 vllm-0.1.1/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11357 2023-05-19 19:30:16.000000 vllm-0.1.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       67 2023-06-06 03:07:23.000000 vllm-0.1.1/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4975 2023-06-22 07:39:10.310857 vllm-0.1.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4257 2023-06-21 15:58:37.000000 vllm-0.1.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.779801 vllm-0.1.1/csrc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      234 2023-04-02 07:37:46.000000 vllm-0.1.1/csrc/activation.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1359 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/activation_kernels.cu
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.839808 vllm-0.1.1/csrc/attention/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      135 2023-06-03 11:19:52.000000 vllm-0.1.1/csrc/attention/attention_dtypes.h
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1721 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/attention_generic.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19900 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/attention_kernels.cu
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1850 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/attention_utils.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10962 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/dtype_bfloat16.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10793 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/dtype_float16.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5559 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/attention/dtype_float32.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      512 2023-05-19 19:30:17.000000 vllm-0.1.1/csrc/attention.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1151 2023-05-19 19:30:17.000000 vllm-0.1.1/csrc/cache.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14699 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/cache_kernels.cu
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      292 2023-03-31 16:51:49.000000 vllm-0.1.1/csrc/layernorm.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1904 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/layernorm_kernels.cu
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      357 2023-05-19 19:30:17.000000 vllm-0.1.1/csrc/pos_encoding.cpp
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2901 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/pos_encoding_kernels.cu
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1592 2023-06-18 04:39:39.000000 vllm-0.1.1/csrc/reduction_utils.cuh
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      153 2023-06-06 03:07:24.000000 vllm-0.1.1/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      228 2023-05-24 04:45:48.000000 vllm-0.1.1/requirements.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-06-22 07:39:10.314858 vllm-0.1.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6082 2023-06-21 15:58:37.000000 vllm-0.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.903815 vllm-0.1.1/vllm/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      580 2023-06-22 07:38:42.000000 vllm-0.1.1/vllm/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1831 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/block.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8486 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/config.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.976822 vllm-0.1.1/vllm/core/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/core/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10341 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/core/block_manager.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      896 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/core/policy.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17867 2023-06-21 15:58:37.000000 vllm-0.1.1/vllm/core/scheduler.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.033828 vllm-0.1.1/vllm/engine/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/engine/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6546 2023-06-18 13:35:33.000000 vllm-0.1.1/vllm/engine/arg_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8927 2023-06-22 07:23:09.000000 vllm-0.1.1/vllm/engine/async_llm_engine.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    13617 2023-06-22 07:38:42.000000 vllm-0.1.1/vllm/engine/llm_engine.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4233 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/engine/ray_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3788 2023-06-21 15:58:37.000000 vllm-0.1.1/vllm/engine/tokenizer_utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.060831 vllm-0.1.1/vllm/entrypoints/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2970 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/api_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5726 2023-06-22 07:23:09.000000 vllm-0.1.1/vllm/entrypoints/llm.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.086834 vllm-0.1.1/vllm/entrypoints/openai/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/openai/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12233 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/openai/api_server.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3895 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/entrypoints/openai/protocol.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1577 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/logger.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.131839 vllm-0.1.1/vllm/model_executor/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2194 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/input_metadata.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.173843 vllm-0.1.1/vllm/model_executor/layers/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1190 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/activation.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9322 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/attention.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      773 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/layernorm.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16062 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/layers/sampler.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1836 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/model_loader.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.216848 vllm-0.1.1/vllm/model_executor/models/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      358 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12118 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/gpt2.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10979 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/gpt_neox.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11763 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/llama.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12958 2023-06-18 04:39:39.000000 vllm-0.1.1/vllm/model_executor/models/opt.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.234849 vllm-0.1.1/vllm/model_executor/parallel_utils/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      244 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    22861 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/parallel_state.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.278854 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1418 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18207 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/layers.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8586 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6056 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/random.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2460 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      546 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4304 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/model_executor/weight_utils.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4093 2023-06-22 07:38:42.000000 vllm-0.1.1/vllm/outputs.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6521 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/sampling_params.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7767 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/sequence.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      730 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/utils.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:10.300856 vllm-0.1.1/vllm/worker/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-18 04:39:40.000000 vllm-0.1.1/vllm/worker/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5503 2023-06-18 08:57:00.000000 vllm-0.1.1/vllm/worker/cache_engine.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12283 2023-06-18 08:56:51.000000 vllm-0.1.1/vllm/worker/worker.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-22 07:39:09.943819 vllm-0.1.1/vllm.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4975 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2290 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      113 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        5 2023-06-22 07:39:09.000000 vllm-0.1.1/vllm.egg-info/top_level.txt
```

### Comparing `vllm-0.1.0/LICENSE` & `vllm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/PKG-INFO` & `vllm-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vllm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A high-throughput and memory-efficient inference and serving engine for LLMs
 Home-page: https://github.com/vllm-project/vllm
 Author: vLLM Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/vllm-project/vllm
 Project-URL: Documentation, https://vllm.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vllm Version: 0.1.0 Summary: A high-throughput and
+Metadata-Version: 2.1 Name: vllm Version: 0.1.1 Summary: A high-throughput and
 memory-efficient inference and serving engine for LLMs Home-page: https://
 github.com/vllm-project/vllm Author: vLLM Team License: Apache 2.0 Project-URL:
 Homepage, https://github.com/vllm-project/vllm Project-URL: Documentation,
 https://vllm.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Topic :: Scientific/Engineering ::
```

### Comparing `vllm-0.1.0/README.md` & `vllm-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/activation_kernels.cu` & `vllm-0.1.1/csrc/activation_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/attention/attention_generic.cuh` & `vllm-0.1.1/csrc/attention/attention_generic.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/attention/attention_kernels.cu` & `vllm-0.1.1/csrc/attention/attention_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/attention/attention_utils.cuh` & `vllm-0.1.1/csrc/attention/attention_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/attention/dtype_bfloat16.cuh` & `vllm-0.1.1/csrc/attention/dtype_bfloat16.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/attention/dtype_float16.cuh` & `vllm-0.1.1/csrc/attention/dtype_float16.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/attention/dtype_float32.cuh` & `vllm-0.1.1/csrc/attention/dtype_float32.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/attention.cpp` & `vllm-0.1.1/csrc/attention.cpp`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/cache.cpp` & `vllm-0.1.1/csrc/cache.cpp`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/cache_kernels.cu` & `vllm-0.1.1/csrc/cache_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/layernorm_kernels.cu` & `vllm-0.1.1/csrc/layernorm_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/pos_encoding_kernels.cu` & `vllm-0.1.1/csrc/pos_encoding_kernels.cu`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/csrc/reduction_utils.cuh` & `vllm-0.1.1/csrc/reduction_utils.cuh`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/setup.py` & `vllm-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/__init__.py` & `vllm-0.1.1/vllm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from vllm.engine.async_llm_engine import AsyncLLMEngine
 from vllm.engine.llm_engine import LLMEngine
 from vllm.engine.ray_utils import initialize_cluster
 from vllm.entrypoints.llm import LLM
 from vllm.outputs import CompletionOutput, RequestOutput
 from vllm.sampling_params import SamplingParams
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 
 __all__ = [
     "LLM",
     "SamplingParams",
     "RequestOutput",
     "CompletionOutput",
     "LLMEngine",
```

### Comparing `vllm-0.1.0/vllm/block.py` & `vllm-0.1.1/vllm/block.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/config.py` & `vllm-0.1.1/vllm/config.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/core/block_manager.py` & `vllm-0.1.1/vllm/core/block_manager.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/core/policy.py` & `vllm-0.1.1/vllm/core/policy.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/core/scheduler.py` & `vllm-0.1.1/vllm/core/scheduler.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/engine/arg_utils.py` & `vllm-0.1.1/vllm/engine/arg_utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/engine/async_llm_engine.py` & `vllm-0.1.1/vllm/engine/async_llm_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
             request_event.clear()
 
             # Decode and return new outputs.
             request_output = self.request_outputs[request_id]
             yield request_output
 
             # Once finished, release the resources of the sequence group.
-            if request_output.finished():
+            if request_output.finished:
                 if self.log_requests:
                     logger.info(f"Finished request {request_id}.")
 
                 del self.request_outputs[request_id]
                 del self.request_events[request_id]
                 # Kick the engine if the engine is not running. This is to
                 # prevent that there are still requests in engine's waiting
```

### Comparing `vllm-0.1.0/vllm/engine/llm_engine.py` & `vllm-0.1.1/vllm/engine/llm_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         assert len(stage_devices) == 1, "Only support one stage for now."
         for rank, node_resource, _ in stage_devices[0]:
             worker_cls = Worker
             if self.parallel_config.worker_use_ray:
                 worker_cls = ray.remote(
                     num_cpus=0,
                     num_gpus=1,
-                    resources={node_resource: 1e-5},
+                    resources={node_resource: 1e-3},
                 )(worker_cls).remote
 
             worker = worker_cls(
                 model_config,
                 parallel_config,
                 scheduler_config,
                 rank,
@@ -123,14 +123,20 @@
         # number of blocks across all workers to make sure all the memory
         # operators can be applied to all workers.
         num_gpu_blocks = min(b[0] for b in num_blocks)
         num_cpu_blocks = min(b[1] for b in num_blocks)
         # FIXME(woosuk): Change to debug log.
         logger.info(f'# GPU blocks: {num_gpu_blocks}, '
                     f'# CPU blocks: {num_cpu_blocks}')
+
+        if num_gpu_blocks <= 0 or num_cpu_blocks <= 0:
+            raise ValueError("No available memory for the cache blocks. "
+                             "Try increasing `gpu_memory_utilization` when "
+                             "initializing the engine.")
+
         self.cache_config.num_gpu_blocks = num_gpu_blocks
         self.cache_config.num_cpu_blocks = num_cpu_blocks
 
         # Initialize the cache.
         self._run_workers("init_cache_engine", cache_config=self.cache_config)
 
     @classmethod
```

### Comparing `vllm-0.1.0/vllm/engine/ray_utils.py` & `vllm-0.1.1/vllm/engine/ray_utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/engine/tokenizer_utils.py` & `vllm-0.1.1/vllm/engine/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/entrypoints/api_server.py` & `vllm-0.1.1/vllm/entrypoints/api_server.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/entrypoints/llm.py` & `vllm-0.1.1/vllm/entrypoints/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,14 @@
             num_requests = self.llm_engine.get_num_unfinished_requests()
             pbar = tqdm(total=num_requests, desc="Processed prompts")
         # Run the engine.
         outputs: List[RequestOutput] = []
         while self.llm_engine.has_unfinished_requests():
             step_outputs = self.llm_engine.step()
             for output in step_outputs:
-                if output.finished():
+                if output.finished:
                     outputs.append(output)
                     if use_tqdm:
                         pbar.update(1)
         if use_tqdm:
             pbar.close()
         return outputs
```

### Comparing `vllm-0.1.0/vllm/entrypoints/openai/api_server.py` & `vllm-0.1.1/vllm/entrypoints/openai/api_server.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/entrypoints/openai/protocol.py` & `vllm-0.1.1/vllm/entrypoints/openai/protocol.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/logger.py` & `vllm-0.1.1/vllm/logger.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/input_metadata.py` & `vllm-0.1.1/vllm/model_executor/input_metadata.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/layers/activation.py` & `vllm-0.1.1/vllm/model_executor/layers/activation.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/layers/attention.py` & `vllm-0.1.1/vllm/model_executor/layers/attention.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/layers/layernorm.py` & `vllm-0.1.1/vllm/model_executor/layers/layernorm.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/layers/sampler.py` & `vllm-0.1.1/vllm/model_executor/layers/sampler.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/model_loader.py` & `vllm-0.1.1/vllm/model_executor/model_loader.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/models/gpt2.py` & `vllm-0.1.1/vllm/model_executor/models/gpt2.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/models/gpt_neox.py` & `vllm-0.1.1/vllm/model_executor/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/models/llama.py` & `vllm-0.1.1/vllm/model_executor/models/llama.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/models/opt.py` & `vllm-0.1.1/vllm/model_executor/models/opt.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/parallel_utils/parallel_state.py` & `vllm-0.1.1/vllm/model_executor/parallel_utils/parallel_state.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py` & `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/__init__.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/layers.py` & `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/layers.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py` & `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/mappings.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/random.py` & `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/random.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/parallel_utils/tensor_parallel/utils.py` & `vllm-0.1.1/vllm/model_executor/parallel_utils/tensor_parallel/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/utils.py` & `vllm-0.1.1/vllm/model_executor/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/model_executor/weight_utils.py` & `vllm-0.1.1/vllm/model_executor/weight_utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/outputs.py` & `vllm-0.1.1/vllm/outputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,26 +49,29 @@
     """The output data of a request to the LLM.
 
     Args:
         request_id: The unique ID of the request.
         prompt: The prompt string of the request.
         prompt_token_ids: The token IDs of the prompt.
         outputs: The output sequences of the request.
+        finished: Whether the whole request is finished.
     """
     def __init__(
         self,
         request_id: str,
         prompt: str,
         prompt_token_ids: List[int],
         outputs: List[CompletionOutput],
+        finished: bool,
     ) -> None:
         self.request_id = request_id
         self.prompt = prompt
         self.prompt_token_ids = prompt_token_ids
         self.outputs = outputs
+        self.finished = finished
 
     @classmethod
     def from_seq_group(cls, seq_group: SequenceGroup) -> "RequestOutput":
         # Get the top-n sequences.
         n = seq_group.sampling_params.n
         seqs = seq_group.get_seqs()
         assert n <= len(seqs)
@@ -91,17 +94,17 @@
                                       seq.get_cumulative_logprob(), logprobs,
                                       finshed_reason)
             outputs.append(output)
 
         # Every sequence in the sequence group should have the same prompt.
         prompt = top_n_seqs[0].prompt
         prompt_token_ids = top_n_seqs[0].data.prompt_token_ids
-        return cls(seq_group.request_id, prompt, prompt_token_ids, outputs)
+        finished = seq_group.is_finished()
+        return cls(seq_group.request_id, prompt, prompt_token_ids, outputs,
+                   finished)
 
     def __repr__(self) -> str:
         return (f"RequestOutput(request_id={self.request_id}, "
                 f"prompt={self.prompt!r}, "
                 f"prompt_token_ids={self.prompt_token_ids}, "
-                f"outputs={self.outputs})")
-
-    def finished(self) -> bool:
-        return all(output.finished() for output in self.outputs)
+                f"outputs={self.outputs}, "
+                f"finished={self.finished})")
```

### Comparing `vllm-0.1.0/vllm/sampling_params.py` & `vllm-0.1.1/vllm/sampling_params.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/sequence.py` & `vllm-0.1.1/vllm/sequence.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/utils.py` & `vllm-0.1.1/vllm/utils.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/worker/cache_engine.py` & `vllm-0.1.1/vllm/worker/cache_engine.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm/worker/worker.py` & `vllm-0.1.1/vllm/worker/worker.py`

 * *Files identical despite different names*

### Comparing `vllm-0.1.0/vllm.egg-info/PKG-INFO` & `vllm-0.1.1/vllm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vllm
-Version: 0.1.0
+Version: 0.1.1
 Summary: A high-throughput and memory-efficient inference and serving engine for LLMs
 Home-page: https://github.com/vllm-project/vllm
 Author: vLLM Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/vllm-project/vllm
 Project-URL: Documentation, https://vllm.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vllm Version: 0.1.0 Summary: A high-throughput and
+Metadata-Version: 2.1 Name: vllm Version: 0.1.1 Summary: A high-throughput and
 memory-efficient inference and serving engine for LLMs Home-page: https://
 github.com/vllm-project/vllm Author: vLLM Team License: Apache 2.0 Project-URL:
 Homepage, https://github.com/vllm-project/vllm Project-URL: Documentation,
 https://vllm.readthedocs.io/en/latest/ Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Topic :: Scientific/Engineering ::
```

### Comparing `vllm-0.1.0/vllm.egg-info/SOURCES.txt` & `vllm-0.1.1/vllm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

