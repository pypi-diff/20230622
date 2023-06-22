# Comparing `tmp/ml-compiler-opt-0.0.1.dev202306210145.tar.gz` & `tmp/ml-compiler-opt-0.0.1.dev202306220007.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-compiler-opt-0.0.1.dev202306210145.tar", last modified: Wed Jun 21 01:45:21 2023, max compression
+gzip compressed data, was "ml-compiler-opt-0.0.1.dev202306220007.tar", last modified: Thu Jun 22 00:07:06 2023, max compression
```

## Comparing `ml-compiler-opt-0.0.1.dev202306210145.tar` & `ml-compiler-opt-0.0.1.dev202306220007.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.165248 ml-compiler-opt-0.0.1.dev202306210145/
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-21 01:45:21.165248 ml-compiler-opt-0.0.1.dev202306210145/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.149248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.153248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_chromium.py
--rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_llvm_test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_report_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_report_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmarking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/filter_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/gtest_executable_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/list_gtests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.153248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/buffered_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/buffered_scheduler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.153248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/local/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/local/local_worker_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/local/local_worker_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/worker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/worker_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.153248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47034 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/blackbox_optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/blackbox_optimizers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/gradient_ascent_optimization_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/package_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.157248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/agent_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/agent_config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/best_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/best_trajectory_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/compilation_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/compilation_runner_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/constant_value_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/constant_value_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/data_collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/data_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/data_reader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.161248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_collect.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_collect_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_eval_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_reverb_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_reverb_server_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_train_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/env_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/feature_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/feature_ops_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/gin_external_configurables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.161248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/inlining_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/local_data_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/local_data_collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/log_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/log_reader_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/policy_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/policy_saver_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/problem_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/random_net_distillation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/random_net_distillation_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.161248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/regalloc_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/regalloc_network_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/regalloc_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.161248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc_priority/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc_priority/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc_priority/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/train_bc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/train_locally.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/trainer_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.165248 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/combine_training_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/combine_training_corpus_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/combine_training_corpus_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/extract_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/extract_ir_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/extract_ir_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/feature_importance_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/feature_importance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/feature_importance_utils_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_default_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_default_trace_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_test_model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/merge_best_trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 01:45:21.165248 ml-compiler-opt-0.0.1.dev202306210145/ml_compiler_opt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-21 01:45:21.000000 ml-compiler-opt-0.0.1.dev202306210145/ml_compiler_opt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-21 01:45:21.000000 ml-compiler-opt-0.0.1.dev202306210145/ml_compiler_opt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 01:45:21.000000 ml-compiler-opt-0.0.1.dev202306210145/ml_compiler_opt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-21 01:45:21.000000 ml-compiler-opt-0.0.1.dev202306210145/ml_compiler_opt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-21 01:45:21.000000 ml-compiler-opt-0.0.1.dev202306210145/ml_compiler_opt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-21 01:45:02.000000 ml-compiler-opt-0.0.1.dev202306210145/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 01:45:21.165248 ml-compiler-opt-0.0.1.dev202306210145/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.029735 ml-compiler-opt-0.0.1.dev202306220007/
+-rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-22 00:07:06.029735 ml-compiler-opt-0.0.1.dev202306220007/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.005735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.009735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_chromium.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8151 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_llvm_test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_report_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_report_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmarking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/filter_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/gtest_executable_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/list_gtests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.009735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/buffered_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/buffered_scheduler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.009735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/local/local_worker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/local/local_worker_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/worker_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.013735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45450 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/blackbox_optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/blackbox_optimizers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6521 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/gradient_ascent_optimization_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/package_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.017735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/agent_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/agent_config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/best_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/best_trajectory_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17003 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/compilation_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/compilation_runner_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/constant_value_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/constant_value_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/data_collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/data_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7756 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/data_reader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.021735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18967 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_collect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_collect_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_eval_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_reverb_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_reverb_server_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_train_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11070 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/env_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/feature_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/feature_ops_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/gin_external_configurables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.021735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/inlining_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8518 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/local_data_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8494 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/local_data_collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/log_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/log_reader_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8885 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/policy_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/policy_saver_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/problem_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8567 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/random_net_distillation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/random_net_distillation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.025735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/regalloc_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/regalloc_network_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/regalloc_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.025735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc_priority/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc_priority/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc_priority/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/train_bc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7856 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/train_locally.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/trainer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.029735 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/combine_training_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/combine_training_corpus_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/combine_training_corpus_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/extract_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/extract_ir_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/extract_ir_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/feature_importance_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/feature_importance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/feature_importance_utils_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_default_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_default_trace_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_test_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/merge_best_trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 00:07:06.029735 ml-compiler-opt-0.0.1.dev202306220007/ml_compiler_opt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-06-22 00:07:05.000000 ml-compiler-opt-0.0.1.dev202306220007/ml_compiler_opt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-22 00:07:06.000000 ml-compiler-opt-0.0.1.dev202306220007/ml_compiler_opt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 00:07:05.000000 ml-compiler-opt-0.0.1.dev202306220007/ml_compiler_opt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 00:07:05.000000 ml-compiler-opt-0.0.1.dev202306220007/ml_compiler_opt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 00:07:05.000000 ml-compiler-opt-0.0.1.dev202306220007/ml_compiler_opt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 00:06:45.000000 ml-compiler-opt-0.0.1.dev202306220007/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 00:07:06.029735 ml-compiler-opt-0.0.1.dev202306220007/setup.cfg
```

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/LICENSE` & `ml-compiler-opt-0.0.1.dev202306220007/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/PKG-INFO` & `ml-compiler-opt-0.0.1.dev202306220007/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-compiler-opt
-Version: 0.0.1.dev202306210145
+Version: 0.0.1.dev202306220007
 Summary: Tooling for ML in LLVM
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Infrastructure for MLGO - a Machine Learning Guided Compiler Optimizations Framework.
```

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/README.md` & `ml-compiler-opt-0.0.1.dev202306220007/README.md`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_chromium.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_chromium.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_llvm_test_suite.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_llvm_test_suite.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_report.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_report.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_report_converter.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_report_converter.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmark_report_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmark_report_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/benchmarking_utils.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/benchmarking_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/filter_tests.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/filter_tests.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/gtest_executable_utils.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/gtest_executable_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/benchmark/list_gtests.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/benchmark/list_gtests.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/buffered_scheduler.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/buffered_scheduler.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/buffered_scheduler_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/buffered_scheduler_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/local/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/local/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/local/local_worker_manager.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/local/local_worker_manager.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/local/local_worker_manager_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/local/local_worker_manager_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/worker.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/worker.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/distributed/worker_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/distributed/worker_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/blackbox_optimizers.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/blackbox_optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 point obtained after conducting one optimization step.
 """
 
 import abc
 import enum
 import math
 
-from absl import flags
 import numpy as np
 import numpy.typing as npt
 import scipy.optimize as sp_opt
 from sklearn import linear_model
 from typing import Any, Callable, Dict, List, Mapping, Tuple, Optional, Sequence, Union
 
 from compiler_opt.es import gradient_ascent_optimization_algorithms
@@ -55,14 +54,17 @@
 
 
 class LinearModel(enum.Enum):
   LASSO = linear_model.Lasso
   RIDGE = linear_model.Ridge
 
 
+DEFAULT_ARMIJO = 1e-4
+
+
 def filter_top_directions(
     perturbations: npt.NDArray[np.float32],
     function_values: npt.NDArray[np.float32], est_type: EstimatorType,
     num_top_directions: int
 ) -> Tuple[npt.NDArray[np.float32], npt.NDArray[np.float32]]:
   """Select the subset of top-performing perturbations.
 
@@ -320,42 +322,14 @@
 # pylint: disable=pointless-string-statement
 """Secondorder optimizers.
 
 Experimental optimizers based on blackbox ES.
 
 See class descriptions for more detailed notes on each algorithm.
 """
-
-_GRAD_TYPE = flags.DEFINE_string('grad_type', 'MC', 'Gradient estimator.')
-_TR_INIT_RADIUS = flags.DEFINE_float('tr_init_radius', 1,
-                                     'Initial radius for TR method.')
-_TR_GROW_THRESHOLD = flags.DEFINE_float('tr_grow_threshold', 1e-4,
-                                        'Growth test for TR method.')
-_TR_GROW_FACTOR = flags.DEFINE_float('tr_grow_factor', 1.1,
-                                     'Growth factor for TR method.')
-_TR_SHRINK_NEG_THRESHOLD = flags.DEFINE_float('tr_shrink_neg_threshold', 0.1,
-                                              'Shrink test for TR method')
-_TR_SHRINK_FACTOR = flags.DEFINE_float('tr_shrink_factor', 0.9,
-                                       'Shrink factor for TR method.')
-_TR_REJECT_THRESHOLD = flags.DEFINE_float('tr_reject_threshold', 0.5,
-                                          'Reject test for TR method.')
-_TR_REJECT_FACTOR = flags.DEFINE_float(
-    'tr_reject_factor', 0.5, 'Rejection shrink factor for TR method.')
-_TR_DENSE_HESSIAN = flags.DEFINE_bool('tr_dense_hessian', True,
-                                      'Store dense Hessian for TR.')
-_TR_SUB_TERMINATION = flags.DEFINE_float(
-    'tr_sub_termination', 1e-3,
-    'Subproblem gradient norm termination for TR method.')
-_TR_SUBPROBLEM_MAXITER = flags.DEFINE_integer(
-    'tr_subproblem_maxiter', 10,
-    'Maximum iterations when TR subproblem line search fails.')
-_TR_MINIMUM_RADIUS = flags.DEFINE_float('tr_minimum_radius', 0.1,
-                                        'Minimum radius of trust region.')
-
-DEFAULT_ARMIJO = 1e-4
 """Gradient estimators.
 The blackbox pipeline has two steps:
 estimate gradient/Hessian --> optimizer --> next weight
 which are decoupled.
 
 Implemented: monte_carlo_gradient
              sklearn_regression_gradient
```

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/blackbox_optimizers_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/blackbox_optimizers_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/gradient_ascent_optimization_algorithms.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/gradient_ascent_optimization_algorithms.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/es/gradient_ascent_optimization_algorithms_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/package_config.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/package_config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/agent_config.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/agent_config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/agent_config_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/agent_config_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/best_trajectory.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/best_trajectory.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/best_trajectory_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/best_trajectory_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/compilation_runner.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/compilation_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/compilation_runner_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/compilation_runner_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/constant.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/constant.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/constant_value_network.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/constant_value_network.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/constant_value_network_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/constant_value_network_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/corpus.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/corpus.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/corpus_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/corpus_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/data_collector.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/data_collector.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/data_collector_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/data_collector_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/data_reader.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/data_reader.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/data_reader_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/data_reader_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/agent.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/agent.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/learner.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/learner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_collect.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_collect.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_collect_lib.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_collect_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_eval.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_eval.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_eval_lib.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_eval_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_reverb_server.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_reverb_server.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_reverb_server_lib.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_reverb_server_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_train.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_train.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/distributed/ppo_train_lib.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/distributed/ppo_train_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/env.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/env.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/env_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/env_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/feature_ops.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/feature_ops.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/feature_ops_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/feature_ops_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/gin_external_configurables.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/gin_external_configurables.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/config.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/env.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/env.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/inlining/inlining_runner.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/inlining/inlining_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/local_data_collector.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/local_data_collector.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/local_data_collector_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/local_data_collector_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/log_reader.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/log_reader.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/log_reader_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/log_reader_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/policy_saver.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/policy_saver.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/policy_saver_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/policy_saver_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/problem_configuration.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/problem_configuration.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/random_net_distillation.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/random_net_distillation.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/random_net_distillation_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/random_net_distillation_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/config.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/regalloc_network.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/regalloc_network.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/regalloc_network_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/regalloc_network_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc/regalloc_runner.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc/regalloc_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc_priority/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc_priority/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc_priority/config.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc_priority/config.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/regalloc_priority/regalloc_priority_runner.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/registry.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/registry.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/train_bc.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/train_bc.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/train_locally.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/train_locally.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/trainer.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/trainer.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/rl/trainer_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/rl/trainer_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/__init__.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/combine_training_corpus.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/combine_training_corpus.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/combine_training_corpus_lib.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/combine_training_corpus_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/combine_training_corpus_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/combine_training_corpus_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/extract_ir.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/extract_ir.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/extract_ir_lib.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/extract_ir_lib.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/extract_ir_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/extract_ir_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/feature_importance.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/feature_importance.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/feature_importance_graphs.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/feature_importance_graphs.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/feature_importance_utils.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/feature_importance_utils.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/feature_importance_utils_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/feature_importance_utils_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_default_trace.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_default_trace.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_default_trace_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_default_trace_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_test_model.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_test_model.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_test_model_test.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_test_model_test.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/generate_vocab.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/generate_vocab.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/compiler_opt/tools/merge_best_trajectory.py` & `ml-compiler-opt-0.0.1.dev202306220007/compiler_opt/tools/merge_best_trajectory.py`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/ml_compiler_opt.egg-info/PKG-INFO` & `ml-compiler-opt-0.0.1.dev202306220007/ml_compiler_opt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-compiler-opt
-Version: 0.0.1.dev202306210145
+Version: 0.0.1.dev202306220007
 Summary: Tooling for ML in LLVM
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Infrastructure for MLGO - a Machine Learning Guided Compiler Optimizations Framework.
```

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/ml_compiler_opt.egg-info/SOURCES.txt` & `ml-compiler-opt-0.0.1.dev202306220007/ml_compiler_opt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-compiler-opt-0.0.1.dev202306210145/pyproject.toml` & `ml-compiler-opt-0.0.1.dev202306220007/pyproject.toml`

 * *Files identical despite different names*

