# Comparing `tmp/seldonian_engine-0.7.9.tar.gz` & `tmp/seldonian_engine-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seldonian_engine-0.7.9.tar", last modified: Mon Feb 13 21:05:08 2023, max compression
+gzip compressed data, was "seldonian_engine-0.8.0.tar", last modified: Thu Jun 22 21:25:55 2023, max compression
```

## Comparing `seldonian_engine-0.7.9.tar` & `seldonian_engine-0.8.0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.596513 seldonian_engine-0.7.9/
--rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/LICENSE
--rw-r--r--   0 ahoag      (501) staff       (20)     2134 2023-02-13 21:05:08.596308 seldonian_engine-0.7.9/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)     1643 2022-11-11 22:25:32.000000 seldonian_engine-0.7.9/README.md
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.576499 seldonian_engine-0.7.9/seldonian/
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.579009 seldonian_engine-0.7.9/seldonian/RL/
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.580485 seldonian_engine-0.7.9/seldonian/RL/Agents/
--rw-r--r--   0 ahoag      (501) staff       (20)     1761 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.580949 seldonian_engine-0.7.9/seldonian/RL/Agents/Bases/
--rw-r--r--   0 ahoag      (501) staff       (20)     4301 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Bases/Fourier.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Bases/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1021 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Discrete_Random_Agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.581790 seldonian_engine-0.7.9/seldonian/RL/Agents/Function_Approximators/
--rw-r--r--   0 ahoag      (501) staff       (20)      527 2022-09-13 15:24:12.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1334 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Function_Approximators/Linear_FA.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2792 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Function_Approximators/Table.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Function_Approximators/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2662 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.582431 seldonian_engine-0.7.9/seldonian/RL/Agents/Policies/
--rw-r--r--   0 ahoag      (501) staff       (20)     4808 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Policies/Policy.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4620 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Policies/Softmax.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/Policies/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)      793 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/keyboard_gridworld.py
--rw-r--r--   0 ahoag      (501) staff       (20)      404 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/Agents/mountain_car_rough_solution.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.582908 seldonian_engine-0.7.9/seldonian/RL/Env_Description/
--rw-r--r--   0 ahoag      (501) staff       (20)     2052 2022-09-13 15:24:12.000000 seldonian_engine-0.7.9/seldonian/RL/Env_Description/Env_Description.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2264 2022-09-13 15:24:12.000000 seldonian_engine-0.7.9/seldonian/RL/Env_Description/Spaces.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/Env_Description/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3669 2022-09-13 15:24:12.000000 seldonian_engine-0.7.9/seldonian/RL/RL_generate_dataset_and_spec_file.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1842 2022-09-13 15:24:12.000000 seldonian_engine-0.7.9/seldonian/RL/RL_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6592 2022-11-15 01:50:32.000000 seldonian_engine-0.7.9/seldonian/RL/RL_runner.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/__init__.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.584616 seldonian_engine-0.7.9/seldonian/RL/environments/
--rw-r--r--   0 ahoag      (501) staff       (20)     1407 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/environments/Environment.py
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/environments/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4095 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/environments/gridworld.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2297 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/environments/mountaincar.py
--rw-r--r--   0 ahoag      (501) staff       (20)      983 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/environments/n_step_mountaincar.py
--rw-r--r--   0 ahoag      (501) staff       (20)     2722 2022-09-13 15:24:12.000000 seldonian_engine-0.7.9/seldonian/RL/environments/simglucose_env.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1203 2022-11-15 01:50:32.000000 seldonian_engine-0.7.9/seldonian/RL/generate_gridworld_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1244 2022-09-21 21:26:26.000000 seldonian_engine-0.7.9/seldonian/RL/generate_mountaincar_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1344 2022-09-13 15:24:12.000000 seldonian_engine-0.7.9/seldonian/RL/generate_simglucose_episodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)      615 2022-09-13 15:24:12.000000 seldonian_engine-0.7.9/seldonian/RL/hyperparams_and_settings.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3953 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/RL/profiling_seldonian_RL.py
--rw-r--r--   0 ahoag      (501) staff       (20)       32 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/__init__.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.585134 seldonian_engine-0.7.9/seldonian/candidate_selection/
--rw-r--r--   0 ahoag      (501) staff       (20)       39 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/candidate_selection/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    14552 2022-12-20 22:01:23.000000 seldonian_engine-0.7.9/seldonian/candidate_selection/candidate_selection.py
--rw-r--r--   0 ahoag      (501) staff       (20)     7907 2022-12-13 21:49:32.000000 seldonian_engine-0.7.9/seldonian/dataset.py
--rw-r--r--   0 ahoag      (501) staff       (20)    20961 2023-01-03 20:20:35.000000 seldonian_engine-0.7.9/seldonian/hyperparam_search.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.587202 seldonian_engine-0.7.9/seldonian/models/
--rw-r--r--   0 ahoag      (501) staff       (20)       47 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/models/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     7237 2023-02-09 17:42:02.000000 seldonian_engine-0.7.9/seldonian/models/models.py
--rw-r--r--   0 ahoag      (501) staff       (20)    33863 2023-02-09 17:42:02.000000 seldonian_engine-0.7.9/seldonian/models/objectives.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1188 2023-02-09 17:42:02.000000 seldonian_engine-0.7.9/seldonian/models/pytorch_cnn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     5982 2022-12-20 22:01:23.000000 seldonian_engine-0.7.9/seldonian/models/pytorch_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)      978 2023-02-13 21:03:19.000000 seldonian_engine-0.7.9/seldonian/models/sklearn_lr.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4286 2023-02-13 21:03:19.000000 seldonian_engine-0.7.9/seldonian/models/sklearn_model.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1192 2022-12-08 20:24:26.000000 seldonian_engine-0.7.9/seldonian/models/tensorflow_cnn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     5293 2022-12-20 22:01:23.000000 seldonian_engine-0.7.9/seldonian/models/tensorflow_model.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.587851 seldonian_engine-0.7.9/seldonian/optimizers/
--rw-r--r--   0 ahoag      (501) staff       (20)       42 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/optimizers/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    10499 2023-02-09 17:42:02.000000 seldonian_engine-0.7.9/seldonian/optimizers/gradient_descent.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.589005 seldonian_engine-0.7.9/seldonian/parse_tree/
--rw-r--r--   0 ahoag      (501) staff       (20)       75 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/parse_tree/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    38411 2023-01-04 18:37:56.000000 seldonian_engine-0.7.9/seldonian/parse_tree/nodes.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3153 2022-11-02 17:40:20.000000 seldonian_engine-0.7.9/seldonian/parse_tree/operators.py
--rw-r--r--   0 ahoag      (501) staff       (20)    34928 2022-12-20 22:01:23.000000 seldonian_engine-0.7.9/seldonian/parse_tree/parse_tree.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.589718 seldonian_engine-0.7.9/seldonian/safety_test/
--rw-r--r--   0 ahoag      (501) staff       (20)       35 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/safety_test/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     3509 2023-01-04 18:37:56.000000 seldonian_engine-0.7.9/seldonian/safety_test/safety_test.py
--rw-r--r--   0 ahoag      (501) staff       (20)    12975 2023-02-09 17:42:02.000000 seldonian_engine-0.7.9/seldonian/seldonian_algorithm.py
--rw-r--r--   0 ahoag      (501) staff       (20)    16824 2023-02-09 17:42:02.000000 seldonian_engine-0.7.9/seldonian/spec.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.591243 seldonian_engine-0.7.9/seldonian/utils/
--rw-r--r--   0 ahoag      (501) staff       (20)      466 2022-09-29 23:20:05.000000 seldonian_engine-0.7.9/seldonian/utils/RL_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)       23 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/utils/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1677 2022-11-07 22:08:04.000000 seldonian_engine-0.7.9/seldonian/utils/io_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     5638 2023-01-03 20:20:35.000000 seldonian_engine-0.7.9/seldonian/utils/plot_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1418 2022-11-02 17:40:20.000000 seldonian_engine-0.7.9/seldonian/utils/stats_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4241 2022-12-08 20:24:26.000000 seldonian_engine-0.7.9/seldonian/utils/tutorial_utils.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.591596 seldonian_engine-0.7.9/seldonian/warnings/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/warnings/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)      344 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/seldonian/warnings/custom_warnings.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.592336 seldonian_engine-0.7.9/seldonian_engine.egg-info/
--rw-r--r--   0 ahoag      (501) staff       (20)     2134 2023-02-13 21:05:08.000000 seldonian_engine-0.7.9/seldonian_engine.egg-info/PKG-INFO
--rw-r--r--   0 ahoag      (501) staff       (20)     2998 2023-02-13 21:05:08.000000 seldonian_engine-0.7.9/seldonian_engine.egg-info/SOURCES.txt
--rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-02-13 21:05:08.000000 seldonian_engine-0.7.9/seldonian_engine.egg-info/dependency_links.txt
--rw-r--r--   0 ahoag      (501) staff       (20)      148 2023-02-13 21:05:08.000000 seldonian_engine-0.7.9/seldonian_engine.egg-info/requires.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       16 2023-02-13 21:05:08.000000 seldonian_engine-0.7.9/seldonian_engine.egg-info/top_level.txt
--rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-02-13 21:05:08.596567 seldonian_engine-0.7.9/setup.cfg
--rw-r--r--   0 ahoag      (501) staff       (20)     1070 2023-02-13 21:05:02.000000 seldonian_engine-0.7.9/setup.py
-drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-02-13 21:05:08.595938 seldonian_engine-0.7.9/tests/
--rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/tests/__init__.py
--rw-r--r--   0 ahoag      (501) staff       (20)    13711 2022-12-13 21:49:32.000000 seldonian_engine-0.7.9/tests/conftest.py
--rw-r--r--   0 ahoag      (501) staff       (20)    10918 2022-12-13 21:49:32.000000 seldonian_engine-0.7.9/tests/test_RL.py
--rw-r--r--   0 ahoag      (501) staff       (20)     5697 2022-12-13 21:49:32.000000 seldonian_engine-0.7.9/tests/test_dataset.py
--rw-r--r--   0 ahoag      (501) staff       (20)      828 2022-09-21 21:32:24.000000 seldonian_engine-0.7.9/tests/test_io_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     5508 2022-12-08 20:24:26.000000 seldonian_engine-0.7.9/tests/test_objectives.py
--rw-r--r--   0 ahoag      (501) staff       (20)    58872 2022-12-13 21:49:32.000000 seldonian_engine-0.7.9/tests/test_parse_tree.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1223 2022-09-12 23:15:58.000000 seldonian_engine-0.7.9/tests/test_plot_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)     4892 2022-12-13 21:49:32.000000 seldonian_engine-0.7.9/tests/test_safety_test.py
--rw-r--r--   0 ahoag      (501) staff       (20)    59333 2023-01-04 18:37:56.000000 seldonian_engine-0.7.9/tests/test_seldonian_algorithm.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1582 2023-02-09 17:42:02.000000 seldonian_engine-0.7.9/tests/test_sklearn.py
--rw-r--r--   0 ahoag      (501) staff       (20)     6389 2022-11-07 22:08:04.000000 seldonian_engine-0.7.9/tests/test_spec.py
--rw-r--r--   0 ahoag      (501) staff       (20)     1272 2022-09-21 21:32:24.000000 seldonian_engine-0.7.9/tests/test_stats_utils.py
--rw-r--r--   0 ahoag      (501) staff       (20)      544 2022-09-21 21:32:24.000000 seldonian_engine-0.7.9/tests/test_tutorial_utils.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.821403 seldonian_engine-0.8.0/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1527 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/LICENSE
+-rw-r--r--   0 ahoag      (501) staff       (20)     2134 2023-06-22 21:25:55.821215 seldonian_engine-0.8.0/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)     1643 2022-11-11 22:25:32.000000 seldonian_engine-0.8.0/README.md
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.800861 seldonian_engine-0.8.0/seldonian/
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.803227 seldonian_engine-0.8.0/seldonian/RL/
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.804289 seldonian_engine-0.8.0/seldonian/RL/Agents/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1733 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.804610 seldonian_engine-0.8.0/seldonian/RL/Agents/Bases/
+-rw-r--r--   0 ahoag      (501) staff       (20)     4537 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Bases/Fourier.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Bases/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1043 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Discrete_Random_Agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.805246 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/
+-rw-r--r--   0 ahoag      (501) staff       (20)      554 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1333 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Linear_FA.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2854 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Table.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3054 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Parameterized_non_learning_softmax_agent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.805791 seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/
+-rw-r--r--   0 ahoag      (501) staff       (20)     4906 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/Policy.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6459 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/Softmax.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      794 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/keyboard_gridworld.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      406 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Agents/mountain_car_rough_solution.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.806233 seldonian_engine-0.8.0/seldonian/RL/Env_Description/
+-rw-r--r--   0 ahoag      (501) staff       (20)     2001 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Env_Description/Env_Description.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2311 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/Env_Description/Spaces.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/Env_Description/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3698 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/RL_generate_dataset_and_spec_file.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2335 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/RL/RL_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6614 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/RL_runner.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/__init__.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.807120 seldonian_engine-0.8.0/seldonian/RL/environments/
+-rw-r--r--   0 ahoag      (501) staff       (20)     1364 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/Environment.py
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/RL/environments/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4075 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/gridworld.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2352 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/mountaincar.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      984 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/n_step_mountaincar.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2807 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/environments/simglucose_env.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1196 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/generate_gridworld_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1236 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/generate_mountaincar_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1337 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/generate_simglucose_episodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      615 2022-09-13 15:24:12.000000 seldonian_engine-0.8.0/seldonian/RL/hyperparams_and_settings.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3991 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/RL/profiling_seldonian_RL.py
+-rw-r--r--   0 ahoag      (501) staff       (20)       33 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/__init__.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.807449 seldonian_engine-0.8.0/seldonian/candidate_selection/
+-rw-r--r--   0 ahoag      (501) staff       (20)       40 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/candidate_selection/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    19265 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/candidate_selection/candidate_selection.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    12880 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/dataset.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    21029 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/hyperparam_search.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.809226 seldonian_engine-0.8.0/seldonian/models/
+-rw-r--r--   0 ahoag      (501) staff       (20)       48 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     8288 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/models/models.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    40182 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/models/objectives.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1284 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/pytorch_cnn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6883 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/models/pytorch_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1084 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/sklearn_lr.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4758 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/sklearn_model.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1559 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/tensorflow_cnn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6068 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/models/tensorflow_model.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.809580 seldonian_engine-0.8.0/seldonian/optimizers/
+-rw-r--r--   0 ahoag      (501) staff       (20)       43 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/optimizers/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    10884 2023-04-03 17:05:25.000000 seldonian_engine-0.8.0/seldonian/optimizers/gradient_descent.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.811134 seldonian_engine-0.8.0/seldonian/parse_tree/
+-rw-r--r--   0 ahoag      (501) staff       (20)       75 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/parse_tree/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    40039 2023-06-06 19:58:26.000000 seldonian_engine-0.8.0/seldonian/parse_tree/nodes.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     3828 2023-04-19 20:33:28.000000 seldonian_engine-0.8.0/seldonian/parse_tree/operators.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    46725 2023-06-13 16:21:42.000000 seldonian_engine-0.8.0/seldonian/parse_tree/parse_tree.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.812065 seldonian_engine-0.8.0/seldonian/safety_test/
+-rw-r--r--   0 ahoag      (501) staff       (20)       36 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/safety_test/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4272 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/safety_test/safety_test.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    15854 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/seldonian_algorithm.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    22099 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/spec.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.813761 seldonian_engine-0.8.0/seldonian/utils/
+-rw-r--r--   0 ahoag      (501) staff       (20)      468 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/utils/RL_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)       24 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/utils/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1685 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/utils/io_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6891 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/utils/plot_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     2011 2023-05-31 21:23:44.000000 seldonian_engine-0.8.0/seldonian/utils/stats_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4210 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/seldonian/utils/tutorial_utils.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.814195 seldonian_engine-0.8.0/seldonian/warnings/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/seldonian/warnings/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      344 2023-03-08 18:13:56.000000 seldonian_engine-0.8.0/seldonian/warnings/custom_warnings.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.816011 seldonian_engine-0.8.0/seldonian_engine.egg-info/
+-rw-r--r--   0 ahoag      (501) staff       (20)     2134 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/PKG-INFO
+-rw-r--r--   0 ahoag      (501) staff       (20)     2998 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)        1 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)      148 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/requires.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       16 2023-06-22 21:25:55.000000 seldonian_engine-0.8.0/seldonian_engine.egg-info/top_level.txt
+-rw-r--r--   0 ahoag      (501) staff       (20)       38 2023-06-22 21:25:55.821450 seldonian_engine-0.8.0/setup.cfg
+-rw-r--r--   0 ahoag      (501) staff       (20)     1070 2023-06-22 21:25:20.000000 seldonian_engine-0.8.0/setup.py
+drwxr-xr-x   0 ahoag      (501) staff       (20)        0 2023-06-22 21:25:55.820909 seldonian_engine-0.8.0/tests/
+-rw-r--r--   0 ahoag      (501) staff       (20)        0 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/tests/__init__.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    14897 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/conftest.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    13340 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/test_RL.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6913 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/test_dataset.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      828 2022-09-21 21:32:24.000000 seldonian_engine-0.8.0/tests/test_io_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     5508 2022-12-08 20:24:26.000000 seldonian_engine-0.8.0/tests/test_objectives.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    64110 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/test_parse_tree.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1223 2022-09-12 23:15:58.000000 seldonian_engine-0.8.0/tests/test_plot_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     4820 2023-06-22 21:24:25.000000 seldonian_engine-0.8.0/tests/test_safety_test.py
+-rw-r--r--   0 ahoag      (501) staff       (20)    61690 2023-06-13 16:21:42.000000 seldonian_engine-0.8.0/tests/test_seldonian_algorithm.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1582 2023-02-09 17:42:02.000000 seldonian_engine-0.8.0/tests/test_sklearn.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     6389 2022-11-07 22:08:04.000000 seldonian_engine-0.8.0/tests/test_spec.py
+-rw-r--r--   0 ahoag      (501) staff       (20)     1272 2022-09-21 21:32:24.000000 seldonian_engine-0.8.0/tests/test_stats_utils.py
+-rw-r--r--   0 ahoag      (501) staff       (20)      544 2022-09-21 21:32:24.000000 seldonian_engine-0.8.0/tests/test_tutorial_utils.py
```

### Comparing `seldonian_engine-0.7.9/LICENSE` & `seldonian_engine-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/PKG-INFO` & `seldonian_engine-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian_engine
-Version: 0.7.9
+Version: 0.8.0
 Summary: Core library for Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_engine-0.7.9/README.md` & `seldonian_engine-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Agents/Agent.py` & `seldonian_engine-0.8.0/seldonian/RL/Agents/Agent.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,55 @@
-
 class Agent:
     def __init__(self):
         pass
         """ Base class for all RL agents. Override all methods
         below in child class implementation """
+
     def choose_action(self, observation):
-        """ Choose an action given an observation. To be overridden 
+        """Choose an action given an observation. To be overridden
 
         :param observation: The current observation of the agent,
             type depends on environment.
         """
         raise NotImplementedError()
 
     def update(self, observation, next_observation, reward, terminated):
-        """ 
+        """
         Updates agent's parameters according to the learning rule
         To be overriden
-        
+
         :param observation: The current observation of the agent,
             type depends on environment.
 
         :param next_observation: The observation of the agent after
             an action is taken
 
-        :param reward: The reward for taking the action 
+        :param reward: The reward for taking the action
 
-        :param terminated: Whether next_observation is the 
+        :param terminated: Whether next_observation is the
             terminal observation
         :type terminated: bool
         """
         raise NotImplementedError()
 
     def get_prob_this_action(self, observation, action):
-        """ Get probability of a given action provided environment 
-        is in a observation. To be overridden 
+        """Get probability of a given action provided environment
+        is in a observation. To be overridden
 
         :param observation: The current observation of the agent,
             type depends on environment.
         """
         raise NotImplementedError()
 
     def set_new_params(self, theta):
-        """ Update the parameters of the agent's policy 
+        """Update the parameters of the agent's policy
 
         :param theta: model parameters
         """
         raise NotImplementedError()
 
     def get_params(self):
-        """ Retrieve the parameters of the agent's policy
-        """
+        """Retrieve the parameters of the agent's policy"""
         raise NotImplementedError()
 
     def get_policy(self):
         raise NotImplementedError()
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Agents/Bases/Fourier.py` & `seldonian_engine-0.8.0/seldonian/RL/Agents/Bases/Fourier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from seldonian.utils.RL_utils import *
 from math import factorial, pi
 
+
 class Fourier:
     def __init__(self, hyperparam_and_setting_dict, env_desc):
-        """ Fourier basis used for linear value function 
+        """Fourier basis used for linear value function
         approximation. See http://irl.cs.brown.edu/fb.php for
         a reference
 
         :param hyperparameter_and_setting_dict: Specifies the
             environment, agent, number of episodes per trial,
             and number of trials
 
@@ -31,53 +32,69 @@
         if self.max_coupled_vars > self.num_observation_dims:
             error("max_coupled_vars > num_observation_dims")
 
         self.mins = env_desc.observation_space.bounds[:, 0]
         self.maxes = env_desc.observation_space.bounds[:, 1]
         self.ranges = self.maxes - self.mins
 
-        self.num_features = self.calculate_num_features(self.order, self.max_coupled_vars, self.num_observation_dims)
+        self.num_features = self.calculate_num_features(
+            self.order, self.max_coupled_vars, self.num_observation_dims
+        )
         self.basis_matrix = self.construct_basis_matrix()
 
     def calculate_num_features(self, order, max_coupled_vars, num_obs_dims):
-        """ Determine the number of features in the basis 
-        """
+        """Determine the number of features in the basis"""
         num_features = (order + 1) ** num_obs_dims
-        for mandatory_0_observation_variables in range(max_coupled_vars+1, num_obs_dims + 1):
-            num_features -= order ** mandatory_0_observation_variables * factorial(num_obs_dims) / factorial(num_obs_dims - mandatory_0_observation_variables) / factorial(mandatory_0_observation_variables)
+        for mandatory_0_observation_variables in range(
+            max_coupled_vars + 1, num_obs_dims + 1
+        ):
+            num_features -= (
+                order**mandatory_0_observation_variables
+                * factorial(num_obs_dims)
+                / factorial(num_obs_dims - mandatory_0_observation_variables)
+                / factorial(mandatory_0_observation_variables)
+            )
         return num_features
 
     def construct_basis_matrix(self):
-        """ Create the basis matrix """
-        basis_matrix = np.zeros((self.num_features, self.num_observation_dims), dtype=int)
+        """Create the basis matrix"""
+        basis_matrix = np.zeros(
+            (self.num_features, self.num_observation_dims), dtype=int
+        )
         row = 0  # row of the matrix corresponds to the features
         fully_coupled_num_features = (self.order + 1) ** self.num_observation_dims
         for fully_coupled_feature in range(fully_coupled_num_features):
             num_in_row_non_zero = 0
             for observation_dim in range(self.num_observation_dims):
-                rep_size = (self.order + 1) ** (self.num_observation_dims - observation_dim - 1)  # representation size of count on this entry (e.g. if binary (meaning order = 1) then last column has rep_size 1, 2nd-to last has 2, 3rd to last has 4, etc.)
+                rep_size = (self.order + 1) ** (
+                    self.num_observation_dims - observation_dim - 1
+                )  # representation size of count on this entry (e.g. if binary (meaning order = 1) then last column has rep_size 1, 2nd-to last has 2, 3rd to last has 4, etc.)
                 entry_value = (fully_coupled_feature / rep_size) % (self.order + 1)
                 if entry_value != 0:
                     num_in_row_non_zero += 1
-                basis_matrix[row, observation_dim] = entry_value  # adding plus one for C++-to-Julia translation
+                basis_matrix[
+                    row, observation_dim
+                ] = entry_value  # adding plus one for C++-to-Julia translation
             if num_in_row_non_zero > self.max_coupled_vars:  # redo the row
                 row -= 1
             row += 1
             if row == self.num_features:
                 break  # don't want it to keep running invalid lines if it got all the good ones (they'll be out of range of the matrix)
         if row != self.num_features:
             error("row != num_features at this point, this should never happen")
         return basis_matrix
 
     def get_features(self, obs):
-        """ Get the basis feature given an observation """
+        """Get the basis feature given an observation"""
         normalized_obs = self.get_normalized_observation(obs)
         ret_matrix = np.dot(self.basis_matrix, normalized_obs)
-        ret_matrix = np.cos(pi*ret_matrix)
+        ret_matrix = np.cos(pi * ret_matrix)
         return ret_matrix
 
     def get_normalized_observation(self, obs):
-        """ Get the normalized observation given an observation """
+        """Get the normalized observation given an observation"""
         norm_obs = np.zeros(self.num_observation_dims)
         for obs_dim in range(self.num_observation_dims):
-            norm_obs[obs_dim] = (obs[obs_dim] - self.mins[obs_dim]) / self.ranges[obs_dim]
+            norm_obs[obs_dim] = (obs[obs_dim] - self.mins[obs_dim]) / self.ranges[
+                obs_dim
+            ]
         return norm_obs
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Agents/Discrete_Random_Agent.py` & `seldonian_engine-0.8.0/seldonian/RL/Agents/Discrete_Random_Agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from seldonian.RL.Agents.Agent import *
 import autograd.numpy as np
 
+
 class Discrete_Random_Agent(Agent):
     def __init__(self, env_description):
-        """ An agent that acts on discrete 
+        """An agent that acts on discrete
         observation and action spaces.
-        Picks actions according to uniform random policy. 
+        Picks actions according to uniform random policy.
         Is not capable of learning.
 
         :param env_description: an object for accessing attributes
             of the environment
         :type env_description: :py:class:`.Env_Description`
         """
         self.min_action = env_description.action_space.min
         self.max_action = env_description.action_space.max
         self.num_actions = self.max_action - self.min_action + 1
 
     def choose_action(self, observation):
-        return np.random.randint(self.min_action, self.max_action + 1) #+1 because this function's high is exclusive
+        return np.random.randint(
+            self.min_action, self.max_action + 1
+        )  # +1 because this function's high is exclusive
 
     def update(self, observation, next_observation, reward, terminated):
         pass
 
     def get_prob_this_action(self, observation, action):
         return 1.0 / self.num_actions
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py` & `seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Function_Approximator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import autograd.numpy as np
 from seldonian.utils.RL_utils import *
 
+
 class Function_Approximator:
-    """ Base class for a function approximator """
+    """Base class for a function approximator"""
 
     def set_new_params(self, new_params):
-        """ Set the new model parameter weights """
+        """Set the new model parameter weights"""
         old_shape = np.shape(self.weights)
         new_shape = np.shape(new_params)
         if old_shape != new_shape:
-            error(f"Trying to set new params, but old shape is {old_shape} and new shape is {new_shape}. They should be the same")
+            error(
+                f"Trying to set new params, but old shape is {old_shape} and new shape is {new_shape}. They should be the same"
+            )
         self.weights = new_params
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Agents/Function_Approximators/Linear_FA.py` & `seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Linear_FA.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from seldonian.RL.Agents.Function_Approximators.Function_Approximator import *
 
+
 class Linear_FA(Function_Approximator):
     def __init__(self, basis, env_description):
-        """ Base class for linear function approximators. 
+        """Base class for linear function approximators.
 
         :param basis: The basis to use for encoding features
         :param env_description: an object for accessing attributes
             of the environment
         :type env_description: :py:class:`.Env_Description`
         """
         self.basis = basis
         self.weights = np.zeros((basis.num_features, env_description.get_num_actions()))
 
+
 class Linear_state_action_value_FA(Linear_FA):
     def __init__(self, basis, env_description):
-        """A linear state action value function approximator. 
+        """A linear state action value function approximator.
 
         :param basis: The basis to use for encoding features
         :param env_description: an object for accessing attributes
             of the environment
         :type env_description: :py:class:`.Env_Description`
         """
         super().__init__(basis, env_description)
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Agents/Function_Approximators/Table.py` & `seldonian_engine-0.8.0/seldonian/RL/Agents/Function_Approximators/Table.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from seldonian.RL.Agents.Function_Approximators.Function_Approximator import *
 import autograd.numpy as np
 
+
 class Table(Function_Approximator):
     def __init__(self, min_state, num_states):
-        """ Table holding states, capable of reindexing states
-        
+        """Table holding states, capable of reindexing states
+
         :param min_state: The smallest obs number
         :type min_state: int
         :param num_states: Number of total states
         :type num_states: int
         """
         self.min_state = min_state
         self.num_states = num_states
@@ -19,52 +20,62 @@
 
         :param env_state: The environment obs you want to convert
         :type env: int
         :return: 0-indexed obs in the table
         """
         return env_state - self.min_state
 
+
 class Q_Table(Table):
     def __init__(self, min_state, num_states, num_actions):
-        """ A Q table containing transition probabilities 
+        """A Q table containing transition probabilities
 
         :param min_state: The smallest obs number
         :type min_state: int
         :param num_states: Number of total states
         :type num_states: int
         :param num_actions: Number of actions in a given obs
         :type num_actions: int
         """
         super().__init__(min_state, num_states)
         self.weights = np.zeros((num_states, num_actions))
         self.num_actions = num_actions
 
     def get_action_values_given_state(self, state_number_not_zero_indexed):
-        """ Get possible Q-table values given environmental obs
+        """Get possible Q-table values given environmental obs
 
         :param state_number_not_zero_indexed: The environment-specific obs number
         :type state_number_not_zero_indexed: int
         :return: array of possible Q-table values
         """
 
-        zero_indexed_state_number = self.from_environment_state_to_0_indexed_state(state_number_not_zero_indexed)
-        return self.get_action_values_given_zero_indexed_state(zero_indexed_state_number)
+        zero_indexed_state_number = self.from_environment_state_to_0_indexed_state(
+            state_number_not_zero_indexed
+        )
+        return self.get_action_values_given_zero_indexed_state(
+            zero_indexed_state_number
+        )
 
     def get_action_values_given_zero_indexed_state(self, zero_indexed_state_number):
-        """ Get possible Q-table values given 0-indexed obs number in the table
+        """Get possible Q-table values given 0-indexed obs number in the table
 
         :param zero_indexed_state_number: The 0-indexed obs number in the table
         :type zero_indexed_state_number: int
         :return: array of possible actions
         """
         return self.weights[zero_indexed_state_number, :]
 
+
 def construct_Q_Table_From_Env_Description(env_description):
-    """ Create a Q table given an environment description 
+    """Create a Q table given an environment description
 
     :param env_description: an object for accessing attributes
             of the environment
     :type env_description: :py:class:`.Env_Description`
-    :return: A Q Table 
+    :return: A Q Table
     :rtype: :py:class:`.Q_Table`
     """
-    return Q_Table(env_description.get_min_state(), env_description.get_num_states(), env_description.get_num_actions())
+    return Q_Table(
+        env_description.get_min_state(),
+        env_description.get_num_states(),
+        env_description.get_num_actions(),
+    )
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Agents/Policies/Policy.py` & `seldonian_engine-0.8.0/seldonian/RL/Agents/Policies/Policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,97 @@
 from seldonian.RL.Agents.Function_Approximators.Table import *
 from seldonian.RL.Agents.Function_Approximators.Linear_FA import *
 from seldonian.RL.Agents.Bases.Fourier import *
 from seldonian.RL.Env_Description.Env_Description import *
 
+
 class Policy:
     def __init__(self):
-        """ Base class for policies. Contains four methods which
-        must be overridden in any policy implementation """
+        """Base class for policies. Contains four methods which
+        must be overridden in any policy implementation"""
         pass
 
     def choose_action(self, obs):
-        """ Defines how to select an action given an observation, obs
-        """
+        """Defines how to select an action given an observation, obs"""
         raise NotImplementedError()
 
     def set_new_params(self, new_params):
-        """ Update policy parameters 
-        """
+        """Update policy parameters"""
         raise NotImplementedError()
 
     def get_params(self):
-        """ Get current policy parameters 
-        """
+        """Get current policy parameters"""
         raise NotImplementedError()
 
     def get_prob_this_action(self, obs, action):
-        """ Get probability of taking an action given an observation
-        """
+        """Get probability of taking an action given an observation"""
         raise NotImplementedError()
 
 
 class Discrete_Action_Policy(Policy):
     def __init__(self, hyperparam_and_setting_dict, env_description):
-        """ General policy class where actions are discrete
+        """General policy class where actions are discrete
 
         :param hyperparameter_and_setting_dict: Specifies the
             environment, agent, number of episodes per trial,
             and number of trials
         :param env_description: an object for accessing attributes
             of the environment
         :type env_description: :py:class:`.Env_Description`
         """
-        self.min_action = env_description.get_min_action() #e.g., if environment actions are {-1, 0, 1}, then this is -1
+        self.min_action = (
+            env_description.get_min_action()
+        )  # e.g., if environment actions are {-1, 0, 1}, then this is -1
         self.num_actions = env_description.get_num_actions()
-        self.FA = self.make_state_action_FA(env_description, hyperparam_and_setting_dict)
+        self.FA = self.make_state_action_FA(
+            env_description, hyperparam_and_setting_dict
+        )
 
     def from_0_indexed_action_to_environment_action(self, action_0_indexed):
-        """ Convert 0-indexed action to env-specific action """
+        """Convert 0-indexed action to env-specific action"""
         return action_0_indexed + self.min_action
 
     def from_environment_action_to_0_indexed_action(self, env_action):
-        """ Convert env-specific action to 0 indexed action """
+        """Convert env-specific action to 0 indexed action"""
         return env_action - self.min_action
 
     def make_state_action_FA(self, env_description, hyperparam_and_setting_dict):
-        """ Create a function approximator from an environment description and
+        """Create a function approximator from an environment description and
         dictionary specification
 
         :param env_description: an object for accessing attributes
             of the environment
         :type env_description: :py:class:`.Env_Description`
         :param hyperparameter_and_setting_dict: Specifies the
             environment, agent, number of episodes per trial,
             and number of trials
 
         :return: function approximator, type depends on whether observation
             space is discrete or continous
         """
-        if type(env_description.observation_space) == Discrete_Space and type(
-                env_description.action_space) == Discrete_Space:
+        if (
+            type(env_description.observation_space) == Discrete_Space
+            and type(env_description.action_space) == Discrete_Space
+        ):
             return construct_Q_Table_From_Env_Description(env_description)
-        if type(env_description.observation_space) == Continuous_Space and type(
-                env_description.action_space) == Discrete_Space:
-            return self.construct_basis_and_linear_FA(env_description, hyperparam_and_setting_dict)
+        if (
+            type(env_description.observation_space) == Continuous_Space
+            and type(env_description.action_space) == Discrete_Space
+        ):
+            return self.construct_basis_and_linear_FA(
+                env_description, hyperparam_and_setting_dict
+            )
         else:
-            error(f"unhandled state type {type(env_description.observation_space)} and action type {type(env_description.action_space)} for make_state_action_FA()")
-
-    def construct_basis_and_linear_FA(self, env_description, hyperparam_and_setting_dict):
+            error(
+                f"unhandled state type {type(env_description.observation_space)} and action type {type(env_description.action_space)} for make_state_action_FA()"
+            )
+
+    def construct_basis_and_linear_FA(
+        self, env_description, hyperparam_and_setting_dict
+    ):
         """Create a basis and linear function approximator
         from an environment description and dictionary specification
 
         :param env_description: an object for accessing attributes
             of the environment
         :type env_description: :py:class:`.Env_Description`
         :param hyperparameter_and_setting_dict: Specifies the
@@ -92,24 +103,23 @@
         if basis_type == "Fourier":
             basis = Fourier(hyperparam_and_setting_dict, env_description)
         else:
             error("unknown basis type ", basis_type)
         return Linear_state_action_value_FA(basis, env_description)
 
     def get_action_values_given_state(self, obs):
-        """ Get all parameter weights possible in a given observation
-        """ 
+        """Get all parameter weights possible in a given observation"""
         return self.FA.get_action_values_given_state(obs)
 
     def set_new_params(self, new_params):
-        """ Set the parameters of the agent
+        """Set the parameters of the agent
 
         :param new_params: array of weights
         """
         self.FA.set_new_params(new_params)
 
     def get_params(self):
-        """ Get the current parameters (weights) of the agent
+        """Get the current parameters (weights) of the agent
 
         :return: array of weights
         """
         return self.FA.weights
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Agents/keyboard_gridworld.py` & `seldonian_engine-0.8.0/seldonian/RL/Agents/keyboard_gridworld.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from seldonian.RL.Agents.Agent import *
 
+
 class Keyboard_gridworld(Agent):
     def __init__(self, env_description):
-        """ An agent used for debugging the gridworld
-        environment. Not intended for public use. """
+        """An agent used for debugging the gridworld
+        environment. Not intended for public use."""
         pass
 
     def choose_action(self, observation):
         action = self.ask_for_input()
         while action not in [1, 2, 3, 4]:
             print("invalid action, please try again")
             action = self.ask_for_input()
-        return action - 1 #env is zero-indexed
+        return action - 1  # env is zero-indexed
 
     def ask_for_input(self):
         return int(input("Enter 1, 2, 3, or 4 for UP, RIGHT, DOWN, LEFT respectively"))
 
     def update(self, observation, next_observation, reward, terminated):
         pass
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Env_Description/Env_Description.py` & `seldonian_engine-0.8.0/seldonian/RL/Env_Description/Env_Description.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,54 @@
 from seldonian.RL.Env_Description.Spaces import *
 from seldonian.utils.RL_utils import *
 
 
 class Env_Description:
     def __init__(self, observation_space, action_space):
-        """ Describes an environment's observation and action space
+        """Describes an environment's observation and action space
         and provides convenience methods for accessing the
-        environment's attributes 
+        environment's attributes
 
         :param observation_space: Discrete or continuous space
             describing observations made in the environment
         :param action_space: Discrete or continuous space
             describing possible actions taken in the environment
         """
         self.observation_space = observation_space
         self.action_space = action_space
 
     def get_num_states(self):
-        """ Get number of states 
+        """Get number of states
         (also called observations here)
         """
         check_space_type(self.observation_space, Discrete_Space)
         return self.observation_space.get_num_values()
 
     def get_num_actions(self):
-        """ Get number of actions
-        """
+        """Get number of actions"""
         check_space_type(self.action_space, Discrete_Space)
         return self.action_space.get_num_values()
 
     def get_min_action(self):
-        """ Get first action in the action space 
-        """
+        """Get first action in the action space"""
         check_space_type(self.action_space, Discrete_Space)
         return self.action_space.min
 
     def get_min_state(self):
-        """ Get first obs in the observation space
-        """
+        """Get first obs in the observation space"""
         check_space_type(self.action_space, Discrete_Space)
         return self.observation_space.min
 
     def get_num_observation_dims(self):
-        """ Get the number of dimensions in the observation space
-        """
+        """Get the number of dimensions in the observation space"""
         return self.observation_space.get_num_dims()
 
 
 def check_space_type(space, desired_type):
-    """ Validator to ensure space types are equivalent 
-    
+    """Validator to ensure space types are equivalent
+
     :param space: discrete or continous space
     :param desired_type: Discrete_Space or Continous_Space
         which we want type(space) to match
     """
     if type(space) != desired_type:
         error(f"need space of type {desired_type}, but got space of type {type(space)}")
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/Env_Description/Spaces.py` & `seldonian_engine-0.8.0/seldonian/RL/Env_Description/Spaces.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 import autograd.numpy as np
 
 
 class Discrete_Space:
     def __init__(self, min, max):
-        """ Discrete space used for observations or actions
-        
+        """Discrete space used for observations or actions
+
         :param min: Minimum value of the space
         :type min: int
         :param max: Maximum value of the space
         :type max: int
         """
         self.min = min
         self.max = max
 
     def get_num_values(self):
-        """ Get the total number of values in the space
-        """
+        """Get the total number of values in the space"""
         return self.max - self.min + 1
 
 
 class Continuous_Space:
     def __init__(self, bounds):
-        """ Continuous space used for observations or actions
-        
+        """Continuous space used for observations or actions
+
         :param bounds: Defines the min,max in each dimension of the space.
             For example, if the space is 3D with x in [-1.0,1.0], y in [5.1,5.4],
             and z in [-12.5,-6.8], then bounds would be:
             np.array([[-1.0,1.0],[5.1,5.4],[-12.5,-6.8]])
         :type bounds: np.ndarray of shape (num_dims,2)
-    
+
         :ivar num_dims: The number of dimensions in the space
         """
         self.num_dims = bounds.shape[0]
         self.check_bounds_valid(bounds)
         self.bounds = bounds
-    
+
     def check_bounds_valid(self, bounds):
-        """ Check that the bounds are in valid format
-        and that in each dimension the bound maximum is larger 
+        """Check that the bounds are in valid format
+        and that in each dimension the bound maximum is larger
         than the bound minimum
 
         :param bounds: Defines the min,max in each dimension of the space.
             For example, if the space is 3D with x in [-1.0,1.0], y in [5.1,5.4],
             and z in [-12.5,-6.8], then bounds would be:
             np.array([[-1.0,1.0],[5.1,5.4],[-12.5,-6.8]])
         :type bounds: np.ndarray of shape (num_dims,2)
         """
 
         if type(bounds) != np.ndarray:
-            raise(Exception(f"Expected np.ndarray, got {type(bounds)}"))
+            raise (Exception(f"Expected np.ndarray, got {type(bounds)}"))
         shape = bounds.shape
         if len(shape) != 2 or shape[1] != 2:
-            raise(Exception(f"Expected bounds with shape n x 2, got shape {shape}"))
+            raise (Exception(f"Expected bounds with shape n x 2, got shape {shape}"))
         for dim in range(self.num_dims):
             if bounds[dim][0] > bounds[dim][1]:
-                raise(Exception(f"for dimension {dim}, min {bounds[dim][0]} is greater than max {bounds[dim][1]}"))
+                raise (
+                    Exception(
+                        f"for dimension {dim}, min {bounds[dim][0]} is greater than max {bounds[dim][1]}"
+                    )
+                )
 
     def get_num_dims(self):
-        """ Get the number of dimensions of the space """
+        """Get the number of dimensions of the space"""
         return self.num_dims
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/RL_generate_dataset_and_spec_file.py` & `seldonian_engine-0.8.0/seldonian/RL/RL_generate_dataset_and_spec_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,30 +4,29 @@
 from seldonian.RL.RL_runner import run_trial
 from seldonian.utils.RL_utils import *
 from seldonian.utils.io_utils import save_pickle
 from seldonian.spec import createRLSpec
 
 
 def main():
-    """ Run a trial of episodes and create RLSpec object, saving to disk.
-    """  
+    """Run a trial of episodes and create RLSpec object, saving to disk."""
 
     hyperparameter_and_setting_dict = define_hyperparameter_and_setting_dict()
     start_time = time()
     episodes, agent = run_trial(hyperparameter_and_setting_dict)
     print("agent:")
     print(agent)
     # Save episodes as pkl file:
     # save_pickle("n_step_mountaincar_100episodes.pkl",episodes)
     # print(f"data generation took {time() - start_time} seconds")
-    dataset = RLDataSet(episodes=episodes,meta_information=['O','A','R','pi'])
+    dataset = RLDataSet(episodes=episodes, meta_information=["O", "A", "R", "pi"])
 
     env_name = hyperparameter_and_setting_dict["env"]
     metadata_pth = get_metadata_path(env_name)
-    save_dir = '.'
+    save_dir = "."
     constraint_strs = get_constraint_string(env_name)
     deltas = [0.05]
     env_kwargs = get_env_kwargs(env_name)
     # policy = agent.get_policy()
 
     createRLSpec(
         dataset=dataset,
@@ -36,58 +35,66 @@
         deltas=deltas,
         env_kwargs=env_kwargs,
         frac_data_in_safety=0.6,
         initial_solution_fn=None,
         use_builtin_primary_gradient_fn=False,
         save=True,
         save_dir=save_dir,
-        verbose=False)
+        verbose=False,
+    )
+
 
 def get_metadata_path(env_name):
-    """ Given environment name, return path to metadata file """
+    """Given environment name, return path to metadata file"""
     if env_name == "gridworld":
         return "../../static/datasets/RL/gridworld/gridworld_metadata.json"
     elif env_name == "n_step_mountaincar":
         return "../../static/datasets/RL/n_step_mountaincar/n_step_mountaincar_metadata.json"
     elif env_name == "simglucose":
         return "../../static/datasets/RL/simglucose/simglucose.json"
     else:
         error(f"unknown env name {env_name}")
 
 
 def get_constraint_string(env_name):
-    """ Given environment name, return the default constraint string """
+    """Given environment name, return the default constraint string"""
     if env_name == "gridworld":
-        return ['J_pi_new >= -0.25']
+        return ["J_pi_new >= -0.25"]
     elif env_name == "n_step_mountaincar":
-        return ['J_pi_new >= -500'] #uniform random policy averaged a return of roughly -500 (sample size was 10k episodes)
+        return [
+            "J_pi_new >= -500"
+        ]  # uniform random policy averaged a return of roughly -500 (sample size was 10k episodes)
     elif env_name == "simglucose":
-        return ['zzzz'] #needs updating with something reasonable
+        return ["zzzz"]  # needs updating with something reasonable
     else:
         error(f"Unknown env_name {env_name}")
 
+
 def get_env_kwargs(env_name):
-    """ Given environment name, return the default env kwargs """
+    """Given environment name, return the default env kwargs"""
     if env_name == "gridworld":
         from seldonian.RL.environments.gridworld import Gridworld
+
         RL_environment = Gridworld()
         gamma = RL_environment.gamma
-        return {'gamma':gamma}
+        return {"gamma": gamma}
     elif env_name == "n_step_mountaincar":
         from seldonian.RL.environments.n_step_mountaincar import N_step_mountaincar
+
         RL_environment = N_step_mountaincar()
         gamma = RL_environment.gamma
-        return {'gamma':gamma}
+        return {"gamma": gamma}
     elif env_name == "simglucose":
-        return {} #needs updating 
+        return {}  # needs updating
     else:
         error(f"Unknown env_name {env_name}")
 
+
 def print_return_info(episodes):
-    """ Print the return, i.e., the sum of rewards. 
+    """Print the return, i.e., the sum of rewards.
     Used for debugging
 
     :param episodes: List of :py:class:`.Episode` objects.
     """
     the_sum = 0.0
     the_min = 0.0
     for episode in episodes:
@@ -95,9 +102,10 @@
         if the_return < the_min:
             the_min = the_return
         the_sum += the_return
         print(the_return)
     print(f"\navg return = {the_sum / len(episodes)}")
     print(f"lowest return =  {the_min}")
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     main()
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/RL_model.py` & `seldonian_engine-0.8.0/seldonian/RL/RL_model.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,61 +1,66 @@
 import autograd.numpy as np
 from seldonian.models.models import SeldonianModel
 
-class RL_model(SeldonianModel): #consist of agent, env
-	def __init__(self, policy, env_kwargs):
-		""" Base class for all RL models.
-
-		:param policy: A policy parameterization
-		:type policy: :py:class:`.Policy`
-
-		:param env_kwargs: Kwargs pertaining to environment
-			such as gamma, the discount factor 
-		:type env_kwargs: dict
-		"""
-
-		self.policy = policy
-		self.env_kwargs = env_kwargs
-		if 'gamma' not in self.env_kwargs:
-			self.env_kwargs['gamma'] = 1.0
-
-	def get_probs_from_observations_and_actions(self, new_params, observations, actions):
-		""" Get action probablities given a list of observations and actions 
-		taken given those observations
-		
-		:param new_params: Parameter weights to use
-		:param observations: Array of observations
-		:param actions: Array of actions
-
-		:return: Array of probabilities
-		"""
-		self.policy.set_new_params(new_params)
-		num_probs = len(observations)
-		if num_probs != len(actions):
-			error(f"different number of observations ({observations}) and actions ({actions})")
-
-		probs = list(map(self.policy.get_prob_this_action,
-                    observations,
-                    actions))
-		# If the policy uses a cache, make sure to clear it 
-		# This is necessary because cache is only correct 
-		# for a given set of param weights
-		try:
-			self.policy._denom.cache_clear()
-			self.policy._arg.cache_clear()
-		except:
-			pass
-
-		return np.array(probs)
-
-	def get_prob_this_action(self, observation, action):
-		""" Get action probability given a single observation, action
-		pair 
-		
-		:param observations: Array of observations
-		:param actions: Array of actions
-
-		:return: Probability of taking this action given observation
-		:rtype: float
-		"""
 
-		return self.policy.get_prob_this_action(observation, action)
+class RL_model(SeldonianModel):  # consist of agent, env
+    def __init__(self, policy, env_kwargs):
+        """Base class for all RL models.
+
+        :param policy: A policy parameterization
+        :type policy: :py:class:`.Policy`
+
+        :param env_kwargs: Kwargs pertaining to environment
+                such as gamma, the discount factor
+        :type env_kwargs: dict
+        """
+
+        self.policy = policy
+        self.env_kwargs = env_kwargs
+        if "gamma" not in self.env_kwargs:
+            self.env_kwargs["gamma"] = 1.0
+
+    def get_probs_from_observations_and_actions(
+        self, new_params, observations, actions, action_probs,
+    ):
+        """Get action probablities given a list of observations and actions
+        taken given those observations
+
+        :param new_params: Parameter weights to use
+        :param observations: Array of observations
+        :param actions: Array of actions
+        :param action_probs: Array of action probabilities from the behavior policy
+
+        :return: Array of probabilities
+        """
+        self.policy.set_new_params(new_params)
+        num_probs = len(observations)
+        if num_probs != len(actions):
+            error(
+                f"different number of observations ({observations}) and actions ({actions})"
+            )
+
+        probs = list(map(self.policy.get_prob_this_action, observations, actions, action_probs))
+        # If the policy uses a cache, make sure to clear it
+        # This is necessary because cache is only correct
+        # for a given set of param weights
+        try:
+            self.policy._denom.cache_clear()
+            self.policy._arg.cache_clear()
+        except:
+            pass
+
+        return np.array(probs)
+
+    def get_prob_this_action(self, observation, action, action_prob):
+        """Get action probability given a single observation, action
+        pair
+
+        :param observation: Observation on a single timestep
+        :param action: Action on a single timestep
+        :param action_prob: Action probability on a single timestep
+
+        :return: Probability of taking this action given observation
+        :rtype: float
+        """
+
+        return self.policy.get_prob_this_action(observation, action, action_prob)
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/RL_runner.py` & `seldonian_engine-0.8.0/seldonian/RL/RL_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,35 +9,38 @@
 from seldonian.RL.environments.simglucose_env import *
 
 from seldonian.dataset import Episode
 
 import multiprocessing as mp
 from concurrent.futures import ProcessPoolExecutor
 
+
 def run_all_trials(hyperparameter_and_setting_dict):
-    """ Run many trials, each of which consist
+    """Run many trials, each of which consist
     of the same number of episodes.
-    
+
     :param hyperparameter_and_setting_dict: Specifies the
         environment, agent, number of episodes per trial,
         and number of trials
     :type hyperparameter_and_setting_dict: dict
 
     :return: List((List of episodes, agent)_i) for i trials
     """
     num_trials = hyperparameter_and_setting_dict["num_trials"]
     trials = []
     for trial_num in range(num_trials):
         trials.append(run_trial(hyperparameter_and_setting_dict)[0])
     return trials
 
-def run_trial(hyperparameter_and_setting_dict,
-    model_params=None,parallel=False,n_workers=8):
-    """ Run a single trial consists of an arbitrary number of episodes.
-    
+
+def run_trial(
+    hyperparameter_and_setting_dict, model_params=None, parallel=False, n_workers=8
+):
+    """Run a single trial consists of an arbitrary number of episodes.
+
     :param hyperparameter_and_setting_dict: Specifies the
         environment, agent and number of episodes to run
     :type hyperparameter_and_setting_dict: dict
     :model_params: Policy parameters to set before running the trial
     :parallel: Whether to use parallel processing
     :n_workers: Number of cpus if using parallel processing
 
@@ -55,48 +58,52 @@
     env = hyperparameter_and_setting_dict["env"]
     if hyperparameter_and_setting_dict["vis"]:
         env.start_visualizing()
 
     if parallel:
         from concurrent.futures import ProcessPoolExecutor
         import multiprocessing as mp
+
         param1 = (hyperparameter_and_setting_dict for _ in range(num_episodes))
         param2 = (model_params for _ in range(num_episodes))
         # run_episode_from_dict(hyperparameter_and_setting_dict,model_params)
-        with ProcessPoolExecutor(max_workers=n_workers,
-            mp_context=mp.get_context('fork')) as ex:
-            results = ex.map(run_episode_from_dict,param1,param2)
+        with ProcessPoolExecutor(
+            max_workers=n_workers, mp_context=mp.get_context("fork")
+        ) as ex:
+            results = ex.map(run_episode_from_dict, param1, param2)
             for ep in results:
                 episodes.append(ep)
     else:
         for episode_num in range(num_episodes):
             episodes.append(run_episode(agent, env))
     return episodes, agent
 
-def run_trial_given_agent_and_env(agent,env,num_episodes):
-    """ A wrapper for run_trial() where parameters 
+
+def run_trial_given_agent_and_env(agent, env, num_episodes):
+    """A wrapper for run_trial() where parameters
     are specified explicity rather than via a dictionary.
 
-    :param agent: RL Agent 
+    :param agent: RL Agent
     :param env: RL Environment
     :param num_episodes: Number of episodes to run
 
     :return: List of episodes
     """
     episodes = []
 
     for episode_num in range(num_episodes):
         episodes.append(run_episode(agent, env))
     return episodes
 
+
 def run_episode(agent, env):
-    """ Run a single episode 
+    """Run a single episode
 
-    :param agent: RL Agent 
-    :param env: RL Environment 
+    :param agent: RL Agent
+    :param env: RL Environment
 
     :return: RL Episode
     :rtype: :py:class:`.Episode`
     """
     observations = []
     actions = []
     rewards = []
@@ -117,19 +124,20 @@
         rewards.append(reward)
         prob_actions.append(agent.get_prob_this_action(observation, action))
 
         observation = next_observation
 
     return Episode(observations, actions, rewards, prob_actions)
 
-def run_episode_from_dict(hyperparameter_and_setting_dict,model_params=None):
-    """ Run a single episode 
 
-    :param agent: RL Agent 
-    :param env: RL Environment 
+def run_episode_from_dict(hyperparameter_and_setting_dict, model_params=None):
+    """Run a single episode
+
+    :param agent: RL Agent
+    :param env: RL Environment
 
     :return: RL Episode
     :rtype: :py:class:`.Episode`
     """
     env = hyperparameter_and_setting_dict["env"]
     env_desc = env.get_env_description()
     agent = create_agent(hyperparameter_and_setting_dict)
@@ -157,17 +165,18 @@
         rewards.append(reward)
         prob_actions.append(agent.get_prob_this_action(observation, action))
 
         observation = next_observation
 
     return Episode(observations, actions, rewards, prob_actions)
 
+
 def create_agent(hyperparameter_and_setting_dict):
-    """ Create an agent from a dictionary specification
-    
+    """Create an agent from a dictionary specification
+
     :param hyperparameter_and_setting_dict: Specifies the
         environment, agent, number of episodes per trial,
         and number of trials
 
     :return: RL agent
     :rtype: :py:class:`.Agents.Agent`
     """
@@ -175,12 +184,14 @@
     env_desc = env.get_env_description()
     agent_type = hyperparameter_and_setting_dict["agent"]
     if agent_type == "discrete_random":
         return Discrete_Random_Agent(env_desc)
     elif agent_type == "mountain_car_rough_solution":
         return Mountain_car_rough_solution()
     elif agent_type == "Parameterized_non_learning_softmax_agent":
-        return Parameterized_non_learning_softmax_agent(env_desc, hyperparameter_and_setting_dict)
+        return Parameterized_non_learning_softmax_agent(
+            env_desc, hyperparameter_and_setting_dict
+        )
     elif agent_type == "Keyboard_gridworld":
         return Keyboard_gridworld(env_desc)
     else:
         raise Exception(f"unknown agent type {agent_type}")
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/environments/Environment.py` & `seldonian_engine-0.8.0/seldonian/RL/environments/Environment.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 class Environment:
-    """ Base class for all RL environments """
+    """Base class for all RL environments"""
+
     def get_observation(self):
-        """ Get current observation. 
+        """Get current observation.
         Override this method in child class implementation
         """
         raise NotImplementedError()
 
     def transition(self, action):
-        """ Transition to a new observation given an action 
+        """Transition to a new observation given an action
 
-        :param action: A possible action in the environment 
+        :param action: A possible action in the environment
         Override this method in child class implementation
         """
         raise NotImplementedError()
 
     def reset(self):
-        """ Reset observation to initial observation 
+        """Reset observation to initial observation
         Override this method in child class implementation
         """
         raise NotImplementedError()
 
     def get_env_description(self):
-        """ Get environment description 
+        """Get environment description
         Override this method in child class implementation
         """
         return self.env_description
 
     def terminated(self):
-        """ Get the terminal obs
-        """
+        """Get the terminal obs"""
         return self.terminal_state
 
     def visualize(self):
-        """ Print out current observation, useful for debugging 
+        """Print out current observation, useful for debugging
         Override this method in child class implementation
         """
         raise NotImplementedError()
 
     def start_visualizing(self):
-        """ Turn on visualization debugger 
-        """
+        """Turn on visualization debugger"""
         self.vis = True
 
     def stop_visualizing(self):
-        """ Turn off visualization debugger 
-        """
-        self.vis = False
+        """Turn off visualization debugger"""
+        self.vis = False
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/environments/gridworld.py` & `seldonian_engine-0.8.0/seldonian/RL/environments/gridworld.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from seldonian.RL.environments.Environment import *
 from seldonian.RL.Env_Description.Env_Description import *
 
+
 class Gridworld(Environment):
     def __init__(self, size=3):
-        """ Square gridworld RL environment of arbitrary size.
-        
-        :param size: The number of grid cells on a side 
+        """Square gridworld RL environment of arbitrary size.
+
+        :param size: The number of grid cells on a side
         :ivar num_states: The number of distinct grid cells
         :ivar env_description: contains attributes describing the environment
         :vartype env_description: :py:class:`.Env_Description`
         :ivar obs: The current obs
         :vartype obs: int
         :ivar terminal_state: Whether the terminal obs is occupied
         :vartype terminal_state: bool
@@ -17,44 +18,44 @@
         :vartype time: int
         :ivar max_time: Maximum allowed timestep
         :vartype max_time: int
         :ivar gamma: The discount factor in calculating the expected return
         :vartype gamma: float
         """
         self.size = size
-        self.num_states = size*size
+        self.num_states = size * size
         self.env_description = self.create_env_description(self.num_states)
         self.state = 0
         self.terminal_state = False
         self.time = 0
         self.max_time = 101
         # vis is a flag for visual debugging during obs transitions
         self.vis = False
         self.gamma = 0.9
 
     def create_env_description(self, num_states):
-        """ Creates the environment description object.  
+        """Creates the environment description object.
 
         :param num_states: The number of states
         :return: Environment description for the obs and action spaces
         :rtype: :py:class:`.Env_Description`
         """
-        observation_space = Discrete_Space(0, num_states-1)
+        observation_space = Discrete_Space(0, num_states - 1)
         action_space = Discrete_Space(0, 3)
         return Env_Description(observation_space, action_space)
 
     def reset(self):
-        """ Go back to initial obs and timestep """
+        """Go back to initial obs and timestep"""
         self.state = 0
         self.time = 0
         self.terminal_state = False
 
     def transition(self, action):
-        """ Transition between states given an action, return a reward. 
-        
+        """Transition between states given an action, return a reward.
+
         :param action: A possible action at the current obs
         :return: reward for reaching the next obs
         """
         reward = 0
         self.time += 1
         self.update_position(action)
 
@@ -66,48 +67,47 @@
             reward = -1
         if self.vis:
             self.visualize()
             print("reward", reward)
         return reward
 
     def get_observation(self):
-        """ Get the current obs """
+        """Get the current obs"""
         return self.state
 
     def update_position(self, action):
-        """ Helper function for transition() that updates the 
-        current position given an action 
+        """Helper function for transition() that updates the
+        current position given an action
 
         :param action: A possible action at the current obs
         """
-        if action == 0: #up
-            if self.state >= self.size: #if not on top row
+        if action == 0:  # up
+            if self.state >= self.size:  # if not on top row
                 self.state -= self.size
-        elif action == 1: #right
-            if (self.state + 1) % self.size != 0: #not on right column
+        elif action == 1:  # right
+            if (self.state + 1) % self.size != 0:  # not on right column
                 self.state += 1
-        elif action == 2: #down
-            if self.state < self.num_states - self.size: #not on bottom row
+        elif action == 2:  # down
+            if self.state < self.num_states - self.size:  # not on bottom row
                 self.state += self.size
-        elif action == 3: #left
-            if self.state % self.size != 0: #not on left column
+        elif action == 3:  # left
+            if self.state % self.size != 0:  # not on left column
                 self.state -= 1
         else:
             raise Exception(f"invalid gridworld action {action}")
 
     def is_in_goal_state(self):
-        """ Check whether current obs is goal obs
+        """Check whether current obs is goal obs
 
         :return: True if obs is in goal obs, False if not
         """
         return self.state == self.num_states - 1
 
     def visualize(self):
-        """ Print out current obs information
-        """
+        """Print out current obs information"""
         print_state = 0
         for y in range(self.size):
             for x in range(self.size):
                 if print_state == self.state:
                     print("A", end="")
                 else:
                     print("X", end="")
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/environments/mountaincar.py` & `seldonian_engine-0.8.0/seldonian/RL/environments/mountaincar.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from seldonian.RL.environments.Environment import *
 from seldonian.RL.Env_Description.Env_Description import *
 from math import cos
 from seldonian.utils.RL_utils import *
 
+
 class Mountaincar(Environment):
     def __init__(self):
         self.env_description = self.create_env_description()
         self.terminal_state = False
         self.time = 0
-        self.position = -.5
+        self.position = -0.5
         self.velocity = 0.0
         self.max_time = 1000
         self.vis = False
         self.reset()
 
     def create_env_description(self):
-        state_space_bounds = np.array([[-1.2, 0.5], [-.07, .07]])
+        state_space_bounds = np.array([[-1.2, 0.5], [-0.07, 0.07]])
         state_space = Continuous_Space(state_space_bounds)
         action_space = Discrete_Space(-1, 1)
         return Env_Description(state_space, action_space)
 
     def reset(self):
-        self.position = -.5
+        self.position = -0.5
         self.velocity = 0.0
         self.time = 0
         self.terminal_state = False
 
     def transition(self, action):
         self.check_valid_mc_action(action)
         self.time += 1
@@ -35,16 +36,20 @@
 
         reward = -1.0
         if self.terminal_state:
             reward = 0.0
         return reward
 
     def update_velocity(self, action):
-        self.velocity += .001 * action - .0025 * cos(3.0 * self.position)
-        self.velocity = clamp(self.velocity, self.env_description.observation_space.bounds[1][0], self.env_description.observation_space.bounds[1][1])
+        self.velocity += 0.001 * action - 0.0025 * cos(3.0 * self.position)
+        self.velocity = clamp(
+            self.velocity,
+            self.env_description.observation_space.bounds[1][0],
+            self.env_description.observation_space.bounds[1][1],
+        )
 
     def position_and_termination_update(self):
         self.position += self.velocity
         pos_lower_bound = self.env_description.observation_space.bounds[0][0]
         pos_upper_bound = self.env_description.observation_space.bounds[0][1]
         if self.position <= pos_lower_bound:
             self.position = pos_lower_bound
@@ -55,11 +60,11 @@
             self.terminal_state = True
 
     def visualize(self):
         error("mountain car visualize method not implemented")
 
     def check_valid_mc_action(self, action):
         if action != -1 and action != 0 and action != 1:
-            raise(Exception(f"invalid action {action}"))
+            raise (Exception(f"invalid action {action}"))
 
     def get_observation(self):
         return np.array([self.position, self.velocity])
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/environments/n_step_mountaincar.py` & `seldonian_engine-0.8.0/seldonian/RL/environments/n_step_mountaincar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from seldonian.RL.environments.Environment import *
 from seldonian.RL.Env_Description.Env_Description import *
 from seldonian.RL.environments.mountaincar import *
 
+
 class N_step_mountaincar(Environment):
     def __init__(self):
         self.n_steps = 20
         self.mc_env = Mountaincar()
         self.env_description = self.mc_env.create_env_description()
         self.terminal_state = False
         self.vis = False
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/environments/simglucose_env.py` & `seldonian_engine-0.8.0/seldonian/RL/environments/simglucose_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 # WARNING: naming this file "simglucose" causes some very confusing and misleading gym errors (ultimately caused by a silent conflict between that file name and the simglucose package)
 try:
     import gym
     from gym.envs.registration import register
 except ImportError:
-    print("\nWARNING: The module 'gym' was not imported. "
+    print(
+        "\nWARNING: The module 'gym' was not imported. "
         "If you want to use the diabetes simulator, then do:\n"
-        "pip install gym\n")
+        "pip install gym\n"
+    )
 from seldonian.RL.environments.Environment import *
 from seldonian.RL.Env_Description.Env_Description import *
+
 try:
     import simglucose
 except ImportError:
-    print("\nWARNING: The module 'simglucose' was not imported. "
+    print(
+        "\nWARNING: The module 'simglucose' was not imported. "
         "If you want to use the diabetes simulator, then do:\n"
-        "pip install simglucose\n")
+        "pip install simglucose\n"
+    )
+
 
 class Simglucose(Environment):
     def __init__(self):
         self.num_actions = 5  # how many actions to discretize
-        self.id = 'simglucose-adolescent2-v0'
-        self.patient_name = 'adolescent#002'
+        self.id = "simglucose-adolescent2-v0"
+        self.patient_name = "adolescent#002"
 
         self.deregister_and_register()
-        self.action_multiplier = 30. / (self.num_actions - 1)
+        self.action_multiplier = 30.0 / (self.num_actions - 1)
         self.gym_env = gym.make(self.id)
         self.env_description = self.create_env_description()
         self.terminal_state = False
         self.observation = None
-        self.reset() #updates self.observation
+        self.reset()  # updates self.observation
 
     def reset(self):
         self.observation = self.gym_observation_to_observation(self.gym_env.reset())
         self.terminal_state = False
 
     def transition(self, action):
         environment_action = action * self.action_multiplier
-        observation, reward, self.terminal_state, info = self.gym_env.step(environment_action)
+        observation, reward, self.terminal_state, info = self.gym_env.step(
+            environment_action
+        )
         self.observation = self.gym_observation_to_observation(observation)
         return reward
 
     def get_observation(self):
         return self.observation
 
     def gym_observation_to_observation(self, gym_obs):
-        return np.array([gym_obs[0]]) #get the scalar out of the simglucose Observation object, then put it in a numpy array
+        return np.array(
+            [gym_obs[0]]
+        )  # get the scalar out of the simglucose Observation object, then put it in a numpy array
 
     def create_env_description(self):
-        fake_max = 300.0 #in gym it's technically infinity
+        fake_max = 300.0  # in gym it's technically infinity
         obs_space_bounds = np.array([[0, fake_max]])
         obs_space = Continuous_Space(obs_space_bounds)
-        action_space = Discrete_Space(0, self.num_actions-1)
+        action_space = Discrete_Space(0, self.num_actions - 1)
         return Env_Description(obs_space, action_space)
 
     def deregister_and_register(self):
         self.deregister()
         register(
             id=self.id,
-            entry_point='simglucose.envs:T1DSimEnv',
-            kwargs={'patient_name': self.patient_name}
+            entry_point="simglucose.envs:T1DSimEnv",
+            kwargs={"patient_name": self.patient_name},
         )
 
     def deregister(self):
         env_dict = gym.envs.registration.registry.env_specs.copy()
         for env in env_dict:
             if self.id in env:
-                del gym.envs.registration.registry.env_specs[env]
+                del gym.envs.registration.registry.env_specs[env]
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/generate_gridworld_episodes.py` & `seldonian_engine-0.8.0/seldonian/RL/generate_gridworld_episodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 from seldonian.RL.RL_runner import run_trial
 from seldonian.utils.RL_utils import *
 from seldonian.utils.io_utils import save_pickle
 from seldonian.utils.stats_utils import weighted_sum_gamma
 from seldonian.spec import createRLSpec
 from seldonian.RL.environments.gridworld import Gridworld
 
+
 def main():
-    """ Run a trial of episodes and save to disk
-    """  
+    """Run a trial of episodes and save to disk"""
     n_episodes = 1000
     the_dict = {}
     the_dict["env"] = Gridworld()
     the_dict["agent"] = "Parameterized_non_learning_softmax_agent"
     the_dict["num_episodes"] = n_episodes
     the_dict["vis"] = False
     start_time = time()
-    episodes, agent = run_trial(the_dict,parallel=False)
+    episodes, agent = run_trial(the_dict, parallel=False)
     print(len(episodes))
-    save_pickle(f"gridworld_{n_episodes}episodes.pkl",episodes,verbose=True)
+    save_pickle(f"gridworld_{n_episodes}episodes.pkl", episodes, verbose=True)
     assert len(episodes) == n_episodes
     print(f"data generation took {time() - start_time} seconds")
-    
+
     # # Calculate J, the discounted sum of rewards
-    returns = np.array([weighted_sum_gamma(ep.rewards,gamma=0.9) for ep in episodes])
+    returns = np.array([weighted_sum_gamma(ep.rewards, gamma=0.9) for ep in episodes])
     J = np.mean(returns)
     print(f"J = {J}")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/generate_mountaincar_episodes.py` & `seldonian_engine-0.8.0/seldonian/RL/generate_mountaincar_episodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,34 +3,34 @@
 from seldonian.RL.hyperparams_and_settings import *
 from seldonian.RL.RL_runner import run_trial
 from seldonian.utils.RL_utils import *
 from seldonian.utils.io_utils import save_pickle
 from seldonian.utils.stats_utils import weighted_sum_gamma
 from seldonian.spec import createRLSpec
 
+
 def main():
-    """ Run a trial of episodes and save to disk
-    """  
+    """Run a trial of episodes and save to disk"""
     n_episodes = 500
     the_dict = {}
     the_dict["env"] = "n_step_mountaincar"
     the_dict["agent"] = "Parameterized_non_learning_softmax_agent"
     the_dict["basis"] = "Fourier"
     the_dict["order"] = 2
     the_dict["max_coupled_vars"] = -1
     the_dict["num_episodes"] = n_episodes
     the_dict["vis"] = False
     start_time = time()
-    episodes, agent = run_trial(the_dict,parallel=True)
+    episodes, agent = run_trial(the_dict, parallel=True)
     print(len(episodes))
-    save_pickle(f"n_step_mountaincar_{n_episodes}episodes.pkl",episodes)
+    save_pickle(f"n_step_mountaincar_{n_episodes}episodes.pkl", episodes)
     assert len(episodes) == n_episodes
     print(f"data generation took {time() - start_time} seconds")
-    
+
     # Calculate J, the discounted sum of rewards
-    returns = np.array([weighted_sum_gamma(ep.rewards,gamma=1.0) for ep in episodes])
+    returns = np.array([weighted_sum_gamma(ep.rewards, gamma=1.0) for ep in episodes])
     J = np.mean(returns)
     print(f"J = {J}")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/generate_simglucose_episodes.py` & `seldonian_engine-0.8.0/seldonian/RL/generate_simglucose_episodes.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,41 +3,40 @@
 from seldonian.RL.hyperparams_and_settings import *
 from seldonian.RL.RL_runner import run_trial
 from seldonian.utils.RL_utils import *
 from seldonian.utils.io_utils import save_pickle
 from seldonian.utils.stats_utils import weighted_sum_gamma
 from seldonian.spec import createRLSpec
 
+
 def get_max_obs(episodes):
     max_obs = 0
-    for ii,ep in enumerate(episodes):
+    for ii, ep in enumerate(episodes):
         max_obs_this_ep = np.max(ep.observations)
-        max_obs = max(max_obs,max_obs_this_ep)
+        max_obs = max(max_obs, max_obs_this_ep)
     return max_obs
 
 
-
 def main():
-    """ Run a trial of episodes and save to disk
-    """  
+    """Run a trial of episodes and save to disk"""
     n_episodes = 500
     the_dict = {}
     the_dict["env"] = "simglucose"
     the_dict["agent"] = "discrete_random"
     the_dict["num_episodes"] = n_episodes
     the_dict["vis"] = True
     start_time = time()
-    episodes, agent = run_trial(the_dict,parallel=True)
-    save_pickle(f"simglucose_{n_episodes}episodes.pkl",episodes)
+    episodes, agent = run_trial(the_dict, parallel=True)
+    save_pickle(f"simglucose_{n_episodes}episodes.pkl", episodes)
     print(f"data generation took {time() - start_time} seconds")
 
     max_obs = get_max_obs(episodes)
     print(f"Max observation over {n_episodes} episodes={max_obs}")
-    
+
     # Calculate J, the discounted sum of rewards
-    returns = np.array([weighted_sum_gamma(ep.rewards,gamma=1.0) for ep in episodes])
+    returns = np.array([weighted_sum_gamma(ep.rewards, gamma=1.0) for ep in episodes])
     J = np.mean(returns)
     print(f"J = {J}")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `seldonian_engine-0.7.9/seldonian/RL/hyperparams_and_settings.py` & `seldonian_engine-0.8.0/seldonian/RL/hyperparams_and_settings.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/seldonian/RL/profiling_seldonian_RL.py` & `seldonian_engine-0.8.0/seldonian/RL/profiling_seldonian_RL.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,30 +20,31 @@
 from seldonian.models.models import *
 from seldonian.RL.Agents import *
 from seldonian.RL.environments import *
 from seldonian.RL.RL_model import *
 
 
 def main():
-
     hyperparameter_and_setting_dict = define_hyperparameter_and_setting_dict()
     start_time = time()
     episodes, agent = run_trial(hyperparameter_and_setting_dict)
     print(f"data generation took {time() - start_time} seconds")
 
     hyperparameter_and_setting_dict["num_episodes"] = 1
-    dataset = RLDataSet(episodes=episodes,meta_information=['O','A','R','pi'])
+    dataset = RLDataSet(episodes=episodes, meta_information=["O", "A", "R", "pi"])
 
     # print(dataset.episodes[0])
     # print(f"{len(episodes)} episodes")
     metadata_pth = get_metadata_path(hyperparameter_and_setting_dict["env"])
-    save_dir = '.'
+    save_dir = "."
     constraint_string = get_constraint_string(hyperparameter_and_setting_dict["env"])
-    RL_model = fake_dataset2spec(save_dir, metadata_pth, dataset, agent, constraint_string)
-    data_dict = {"episodes" : episodes}
+    RL_model = fake_dataset2spec(
+        save_dir, metadata_pth, dataset, agent, constraint_string
+    )
+    data_dict = {"episodes": episodes}
     start_time_is_estimates = time()
     for _ in range(100000):
         mock_vector_IS_estimate(agent.get_params(), data_dict, RL_model)
     print(f"IS estimates took {time() - start_time_is_estimates}")
     print(f"whole thing took {time() - start_time}")
 
 
@@ -51,61 +52,66 @@
     if env_name == "gridworld":
         return "../../static/datasets/RL/gridworld/gridworld_metadata.json"
     elif env_name == "n_step_mountaincar":
         return "../../static/datasets/RL/mountaincar/n_step_mountaincar_metadata.json"
     else:
         error(f"unknown env name {env_name}")
 
+
 def get_constraint_string(env):
     if env == "gridworld":
-        return ['-0.25 - J_pi_new']
+        return ["-0.25 - J_pi_new"]
     else:
         error(f"Unknown env {env}")
 
+
 def fake_dataset2spec(save_dir, metadata_pth, dataset, agent, constraint_strs):
     # Load metadata
-    with open(metadata_pth, 'r') as infile:
+    with open(metadata_pth, "r") as infile:
         metadata_dict = json.load(infile)
 
-    RL_module_name = metadata_dict['RL_module_name']
+    RL_module_name = metadata_dict["RL_module_name"]
     RL_environment_module = importlib.import_module(
-        f'seldonian.RL.environments.{RL_module_name}')
-    RL_env_class_name = metadata_dict['RL_class_name']
+        f"seldonian.RL.environments.{RL_module_name}"
+    )
+    RL_env_class_name = metadata_dict["RL_class_name"]
     RL_environment_obj = getattr(RL_environment_module, RL_env_class_name)()
 
-    RL_model_instance = RL_model(agent,RL_environment_obj)
+    RL_model_instance = RL_model(agent, RL_environment_obj)
     primary_objective = RL_model_instance.sample_IS_estimate
     return RL_model_instance
 
 
 def mock_vector_IS_estimate(theta, data_dict, rl_model):
-    """ Calculate the unweighted importance sampling estimate
+    """Calculate the unweighted importance sampling estimate
     on each episodes in the dataframe
 
     :param theta: The parameter weights
     :type theta: numpy ndarray
 
     :param dataframe: Contains the episodes
     :type dataframe: pandas dataframe
 
     :return: A vector of IS estimates calculated for each episode
     :rtype: numpy ndarray(float)
     """
-    episodes = data_dict['episodes']
+    episodes = data_dict["episodes"]
     # weighted_reward_sums_by_episode = data_dict['reward_sums_by_episode']
     ep = episodes[0]
 
-    #start loop in real function
-    pi_news = rl_model.get_probs_from_observations_and_actions(theta, ep.observations, ep.actions)
+    # start loop in real function
+    pi_news = rl_model.get_probs_from_observations_and_actions(
+        theta, ep.observations, ep.actions
+    )
     # print("pi news:")
     # print(pi_news)
     pi_ratio_prod = np.prod(pi_news / ep.pis)
     # print("pi_ratio_prod:")
     # print(pi_ratio_prod)
     weighted_return = weighted_sum_gamma(ep.rewards, gamma=0.9)
     # result.append(pi_ratio_prod*weighted_reward_sums_by_episode[ii])
     return pi_ratio_prod * weighted_return
     # end loop in real function
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `seldonian_engine-0.7.9/seldonian/hyperparam_search.py` & `seldonian_engine-0.8.0/seldonian/hyperparam_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,419 +1,472 @@
 """ Wrapper module for hyperparameter selection for Seldonian algorithms """
 
 from sklearn.model_selection import train_test_split
 import autograd.numpy as np
 
 import warnings
-from seldonian.dataset import (SupervisedDataSet, RLDataSet)
+from seldonian.dataset import SupervisedDataSet, RLDataSet
 from seldonian.candidate_selection.candidate_selection import CandidateSelection
 from seldonian.safety_test.safety_test import SafetyTest
 from seldonian.models import objectives
 
 
-class HyperparamSearch():
+class HyperparamSearch:
     def __init__(self, spec, all_frac_data_in_candidate_selection):
-        """ Object for finding the best hyperparameters to use to optimize for probability
+        """Object for finding the best hyperparameters to use to optimize for probability
         of returning a safe solution for Seldonian algorithms. Note: currently only used to
         find optimal data split.
 
         List of hyperparameters to optimize:
         - Percentage of data in candidate and safety datasets
 
         :param spec: The specification object with the complete
                 set of parameters for running the Seldonian algorithm
         :type spec: :py:class:`.Spec` object
-        :param all_frac_data_in_candidate_selection: Array containing the values of fraction of data in 
+        :param all_frac_data_in_candidate_selection: Array containing the values of fraction of data in
                 candidate solution that are being considered
         :type all_frac_data_in_candidate_selection: numpy.ndarray
         """
         self.spec = spec
-        self.all_frac_data_in_candidate_selection = all_frac_data_in_candidate_selection 
+        self.all_frac_data_in_candidate_selection = all_frac_data_in_candidate_selection
 
         self.parse_trees = self.spec.parse_trees
-        # user can pass a dictionary that specifies 
+        # user can pass a dictionary that specifies
         # the bounding method for each base node
         # any base nodes not in this dictionary will
         # be bounded using the default method
         self.base_node_bound_method_dict = self.spec.base_node_bound_method_dict
         if self.base_node_bound_method_dict != {}:
-                all_pt_constraint_strs = [pt.constraint_str for pt in self.parse_trees]
-                for constraint_str in self.base_node_bound_method_dict:
-                        this_bound_method_dict = self.base_node_bound_method_dict[constraint_str]
-                        # figure out which parse tree this comes from
-                        this_pt_index = all_pt_constraint_strs.index(constraint_str)
-                        this_pt = self.parse_trees[this_pt_index]
-                        # change the bound method for each node provided
-                        for node_name in this_bound_method_dict:
-                                this_pt.base_node_dict[node_name]['bound_method'] = this_bound_method_dict[node_name]
+            all_pt_constraint_strs = [pt.constraint_str for pt in self.parse_trees]
+            for constraint_str in self.base_node_bound_method_dict:
+                this_bound_method_dict = self.base_node_bound_method_dict[
+                    constraint_str
+                ]
+                # figure out which parse tree this comes from
+                this_pt_index = all_pt_constraint_strs.index(constraint_str)
+                this_pt = self.parse_trees[this_pt_index]
+                # change the bound method for each node provided
+                for node_name in this_bound_method_dict:
+                    this_pt.base_node_dict[node_name][
+                        "bound_method"
+                    ] = this_bound_method_dict[node_name]
 
         self.dataset = self.spec.dataset
         self.regime = self.dataset.regime
         self.column_names = self.dataset.meta_information
 
         if self.spec.primary_objective is None:
-                if self.regime == 'reinforcement_learning':
-                        self.spec.primary_objective = objectives.IS_estimate
-                elif self.regime == 'supervised_learning':
-                        if self.spec.sub_regime == 'classification':
-                                self.spec.primary_objective = objectives.logistic_loss
-                        elif self.spec.sub_regime == 'regression':
-                                self.spec.primary_objective = objectives.Mean_Squared_Error
-
+            if self.regime == "reinforcement_learning":
+                self.spec.primary_objective = objectives.IS_estimate
+            elif self.regime == "supervised_learning":
+                if self.spec.sub_regime == "classification":
+                    self.spec.primary_objective = objectives.logistic_loss
+                elif self.spec.sub_regime == "regression":
+                    self.spec.primary_objective = objectives.Mean_Squared_Error
 
     def get_safety_size(self, n_total, frac_data_in_safety):
-        """ Determine the number of data points in the safety dataset.
+        """Determine the number of data points in the safety dataset.
 
         :param n_total: the total amount of data
         :type n_total: int
-        :param frac_data_in_safety: fraction of data used in safety test, 
+        :param frac_data_in_safety: fraction of data used in safety test,
                 the remaining fraction will be used in candidate selection
         :type frac_data_in_safety: float
         """
         n_safety = int(frac_data_in_safety * n_total)
-        n_safety = max(n_safety, 2) # >=2 point in safety
-        n_safety = min(n_safety, n_total-2) # >=1 point in selection
+        n_safety = max(n_safety, 2)  # >=2 point in safety
+        n_safety = min(n_safety, n_total - 2)  # >=1 point in selection
 
         return n_safety
 
-
     def create_dataset(self, dataset, frac_data_in_safety, shuffle=False):
-        """ Partition data to create candidate and safety dataset according to frac_data_in_safety
+        """Partition data to create candidate and safety dataset according to frac_data_in_safety
 
         :param dataset: a dataset object containing data
         :type dataset: :py:class:`.DataSet` object
-        :param frac_data_in_safety: fraction of data used in safety test, 
+        :param frac_data_in_safety: fraction of data used in safety test,
                 the remaining fraction will be used in candidate selection
         :type frac_data_in_safety: float
         """
-        if self.regime == 'supervised_learning':
-                n_total = len(dataset.df)
-                if n_total < 4:
-                        warning_msg = (
-                                "Warning: not enough data to "
-                                "run the Seldonian algorithm.")
-                        warnings.warn(warning_msg)
-
-                # Make sure at least two datapoints in safety and candidate.
-                n_safety_split = self.get_safety_size(n_total, frac_data_in_safety)
-
-                # Split the data.
-                candidate_df, safety_df = train_test_split(
-                        dataset.df, test_size=n_safety_split,
-                        shuffle=shuffle)
-
-                # Create candidate and safety datasets
-                candidate_dataset = SupervisedDataSet(
-                        candidate_df,meta_information=self.column_names,
-                        sensitive_column_names=dataset.sensitive_column_names,
-                        include_sensitive_columns=dataset.include_sensitive_columns,
-                        include_intercept_term=dataset.include_intercept_term,
-                        label_column=dataset.label_column)
-
-                safety_dataset = SupervisedDataSet(
-                        safety_df,meta_information=self.column_names,
-                        sensitive_column_names=dataset.sensitive_column_names,
-                        include_sensitive_columns=dataset.include_sensitive_columns,
-                        include_intercept_term=dataset.include_intercept_term,
-                        label_column=dataset.label_column)
-                
-                n_candidate = len(candidate_df)
-                n_safety = len(safety_df)
-                if n_candidate < 2 or n_safety < 2:
-                        warning_msg = (
-                                "Warning: not enough data to "
-                                "run the Seldonian algorithm.")
-                        warnings.warn(warning_msg)
-                        print(n_candidate)
-                        print(n_safety)
-
-
-        elif self.regime == 'reinforcement_learning':
-                self.env_kwargs = self.spec.model.env_kwargs
-
-                episodes = dataset.episodes
-                # Create candidate and safety datasets
-                n_episodes = len(episodes)
-
-                # Make sure at least two datapoints in safety and candidate.
-                n_safety = self.get_safety_size(n_episodes, n_episodes)
-                n_candidate = n_episodes - n_safety
-
-                candidate_episodes = episodes[0:n_candidate]
-                safety_episodes = episodes[n_candidate:]
-
-                candidate_dataset = RLDataSet(
-                        episodes=candidate_episodes,
-                        meta_information=self.column_names)
-
-                safety_dataset = RLDataSet(
-                        episodes=safety_episodes,
-                        meta_information=self.column_names)
+        if self.regime == "supervised_learning":
+            n_total = len(dataset.df)
+            if n_total < 4:
+                warning_msg = (
+                    "Warning: not enough data to " "run the Seldonian algorithm."
+                )
+                warnings.warn(warning_msg)
+
+            # Make sure at least two datapoints in safety and candidate.
+            n_safety_split = self.get_safety_size(n_total, frac_data_in_safety)
+
+            # Split the data.
+            candidate_df, safety_df = train_test_split(
+                dataset.df, test_size=n_safety_split, shuffle=shuffle
+            )
+
+            # Create candidate and safety datasets
+            candidate_dataset = SupervisedDataSet(
+                candidate_df,
+                meta_information=self.column_names,
+                sensitive_column_names=dataset.sensitive_column_names,
+                include_sensitive_columns=dataset.include_sensitive_columns,
+                include_intercept_term=dataset.include_intercept_term,
+                label_column=dataset.label_column,
+            )
+
+            safety_dataset = SupervisedDataSet(
+                safety_df,
+                meta_information=self.column_names,
+                sensitive_column_names=dataset.sensitive_column_names,
+                include_sensitive_columns=dataset.include_sensitive_columns,
+                include_intercept_term=dataset.include_intercept_term,
+                label_column=dataset.label_column,
+            )
+
+            n_candidate = len(candidate_df)
+            n_safety = len(safety_df)
+            if n_candidate < 2 or n_safety < 2:
+                warning_msg = (
+                    "Warning: not enough data to " "run the Seldonian algorithm."
+                )
+                warnings.warn(warning_msg)
+                print(n_candidate)
+                print(n_safety)
+
+        elif self.regime == "reinforcement_learning":
+            self.env_kwargs = self.spec.model.env_kwargs
+
+            episodes = dataset.episodes
+            # Create candidate and safety datasets
+            n_episodes = len(episodes)
+
+            # Make sure at least two datapoints in safety and candidate.
+            n_safety = self.get_safety_size(n_episodes, n_episodes)
+            n_candidate = n_episodes - n_safety
+
+            candidate_episodes = episodes[0:n_candidate]
+            safety_episodes = episodes[n_candidate:]
+
+            candidate_dataset = RLDataSet(
+                episodes=candidate_episodes, meta_information=self.column_names
+            )
+
+            safety_dataset = RLDataSet(
+                episodes=safety_episodes, meta_information=self.column_names
+            )
 
-                print(f"Safety dataset has {n_safety} episodes")
-                print(f"Candidate dataset has {n_candidate} episodes")
+            print(f"Safety dataset has {n_safety} episodes")
+            print(f"Candidate dataset has {n_candidate} episodes")
 
         return candidate_dataset, safety_dataset, n_candidate, n_safety
 
-
     def bootstrap_sample_dataset(self, dataset, n_bootstrap):
-        """ Bootstrap sample a dataset of size n_bootstrap from data points in dataset.
+        """Bootstrap sample a dataset of size n_bootstrap from data points in dataset.
 
         :param dataset: a dataset object containing data
         :type dataset: :py:class:`.DataSet` object
         :param n_bootstrap: the desired number of points in the bootstrapped dataset.
         :type n_bootstrap: int
         """
 
-        if self.regime == 'supervised_learning':
+        if self.regime == "supervised_learning":
             bs_df = dataset.df.sample(n=n_bootstrap, replace=True)
             bs_dataset = SupervisedDataSet(
-                    bs_df,meta_information=self.column_names,
-                    sensitive_column_names=dataset.sensitive_column_names,
-                    include_sensitive_columns=dataset.include_sensitive_columns,
-                    include_intercept_term=dataset.include_intercept_term,
-                    label_column=dataset.label_column)
+                bs_df,
+                meta_information=self.column_names,
+                sensitive_column_names=dataset.sensitive_column_names,
+                include_sensitive_columns=dataset.include_sensitive_columns,
+                include_intercept_term=dataset.include_intercept_term,
+                label_column=dataset.label_column,
+            )
 
-        elif self.regime == 'reinforcement_learning':
+        elif self.regime == "reinforcement_learning":
             bs_episodes = np.random.choice(dataset.episodes, n_bootstrap)
             bs_dataset = RLDataSet(
-                    episodes=bs_episodes,
-                    meta_information=self.column_names)
+                episodes=bs_episodes, meta_information=self.column_names
+            )
 
         return bs_dataset
-                
 
     def get_initial_solution(self, candidate_dataset, frac_data_in_safety):
-        """ Get the initial solution used in candidate selection.
+        """Get the initial solution used in candidate selection.
 
-        :param candidate_dataset: a dataset object containing data that should be used to   
+        :param candidate_dataset: a dataset object containing data that should be used to
                 to find the initial soluion.
         :type candidate_dataset: :py:class:`.DataSet` object
         :param frac_data_in_safety: fraction of data used in safety test.
                 The remaining fraction will be used in candidate selection
         :type frac_data_in_safety: float
         """
-        if self.regime == 'supervised_learning':
-                candidate_df = candidate_dataset.df
-
-                # Set up initial solution
-                initial_solution_fn = self.spec.initial_solution_fn
+        if self.regime == "supervised_learning":
+            candidate_df = candidate_dataset.df
 
-                candidate_labels = candidate_df[candidate_dataset.label_column]
-                candidate_features = candidate_df.loc[:,
-                        candidate_df.columns != candidate_dataset.label_column]
-
-                if not candidate_dataset.include_sensitive_columns:
-                        candidate_features = candidate_features.drop(
-                                columns=candidate_dataset.sensitive_column_names)
-        
-                if candidate_dataset.include_intercept_term:
-                        candidate_features.insert(0,'offset',1.0) # inserts a column of 1's
-
-                if initial_solution_fn is None:
-                        initial_solution = np.zeros(candidate_features.shape[1])
-                else:
-                        try: 
-                                initial_solution = initial_solution_fn(
-                                        candidate_features,candidate_labels)
-                        except Exception as e: 
-                                # handle off-by-one error due to intercept not being included
-                                warning_msg = (
-                                        "Warning: initial solution function failed with this error:"
-                                        f" {e}")
-                                warnings.warn(warning_msg)
-                                initial_solution = np.random.normal(
-                                        loc=0.0,scale=1.0,size=(candidate_features.shape[1]+1)
-                                        )
-
-        elif self.regime == 'reinforcement_learning':
-                self.env_kwargs = self.spec.model.env_kwargs
-
-                initial_solution_fn = self.spec.initial_solution_fn
-
-                if initial_solution_fn is None:
-                        initial_solution = self.spec.model.policy.get_params()
-                else:
-                        initial_solution = initial_solution_fn(candidate_dataset)
+            # Set up initial solution
+            initial_solution_fn = self.spec.initial_solution_fn
 
+            candidate_labels = candidate_df[candidate_dataset.label_column]
+            candidate_features = candidate_df.loc[
+                :, candidate_df.columns != candidate_dataset.label_column
+            ]
+
+            if not candidate_dataset.include_sensitive_columns:
+                candidate_features = candidate_features.drop(
+                    columns=candidate_dataset.sensitive_column_names
+                )
+
+            if candidate_dataset.include_intercept_term:
+                candidate_features.insert(0, "offset", 1.0)  # inserts a column of 1's
+
+            if initial_solution_fn is None:
+                initial_solution = np.zeros(candidate_features.shape[1])
+            else:
+                try:
+                    initial_solution = initial_solution_fn(
+                        candidate_features, candidate_labels
+                    )
+                except Exception as e:
+                    # handle off-by-one error due to intercept not being included
+                    warning_msg = (
+                        "Warning: initial solution function failed with this error:"
+                        f" {e}"
+                    )
+                    warnings.warn(warning_msg)
+                    initial_solution = np.random.normal(
+                        loc=0.0, scale=1.0, size=(candidate_features.shape[1] + 1)
+                    )
+
+        elif self.regime == "reinforcement_learning":
+            self.env_kwargs = self.spec.model.env_kwargs
+
+            initial_solution_fn = self.spec.initial_solution_fn
+
+            if initial_solution_fn is None:
+                initial_solution = self.spec.model.policy.get_params()
+            else:
+                initial_solution = initial_solution_fn(candidate_dataset)
 
         return initial_solution
 
-
-    def candidate_selection(self, candidate_dataset, n_safety, initial_solution,
-            write_logfile=False):
-        """ Create the candidate selection object
+    def candidate_selection(
+        self, candidate_dataset, n_safety, initial_solution, write_logfile=False
+    ):
+        """Create the candidate selection object
 
         :param candidate_dataset: a dataset object containing candidate selection dataset
         :type candidate_dataset: :py:class:`.DataSet` object
         :param n_safety: size of safety dataset
         :type n_safety: int
         :param initial_solution: initial solution that should be used in candidate selection
         :type initial_solution: float
         """
 
         cs_kwargs = dict(
-                model=self.spec.model,
-                candidate_dataset=candidate_dataset,
-                n_safety=n_safety,
-                parse_trees=self.parse_trees,
-                primary_objective=self.spec.primary_objective,
-                optimization_technique=self.spec.optimization_technique,
-                optimizer=self.spec.optimizer,
-                initial_solution=initial_solution,
-                regime=self.regime,
-                write_logfile=write_logfile)
+            model=self.spec.model,
+            candidate_dataset=candidate_dataset,
+            n_safety=n_safety,
+            parse_trees=self.parse_trees,
+            primary_objective=self.spec.primary_objective,
+            optimization_technique=self.spec.optimization_technique,
+            optimizer=self.spec.optimizer,
+            initial_solution=initial_solution,
+            regime=self.regime,
+            write_logfile=write_logfile,
+        )
 
-        cs = CandidateSelection(**cs_kwargs,**self.spec.regularization_hyperparams)
+        cs = CandidateSelection(**cs_kwargs, **self.spec.regularization_hyperparams)
 
         return cs
 
-
     def safety_test(self, safety_dataset):
-        """ Create the safety test object
+        """Create the safety test object
 
         :param safety_dataset: a dataset object containing safety dataset
         :type safety_dataset: :py:class:`.DataSet` object
         """
         st_kwargs = dict(
-                safety_dataset=safety_dataset,
-                model=self.spec.model,parse_trees=self.spec.parse_trees,
-                regime=self.regime,
-                )	
-        
+            safety_dataset=safety_dataset,
+            model=self.spec.model,
+            parse_trees=self.spec.parse_trees,
+            regime=self.regime,
+        )
+
         st = SafetyTest(**st_kwargs)
         return st
 
-
     def run_safety_test(self, candidate_solution, safety_dataset, debug=False):
         """
         Runs safety test using solution from candidate selection
         or some other means
 
         :param candidate_solution: model weights from candidate selection
                 or other process
         :param safety_dataset: a dataset object containing safety dataset
         :type safety_dataset: :py:class:`.DataSet` object
         :param debug: Whether to print out debugging info
-        :return: (passed_safety, solution). passed_safety 
+        :return: (passed_safety, solution). passed_safety
                 indicates whether solution found during candidate selection
                 passes the safety test. solution is the optimized
                 model weights found during candidate selection or 'NSF'.
-        :rtype: Tuple 
+        :rtype: Tuple
         """
-                
+
         st = self.safety_test(safety_dataset)
         passed_safety = st.run(candidate_solution)
         if not passed_safety:
-                if debug:
-                        print("Failed safety test")
-                solution = "NSF"
+            if debug:
+                print("Failed safety test")
+            solution = "NSF"
         else:
-                solution = candidate_solution
-                if debug:
-                        print("Passed safety test!")
+            solution = candidate_solution
+            if debug:
+                print("Passed safety test!")
         return passed_safety, solution
 
-
-
-    def run_core(self, candidate_dataset, safety_dataset, n_safety, frac_data_in_safety, 
-            write_cs_logfile=False,debug=False):
+    def run_core(
+        self,
+        candidate_dataset,
+        safety_dataset,
+        n_safety,
+        frac_data_in_safety,
+        write_cs_logfile=False,
+        debug=False,
+    ):
         """
         Runs seldonian algorithm core using spec object
 
         :param candidate_dataset: a dataset object containing candidate solution dataset
         :type candidate_dataset: :py:class:`.DataSet` object
         :param safety_dataset: a dataset object containing safety dataset
         :type safety_dataset: :py:class:`.DataSet` object
         :param n_safety: size of safety dataset
         :type n_safety: int
-        :param frac_data_in_safety: fraction of data used in safety test, 
+        :param frac_data_in_safety: fraction of data used in safety test,
                 the remaining fraction will be used in candidate selection
         :type frac_data_in_safety: float
         :param write_cs_logfile: Whether to write candidate selection
                 log file
         :param debug: Whether to print out debugging info
-        :return: (passed_safety, solution). passed_safety 
+        :return: (passed_safety, solution). passed_safety
                 indicates whether solution found during candidate selection
                 passes the safety test. solution is the optimized
                 model weights found during candidate selection or 'NSF'.
-        :rtype: Tuple 
+        :rtype: Tuple
         """
 
         # Find candidate solution.
-        initial_solution = self.get_initial_solution(candidate_dataset, frac_data_in_safety)
-        cs = self.candidate_selection(candidate_dataset, n_safety, initial_solution,
-                write_logfile=write_cs_logfile)
-        candidate_solution = cs.run(**self.spec.optimization_hyperparams,
-                use_builtin_primary_gradient_fn=self.spec.use_builtin_primary_gradient_fn,
-                custom_primary_gradient_fn=self.spec.custom_primary_gradient_fn,
-                debug=debug)
-
-        if type(candidate_solution) == str and candidate_solution == 'NSF':
-                # can happen if nan or inf appeared in theta during optimization
-                solution = 'NSF'
-                passed_safety = False
-                return passed_safety,solution
-                
+        initial_solution = self.get_initial_solution(
+            candidate_dataset, frac_data_in_safety
+        )
+        cs = self.candidate_selection(
+            candidate_dataset,
+            n_safety,
+            initial_solution,
+            write_logfile=write_cs_logfile,
+        )
+        candidate_solution = cs.run(
+            **self.spec.optimization_hyperparams,
+            use_builtin_primary_gradient_fn=self.spec.use_builtin_primary_gradient_fn,
+            custom_primary_gradient_fn=self.spec.custom_primary_gradient_fn,
+            debug=debug,
+        )
+
+        if type(candidate_solution) == str and candidate_solution == "NSF":
+            # can happen if nan or inf appeared in theta during optimization
+            solution = "NSF"
+            passed_safety = False
+            return passed_safety, solution
+
         # Safety test
-        passed_safety, solution = self.run_safety_test(candidate_solution, safety_dataset,
-                debug=debug)
+        passed_safety, solution = self.run_safety_test(
+            candidate_solution, safety_dataset, debug=debug
+        )
 
         return passed_safety, solution
 
-
     def find_best_hyperparams(self, write_cs_logfile=False, debug=False):
-        """ Find the best hyperparameter values to use for the Seldonian algorithm.
+        """Find the best hyperparameter values to use for the Seldonian algorithm.
         Note: currently only implemented for frac_data_in_safety.
 
         :return: (frac_data_in_safety, candidate_dataset, safety_dataset). frac_data_in_safety
                 indicates the percentage of total data that is included in the safety dataset.
                 candidate_dataset and safety_dataset are dataset objects containing data from
                 self.dataset split according to frac_data_in_safety
         :rtyle: Tuple
         """
 
         # Sort from lowest amount of data in candidate selection from lowest to highest.
-        self.all_frac_data_in_candidate_selection.sort() 
+        self.all_frac_data_in_candidate_selection.sort()
 
-        for rho in self.all_frac_data_in_candidate_selection: # Move data from safety to cs dataset.
+        for (
+            rho
+        ) in (
+            self.all_frac_data_in_candidate_selection
+        ):  # Move data from safety to cs dataset.
             frac_data_in_safety = 1 - rho
 
             # Partition data according to rho.
-            candidate_dataset, safety_dataset, n_candidate, n_safety = self.create_dataset(
-                    self.dataset, frac_data_in_safety, shuffle=False)
+            (
+                candidate_dataset,
+                safety_dataset,
+                n_candidate,
+                n_safety,
+            ) = self.create_dataset(self.dataset, frac_data_in_safety, shuffle=False)
 
             # Estimate probability of passing.
-            rho_prob_pass = self.est_prob_pass(rho, candidate_dataset, safety_dataset, 
-                    n_candidate, n_safety, write_cs_logfile, debug) # 
+            rho_prob_pass = self.est_prob_pass(
+                rho,
+                candidate_dataset,
+                safety_dataset,
+                n_candidate,
+                n_safety,
+                write_cs_logfile,
+                debug,
+            )  #
 
             # Estimate if any of the future splits of data lead to higher P(pass)
             rho_prime_better = False
-            for rho_prime in self.all_frac_data_in_candidate_selection: 
-                if rho_prime <= rho: # Only look at larger rho.
+            for rho_prime in self.all_frac_data_in_candidate_selection:
+                if rho_prime <= rho:  # Only look at larger rho.
                     continue
-                    
-                rho_prime_prob_pass = self.est_prob_pass(rho_prime, candidate_dataset, 
-                        safety_dataset, n_candidate, n_safety, write_cs_logfile, debug)
-                if rho_prime_prob_pass > rho_prob_pass: # Predict a future split is better.
+
+                rho_prime_prob_pass = self.est_prob_pass(
+                    rho_prime,
+                    candidate_dataset,
+                    safety_dataset,
+                    n_candidate,
+                    n_safety,
+                    write_cs_logfile,
+                    debug,
+                )
+                if (
+                    rho_prime_prob_pass > rho_prob_pass
+                ):  # Predict a future split is better.
                     rho_prime_better = True
-                    break 
+                    break
 
             # If do not predict any greater rho is better, return rho and datasplit.
-            if rho_prime_better is False: 
+            if rho_prime_better is False:
                 break
 
         frac_data_in_safety = 1 - rho
 
         return (frac_data_in_safety, candidate_dataset, safety_dataset)
 
-
-    def est_prob_pass(self, rho_prime, candidate_dataset, safety_dataset, n_candidate, 
-            n_safety, write_cs_logfile=False, debug=False, bootstrap_iter=100):
-        """ Estimates probability of returning a solution with rho_prime fraction of data
+    def est_prob_pass(
+        self,
+        rho_prime,
+        candidate_dataset,
+        safety_dataset,
+        n_candidate,
+        n_safety,
+        write_cs_logfile=False,
+        debug=False,
+        bootstrap_iter=100,
+    ):
+        """Estimates probability of returning a solution with rho_prime fraction of data
             in candidate selection.
 
         :param rho_prime: fraction of data in candidate selection that we want to estimate
                         the probabiilty of returning a solution for
         :type rho_prime: float
         :param candidate_dataset: a dataset object containing candidate solution dataset
         :type candidate_dataset: :py:class:`.DataSet` object
@@ -423,32 +476,45 @@
         :type n_safety: int
         :param n_safety: size of safety dataset
         :type n_safety: int
         """
         frac_data_in_safety_prime = 1 - rho_prime
 
         # Size of bootstrapped datasets according to rho'.
-        total_data = len(self.dataset.df) 
+        total_data = len(self.dataset.df)
         bs_n_candidate = int(total_data * rho_prime)
         bs_n_safety = total_data - bs_n_candidate
 
         pass_count = 0
         for i in range(bootstrap_iter):
-
             # Split candidate_dataset into pools for bootstraping samplinhg.
-            candidate_pool, safety_pool, pool_n_candidate, pool_n_safety = self.create_dataset(
-                    candidate_dataset, frac_data_in_safety_prime, shuffle=True)
+            (
+                candidate_pool,
+                safety_pool,
+                pool_n_candidate,
+                pool_n_safety,
+            ) = self.create_dataset(
+                candidate_dataset, frac_data_in_safety_prime, shuffle=True
+            )
 
             # Bootstrap sample datasets approximating candidate and safety datasets.
-            bs_candidate_dataset = self.bootstrap_sample_dataset(candidate_pool, bs_n_candidate)
+            bs_candidate_dataset = self.bootstrap_sample_dataset(
+                candidate_pool, bs_n_candidate
+            )
             bs_safety_dataset = self.bootstrap_sample_dataset(safety_pool, bs_n_safety)
 
             # Compute a candidate solution using bootstrapped candidate dataset.
-            passed_safety, _ = self.run_core(bs_candidate_dataset, bs_safety_dataset, bs_n_safety, 
-                    frac_data_in_safety_prime, write_cs_logfile, debug=False)
+            passed_safety, _ = self.run_core(
+                bs_candidate_dataset,
+                bs_safety_dataset,
+                bs_n_safety,
+                frac_data_in_safety_prime,
+                write_cs_logfile,
+                debug=False,
+            )
 
             if passed_safety:
-                pass_count +=1
+                pass_count += 1
 
         bs_prob_pass = pass_count / bootstrap_iter
 
         return bs_prob_pass
```

### Comparing `seldonian_engine-0.7.9/seldonian/models/sklearn_lr.py` & `seldonian_engine-0.8.0/seldonian/models/sklearn_lr.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 import autograd.numpy as np
 
 from .sklearn_model import SupervisedSkLearnBaseModel
 from sklearn.linear_model import LinearRegression
 
 
 class SkLearnLinearRegressor(SupervisedSkLearnBaseModel):
-	def __init__(self,**kwargs):
-		""" Implements a linear regressor in Scikit-learn
-		"""
-		self.has_intercept = True
-		super().__init__(**kwargs)
-
-	def create_model(self,**kwargs):
-		""" Create the scikit-learn linear regressor
-		"""
-		model = LinearRegression(**kwargs)
-		return model
-
-	def forward_pass(self,X):
-		""" Make predictions given features
-		"""
-		predictions = self.sklearn_model.predict(X)
-		return predictions
-
-	def backward_pass(self,theta,X):
-		""" Return the Jacobian d(forward_pass)_i/dtheta_{j+1},
-		where i run over datapoints and j run over model parameters,
-		keeping in mind that there is a y-intercept term (hence the j+1 not j)
-		in the predict function 
-		"""
-		m = len(X)
-		X_withintercept = np.hstack([np.ones((m,1)),np.array(X)])
-		return X_withintercept
-
+    def __init__(self, **kwargs):
+        """Implements a linear regressor in Scikit-learn"""
+        self.has_intercept = True
+        super().__init__(**kwargs)
+
+    def create_model(self, **kwargs):
+        """Create the scikit-learn linear regressor"""
+        model = LinearRegression(**kwargs)
+        return model
+
+    def forward_pass(self, X):
+        """Make predictions given features"""
+        predictions = self.sklearn_model.predict(X)
+        return predictions
+
+    def backward_pass(self, theta, X):
+        """Return the Jacobian d(forward_pass)_i/dtheta_{j+1},
+        where i run over datapoints and j run over model parameters,
+        keeping in mind that there is a y-intercept term (hence the j+1 not j)
+        in the predict function
+        """
+        m = len(X)
+        X_withintercept = np.hstack([np.ones((m, 1)), np.array(X)])
+        return X_withintercept
```

### Comparing `seldonian_engine-0.7.9/seldonian/models/tensorflow_model.py` & `seldonian_engine-0.8.0/seldonian/models/tensorflow_model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,178 @@
 # tensorflow_model.py
 
-import autograd.numpy as np   # Thinly-wrapped version of Numpy
+import autograd.numpy as np  # Thinly-wrapped version of Numpy
 from autograd.extend import primitive, defvjp
 from seldonian.models.models import SupervisedModel
 
 import tensorflow as tf
 
 
 @primitive
-def tf_predict(theta,X,model,**kwargs):
-	""" Do a forward pass through the TensorFlow model.
-	Must convert back to numpy array before returning 
-
-	:param theta: model weights
-	:type theta: numpy ndarray
-	:param X: model features
-	:type X: numpy ndarray
-
-	:param model: An instance of a class inheriting from
-		SupervisedTensorFlowBaseModel 
-
-	:return pred_numpy: model predictions 
-	:rtype pred_numpy: numpy ndarray same shape as labels
-	"""
-	# First update model weights
-	model.update_model_params(theta,**kwargs)
-	# Do the forward pass
-	pred = model.forward_pass(X,**kwargs)
-	# set the predictions attribute of the model
-	model.predictions = pred
-	# Convert predictions into a numpy array
-	pred_numpy = pred.numpy()
-	return pred_numpy
-
-def tf_predict_vjp(ans,theta,X,model):
-	""" Do a backward pass through the TensorFlow model,
-	obtaining the Jacobian d pred / dtheta. 
-	Must convert back to numpy array before returning 
-
-	:param ans: The result from tf_predict
-	:type ans: numpy ndarray
-	:param theta: model weights
-	:type theta: numpy ndarray
-	:param X: model features
-	:type X: numpy ndarray
-
-	:param model: An instance of a class inheriting from
-		SupervisedTensorFlowBaseModel 
-
-	:return fn: A function representing the vector Jacobian operator
-	"""
-	def fn(v):
-		# v is a vector of shape ans, the return value of mypredict()
-		# return a 1D array [dF_i/dtheta[0],dF_i/dtheta[1],dF_i/dtheta[2]],
-		# where i is the data row index
-		# print("v:")
-		# print(v)
-		# input("next")
-		dpred_dtheta = model.backward_pass(v)
-		return dpred_dtheta
-	return fn
+def tf_predict(theta, X, model, **kwargs):
+    """Do a forward pass through the TensorFlow model.
+    Must convert back to numpy array before returning
+
+    :param theta: model weights
+    :type theta: numpy ndarray
+    :param X: model features
+    :type X: numpy ndarray
+
+    :param model: An instance of a class inheriting from
+            SupervisedTensorFlowBaseModel
+
+    :return pred_numpy: model predictions
+    :rtype pred_numpy: numpy ndarray same shape as labels
+    """
+    # First update model weights
+    model.update_model_params(theta, **kwargs)
+    # Do the forward pass
+    pred = model.forward_pass(X, **kwargs)
+    # set the predictions attribute of the model
+    model.predictions = pred
+    # Convert predictions into a numpy array
+    pred_numpy = pred.numpy()
+    return pred_numpy
+
+
+def tf_predict_vjp(ans, theta, X, model):
+    """Do a backward pass through the TensorFlow model,
+    obtaining the Jacobian d pred / dtheta.
+    Must convert back to numpy array before returning
+
+    :param ans: The result from tf_predict
+    :type ans: numpy ndarray
+    :param theta: model weights
+    :type theta: numpy ndarray
+    :param X: model features
+    :type X: numpy ndarray
+
+    :param model: An instance of a class inheriting from
+            SupervisedTensorFlowBaseModel
+
+    :return fn: A function representing the vector Jacobian operator
+    """
+
+    def fn(v):
+        # v is a vector of shape ans, the return value of mypredict()
+        # return a 1D array [dF_i/dtheta[0],dF_i/dtheta[1],dF_i/dtheta[2]],
+        # where i is the data row index
+        # print("v:")
+        # print(v)
+        # input("next")
+        dpred_dtheta = model.backward_pass(v)
+        return dpred_dtheta
+
+    return fn
+
 
 # Link the predict function with its gradient,
 # telling autograd not to look inside either of these functions
-defvjp(tf_predict,tf_predict_vjp)
+defvjp(tf_predict, tf_predict_vjp)
 
-class SupervisedTensorFlowBaseModel(SupervisedModel):
-	def __init__(self,**kwargs):
-		""" Base class for Supervised learning Seldonian
-		models implemented in TensorFlow
-		 
-		:param device: The PyTorch device string indicating the
-			hardware on which to run the model,
-			e.g. "cpu", "cuda", "mps".
-		:type device: str
-		"""
-		super().__init__()
-		self.tensorflow_model = self.create_model(**kwargs)
-		self.param_sizes = self.get_param_sizes()
-		self.weights_updated = False
-
-	def predict(self,theta,X,**kwargs):
-		""" Do a forward pass through the PyTorch model.
-		Must convert back to numpy array before returning 
-
-		:param theta: model weights
-		:type theta: numpy ndarray
-
-		:param X: model features
-		:type X: numpy ndarray
-
-		:return pred_numpy: model predictions 
-		:rtype pred_numpy: numpy ndarray same shape as labels
-		"""
-		return tf_predict(theta,X,self)
-
-	def get_model_params(self,*args):
-		""" Return initial weights as a flattened 1D array
-		Also return the number of elements in each model parameter """
-		layer_params_list = []
-		for param in self.tensorflow_model.trainable_weights:
-			layer_params_list.append(param.numpy().flatten())
-		return np.concatenate(layer_params_list)
-
-	def get_param_sizes(self):
-		""" Get the sizes (shapes) of each of the model parameters
-		"""
-		param_sizes = []
-		for param in self.tensorflow_model.trainable_weights:
-			param_sizes.append(np.prod(param.shape))
-		return param_sizes
-
-	def update_model_params(self,theta,**kwargs):
-		""" Update all model parameters using theta,
-		which must be reshaped
-
-		:param theta: model weights
-		:type theta: numpy ndarray
-		"""
-		# Update model parameters using flattened array
-		i = 0
-		startindex = 0
-		for param in self.tensorflow_model.trainable_weights:
-			nparams = self.param_sizes[i]
-			param_shape = param.shape
-			theta_numpy = theta[startindex:startindex+nparams]
-			theta_tf_flat = tf.convert_to_tensor(theta_numpy)
-			theta_tf = tf.reshape(theta_tf_flat,param_shape)
-			param.assign(theta_tf)
-			i+=1
-			startindex+=nparams
-		return
-
-	def forward_pass(self,X,**kwargs):
-		""" Do a forward pass through the TensorFlow model and return the 
-		model outputs (predicted labels). The outputs should be the same shape 
-		as the true labels
-	
-		:param X: model features
-		:type X: numpy ndarray
-
-		:return: predictions
-		:rtype: torch.Tensor
-		"""
-		with tf.GradientTape(persistent=True) as tape:
-			X_tf = tf.convert_to_tensor(X)
-			predictions = self.tensorflow_model(X_tf)
-		self.tape = tape
-		return predictions
-
-	def backward_pass(self,v):
-		""" Do a backward pass through the TensorFlow model and return the
-		(vector) gradient of the model with respect to theta as a numpy ndarray
-
-		:param external_grad: The gradient of the model with respect to itself
-			see: https://pytorch.org/tutorials/beginner/blitz/autograd_tutorial.html#differentiation-in-autograd
-			for more details
-		:type external_grad: torch.Tensor 
-		"""
-		grad_params_list = []
-		grads = self.tape.gradient(self.predictions, 
-			self.tensorflow_model.trainable_weights,output_gradients=v)
-		for grad in grads:
-			grad_numpy = grad.numpy()
-			grad_params_list.append(grad_numpy.flatten())
-		return np.concatenate(grad_params_list)
-
-	def create_model(self,**kwargs):
-		""" Create the TensorFlow model and return it
-		"""
-		raise NotImplementedError("Implement this method in child class")
 
+class SupervisedTensorFlowBaseModel(SupervisedModel):
+    def __init__(self, **kwargs):
+        """Base class for Supervised learning Seldonian
+        models implemented in TensorFlow
+
+        :param device: The PyTorch device string indicating the
+                hardware on which to run the model,
+                e.g. "cpu", "cuda", "mps".
+        :type device: str
+        """
+        super().__init__()
+        self.tensorflow_model = self.create_model(**kwargs)
+        self.param_sizes = self.get_param_sizes()
+        self.weights_updated = False
+
+    def predict(self, theta, X, **kwargs):
+        """Do a forward pass through the PyTorch model.
+        Must convert back to numpy array before returning
+
+        :param theta: model weights
+        :type theta: numpy ndarray
+
+        :param X: model features
+        :type X: numpy ndarray
+
+        :return pred_numpy: model predictions
+        :rtype pred_numpy: numpy ndarray same shape as labels
+        """
+        return tf_predict(theta, X, self)
+
+    def get_model_params(self, *args):
+        """Return initial weights as a flattened 1D array
+        Also return the number of elements in each model parameter"""
+        layer_params_list = []
+        for param in self.tensorflow_model.trainable_weights:
+            layer_params_list.append(param.numpy().flatten())
+        return np.concatenate(layer_params_list)
+
+    def get_param_sizes(self):
+        """Get the sizes (shapes) of each of the model parameters"""
+        param_sizes = []
+        for param in self.tensorflow_model.trainable_weights:
+            param_sizes.append(np.prod(param.shape))
+        return param_sizes
+
+    def update_model_params(self, theta, **kwargs):
+        """Update all model parameters using theta,
+        which must be reshaped
+
+        :param theta: model weights
+        :type theta: numpy ndarray
+        """
+        # Update model parameters using flattened array
+        i = 0
+        startindex = 0
+        for param in self.tensorflow_model.trainable_weights:
+            nparams = self.param_sizes[i]
+            param_shape = param.shape
+            theta_numpy = theta[startindex : startindex + nparams]
+            theta_tf_flat = tf.convert_to_tensor(theta_numpy)
+            theta_tf = tf.reshape(theta_tf_flat, param_shape)
+            param.assign(theta_tf)
+            i += 1
+            startindex += nparams
+        return
+
+    def forward_pass(self, X, **kwargs):
+        """Do a forward pass through the TensorFlow model and return the
+        model outputs (predicted labels). The outputs should be the same shape
+        as the true labels
+
+        :param X: model features
+        :type X: numpy ndarray
+
+        :return: predictions
+        :rtype: torch.Tensor
+        """
+        with tf.GradientTape(persistent=True) as tape:
+            X_tf = tf.convert_to_tensor(X)
+            predictions = self.tensorflow_model(X_tf)
+        self.tape = tape
+        return predictions
+
+    def backward_pass(self, v):
+        """Do a backward pass through the TensorFlow model and return the
+        (vector) gradient of the model with respect to theta as a numpy ndarray
+
+        :param external_grad: The gradient of the model with respect to itself
+                see: https://pytorch.org/tutorials/beginner/blitz/autograd_tutorial.html#differentiation-in-autograd
+                for more details
+        :type external_grad: torch.Tensor
+        """
+        grad_params_list = []
+        grads = self.tape.gradient(
+            self.predictions,
+            self.tensorflow_model.trainable_weights,
+            output_gradients=v,
+        )
+        for grad in grads:
+            grad_numpy = grad.numpy()
+            grad_params_list.append(grad_numpy.flatten())
+        return np.concatenate(grad_params_list)
+
+    def create_model(self, **kwargs):
+        """Create the TensorFlow model and return it"""
+        raise NotImplementedError("Implement this method in child class")
```

### Comparing `seldonian_engine-0.7.9/seldonian/optimizers/gradient_descent.py` & `seldonian_engine-0.8.0/seldonian/optimizers/gradient_descent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 import copy
-import autograd.numpy as np   # Thinly-wrapped version of Numpy
+import autograd.numpy as np  # Thinly-wrapped version of Numpy
 from autograd import grad, jacobian, elementwise_grad as egrad
 
 import warnings
 from seldonian.warnings.custom_warnings import *
 
-def setup_gradients(
-    gradient_library,
-    primary_objective,
-    upper_bounds_function):
-    """ Wrapper to obtain the gradient functions
+
+def setup_gradients(gradient_library, primary_objective, upper_bounds_function):
+    """Wrapper to obtain the gradient functions
     of the primary objective and upper bounds function
     given a gradient library
 
-    :param gradient_library: The name of the library to use for computing 
-        automatic gradients. 
+    :param gradient_library: The name of the library to use for computing
+        automatic gradients.
     :type gradient_library: str, defaults to "autograd"
-    :param primary_objective: Primary objective function 
+    :param primary_objective: Primary objective function
     :param upper_bounds_function: Function for computing upper bounds
-        on the constraints 
+        on the constraints
     """
     if gradient_library == "autograd":
-        grad_primary_theta = grad(primary_objective,argnum=0)
-        grad_upper_bound_theta = jacobian(upper_bounds_function,argnum=0)
+        grad_primary_theta = grad(primary_objective, argnum=0)
+        grad_upper_bound_theta = jacobian(upper_bounds_function, argnum=0)
     else:
         raise NotImplementedError(
-            f"gradient library: {gradient_library}"
-            " not supported")
-    return grad_primary_theta,grad_upper_bound_theta
+            f"gradient library: {gradient_library}" " not supported"
+        )
+    return grad_primary_theta, grad_upper_bound_theta
+
 
 def gradient_descent_adam(
     primary_objective,
     n_constraints,
     upper_bounds_function,
     theta_init,
     lambda_init,
@@ -42,130 +41,140 @@
     alpha_theta=0.05,
     alpha_lamb=0.05,
     beta_velocity=0.9,
     beta_rmsprop=0.9,
     gradient_library="autograd",
     verbose=False,
     debug=False,
-    **kwargs):
-    """ Implements simultaneous gradient descent/ascent using 
+    **kwargs,
+):
+    """Implements simultaneous gradient descent/ascent using
     the Adam optimizer on a Lagrangian:
     L(theta,lambda) = f(theta) + lambda*g(theta),
-    where f is the primary objective, lambda is a vector of 
-    Lagrange multipliers, and g is a vector of the 
-    upper bound functions. Gradient descent is done for theta 
-    and gradient ascent is done for lambda to find the saddle 
-    points of L. Being part of candidate selection, 
+    where f is the primary objective, lambda is a vector of
+    Lagrange multipliers, and g is a vector of the
+    upper bound functions. Gradient descent is done for theta
+    and gradient ascent is done for lambda to find the saddle
+    points of L. Being part of candidate selection,
     it is important that this function always returns a solution.
     The safety test determines if No Solution Found.
 
     :param primary_objective: The objective function that would
         be solely optimized in the absence of behavioral constraints,
         i.e., the loss function
     :type primary_objective: function or class method
-    :param n_constraints: The number of constraints 
+    :param n_constraints: The number of constraints
     :param upper_bounds_function: The function that calculates
         the upper bounds on the constraints
     :type upper_bounds_function: function or class method
-    :param theta_init: Initial model weights 
+    :param theta_init: Initial model weights
     :type theta_init: numpy ndarray
-    :param lambda_init: Initial values for Lagrange multiplier terms 
+    :param lambda_init: Initial values for Lagrange multiplier terms
     :type theta_init: float
     :param alpha_theta: Initial learning rate for theta
     :type alpha_theta: float
     :param alpha_lamb: Initial learning rate for lambda
     :type alpha_lamb: float
     :param beta_velocity: Exponential decay rate for velocity term
     :type beta_velocity: float
     :param beta_rmsprop: Exponential decay rate for rmsprop term
     :type beta_rmsprop: float
     :param num_iters: The number of iterations of gradient descent to run
     :type num_iters: int
-    :param gradient_library: The name of the library to use for computing 
-        automatic gradients. 
+    :param gradient_library: The name of the library to use for computing
+        automatic gradients.
     :type gradient_library: str, defaults to "autograd"
     :param verbose: Boolean flag to control verbosity
     :param debug: Boolean flag to print out info useful for debugging
 
-    :return: solution, a dictionary containing the solution and metadata 
+    :return: solution, a dictionary containing the solution and metadata
         about the gradient descent run
     :rtype: dict
     """
-    
+
     # initialize theta, lambda
     theta = theta_init
-    # If lambda provided as a float, make a vector 
+    # If lambda provided as a float, make a vector
     # with this value for all constraints
     if type(lambda_init) == float:
-        lamb = np.repeat(lambda_init,n_constraints)
+        lamb = np.repeat(lambda_init, n_constraints)
     else:
-        lamb = np.array(lambda_init) 
+        lamb = np.array(lambda_init)
 
     if len(lamb) != n_constraints:
         raise RuntimeError(
             "lambda has wrong shape. Shape must be (n_constraints,), "
-            f"but shape is {lamb.shape}")
-        
+            f"but shape is {lamb.shape}"
+        )
+
     # initialize Adam parameters
-    velocity_theta, velocity_lamb = 0.0,0.0
-    s_theta, s_lamb = 0.0,0.0
-    rms_offset = 1e-6 # small offset to make sure we don't take 1/sqrt(very small) in weight update
+    velocity_theta, velocity_lamb = 0.0, 0.0
+    s_theta, s_lamb = 0.0, 0.0
+    rms_offset = 1e-6  # small offset to make sure we don't take 1/sqrt(very small) in weight update
 
     # Initialize params for tracking best solution
-    best_primary = np.inf # minimizing f so want it to be lowest possible
-    best_index = 0  
+    best_primary = np.inf  # minimizing f so want it to be lowest possible
+    best_index = 0
     candidate_solution = None
 
     # If we never enter feasible set, we still need to know what the solution was
     # when g was minimum
     found_feasible_solution = False
     # Store values at each step in gradient descent, if requested
     theta_vals = []
     lamb_vals = []
     L_vals = []
-    f_vals = [] # primary
-    g_vals = [] # constraint upper bound values
+    f_vals = []  # primary
+    g_vals = []  # constraint upper bound values
 
     # Get df/dtheta and dg/dtheta automatic gradients
-    (grad_primary_theta,
-        grad_upper_bound_theta) = setup_gradients(
-        gradient_library,
-        primary_objective,
-        upper_bounds_function)
-        
+    (grad_primary_theta, grad_upper_bound_theta) = setup_gradients(
+        gradient_library, primary_objective, upper_bounds_function
+    )
+
     # It is possible that the user provided the function df/dtheta,
     # which can often speed up computing the gradients.
     # In that case, override the automatic gradient function
-    if 'primary_gradient' in kwargs:
-        grad_primary_theta = kwargs['primary_gradient']
-    
+    if "primary_gradient" in kwargs:
+        grad_primary_theta = kwargs["primary_gradient"]
+
     # Start gradient descent
     gd_index = 0
     if verbose:
-        n_iters_tot = n_epochs*n_batches
+        n_iters_tot = n_epochs * n_batches
         print(
             f"Have {n_epochs} epochs and {n_batches} batches of size {batch_size} "
-            f"for a total of {n_iters_tot} iterations")
+            f"for a total of {n_iters_tot} iterations"
+        )
+
     for epoch in range(n_epochs):
         for batch_index in range(n_batches):
             if verbose:
                 if batch_index % 10 == 0:
                     print(f"Epoch: {epoch}, batch iteration {batch_index}")
-
-            batch_calculator(batch_index,batch_size)
+            is_small_batch = batch_calculator(batch_index, batch_size)
             primary_val = primary_objective(theta)
             g_vec = upper_bounds_function(theta)
-            L_val = primary_val + sum(lamb*g_vec) 
-         
+            L_val = primary_val + sum(lamb * g_vec)
+
             if debug:
-                print("epoch,batch_i,overall_i,f,g,theta,lambda:",epoch,batch_index,gd_index,primary_val,g_vec,theta,lamb)
+                print(
+                    "epoch,batch_i,overall_i,f,g,theta,lambda:",
+                    epoch,
+                    batch_index,
+                    gd_index,
+                    primary_val,
+                    g_vec,
+                    theta,
+                    lamb,
+                )
                 print()
-            
+
             # Check if this is best feasible value so far
-            if all([g<= 0 for g in g_vec]) and primary_val < best_primary:
+            if (not is_small_batch) and all([g <= 0 for g in g_vec]) and primary_val < best_primary:
                 found_feasible_solution = True
                 best_index = gd_index
                 best_primary = primary_val
                 best_lamb = lamb
                 best_g_vec = g_vec
                 best_L = L_val
                 candidate_solution = np.copy(theta)
@@ -175,96 +184,110 @@
             lamb_vals.append(np.copy(lamb))
             f_vals.append(primary_val)
             g_vals.append(g_vec)
             L_vals.append(L_val)
 
             # if nans or infs appear in any quantities,
             # then stop gradient descent and return NSF
-            if np.isinf(primary_val) or np.isnan(primary_val) \
-                or np.isinf(lamb).any() or np.isnan(lamb).any() \
-                or np.isinf(theta).any() or np.isnan(theta).any() \
-                or np.isinf(g_vec).any() or np.isnan(g_vec).any():
+            if (
+                np.isinf(primary_val)
+                or np.isnan(primary_val)
+                or np.isinf(lamb).any()
+                or np.isnan(lamb).any()
+                or np.isinf(theta).any()
+                or np.isnan(theta).any()
+                or np.isinf(g_vec).any()
+                or np.isnan(g_vec).any()
+            ):
                 warning_msg = (
                     "Warning: a nan or inf was found during "
                     "gradient descent. Stopping prematurely "
-                    "and returning NSF.")
+                    "and returning NSF."
+                )
                 warnings.warn(warning_msg)
                 candidate_solution = "NSF"
                 break
 
-            # Obtain gradients of both terms in Lagrangian 
+            # Obtain gradients of both terms in Lagrangian
             # at current values of theta and lambda
             grad_primary_theta_val = grad_primary_theta(theta)
             gu_theta_vec = grad_upper_bound_theta(theta)
 
-            grad_secondary_theta_val_vec = gu_theta_vec * lamb[:, None] ## to multiply each row of gu_theta_vec by elements of lamb
-            gradient_theta = grad_primary_theta_val + np.sum(grad_secondary_theta_val_vec,axis=0)
-            
+            grad_secondary_theta_val_vec = (
+                gu_theta_vec * lamb[:, None]
+            )  ## to multiply each row of gu_theta_vec by elements of lamb
+            gradient_theta = grad_primary_theta_val + np.sum(
+                grad_secondary_theta_val_vec, axis=0
+            )
+
             # gradient w.r.t. to lambda is just g
             gradient_lamb_vec = g_vec
 
             # Momementum term
-            velocity_theta = beta_velocity*velocity_theta + (1.0-beta_velocity)*gradient_theta
+            velocity_theta = (
+                beta_velocity * velocity_theta + (1.0 - beta_velocity) * gradient_theta
+            )
 
             # RMS prop term
-            s_theta = beta_rmsprop*s_theta + (1.0-beta_rmsprop)*pow(gradient_theta,2)
+            s_theta = beta_rmsprop * s_theta + (1.0 - beta_rmsprop) * pow(
+                gradient_theta, 2
+            )
 
             # bias-correction
-            velocity_theta /= (1-pow(beta_velocity,gd_index+1))
-            s_theta /= (1-pow(beta_rmsprop,gd_index+1))
+            velocity_theta /= 1 - pow(beta_velocity, gd_index + 1)
+            s_theta /= 1 - pow(beta_rmsprop, gd_index + 1)
 
             # update weights
-            theta -= alpha_theta*velocity_theta/(np.sqrt(s_theta)+rms_offset) # gradient descent
-            lamb += alpha_lamb*gradient_lamb_vec # element wise update
-            
+            theta -= (
+                alpha_theta * velocity_theta / (np.sqrt(s_theta) + rms_offset)
+            )  # gradient descent
+            lamb += alpha_lamb * gradient_lamb_vec  # element wise update
+
             # If any values in lambda vector dip below 0, force them to be zero
-            lamb[lamb<0]=0
-            
+            lamb[lamb < 0] = 0
+
             gd_index += 1
-        else: # only executed if inner loop did not break
+        else:  # only executed if inner loop did not break
             continue
-        break # only executed if inner loop broke
+        break  # only executed if inner loop broke
 
     solution = {}
     solution_found = True
 
     # If theta never entered feasible set pick best g
     if not found_feasible_solution:
-        if candidate_solution == 'NSF':
+        if candidate_solution == "NSF":
             if debug:
-                print(
-                    "NaN or Inf appeared in gradient descent terms "
-                    "Returning NSF"
-                    )
+                print("NaN or Inf appeared in gradient descent terms " "Returning NSF")
             best_index = None
             best_primary = None
             best_lamb = None
             best_g_vec = None
             best_L = None
-        else:   
+        else:
             if debug:
                 print(
                     "Never found feasible solution. "
                     "Returning solution with lowest sqrt(|g|**2)"
-                    )
+                )
             # best g is when norm of g is minimized
-            best_index = np.argmin(np.linalg.norm(g_vals,axis=1))
+            best_index = np.argmin(np.linalg.norm(g_vals, axis=1))
             best_primary = f_vals[best_index]
             best_lamb = lamb_vals[best_index]
             best_g_vec = g_vals[best_index]
             best_L = L_vals[best_index]
             candidate_solution = theta_vals[best_index]
 
-    solution['candidate_solution'] = candidate_solution
-    solution['best_index'] = best_index
-    solution['best_f'] = best_primary
-    solution['best_g'] = best_g_vec
-    solution['best_lamb'] = best_lamb
-    solution['best_L'] = best_L
-    solution['found_feasible_solution'] = found_feasible_solution
-    solution['theta_vals'] = np.array(theta_vals)
-    solution['f_vals'] = np.array(f_vals)
-    solution['lamb_vals'] = np.array(lamb_vals)
-    solution['g_vals'] = np.array(g_vals)
-    solution['L_vals'] = np.array(L_vals)
+    solution["candidate_solution"] = candidate_solution
+    solution["best_index"] = best_index
+    solution["best_f"] = best_primary
+    solution["best_g"] = best_g_vec
+    solution["best_lamb"] = best_lamb
+    solution["best_L"] = best_L
+    solution["found_feasible_solution"] = found_feasible_solution
+    # solution["theta_vals"] = np.array(theta_vals) # takes up too much disk
+    solution["f_vals"] = np.array(f_vals)
+    solution["lamb_vals"] = np.array(lamb_vals)
+    solution["g_vals"] = np.array(g_vals)
+    solution["L_vals"] = np.array(L_vals)
 
-    return solution
+    return solution
```

### Comparing `seldonian_engine-0.7.9/seldonian/parse_tree/nodes.py` & `seldonian_engine-0.8.0/seldonian/parse_tree/nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,582 +1,583 @@
 from operator import itemgetter
-from functools import reduce,partial
+from functools import reduce, partial
 import pandas as pd
 import autograd.numpy as np
 
-from seldonian.models.objectives import (
-    sample_from_statistic,evaluate_statistic)
+from seldonian.models.objectives import sample_from_statistic, evaluate_statistic
 from seldonian.utils.stats_utils import *
 
+
 class Node(object):
-    def __init__(self,name,lower,upper):
+    def __init__(self, name, lower, upper):
         """The base class for all parse tree nodes
-        
-        :param name: 
+
+        :param name:
             The name of the node
         :type name: str
 
-        :param lower: 
+        :param lower:
             Lower confidence bound
         :type lower: float
 
-        :param upper: 
+        :param upper:
             Upper confidence bound
         :type upper: float
-        
-        :ivar index: 
+
+        :ivar index:
             The index of the node in the tree
         :vartype index: int
 
-        :ivar left: 
+        :ivar left:
             Left child node
         :vartype left: Node object, defaults to None
 
-        :ivar right: 
+        :ivar right:
             Right child node
         :vartype right: Node object, defaults to None
-        
-        :ivar will_lower_bound: 
+
+        :ivar will_lower_bound:
             Whether this node needs a lower bound
         :vartype will_lower_bound: bool
-        
-        :ivar will_upper_bound: 
+
+        :ivar will_upper_bound:
             Whether this node needs an upper bound
         :vartype will_upper_bound: bool
 
         """
         self.name = name
-        self.index = None 
-        self.left  = None 
-        self.right = None 
-        self.lower = lower 
-        self.upper = upper 
+        self.index = None
+        self.left = None
+        self.right = None
+        self.lower = lower
+        self.upper = upper
         self.will_lower_bound = True
         self.will_upper_bound = True
 
     def __repr__(self):
-        """ The string representation of the node. 
-        Also, what is displayed inside the node box 
-        in the visual graph 
-        """
-        lower_bracket = '(' if np.isinf(self.lower) else '[' 
-        upper_bracket = ')' if np.isinf(self.upper) else ']'
-
-        lower_str = f'{self.lower:g}' if self.will_lower_bound else '_'
-        upper_str = f'{self.upper:g}' if self.will_upper_bound else '_'
-
-
-        bounds_str = \
-            f'{lower_bracket}{lower_str}, {upper_str}{upper_bracket}' \
-            if (self.lower!= None or self.upper!=None) else '()'
-
-        return '\n'.join(
-            [
-                '['+str(self.index)+']',
-                str(self.name),
-                u'\u03B5' + ' ' + bounds_str
-            ]
-        ) 
-  
+        """The string representation of the node.
+        Also, what is displayed inside the node box
+        in the visual graph
+        """
+        lower_bracket = "(" if np.isinf(self.lower) else "["
+        upper_bracket = ")" if np.isinf(self.upper) else "]"
+
+        lower_str = f"{self.lower:g}" if self.will_lower_bound else "_"
+        upper_str = f"{self.upper:g}" if self.will_upper_bound else "_"
+
+        bounds_str = (
+            f"{lower_bracket}{lower_str}, {upper_str}{upper_bracket}"
+            if (self.lower != None or self.upper != None)
+            else "()"
+        )
+
+        return "\n".join(
+            ["[" + str(self.index) + "]", str(self.name), "\u03B5" + " " + bounds_str]
+        )
+
 
 class BaseNode(Node):
-    def __init__(self,
+    def __init__(
+        self,
         name,
-        lower=float('-inf'),
-        upper=float('inf'),
+        lower=float("-inf"),
+        upper=float("inf"),
         conditional_columns=[],
-        **kwargs):
-        """ Class for base variable leaf nodes
+        **kwargs,
+    ):
+        """Class for base variable leaf nodes
         in the parse tree.
 
-        :param name: 
+        :param name:
             The name of the node
         :type name: str
-        :param lower: 
+        :param lower:
             Lower confidence bound
         :type lower: float
-        :param upper: 
+        :param upper:
             Upper confidence bound
         :type upper: float
-        :param conditional_columns: 
-            When calculating confidence bounds on a measure 
+        :param conditional_columns:
+            When calculating confidence bounds on a measure
             function, condition on these columns being == 1
         :type conditional_columns: List(str)
-        :ivar node_type: 
+        :ivar node_type:
             equal to 'base_node'
         :vartype node_type: str
-        :ivar delta: 
+        :ivar delta:
             The share of the confidence put into this node
         :vartype delta: float
         :ivar measure_function_name: str
             The name of the statistical measurement
-            function that this node represents, e.g. "FPR". 
+            function that this node represents, e.g. "FPR".
             Must be contained in measure_functions
             list in :py:mod:`.operators`
         :vartype measure_function_name: str
         """
-        super().__init__(name,lower,upper,**kwargs)
+        super().__init__(name, lower, upper, **kwargs)
         self.conditional_columns = conditional_columns
-        self.node_type = 'base_node'
-        self.delta = 0  
-        self.measure_function_name = '' 
+        self.node_type = "base_node"
+        self.delta = 0
+        self.measure_function_name = ""
 
     def __repr__(self):
-        """ Overrides Node.__repr__()
-        """
-        return super().__repr__() + ', ' + u'\u03B4' + f'={self.delta:g}'
-    
-    def calculate_value(self,
-        **kwargs):
+        """Overrides Node.__repr__()"""
+        return super().__repr__() + ", " + "\u03B4" + f"={self.delta:g}"
+
+    def calculate_value(self, **kwargs):
         """
-        Calculate the value of the node 
+        Calculate the value of the node
         given model weights, etc. This is
         the expected value of the base variable,
         not the bound.
-        """ 
-    
-        value = evaluate_statistic(
-            statistic_name=self.measure_function_name,
-            **kwargs)
+        """
+
+        value = evaluate_statistic(statistic_name=self.measure_function_name, **kwargs)
         return value
 
-    def mask_data(self,
-        dataset,
-        conditional_columns):
-        """Mask features and labels using 
+    def mask_data(self, dataset, conditional_columns):
+        """Mask features and labels using
         a joint AND mask where each of the
         conditional columns is True.
 
-        :param dataset: 
+        :param dataset:
             The candidate or safety dataset
         :type dataset: dataset.Dataset object
-        :param conditional_columns: 
+        :param conditional_columns:
             List of columns for which to create
             the joint AND mask on the dataset
         :type conditional_columns: List(str)
 
-        :return: The masked dataframe 
+        :return: The masked dataframe
         :rtype: numpy ndarray
         """
         # Figure out indices of sensitive attributes from their column names
-        sensitive_col_indices = [dataset.sensitive_col_names.index(
-            col) for col in conditional_columns]
-
-        joint_mask = reduce(np.logical_and,
-            (dataset.sensitive_attrs[:,col_index]==1 for col_index in sensitive_col_indices))
-        if dataset.regime == 'supervised_learning':
+        sensitive_col_indices = [
+            dataset.sensitive_col_names.index(col) for col in conditional_columns
+        ]
+
+        joint_mask = reduce(
+            np.logical_and,
+            (
+                dataset.sensitive_attrs[:, col_index] == 1
+                for col_index in sensitive_col_indices
+            ),
+        )
+        if dataset.regime == "supervised_learning":
             if type(dataset.features) == list:
                 masked_features = [x[joint_mask] for x in dataset.features]
                 masked_labels = [x[joint_mask] for x in dataset.labels]
-                # If possible, convert to numpy array. Not always possible, 
+                # If possible, convert to numpy array. Not always possible,
                 # e.g., if features are of different dimensions.
                 try:
                     masked_features = np.array(masked_features)
                     masked_labels = np.array(masked_labels)
                     n_masked = len(masked_features)
                 except Exception as e:
                     # masked_features and masked_labels stay as lists
                     n_masked = len(masked_features[0])
             else:
-                # numpy array 
-                masked_features = dataset.features[joint_mask] 
+                # numpy array
+                masked_features = dataset.features[joint_mask]
                 masked_labels = dataset.labels[joint_mask]
                 n_masked = len(masked_features)
 
-            return masked_features,masked_labels,n_masked
-        
-        elif dataset.regime == 'reinforcement_learning':
+            return masked_features, masked_labels, n_masked
+
+        elif dataset.regime == "reinforcement_learning":
             masked_episodes = np.asarray(dataset.episodes)[joint_mask]
             n_masked = len(masked_episodes)
-            return masked_episodes,n_masked
+            return masked_episodes, n_masked
 
-    def calculate_data_forbound(self,**kwargs):
+    def calculate_data_forbound(self, **kwargs):
         """
         Prepare data inputs
         for confidence bound calculation.
         """
-        theta,dataset,model,regime,branch = itemgetter(
-                    'theta','dataset','model',
-                    'regime','branch')(kwargs)
+        theta, dataset, model, regime, branch = itemgetter(
+            "theta", "dataset", "model", "regime", "branch"
+        )(kwargs)
 
-        if branch == 'candidate_selection':
+        if branch == "candidate_selection":
             # Then we're in candidate selection
-            n_safety = kwargs['n_safety']
+            n_safety = kwargs["n_safety"]
 
         # If in candidate selection want to use safety data size
         # in bound calculation
-        
-        if regime == 'supervised_learning':
+
+        if regime == "supervised_learning":
             # mask the data using the conditional columns, if present
-            
+
             features = dataset.features
             labels = dataset.labels
-            
+
             if self.conditional_columns:
-                masked_features,masked_labels,n_masked = self.mask_data(
-                    dataset,self.conditional_columns)
+                masked_features, masked_labels, n_masked = self.mask_data(
+                    dataset, self.conditional_columns
+                )
             else:
-                (masked_features,
-                    masked_labels,
-                    n_masked) = features,labels,dataset.num_datapoints
-
-            if branch == 'candidate_selection':
-                frac_masked = n_masked/dataset.num_datapoints
-                datasize = int(round(frac_masked*n_safety))
+                (masked_features, masked_labels, n_masked) = (
+                    features,
+                    labels,
+                    dataset.num_datapoints,
+                )
+
+            if branch == "candidate_selection":
+                frac_masked = n_masked / dataset.num_datapoints
+                datasize = int(round(frac_masked * n_safety))
             else:
                 datasize = n_masked
-            data_dict = {'features':masked_features,'labels':masked_labels}  
-            
-        elif regime == 'reinforcement_learning':
-            gamma = model.env_kwargs['gamma']
+            data_dict = {"features": masked_features, "labels": masked_labels}
+
+        elif regime == "reinforcement_learning":
+            gamma = model.env_kwargs["gamma"]
             episodes = dataset.episodes
 
             if self.conditional_columns:
-                masked_episodes,n_masked = self.mask_data(
-                    dataset,self.conditional_columns)
+                masked_episodes, n_masked = self.mask_data(
+                    dataset, self.conditional_columns
+                )
             else:
-                (masked_episodes,
-                    n_masked) = episodes,dataset.num_datapoints
+                (masked_episodes, n_masked) = episodes, dataset.num_datapoints
 
-            if branch == 'candidate_selection':
-                frac_masked = n_masked/dataset.num_datapoints
-                datasize = int(round(frac_masked*n_safety))
+            if branch == "candidate_selection":
+                frac_masked = n_masked / dataset.num_datapoints
+                datasize = int(round(frac_masked * n_safety))
             else:
                 datasize = n_masked
-            
+
             # Precalculate expected return from behavioral policy
-            masked_returns = [weighted_sum_gamma(ep.rewards,gamma) for ep in masked_episodes]
+            if "alt_reward_number" in kwargs:
+                # use the alternate reward specified in the constraint string
+                # when calculating the return
+                alt_reward_number = kwargs["alt_reward_number"]
+                alt_reward_index = alt_reward_number - 1
+                masked_returns = [
+                    weighted_sum_gamma(ep.alt_rewards[:, alt_reward_index], gamma)
+                    for ep in masked_episodes
+                ]
+            else:
+                masked_returns = [
+                    weighted_sum_gamma(ep.rewards, gamma) for ep in masked_episodes
+                ]
 
             data_dict = {
-                'episodes':masked_episodes,
-                'weighted_returns':masked_returns
+                "episodes": masked_episodes,
+                "weighted_returns": masked_returns,
             }
 
-        return data_dict,datasize
-                    
-    def calculate_bounds(self,
-        **kwargs):
-        """Calculate confidence bounds given a bound_method, 
+        return data_dict, datasize
+
+    def calculate_bounds(self, **kwargs):
+        """Calculate confidence bounds given a bound_method,
         such as t-test.
-        """ 
-        if 'bound_method' in kwargs:
-            bound_method = kwargs['bound_method']
-            if bound_method == 'manual':
+        """
+        if "bound_method" in kwargs:
+            bound_method = kwargs["bound_method"]
+            if bound_method == "manual":
                 # Bounds set by user
-                return {'lower':self.lower,
-                        'upper':self.upper}
+                return {"lower": self.lower, "upper": self.upper}
 
-            elif bound_method == 'random':
+            elif bound_method == "random":
                 # Randomly assign lower and upper bounds
-                lower, upper = (
-                    np.random.randint(0,2),
-                    np.random.randint(2,4)
-                    )
-                return {'lower':lower,'upper':upper}
-        
+                lower, upper = (np.random.randint(0, 2), np.random.randint(2, 4))
+                return {"lower": lower, "upper": upper}
+
             else:
-                # Real confidence bound 
+                # Real confidence bound
 
-                # --TODO-- abstract away to support things like 
+                # --TODO-- abstract away to support things like
                 # getting confidence intervals from bootstrap
                 # and RL cases
                 estimator_samples = self.zhat(**kwargs)
 
-                branch = kwargs['branch']
-                data_dict = kwargs['data_dict']
+                branch = kwargs["branch"]
+                data_dict = kwargs["data_dict"]
                 bound_kwargs = kwargs
-                bound_kwargs['data'] = estimator_samples
-                bound_kwargs['delta'] = self.delta
-                
-                # If lower and upper are both needed, 
+                bound_kwargs["data"] = estimator_samples
+                bound_kwargs["delta"] = self.delta
+
+                # If lower and upper are both needed,
                 # can't necessarily call lower and upper
                 # bound functions separately. Sometimes the joint bound
                 # is different from the individual bounds combined
                 if self.will_lower_bound and self.will_upper_bound:
-                    if branch == 'candidate_selection':
-                        lower,upper = self.predict_HC_upper_and_lowerbound(
-                            **bound_kwargs)
-                    elif branch == 'safety_test':
-                        lower,upper = self.compute_HC_upper_and_lowerbound(
-                            **bound_kwargs)
-                    return {'lower':lower,'upper':upper}
-                
+                    if branch == "candidate_selection":
+                        lower, upper = self.predict_HC_upper_and_lowerbound(
+                            **bound_kwargs
+                        )
+                    elif branch == "safety_test":
+                        lower, upper = self.compute_HC_upper_and_lowerbound(
+                            **bound_kwargs
+                        )
+                    return {"lower": lower, "upper": upper}
+
                 elif self.will_lower_bound:
-                    if branch == 'candidate_selection':
-                        lower = self.predict_HC_lowerbound(
-                            **bound_kwargs)
-                    elif branch == 'safety_test':
-                        lower = self.compute_HC_lowerbound(
-                            **bound_kwargs)
-                    return {'lower':lower}
+                    if branch == "candidate_selection":
+                        lower = self.predict_HC_lowerbound(**bound_kwargs)
+                    elif branch == "safety_test":
+                        lower = self.compute_HC_lowerbound(**bound_kwargs)
+                    return {"lower": lower}
 
                 elif self.will_upper_bound:
-                    if branch == 'candidate_selection':
-                        upper = self.predict_HC_upperbound(
-                            **bound_kwargs)
-                    elif branch == 'safety_test':
-                        upper = self.compute_HC_upperbound(
-                            **bound_kwargs)
-                    return {'upper':upper}
+                    if branch == "candidate_selection":
+                        upper = self.predict_HC_upperbound(**bound_kwargs)
+                    elif branch == "safety_test":
+                        upper = self.compute_HC_upperbound(**bound_kwargs)
+                    return {"upper": upper}
 
                 raise AssertionError(
-                    "will_lower_bound and will_upper_bound "
-                    "cannot both be False") 
+                    "will_lower_bound and will_upper_bound " "cannot both be False"
+                )
 
         else:
             raise RuntimeError("bound_method not specified!")
-    
-    def zhat(self,model,theta,data_dict,datasize,**kwargs):
+
+    def zhat(self, model, theta, data_dict, datasize, **kwargs):
         """
-        Calculate an unbiased estimate of the 
+        Calculate an unbiased estimate of the
         base variable node.
-    
+
         :param model: The machine learning model
         :type model: models.SeldonianModel object
-        :param theta: 
+        :param theta:
             model weights
         :type theta: numpy ndarray
-        :param data_dict: 
-            Contains inputs to model, 
+        :param data_dict:
+            Contains inputs to model,
             such as features and labels
         :type data_dict: dict
         """
 
-        return sample_from_statistic(model=model,
+        return sample_from_statistic(
+            model=model,
             statistic_name=self.measure_function_name,
-            theta=theta,data_dict=data_dict,
-            datasize=datasize,**kwargs)
+            theta=theta,
+            data_dict=data_dict,
+            datasize=datasize,
+            **kwargs,
+        )
 
-    def predict_HC_lowerbound(self,
-        data,
-        datasize,
-        delta,
-        **kwargs):
+    def predict_HC_lowerbound(self, data, datasize, delta, **kwargs):
         """
         Calculate high confidence lower bound
         that we expect to pass the safety test.
         Used in candidate selection
 
-        :param data: 
-            Vector containing base variable  
+        :param data:
+            Vector containing base variable
             evaluated at each observation in dataset
-        :type data: numpy ndarray 
-        :param datasize: 
+        :type data: numpy ndarray
+        :param datasize:
             The number of observations in the safety dataset
         :type datasize: int
-        :param delta: 
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
-        """ 
-        if 'bound_method' in kwargs:
-            bound_method = kwargs['bound_method']
+        """
+        if "bound_method" in kwargs:
+            bound_method = kwargs["bound_method"]
 
-            if bound_method == 'ttest':
-                lower = data.mean() - 2*stddev(data) / np.sqrt(datasize) * tinv(1.0 - delta, datasize - 1)
+            if bound_method == "ttest":
+                lower = data.mean() - 2 * stddev(data) / np.sqrt(datasize) * tinv(
+                    1.0 - delta, datasize - 1
+                )
             else:
-                raise NotImplementedError(f"Bounding method {bound_method} is not supported")
-        
+                raise NotImplementedError(
+                    f"Bounding method {bound_method} is not supported"
+                )
+
         return lower
 
-    def predict_HC_upperbound(self,
-        data,
-        datasize,
-        delta,
-        **kwargs):
+    def predict_HC_upperbound(self, data, datasize, delta, **kwargs):
         """
         Calculate high confidence upper bound
         that we expect to pass the safety test.
         Used in candidate selection
 
-        :param data: 
-            Vector containing base variable  
+        :param data:
+            Vector containing base variable
             evaluated at each observation in dataset
-        :type data: numpy ndarray 
-        :param datasize: 
+        :type data: numpy ndarray
+        :param datasize:
             The number of observations in the safety dataset
         :type datasize: int
-        :param delta: 
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
-        """  
-        if 'bound_method' in kwargs:
-            bound_method = kwargs['bound_method']
-            if bound_method == 'ttest':
-                lower = data.mean() + 2*stddev(data) / np.sqrt(datasize) * tinv(1.0 - delta, datasize - 1)
+        """
+        if "bound_method" in kwargs:
+            bound_method = kwargs["bound_method"]
+            if bound_method == "ttest":
+                lower = data.mean() + 2 * stddev(data) / np.sqrt(datasize) * tinv(
+                    1.0 - delta, datasize - 1
+                )
             else:
-                raise NotImplementedError(f"Bounding method {bound_method} is not supported")
-            
+                raise NotImplementedError(
+                    f"Bounding method {bound_method} is not supported"
+                )
+
         return lower
 
-    def predict_HC_upper_and_lowerbound(self,
-        data,
-        datasize,
-        delta,
-        **kwargs):
+    def predict_HC_upper_and_lowerbound(self, data, datasize, delta, **kwargs):
         """
         Calculate high confidence lower and upper bounds
         that we expect to pass the safety test.
         Used in candidate selection.
-    
+
         Depending on the bound_method,
         this is not always equivalent
-        to calling predict_HC_lowerbound() and 
+        to calling predict_HC_lowerbound() and
         predict_HC_upperbound() independently.
 
-        :param data: 
-            Vector containing base variable  
+        :param data:
+            Vector containing base variable
             evaluated at each observation in dataset
-        :type data: numpy ndarray 
-        :param datasize: 
+        :type data: numpy ndarray
+        :param datasize:
             The number of observations in the safety dataset
         :type datasize: int
-        :param delta: 
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
-        """ 
-        if 'bound_method' in kwargs:
-            bound_method = kwargs['bound_method']
-            if bound_method == 'ttest':
-                lower = self.predict_HC_lowerbound(data=data,
-                    datasize=datasize,delta=delta/2,
-                    **kwargs)
-                upper = self.predict_HC_upperbound(data=data,
-                    datasize=datasize,delta=delta/2,
-                    **kwargs)
+        """
+        if "bound_method" in kwargs:
+            bound_method = kwargs["bound_method"]
+            if bound_method == "ttest":
+                lower = self.predict_HC_lowerbound(
+                    data=data, datasize=datasize, delta=delta / 2, **kwargs
+                )
+                upper = self.predict_HC_upperbound(
+                    data=data, datasize=datasize, delta=delta / 2, **kwargs
+                )
 
-            elif bound_method == 'manual':
+            elif bound_method == "manual":
                 pass
             else:
                 raise NotImplementedError(
-                    f"Bounding method {bound_method}"
-                    " is not supported")
+                    f"Bounding method {bound_method}" " is not supported"
+                )
 
-            
-        return lower,upper
+        return lower, upper
 
-    def compute_HC_lowerbound(self,
-        data,
-        datasize,
-        delta,
-        **kwargs):
+    def compute_HC_lowerbound(self, data, datasize, delta, **kwargs):
         """
         Calculate high confidence lower bound
         Used in safety test
 
-        :param data: 
-            Vector containing base variable  
+        :param data:
+            Vector containing base variable
             evaluated at each observation in dataset
         :type data: numpy ndarray
-        :param datasize: 
+        :param datasize:
             The number of observations in the safety dataset
         :type datasize: int
-        :param delta: 
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
-        """  
-        if 'bound_method' in kwargs:
-            bound_method = kwargs['bound_method']
-            if bound_method == 'ttest': 
-                lower = data.mean() - stddev(data) / np.sqrt(datasize) * tinv(1.0 - delta, datasize - 1)
+        """
+        if "bound_method" in kwargs:
+            bound_method = kwargs["bound_method"]
+            if bound_method == "ttest":
+                lower = data.mean() - stddev(data) / np.sqrt(datasize) * tinv(
+                    1.0 - delta, datasize - 1
+                )
             else:
                 raise NotImplementedError(
-                    f"Bounding method {bound_method}"
-                    " is not supported")
+                    f"Bounding method {bound_method}" " is not supported"
+                )
         return lower
 
-    def compute_HC_upperbound(self,
-        data,
-        datasize,
-        delta,
-        **kwargs):
+    def compute_HC_upperbound(self, data, datasize, delta, **kwargs):
         """
         Calculate high confidence upper bound
         Used in safety test
 
-        :param data: 
-            Vector containing base variable  
+        :param data:
+            Vector containing base variable
             evaluated at each observation in dataset
-        :type data: numpy ndarray 
-        :param datasize: 
+        :type data: numpy ndarray
+        :param datasize:
             The number of observations in the safety dataset
         :type datasize: int
-        :param delta: 
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
         """
-        if 'bound_method' in kwargs:
-            bound_method = kwargs['bound_method']
-            if bound_method == 'ttest':
-                upper = data.mean() + stddev(data) / np.sqrt(datasize) \
-                    * tinv(1.0 - delta, datasize - 1)
+        if "bound_method" in kwargs:
+            bound_method = kwargs["bound_method"]
+            if bound_method == "ttest":
+                upper = data.mean() + stddev(data) / np.sqrt(datasize) * tinv(
+                    1.0 - delta, datasize - 1
+                )
             else:
                 raise NotImplementedError(
-                    f"Bounding method {bound_method}"
-                    " is not supported")
-            
+                    f"Bounding method {bound_method}" " is not supported"
+                )
+
         return upper
-    
-    def compute_HC_upper_and_lowerbound(self,
-        data,
-        datasize,
-        delta,
-        **kwargs):
+
+    def compute_HC_upper_and_lowerbound(self, data, datasize, delta, **kwargs):
         """
         Calculate high confidence lower and upper bounds
         Used in safety test.
-    
+
         Depending on the bound_method,
         this is not always equivalent
-        to calling compute_HC_lowerbound() and 
+        to calling compute_HC_lowerbound() and
         compute_HC_upperbound() independently.
 
-        :param data: 
-            Vector containing base variable  
+        :param data:
+            Vector containing base variable
             evaluated at each observation in dataset
-        :type data: numpy ndarray 
-        :param datasize: 
+        :type data: numpy ndarray
+        :param datasize:
             The number of observations in the safety dataset
         :type datasize: int
-        :param delta: 
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
         """
-        if 'bound_method' in kwargs:
-            bound_method = kwargs['bound_method']
-            if bound_method == 'ttest':
-                lower = self.compute_HC_lowerbound(data=data,
-                    datasize=datasize,delta=delta/2,
-                    **kwargs)
-                upper = self.compute_HC_upperbound(data=data,
-                    datasize=datasize,delta=delta/2,
-                    **kwargs)
+        if "bound_method" in kwargs:
+            bound_method = kwargs["bound_method"]
+            if bound_method == "ttest":
+                lower = self.compute_HC_lowerbound(
+                    data=data, datasize=datasize, delta=delta / 2, **kwargs
+                )
+                upper = self.compute_HC_upperbound(
+                    data=data, datasize=datasize, delta=delta / 2, **kwargs
+                )
 
-            elif bound_method == 'manual':
+            elif bound_method == "manual":
                 pass
             else:
                 raise NotImplementedError(
-                    f"Bounding method {bound_method}"
-                    " is not supported")
+                    f"Bounding method {bound_method}" " is not supported"
+                )
         else:
-            raise NotImplementedError("Have not implemented" 
-                    "confidence bounds without the keyword bound_method")
+            raise NotImplementedError(
+                "Have not implemented"
+                "confidence bounds without the keyword bound_method"
+            )
+
+        return lower, upper
 
-        return lower,upper
- 
 
 class ConfusionMatrixBaseNode(BaseNode):
-    def __init__(self,
+    def __init__(
+        self,
         name,
         cm_true_index,
         cm_pred_index,
-        lower=float('-inf'),
-        upper=float('inf'),
+        lower=float("-inf"),
+        upper=float("inf"),
         conditional_columns=[],
-        **kwargs):
-        """ A confusion matrix base node. 
+        **kwargs,
+    ):
+        """A confusion matrix base node.
         Inherits all of the attributes/methods
         of basenode and sets the i,j indices
         of the K x K confusion matrix, C:
 
         ::
 
                             Predicted labels
@@ -586,300 +587,349 @@
                         |______|______|_____|_____|
             True    i=1 | C_10 | C_11 | ... | C_1K|
             labels      |______|______|_____|_____|
                     ... | ...  | ...  | ... | ... |
                         |______|______|_____|_____|
                     i=K | C_K0 | C_K1 | ... | C_KK|
                         |______|______|_____|_____|
-                        
-        :param name: 
+
+        :param name:
             The name of the node
         :type name: str
-        :param cm_true_index: 
-            The index of the row in the confusion matrix. 
+        :param cm_true_index:
+            The index of the row in the confusion matrix.
             Rows are the true values
-        :param cm_pred_index: 
+        :param cm_pred_index:
             The index of the column in the confusion matrix.
             Columns are the predicted values
-        :param lower: 
+        :param lower:
             Lower confidence bound
         :type lower: float
-        :param upper: 
+        :param upper:
             Upper confidence bound
         :type upper: float
-        :param conditional_columns: 
-            When calculating confidence bounds on a measure 
+        :param conditional_columns:
+            When calculating confidence bounds on a measure
             function, condition on these columns being == 1
         :type conditional_columns: List(str)
         """
         super().__init__(
             name=name,
             lower=lower,
             upper=upper,
             conditional_columns=conditional_columns,
-            **kwargs)
+            **kwargs,
+        )
         self.cm_true_index = cm_true_index
         self.cm_pred_index = cm_pred_index
 
 
 class MultiClassBaseNode(BaseNode):
-    def __init__(self,
+    def __init__(
+        self,
         name,
         class_index,
-        lower=float('-inf'),
-        upper=float('inf'),
+        lower=float("-inf"),
+        upper=float("inf"),
         conditional_columns=[],
-        **kwargs):
-        """ A base node for computing 
-        the classification statistic 
+        **kwargs,
+    ):
+        """A base node for computing
+        the classification statistic
         for a single class against all
-        other classes. For example, 
-        if one has 3 classes and wants the 
+        other classes. For example,
+        if one has 3 classes and wants the
         false positive rate of the first class,
         they would write "FPR_[0]" in their constraint
         and we would calculate the rate at which
         the model predicted class 0 when the true
         label was not class 0 (i.e., class 1 or 2).
         Inherits all of the attributes/methods
-        of basenode 
-                        
-        :param name: 
+        of basenode
+
+        :param name:
             The name of the node, e.g. "FPR_[0]"
         :type name: str
-        :param class_index: 
+        :param class_index:
             The class index against which to calculate
             the statistic, e.g. false positive rate
-        :param lower: 
+        :param lower:
             Lower confidence bound
         :type lower: float
-        :param upper: 
+        :param upper:
             Upper confidence bound
         :type upper: float
-        :param conditional_columns: 
-            When calculating confidence bounds on a measure 
+        :param conditional_columns:
+            When calculating confidence bounds on a measure
             function, condition on these columns being == 1
         :type conditional_columns: List(str)
         """
         super().__init__(
             name=name,
             lower=lower,
             upper=upper,
             conditional_columns=conditional_columns,
-            **kwargs)
+            **kwargs,
+        )
         self.class_index = class_index
 
 
-class MEDCustomBaseNode(BaseNode):
-    def __init__(self,
+class RLAltRewardBaseNode(BaseNode):
+    def __init__(
+        self,
         name,
-        lower=float('-inf'),
-        upper=float('inf'),
-        **kwargs):
-        """ 
+        alt_reward_number,
+        lower=float("-inf"),
+        upper=float("inf"),
+        conditional_columns=[],
+        **kwargs,
+    ):
+        """A base node for computing
+        the IS estimate using an alternate
+        reward function (i.e. one besides the primary reward).
+        There can be an arbitrary number of
+        alternate rewards, so the "alt_reward_number"
+        attribute allows one to reference the specific
+        alternate reward. These are 1-indexed,
+        so if one wants to reference the second
+        alternate reward, the base node string would be:
+        "J_pi_new_[2]"
+        Inherits all of the attributes/methods
+        of basenode
+
+        :param name:
+            The name of the node, e.g. "J_pi_new_[1]"
+        :type name: str
+        :param alt_reward_number:
+            Which alternate reward to use when
+            calculating the IS estimate. 1-indexed.
+        :param lower:
+            Lower confidence bound
+        :type lower: float
+        :param upper:
+            Upper confidence bound
+        :type upper: float
+        :param conditional_columns:
+            When calculating confidence bounds on a measure
+            function, condition on these columns being == 1
+        :type conditional_columns: List(str)
+        """
+        super().__init__(
+            name=name,
+            lower=lower,
+            upper=upper,
+            conditional_columns=conditional_columns,
+            **kwargs,
+        )
+        self.alt_reward_number = alt_reward_number
+
+
+class MEDCustomBaseNode(BaseNode):
+    def __init__(self, name, lower=float("-inf"), upper=float("inf"), **kwargs):
+        """
         Custom base node that calculates pair-wise
         mean error differences between male and female
-        points. This was used in the Seldonian regression algorithm 
+        points. This was used in the Seldonian regression algorithm
         presented by Thomas et al. (2019):
         https://www.science.org/stoken/author-tokens/ST-119/full
         see Figure 2.
 
-        Overrides several parent class methods 
-        
-        :param name: 
+        Overrides several parent class methods
+
+        :param name:
             The name of the node
         :type name: str
-        
-        :param lower: 
+
+        :param lower:
             Lower confidence bound
         :type lower: float
-        
-        :param upper: 
+
+        :param upper:
             Upper confidence bound
         :type upper: float
 
-        :ivar delta: 
+        :ivar delta:
             The share of the confidence put into this node
         :vartype delta: float
         """
-        super().__init__(name,lower,upper,**kwargs)
-        
-    def calculate_data_forbound(self,**kwargs):
-        """ 
+        super().__init__(name, lower, upper, **kwargs)
+
+    def calculate_data_forbound(self, **kwargs):
+        """
         Overrides same method from parent class, :py:class:`.BaseNode`
         """
-        dataset = kwargs['dataset']
+        dataset = kwargs["dataset"]
         features = dataset.features
-        labels = np.expand_dims(dataset.labels,axis=1)
+        labels = np.expand_dims(dataset.labels, axis=1)
         sensitive_attrs = dataset.sensitive_attrs
-        
-        data_dict,datasize = self.precalculate_data(
-            features,labels,sensitive_attrs)
-
-        if kwargs['branch'] == 'candidate_selection':
-            n_safety = kwargs['n_safety']
-            frac_masked = datasize/len(features)
-            datasize = int(round(frac_masked*n_safety))
-
-        return data_dict,datasize
-
-    def precalculate_data(self,X,Y,S):
-        """ 
-        Preconfigure dataset for candidate selection or 
-        safety test so that it does not need to be 
+
+        data_dict, datasize = self.precalculate_data(features, labels, sensitive_attrs)
+
+        if kwargs["branch"] == "candidate_selection":
+            n_safety = kwargs["n_safety"]
+            frac_masked = datasize / len(features)
+            datasize = int(round(frac_masked * n_safety))
+
+        return data_dict, datasize
+
+    def precalculate_data(self, X, Y, S):
+        """
+        Preconfigure dataset for candidate selection or
+        safety test so that it does not need to be
         recalculated on each iteration through the parse tree
 
         :param X: features
         :type X: pandas dataframe
 
         :param Y: labels
-        :type Y: pandas dataframe       
+        :type Y: pandas dataframe
         """
-        male_mask = S[:,0] == 1
-        
+        male_mask = S[:, 0] == 1
+
         X_male = X[male_mask]
         Y_male = Y[male_mask]
         X_female = X[~male_mask]
         Y_female = Y[~male_mask]
         N_male = len(X_male)
         N_female = len(X_female)
-        N_least = min(N_male,N_female)
-        
-        # sample N_least from both without repeats 
-        XY_male = np.hstack([X_male,Y_male]) # column stack
-        ix_sample_male = np.random.choice(range(len(XY_male))
-            ,size=N_least,replace=True)
-        XY_male = XY_male[ix_sample_male,:]
-        X_male = XY_male[:,:-1]
-        Y_male = XY_male[:,-1]
-
-        XY_female = np.hstack([X_female,Y_female]) # column stack
-        ix_sample_female = np.random.choice(range(len(XY_female)),
-            size=N_least,replace=True)
-        XY_female = XY_female[ix_sample_female,:]
-        X_female = XY_female[:,:-1]
-        Y_female = XY_female[:,-1]
-        
+        N_least = min(N_male, N_female)
+
+        # sample N_least from both without repeats
+        XY_male = np.hstack([X_male, Y_male])  # column stack
+        ix_sample_male = np.random.choice(
+            range(len(XY_male)), size=N_least, replace=True
+        )
+        XY_male = XY_male[ix_sample_male, :]
+        X_male = XY_male[:, :-1]
+        Y_male = XY_male[:, -1]
+
+        XY_female = np.hstack([X_female, Y_female])  # column stack
+        ix_sample_female = np.random.choice(
+            range(len(XY_female)), size=N_least, replace=True
+        )
+        XY_female = XY_female[ix_sample_female, :]
+        X_female = XY_female[:, :-1]
+        Y_female = XY_female[:, -1]
+
         data_dict = {
-            'X_male':X_male,
-            'Y_male':Y_male,
-            'X_female':X_female,
-            'Y_female':Y_female}
-        datasize=N_least
-        return data_dict,datasize
+            "X_male": X_male,
+            "Y_male": Y_male,
+            "X_female": X_female,
+            "Y_female": Y_female,
+        }
+        datasize = N_least
+        return data_dict, datasize
 
-    def zhat(self,model,theta,data_dict,**kwargs):
+    def zhat(self, model, theta, data_dict, **kwargs):
         """
         Pair up male and female columns and compute a vector of:
         (y_i - y_hat_i | M) - (y_j - y_hat_j | F).
         There may not be the same number of male and female rows
         so the number of pairs is min(N_male,N_female)
 
         :param model: machine learning model
         :type model: models.SeldonianModel object
 
-        :param theta: 
+        :param theta:
             model weights
         :type theta: numpy ndarray
-        
-        :param data_dict: 
-            contains inputs to model, 
+
+        :param data_dict:
+            contains inputs to model,
             such as features and labels
         :type data_dict: dict
         """
-        X_male = data_dict['X_male']
-        Y_male = data_dict['Y_male']
-        X_female = data_dict['X_female']
-        Y_female = data_dict['Y_female']
+        X_male = data_dict["X_male"]
+        Y_male = data_dict["Y_male"]
+        X_female = data_dict["X_female"]
+        Y_female = data_dict["Y_female"]
 
-        prediction_male = model.predict(theta,X_male)
-        mean_error_male = prediction_male-Y_male
+        prediction_male = model.predict(theta, X_male)
+        mean_error_male = prediction_male - Y_male
 
-        prediction_female = model.predict(theta,X_female)
-        mean_error_female = prediction_female-Y_female
+        prediction_female = model.predict(theta, X_female)
+        mean_error_female = prediction_female - Y_female
 
         return mean_error_male - mean_error_female
 
- 
+
 class CVaRSQeBaseNode(BaseNode):
-    def __init__(self,
-        name,
-        lower=float('-inf'),
-        upper=float('inf'),
-        **kwargs):
-        """ 
-        Custom base node that calculates the upper and 
+    def __init__(self, name, lower=float("-inf"), upper=float("inf"), **kwargs):
+        """
+        Custom base node that calculates the upper and
         lower bounds on CVaR_alpha (with alpha fixed to 0.1)
         of the squared error. We are using the positive
-        definition of CVaR_alpha, i.e. "...the expected value 
+        definition of CVaR_alpha, i.e. "...the expected value
         if we only consider the samples that are at least VaR_alpha,"
         where VaR_alpha "... is the largest value such that at least 100*alpha%
         of samples will be larger than it." - Thomas & Miller 2019:
         https://people.cs.umass.edu/~pthomas/papers/Thomas2019.pdf
         See Theorem 3 for upper bound and Theorem 4 for lower bound
 
-        Overrides several parent class methods 
-        
-        :param name: 
+        Overrides several parent class methods
+
+        :param name:
             The name of the node
         :type name: str
-        :param lower: 
+        :param lower:
             Lower confidence bound
         :type lower: float
-        :param upper: 
+        :param upper:
             Upper confidence bound
         :type upper: float
-        :ivar delta: 
+        :ivar delta:
             The share of the confidence put into this node
         :vartype delta: float
-        :ivar alpha: 
+        :ivar alpha:
             The probability threshold used to define CVAR
         :vartype alpha: float
         """
-        super().__init__(name,lower,upper,**kwargs)
+        super().__init__(name, lower, upper, **kwargs)
         self.alpha = 0.1
-    
-    def calculate_value(self,**kwargs):
+
+    def calculate_value(self, **kwargs):
         """
         Calculate the actual value of CVAR_alpha,
         not the bound.
-        """ 
+        """
         from seldonian.models import objectives
-        model = kwargs['model']
-        theta = kwargs['theta']
-        data_dict = kwargs['data_dict']
+
+        model = kwargs["model"]
+        theta = kwargs["theta"]
+        data_dict = kwargs["data_dict"]
 
         # Get squashed squared errors
-        X = data_dict['features']
-        y = data_dict['labels']
-        squared_errors = objectives.vector_Squared_Error(model,theta,X,y)
+        X = data_dict["features"]
+        y = data_dict["labels"]
+        squared_errors = objectives.vector_Squared_Error(model, theta, X, y)
         # sort
         Z = np.array(sorted(squared_errors))
         # Now calculate cvar
-        percentile_thresh = (1-self.alpha)*100
-        # calculate var_alpha 
-        var_alpha = np.percentile(Z,percentile_thresh)
+        percentile_thresh = (1 - self.alpha) * 100
+        # calculate var_alpha
+        var_alpha = np.percentile(Z, percentile_thresh)
         # cvar is the mean of all values >= var_alpha
         cvar_mask = Z >= var_alpha
         Z_cvar = Z[cvar_mask]
         cvar = np.mean(Z_cvar)
         return cvar
 
-    def calculate_bounds(self,
-        **kwargs):
+    def calculate_bounds(self, **kwargs):
         from seldonian.models import objectives
+
         """Calculate confidence bounds using the concentration 
         inequalities in Thomas & Miller 2019, Theorem's 3 and 4.
-        """ 
-        branch = kwargs['branch']
-        model = kwargs['model']
-        theta = kwargs['theta']
-        data_dict = kwargs['data_dict']
+        """
+        branch = kwargs["branch"]
+        model = kwargs["model"]
+        theta = kwargs["theta"]
+        data_dict = kwargs["data_dict"]
 
-        X = data_dict['features']
-        y = data_dict['labels']
+        X = data_dict["features"]
+        y = data_dict["labels"]
 
         # import matplotlib.pyplot as plt
         # y_hat = model.predict(theta,X)
         # def MSE(y_true,y_pred):
         #     N = len(y_true)
         #     return 1/N*sum(pow(y_true-y_pred,2))
         # mse = MSE(y,y_hat)
@@ -892,248 +942,236 @@
         # ax.set_ylabel("Y")
         # ax.set_title("X=N(0,1), Y=X+N(0,0.2)")
         # ax.legend()
         # plt.show()
         # input("Wait!")
         # assume labels have been clipped to -3,3
         # theoretical min and max (not actual min and max) are:
-        y_min,y_max = -3,3
+        y_min, y_max = -3, 3
         # Increase bounds of y_hat to s times the size of y bounds
-        s=2.0
-        y_hat_min = y_min*(1+s)/2 + y_max*(1-s)/2
-        y_hat_max = y_max*(1+s)/2 + y_min*(1-s)/2
+        s = 2.0
+        y_hat_min = y_min * (1 + s) / 2 + y_max * (1 - s) / 2
+        y_hat_max = y_max * (1 + s) / 2 + y_min * (1 - s) / 2
 
         min_squared_error = 0
-        max_squared_error = max(
-            pow(y_hat_max-y_min,2),
-            pow(y_max - y_hat_min,2))
-        
-        squared_errors = objectives.vector_Squared_Error(model,theta,X,y)
+        max_squared_error = max(pow(y_hat_max - y_min, 2), pow(y_max - y_hat_min, 2))
+
+        squared_errors = objectives.vector_Squared_Error(model, theta, X, y)
 
-        a=min_squared_error
-        b=max_squared_error
+        a = min_squared_error
+        b = max_squared_error
         # Need to sort squared errors to get Z1, ..., Zn
         sorted_squared_errors = sorted(squared_errors)
 
         bound_kwargs = {
-            "Z":sorted_squared_errors,
-            "delta":self.delta,
-            "n_safety":kwargs['datasize'],
-            "a":a,
-            "b":b
-            }
-        
+            "Z": sorted_squared_errors,
+            "delta": self.delta,
+            "n_safety": kwargs["datasize"],
+            "a": a,
+            "b": b,
+        }
+
         if self.will_lower_bound and self.will_upper_bound:
-            if branch == 'candidate_selection':
+            if branch == "candidate_selection":
                 lower = self.predict_HC_lowerbound(**bound_kwargs)
-                upper = self.predict_HC_upperbound(**bound_kwargs)  
-            elif branch == 'safety_test':
-                lower = self.compute_HC_lowerbound(**bound_kwargs)  
-                upper = self.compute_HC_upperbound(**bound_kwargs)  
-            return {'lower':lower,'upper':upper}
-        
+                upper = self.predict_HC_upperbound(**bound_kwargs)
+            elif branch == "safety_test":
+                lower = self.compute_HC_lowerbound(**bound_kwargs)
+                upper = self.compute_HC_upperbound(**bound_kwargs)
+            return {"lower": lower, "upper": upper}
+
         elif self.will_lower_bound:
-            if branch == 'candidate_selection':
-                lower = self.predict_HC_lowerbound(**bound_kwargs)  
-            elif branch == 'safety_test':
-                lower = self.compute_HC_lowerbound(**bound_kwargs)  
-            return {'lower':lower}
+            if branch == "candidate_selection":
+                lower = self.predict_HC_lowerbound(**bound_kwargs)
+            elif branch == "safety_test":
+                lower = self.compute_HC_lowerbound(**bound_kwargs)
+            return {"lower": lower}
 
         elif self.will_upper_bound:
-            if branch == 'candidate_selection':
-                upper = self.predict_HC_upperbound(**bound_kwargs)  
-            elif branch == 'safety_test':
-                upper = self.compute_HC_upperbound(**bound_kwargs)  
-            return {'upper':upper}
-
-        raise AssertionError("will_lower_bound and will_upper_bound cannot both be False")
-
-    def predict_HC_lowerbound(self,
-        Z,
-        delta,
-        n_safety,
-        a,**kwargs):
+            if branch == "candidate_selection":
+                upper = self.predict_HC_upperbound(**bound_kwargs)
+            elif branch == "safety_test":
+                upper = self.compute_HC_upperbound(**bound_kwargs)
+            return {"upper": upper}
+
+        raise AssertionError(
+            "will_lower_bound and will_upper_bound cannot both be False"
+        )
+
+    def predict_HC_lowerbound(self, Z, delta, n_safety, a, **kwargs):
         """
         Calculate high confidence lower bound
         that we expect to pass the safety test.
         Used in candidate selection
 
-        :param Z: 
+        :param Z:
             Vector containing sorted squared errors
-        :type Z: numpy ndarray of length n_candidate 
-        :param delta: 
+        :type Z: numpy ndarray of length n_candidate
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
-        :param n_safety: 
+        :param n_safety:
             The number of observations in the safety dataset
         :type n_safety: int
         :param a: The minimum possible value of the squared error
         :type a: float
-        """ 
+        """
         Znew = Z.copy()
         Znew = np.array([a] + Znew)
         n_candidate = len(Znew) - 1
 
-        sqrt_term = np.sqrt((np.log(1/delta))/(2*n_safety))
+        sqrt_term = np.sqrt((np.log(1 / delta)) / (2 * n_safety))
         max_term = np.maximum(
             np.zeros(n_candidate),
             np.minimum(
                 np.ones(n_candidate),
-                np.arange(n_candidate)/n_candidate+2*sqrt_term)-(1-self.alpha))
-        
-        lower = Znew[-1] - 1/self.alpha*sum(np.diff(Znew)*max_term)
+                np.arange(n_candidate) / n_candidate + 2 * sqrt_term,
+            )
+            - (1 - self.alpha),
+        )
+
+        lower = Znew[-1] - 1 / self.alpha * sum(np.diff(Znew) * max_term)
 
         return lower
 
-    def predict_HC_upperbound(self,
-        Z,
-        delta,
-        n_safety,
-        b,**kwargs):
+    def predict_HC_upperbound(self, Z, delta, n_safety, b, **kwargs):
         """
         Calculate high confidence upper bound
         that we expect to pass the safety test.
         Used in candidate selection
 
-        :param Z: 
+        :param Z:
             Vector containing sorted squared errors
-        :type Z: numpy ndarray of length n_candidate 
-        :param delta: 
+        :type Z: numpy ndarray of length n_candidate
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
-        :param n_safety: 
+        :param n_safety:
             The number of observations in the safety dataset
         :type n_safety: int
         :param b: The maximum possible value of the squared error
         :type b: float
-        """  
-        assert(0<delta<=0.5)
+        """
+        assert 0 < delta <= 0.5
         Znew = Z.copy()
         Znew.append(b)
-        
+
         n_candidate = len(Znew) - 1
 
         # sqrt term is independent of loop index
-        sqrt_term = np.sqrt((np.log(1/delta))/(2*n_safety))
+        sqrt_term = np.sqrt((np.log(1 / delta)) / (2 * n_safety))
         max_term = np.maximum(
             np.zeros(n_candidate),
-            (1+np.arange(n_candidate))/n_candidate-2*sqrt_term-(1-self.alpha))
-        upper = Znew[-1] - (1/self.alpha)*sum(np.diff(Znew)*max_term)
-            
+            (1 + np.arange(n_candidate)) / n_candidate
+            - 2 * sqrt_term
+            - (1 - self.alpha),
+        )
+        upper = Znew[-1] - (1 / self.alpha) * sum(np.diff(Znew) * max_term)
+
         return upper
 
-    def compute_HC_lowerbound(self,
-        Z,
-        delta,
-        n_safety,
-        a,**kwargs
-        ):
+    def compute_HC_lowerbound(self, Z, delta, n_safety, a, **kwargs):
         """
         Calculate high confidence lower bound
         Used in safety test.
 
-        :param Z: 
+        :param Z:
             Vector containing sorted squared errors
-        :type Z: numpy ndarray of length n_safety       
-        :param delta: 
+        :type Z: numpy ndarray of length n_safety
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
-        :param n_safety: 
+        :param n_safety:
             The number of observations in the safety dataset
         :type n_safety: int
         :param a: The minimum possible value of the squared error
         :type a: float
-        """  
+        """
         Znew = Z.copy()
         Znew = np.array([a] + Znew)
         n_candidate = len(Znew) - 1
 
-        sqrt_term = np.sqrt((np.log(1/delta))/(2*n_safety))
+        sqrt_term = np.sqrt((np.log(1 / delta)) / (2 * n_safety))
         max_term = np.maximum(
             np.zeros(n_safety),
-            np.minimum(
-                np.ones(n_safety),
-                np.arange(n_safety)/n_safety+sqrt_term)-(1-self.alpha))
-        
-        lower = Znew[-1] - 1/self.alpha*sum(np.diff(Znew)*max_term)
+            np.minimum(np.ones(n_safety), np.arange(n_safety) / n_safety + sqrt_term)
+            - (1 - self.alpha),
+        )
+
+        lower = Znew[-1] - 1 / self.alpha * sum(np.diff(Znew) * max_term)
 
         return lower
 
-    def compute_HC_upperbound(self,
-        Z,
-        delta,
-        n_safety,
-        b,**kwargs):
+    def compute_HC_upperbound(self, Z, delta, n_safety, b, **kwargs):
         """
         Calculate high confidence upper bound
         Used in safety test
 
-        :param Z: 
+        :param Z:
             Vector containing sorted squared errors
         :type Z: numpy ndarray of length n_safety
-        :param delta: 
+        :param delta:
             Confidence level, e.g. 0.05
         :type delta: float
-        :param n_safety: 
+        :param n_safety:
             The number of observations in the safety dataset
         :type n_safety: int
         :param b: The maximum possible value of the squared error
         :type b: float
         """
-        assert(0<delta<=0.5)
+        assert 0 < delta <= 0.5
         Znew = Z.copy()
         Znew.append(b)
         # sqrt term is independent of loop index
-        sqrt_term = np.sqrt((np.log(1/delta))/(2*n_safety))
+        sqrt_term = np.sqrt((np.log(1 / delta)) / (2 * n_safety))
         max_term = np.maximum(
             np.zeros(n_safety),
-            (1+np.arange(n_safety))/n_safety-sqrt_term-(1-self.alpha))
-        upper = Znew[-1] - 1/self.alpha*sum(np.diff(Znew)*max_term)
-            
+            (1 + np.arange(n_safety)) / n_safety - sqrt_term - (1 - self.alpha),
+        )
+        upper = Znew[-1] - 1 / self.alpha * sum(np.diff(Znew) * max_term)
+
         return upper
-    
-    
+
+
 class ConstantNode(Node):
-    def __init__(self,name,value,**kwargs):
-        """ 
-        Class for constant leaf nodes 
+    def __init__(self, name, value, **kwargs):
+        """
+        Class for constant leaf nodes
         in the parse tree. Sets lower and upper
         bound as the value of the constant.
 
-        :param name: 
+        :param name:
             The name of the node
         :type name: str
-        :param value: 
+        :param value:
             The value of the constant the node represents
         :type value: float
-        :ivar node_type: 
+        :ivar node_type:
             'constant_node'
         :vartype node_type: str
         """
-        super().__init__(name=name,
-            lower=value,upper=value,**kwargs)
+        super().__init__(name=name, lower=value, upper=value, **kwargs)
         self.value = value
-        self.node_type = 'constant_node'
-  
+        self.node_type = "constant_node"
+
 
 class InternalNode(Node):
-    def __init__(self,name,
-        lower=float('-inf'),upper=float('inf'),**kwargs):
-        """ 
-        Class for internal (non-leaf) nodes 
+    def __init__(self, name, lower=float("-inf"), upper=float("inf"), **kwargs):
+        """
+        Class for internal (non-leaf) nodes
         in the parse tree.
         These represent operators, such as +,-,*,/ etc.
 
-        :param name: 
-            The name of the node, which is the 
-            string representation of the operation 
+        :param name:
+            The name of the node, which is the
+            string representation of the operation
             the node performs
         :type name: str
-        :param lower: 
+        :param lower:
             Lower confidence bound
         :type lower: float
-        :param upper: 
+        :param upper:
             Upper confidence bound
         :type upper: float
         """
-        super().__init__(name,lower,upper,**kwargs)
-        self.node_type = 'internal_node'
+        super().__init__(name, lower, upper, **kwargs)
+        self.node_type = "internal_node"
```

### Comparing `seldonian_engine-0.7.9/seldonian/utils/io_utils.py` & `seldonian_engine-0.8.0/seldonian/utils/io_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 import os
 import pickle
 import json
 
+
 def dir_path(path):
-    """ A utility for checking whether a path is a directory
+    """A utility for checking whether a path is a directory
 
     :param path: An input path that may or may not be a directory
     :type path: str
     """
     if os.path.isdir(path):
         return path
     else:
         raise NotADirectoryError(path)
 
+
 def load_pickle(filename):
-    """ A wrapper for loading an object from a pickle file
+    """A wrapper for loading an object from a pickle file
 
     :param filename: A filename pointing to a pickle file
     :type filename: str
     """
-    with open(filename,'rb') as infile:
+    with open(filename, "rb") as infile:
         data = pickle.load(infile)
     return data
 
-def save_pickle(filename,data,verbose=False):
-    """ A wrapper for saving an object to a pickle file
+
+def save_pickle(filename, data, verbose=False):
+    """A wrapper for saving an object to a pickle file
 
     :param filename: A filename for the saved pickle file
     :type filename: str
     :param data: The object you want to pickle
     :type data: Pickle-able object
     :param verbose: Boolean verbosity flag
     """
-    with open(filename,'wb') as outfile:
-        pickle.dump(data,outfile,protocol=pickle.HIGHEST_PROTOCOL)
+    with open(filename, "wb") as outfile:
+        pickle.dump(data, outfile, protocol=pickle.HIGHEST_PROTOCOL)
         if verbose:
             print(f"Saved {filename}\n")
 
+
 def load_json(filename):
-    """ A wrapper for loading an object from a JSON file
+    """A wrapper for loading an object from a JSON file
 
     :param filename: An input filename pointing to a JSON file
     :type filename: str
     """
-    with open(filename,'r') as infile:
+    with open(filename, "r") as infile:
         data = json.load(infile)
     return data
 
-def save_json(filename,data,indent=2,verbose=False):
-    """ A wrapper for saving an object to a JSON file
+
+def save_json(filename, data, indent=2, verbose=False):
+    """A wrapper for saving an object to a JSON file
 
     :param filename: A filename where the JSON file will be saved
     :type filename: str
     """
-    with open(filename,'w') as outfile:
-        data = json.dump(data,outfile)
+    with open(filename, "w") as outfile:
+        data = json.dump(data, outfile)
     if verbose:
         print(f"Saved {filename}\n")
-
```

### Comparing `seldonian_engine-0.7.9/seldonian/utils/tutorial_utils.py` & `seldonian_engine-0.8.0/seldonian/utils/tutorial_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,133 +1,137 @@
-import autograd.numpy as np   # Thinly-wrapped version of Numpy
+import autograd.numpy as np  # Thinly-wrapped version of Numpy
 import pandas as pd
 
-from seldonian.dataset import SupervisedDataSet
+from seldonian.dataset import SupervisedDataSet,SupervisedMetaData
 from seldonian.parse_tree.parse_tree import ParseTree
 
 
-def generate_data(
-    num_points,
-    loc_X=0.0,
-    loc_Y=0.0,
-    sigma_X=1.0,
-    sigma_Y=1.0):
-    """ Generate 2D random normal data
-    
+def generate_data(num_points, loc_X=0.0, loc_Y=0.0, sigma_X=1.0, sigma_Y=1.0):
+    """Generate 2D random normal data
+
     :param num_points: The number of data points to generate
     :type num_points: int
-    :param loc_X: The mean of the normal distribution 
+    :param loc_X: The mean of the normal distribution
         in the X dimension
     :type loc_X: float
-    :param loc_Y: The mean of the normal distribution 
+    :param loc_Y: The mean of the normal distribution
         in the Y dimension
     :type loc_Y: float
-    :param sigma_X: The standard deviation of the normal distribution 
+    :param sigma_X: The standard deviation of the normal distribution
         in the X dimension
     :type sigma_X: float
-    :param sigma_Y: The standard deviation of the normal distribution 
+    :param sigma_Y: The standard deviation of the normal distribution
         in the Y dimension
     :type sigma_Y: float
     """
-    X =     np.random.normal(loc_X, sigma_X, num_points) # Sample x from a standard normal distribution
-    Y = X + np.random.normal(loc_Y, sigma_Y, num_points) # Set y to be x, plus noise from a standard normal distribution
-    return (X,Y)
+    X = np.random.normal(
+        loc_X, sigma_X, num_points
+    )  # Sample x from a standard normal distribution
+    Y = X + np.random.normal(
+        loc_Y, sigma_Y, num_points
+    )  # Set y to be x, plus noise from a standard normal distribution
+    return (X, Y)
 
 
 def generate_clipped_data(
-    num_points,
-    loc_X=0.0,
-    loc_Y=0.0,
-    sigma_X=1.0,
-    sigma_Y=1.0,
-    clip_min=-3,
-    clip_max=3):
-    """ Generate 2D random normal data
-    
+    num_points, loc_X=0.0, loc_Y=0.0, sigma_X=1.0, sigma_Y=1.0, clip_min=-3, clip_max=3
+):
+    """Generate 2D random normal data
+
     :param num_points: The number of data points to generate
     :type num_points: int
-    :param loc_X: The mean of the normal distribution 
+    :param loc_X: The mean of the normal distribution
         in the X dimension
     :type loc_X: float
-    :param loc_Y: The mean of the normal distribution 
+    :param loc_Y: The mean of the normal distribution
         in the Y dimension
     :type loc_Y: float
-    :param sigma_X: The standard deviation of the normal distribution 
+    :param sigma_X: The standard deviation of the normal distribution
         in the X dimension
     :type sigma_X: float
-    :param sigma_Y: The standard deviation of the normal distribution 
+    :param sigma_Y: The standard deviation of the normal distribution
         in the Y dimension
     :type sigma_Y: float
     :param clip_min: Clip values to be >= this value
     :type clip_max: Clip values to be <= this value
     """
-    X =     np.random.normal(loc_X, sigma_X, num_points) # Sample x from a standard normal distribution
-    Y = X + np.random.normal(loc_Y, sigma_Y, num_points) # Set y to be x, plus noise from a standard normal distribution
-    Y = np.clip(Y,clip_min,clip_max)
-    return (X,Y)
+    X = np.random.normal(
+        loc_X, sigma_X, num_points
+    )  # Sample x from a standard normal distribution
+    Y = X + np.random.normal(
+        loc_Y, sigma_Y, num_points
+    )  # Set y to be x, plus noise from a standard normal distribution
+    Y = np.clip(Y, clip_min, clip_max)
+    return (X, Y)
+
 
 def make_synthetic_regression_dataset(
     num_points,
     loc_X=0.0,
     loc_Y=0.0,
     sigma_X=1.0,
     sigma_Y=1.0,
     clipped=False,
     clip_min=-3,
-    clip_max=3):
-    """ Generate 2D dataset from random normal distributions,
+    clip_max=3,
+):
+    """Generate 2D dataset from random normal distributions,
     with optional clipping
-    
+
     :param num_points: The number of data points to generate
     :type num_points: int
-    :param loc_X: The mean of the normal distribution 
+    :param loc_X: The mean of the normal distribution
         in the X dimension
     :type loc_X: float
-    :param loc_Y: The mean of the normal distribution 
+    :param loc_Y: The mean of the normal distribution
         in the Y dimension
     :type loc_Y: float
-    :param sigma_X: The standard deviation of the normal distribution 
+    :param sigma_X: The standard deviation of the normal distribution
         in the X dimension
     :type sigma_X: float
-    :param sigma_Y: The standard deviation of the normal distribution 
+    :param sigma_Y: The standard deviation of the normal distribution
         in the Y dimension
     :type sigma_Y: float
     :param clipped: Boolean flag controlling whether to use clipping
     :param clip_min: Clip values to be >= this value
     :type clip_max: Clip values to be <= this value
     """
     if clipped:
-        X,Y = generate_clipped_data(
+        X, Y = generate_clipped_data(
             num_points=num_points,
             loc_X=loc_X,
             loc_Y=loc_Y,
             sigma_X=sigma_X,
             sigma_Y=sigma_Y,
             clip_min=clip_min,
-            clip_max=clip_max)
-    else: 
-        X,Y = generate_data(
+            clip_max=clip_max,
+        )
+    else:
+        X, Y = generate_data(
             num_points=num_points,
             loc_X=loc_X,
             loc_Y=loc_Y,
             sigma_X=sigma_X,
-            sigma_Y=sigma_Y)
+            sigma_Y=sigma_Y,
+        )
 
     # 2. Define the metadata
-    meta_information = {}
-    meta_information['feature_col_names'] = ['feature1']
-    meta_information['label_col_names'] = ['label']
-    meta_information['sensitive_col_names'] = []
-    meta_information['sub_regime'] = 'regression'
+    meta = SupervisedMetaData(
+        sub_regime="regression",
+        all_col_names=["feature1","label"],
+        feature_col_names = ["feature1"],
+        label_col_names = ["label"]
+    )
 
     # 3. Make a dataset object
-    features = np.expand_dims(X,axis=1)
+    features = np.expand_dims(X, axis=1)
     labels = Y
 
     dataset = SupervisedDataSet(
         features=features,
         labels=labels,
         sensitive_attrs=[],
         num_datapoints=num_points,
-        meta_information=meta_information)
+        meta=meta,
+    )
 
-    return dataset
+    return dataset
```

### Comparing `seldonian_engine-0.7.9/seldonian_engine.egg-info/PKG-INFO` & `seldonian_engine-0.8.0/seldonian_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seldonian-engine
-Version: 0.7.9
+Version: 0.8.0
 Summary: Core library for Seldonian algorithms
 Home-page: 
 Author: Austin Hoag
 Author-email: austinthomashoag@gmail.com
 Project-URL: Bug Tracker, https://github.com/seldonian-framework/Engine/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `seldonian_engine-0.7.9/seldonian_engine.egg-info/SOURCES.txt` & `seldonian_engine-0.8.0/seldonian_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/setup.py` & `seldonian_engine-0.8.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="seldonian_engine",
-    version="0.7.9",
+    version="0.8.0",
     author="Austin Hoag",
     author_email="austinthomashoag@gmail.com",
     description="Core library for Seldonian algorithms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     include_package_data=True,
     url="",
@@ -21,18 +21,18 @@
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         "autograd>=1.4",
         "cma>=3.2.2",
         "graphviz>=0.19.1",
-        "matplotlib==3.5.1", 
+        "matplotlib==3.5.1",
         "numpy>=1.21.4",
         "pandas>=1.4.1",
         "pytest>=7.0.1",
         "scikit_learn>=1.1.1",
         "scipy>=1.7.3",
         "tqdm>=4.64.0",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.8",
-)
+)
```

### Comparing `seldonian_engine-0.7.9/tests/conftest.py` & `seldonian_engine-0.8.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 import autograd.numpy as np   # Thinly-wrapped version of Numpy
 import pytest
 
 from seldonian.parse_tree.parse_tree import *
 from seldonian.utils.io_utils import (load_json,
 	load_pickle)
 from seldonian.utils.tutorial_utils import generate_data
-from seldonian.dataset import (DataSetLoader,
-	RLDataSet,SupervisedDataSet)
+from seldonian.dataset import *
 from seldonian.spec import SupervisedSpec
 from seldonian.models import objectives 
 from seldonian.models.models import *
 
 
 @pytest.fixture
 def stump():
@@ -57,15 +56,15 @@
 	return stump_function
 
 @pytest.fixture
 def edge():
 	def edge_function(operator_type,left_bounds,
 		regime='supervised_learning',sub_regime='classification'):
 		# A parse tree with a single edge
-		assert operator_type in ['abs','exp']
+		assert operator_type in ['abs','exp','log']
 		root = InternalNode(operator_type)
 		root.left = BaseNode('a')
 		pt = ParseTree(delta=0.05,regime=regime,sub_regime=sub_regime)
 		pt.root = root
 		pt.root.left.lower  = left_bounds[0]
 		pt.root.left.upper  = left_bounds[1]
 		pt.n_nodes = 2
@@ -104,19 +103,21 @@
 		np.random.seed(0)
 
 		model = LinearRegressionModelListFeatures() # we don't have a model that supports lists of 
 		# features/arrays yet, but one could create one.
 		X1,Y = generate_data(
 			numPoints,loc_X=0.0,loc_Y=0.0,sigma_X=1.0,sigma_Y=1.0)
 		X2 = X1**2
-		meta_information = {}
-		meta_information['feature_col_names'] = ['feature1']
-		meta_information['label_col_names'] = ['label']
-		meta_information['sensitive_col_names'] = []
-		meta_information['sub_regime'] = sub_regime
+		meta = SupervisedMetaData(
+	        sub_regime="regression", 
+	        all_col_names=["feature1","label"], 
+	        feature_col_names=["feature1"],
+	        label_col_names=["label"],
+	        sensitive_col_names=[]
+	        )
 
 		# 3. Make a dataset object
 		features = [np.expand_dims(X1,axis=1),np.expand_dims(X2,axis=1)]
 		labels = Y
 		sensitive_attrs=list()
 
 		# Mean squared error
@@ -127,15 +128,15 @@
 			regime=regime)
 
 		dataset = SupervisedDataSet(
 			features=features,
 			labels=labels,
 			sensitive_attrs=sensitive_attrs,
 			num_datapoints=numPoints,
-			meta_information=meta_information)
+			meta=meta)
 
 		# For each constraint, make a parse tree
 		parse_trees = []
 		for ii in range(len(constraint_strs)):
 			constraint_str = constraint_strs[ii]
 
 			delta = deltas[ii]
@@ -169,19 +170,21 @@
 		sub_regime='regression'
 		np.random.seed(0)
 
 		model = LinearRegressionModel()
 		X,Y = generate_data(
 			numPoints,loc_X=0.0,loc_Y=0.0,sigma_X=1.0,sigma_Y=1.0)
 		
-		meta_information = {}
-		meta_information['feature_col_names'] = ['feature1']
-		meta_information['label_col_names'] = ['label']
-		meta_information['sensitive_col_names'] = []
-		meta_information['sub_regime'] = sub_regime
+		meta = SupervisedMetaData(
+	        sub_regime="regression", 
+	        all_col_names=["feature1","label"], 
+	        feature_col_names=["feature1"],
+	        label_col_names=["label"],
+	        sensitive_col_names=[]
+	        )
 
 		# 3. Make a dataset object
 		features = np.expand_dims(X,axis=1)
 		labels = Y
 
 		# Mean squared error
 		primary_objective = objectives.Mean_Squared_Error
@@ -191,15 +194,15 @@
 			regime=regime)
 
 		dataset = SupervisedDataSet(
 			features=features,
 			labels=labels,
 			sensitive_attrs=[],
 			num_datapoints=numPoints,
-			meta_information=meta_information)
+			meta=meta)
 
 		# For each constraint, make a parse tree
 		parse_trees = []
 		for ii in range(len(constraint_strs)):
 			constraint_str = constraint_strs[ii]
 
 			delta = deltas[ii]
@@ -469,8 +472,47 @@
 
 		env_kwargs={'gamma':1.0}
 
 		primary_objective = objectives.IS_estimate
 
 		return dataset,policy,env_kwargs,primary_objective
 	
-	return generate_dataset
+	return generate_dataset
+
+@pytest.fixture
+def RL_gridworld_dataset_alt_rewards():
+	from seldonian.RL.environments import gridworld
+	from seldonian.RL.RL_model import RL_model
+	from seldonian.RL.Agents.Policies.Softmax import DiscreteSoftmax
+	from seldonian.RL.Env_Description import Spaces, Env_Description
+
+	def generate_dataset():
+		np.random.seed(0)
+
+		# Load data from file into dataset
+		data_pth = 'static/datasets/RL/gridworld/gridworld_100episodes_2altrewards.pkl'
+		metadata_pth = 'static/datasets/RL/gridworld/gridworld_2altrewards_metadata.json'
+
+		loader = DataSetLoader(
+			regime="reinforcement_learning")
+
+		dataset = loader.load_RL_dataset_from_episode_file(
+			filename=data_pth)
+
+		# Env description 
+		num_states = 9 # 3x3 gridworld
+		observation_space = Spaces.Discrete_Space(0, num_states-1)
+		action_space = Spaces.Discrete_Space(0, 3)
+		env_description = Env_Description.Env_Description(observation_space, action_space)
+		# RL model. setting dict not needed for discrete observation and action space
+		policy = DiscreteSoftmax(
+			env_description=env_description,
+			hyperparam_and_setting_dict={}
+		)
+
+		env_kwargs={'gamma':0.9}
+
+		primary_objective = objectives.IS_estimate
+
+		return dataset,policy,env_kwargs,primary_objective
+	
+	return generate_dataset
```

### Comparing `seldonian_engine-0.7.9/tests/test_RL.py` & `seldonian_engine-0.8.0/tests/test_RL.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from seldonian.RL.Agents.Policies.Softmax import *
 from seldonian.RL.environments.mountaincar import Mountaincar
 from seldonian.RL.environments.n_step_mountaincar import N_step_mountaincar
 from seldonian.RL.environments.gridworld import Gridworld
 from seldonian.RL.Agents.Parameterized_non_learning_softmax_agent import *
 from seldonian.RL.Agents.Discrete_Random_Agent import *
 from seldonian.RL.RL_runner import run_trial
-from seldonian.dataset import RLDataSet
+from seldonian.dataset import RLDataSet,RLMetaData
 import autograd.numpy as np
 
 def test_tables():
     """tests Table class methods"""
 
     min_state = -3
     num_states = 6
@@ -58,23 +58,60 @@
     assert p.from_0_indexed_action_to_environment_action(1) == 0
     assert p.from_0_indexed_action_to_environment_action(2) == 1
 
 def test_Softmax():
     """test Softmax functions"""
     min_action = -1
     max_action = 1
-    observation_space = Discrete_Space(-1, 2)  # irrelevant for test
+    observation_space = Discrete_Space(-1, 2)  
     action_space = Discrete_Space(min_action, max_action)
     env_description = Env_Description(observation_space, action_space)
     hyperparam_and_setting_dict = {}
 
     sm = Softmax(hyperparam_and_setting_dict, env_description)
     e_to_something_stable = np.array([0.1108031584, 0.0040867714, 1.0])
     assert np.allclose(sm.get_e_to_the_something_terms([1.1, -2.2, 3.3]), e_to_something_stable)
     assert np.allclose(sm.get_action_probs_from_action_values([1.1, -2.2, 3.3]), e_to_something_stable / sum(e_to_something_stable))
+    assert sm.get_prob_this_action(0,0) == 1/3
+    assert sm.get_prob_this_action(0,1) == 1/3
+    assert sm.get_prob_this_action(-1,0) == 1/3
+    assert sm.get_prob_this_action(1,-1) == 1/3
+
+def test_MixedSoftmax():
+    """test Mixed Softmax (for policy regularization)"""
+    min_action = -1
+    max_action = 1
+    observation_space = Discrete_Space(-1, 2)  # irrelevant for test
+    action_space = Discrete_Space(min_action, max_action)
+    env_description = Env_Description(observation_space, action_space)
+    hyperparam_and_setting_dict = {}
+
+    alpha1 = 1.0 # mixing hyperparam
+    sm1 = MixedSoftmax(hyperparam_and_setting_dict, env_description, alpha1)
+    e_to_something_stable = np.array([0.1108031584, 0.0040867714, 1.0])
+    assert np.allclose(sm1.get_e_to_the_something_terms([1.1, -2.2, 3.3]), e_to_something_stable)
+    assert np.allclose(sm1.get_action_probs_from_action_values([1.1, -2.2, 3.3]), e_to_something_stable / sum(e_to_something_stable))
+    assert sm1.get_prob_this_action(0,0,1/4) == 1/3
+    assert sm1.get_prob_this_action(0,0,1/2) == 1/3
+
+    alpha2 = 0.0 # mixing hyperparam
+    sm2 = MixedSoftmax(hyperparam_and_setting_dict, env_description, alpha2)
+    e_to_something_stable = np.array([0.1108031584, 0.0040867714, 1.0])
+    assert np.allclose(sm2.get_e_to_the_something_terms([1.1, -2.2, 3.3]), e_to_something_stable)
+    assert np.allclose(sm2.get_action_probs_from_action_values([1.1, -2.2, 3.3]), e_to_something_stable / sum(e_to_something_stable))
+    assert sm2.get_prob_this_action(0,0,1/4) == 1/4
+    assert sm2.get_prob_this_action(0,0,1/2) == 1/2
+
+    alpha3 = 0.5 # mixing hyperparam
+    sm3 = MixedSoftmax(hyperparam_and_setting_dict, env_description, alpha3)
+    e_to_something_stable = np.array([0.1108031584, 0.0040867714, 1.0])
+    assert np.allclose(sm3.get_e_to_the_something_terms([1.1, -2.2, 3.3]), e_to_something_stable)
+    assert np.allclose(sm3.get_action_probs_from_action_values([1.1, -2.2, 3.3]), e_to_something_stable / sum(e_to_something_stable))
+    assert sm3.get_prob_this_action(0,0,1/4) == 1/3*alpha3 + 1/4*(1-alpha3)
+    assert sm3.get_prob_this_action(0,0,1/2) == 1/3*alpha3 + 1/2*(1-alpha3)
 
 def test_Parameterized_non_learning_softmax_agent():
     """test Parameterized_non_learning_softmax_agent"""
     observation_space = Discrete_Space(-1, 2)
     action_space = Discrete_Space(-1, 1)
     env_desc = Env_Description(observation_space, action_space)
     hyperparam_and_setting_dict = {}
@@ -231,15 +268,19 @@
     assert first_observation == 0
     first_action = actions[0]
     assert first_action in [0,1,2,3]
     first_reward = rewards[0]
     assert first_reward == 0
     assert all([pi == 0.25 for pi in pis])
 
-    dataset = RLDataSet(episodes=episodes)
+    meta = RLMetaData(
+        all_col_names=["episode_index", "O", "A", "R", "pi_b"],
+        sensitive_col_names=[]
+    )
+    dataset = RLDataSet(episodes=episodes,meta=meta)
     assert len(dataset.episodes) == 10
 
 def test_generate_n_step_mountaincar_episodes():
     """ Test that we can generate proper episodes for n_step_mountaincar
     with the behavior policy (uniform random). """
     hyperparam_and_setting_dict = {}
     hyperparam_and_setting_dict["env"] = N_step_mountaincar()
@@ -267,9 +308,13 @@
     assert np.allclose(first_observation,np.array([-0.5,0.0]))
     first_action = actions[0]
     assert first_action in [-1,0,1]
     first_reward = rewards[0]
     assert first_reward == -20.0
     assert all([pi == 1/3. for pi in pis])
 
-    dataset = RLDataSet(episodes=episodes)
+    meta = RLMetaData(
+        all_col_names=["episode_index", "O", "A", "R", "pi_b"],
+        sensitive_col_names=[]
+    )
+    dataset = RLDataSet(episodes=episodes,meta=meta)
     assert len(dataset.episodes) == 10
```

### Comparing `seldonian_engine-0.7.9/tests/test_io_utils.py` & `seldonian_engine-0.8.0/tests/test_io_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/tests/test_objectives.py` & `seldonian_engine-0.8.0/tests/test_objectives.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/tests/test_parse_tree.py` & `seldonian_engine-0.8.0/tests/test_parse_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from seldonian.parse_tree.parse_tree import *
 from seldonian.dataset import (DataSetLoader,
 	SupervisedDataSet)
 from seldonian.safety_test.safety_test import SafetyTest
 from seldonian.utils.io_utils import load_json,load_pickle
 from seldonian.models.models import LinearRegressionModel
-from seldonian.dataset import RLDataSet
+from seldonian.dataset import RLDataSet,RLMetaData
 from seldonian.RL.RL_model import RL_model
 
 
 two_interval_options = [
 	[[2.0,3.0],[4.0,5.0]],
 	[[-2.0,1.0],[2.0,3.0]],
 	[[0.5,0.75],[2,4]],
@@ -27,14 +27,15 @@
 	[[0.0,float('inf')],[5.0,10.0]],
 	[[float('-inf'),float('inf')],[5.0,10.0]],
 	[[float('-inf'),float('inf')],[float('-inf'),float('inf')]],
 	[[float('inf'),float('inf')],[float('inf'),float('inf')]],
 ]
 
 single_interval_options = [
+	[1,2],
 	[-3.2,-2.0],
 	[-3.2,2.0],
 	[-5.1,0],
 	[0.0,0.5],
 	[float('-inf'),0.0],
 	[float('-inf'),15342],
 	[0.0,float('inf')],
@@ -153,23 +154,36 @@
 		[-6.8,5.0],
 		[5.0,float('inf')],
 		[5.0,float('inf')],
 		[float('-inf'),float('inf')],
 		[float('inf'),float('inf')]
 	],
 	'abs': [
+		[1.0,2.0],
 		[2.0,3.2],
 		[0,3.2],
 		[0,5.1],
 		[0,0.5],
 		[0,float('inf')],
 		[0,float('inf')],
 		[0,float('inf')],
 		[0,float('inf')],
 		[float('inf'),float('inf')]
+	],
+	'log': [
+		[0.0,np.log(2)],
+		[float('-inf'),float('inf')],
+		[float('-inf'),np.log(2)],
+		[float('-inf'),float('-inf')],
+		[float('-inf'),np.log(0.5)],
+		[float('-inf'),float('-inf')],
+		[float('-inf'),np.log(15342)],
+		[float('-inf'),float('inf')],
+		[float('-inf'),float('inf')],
+		[float('inf'),float('inf')],
 	]
 
 }
 
 ### Begin tests
 
 ########################
@@ -311,14 +325,28 @@
 	pt = edge('abs',a)
 	pt.propagate_bounds()
 	# Use approx due to floating point imprecision
 	assert pt.root.lower == pytest.approx(answer[0])
 	assert pt.root.upper == pytest.approx(answer[1])
 	assert pt.base_node_dict['a']['bound_computed'] == True
 
+@pytest.mark.parametrize('interval_index',range(len(single_interval_options)))
+def test_log_bounds(interval_index,edge):
+	### Absolute value ###
+
+	a=single_interval_options[interval_index]
+	answer = answer_dict['log'][interval_index]
+	pt = edge('log',a)
+	pt.propagate_bounds()
+	# Use approx due to floating point imprecision
+	assert pt.root.lower == pytest.approx(answer[0])
+	assert pt.root.upper == pytest.approx(answer[1])
+	assert pt.base_node_dict['a']['bound_computed'] == True
+
+
 ##################
 ### Node tests ###
 ##################
 
 def test_node_reprs(stump):
 	a,b=[[2.0,3.0],[4.0,5.0]]
 
@@ -545,14 +573,29 @@
 		pt.create_from_ast(constraint_str)
 	
 	error_str = ("Please check the syntax of the function: "
 				f"exp(). "
 				"It appears you provided more than one argument")
 	assert str(excinfo.value) == error_str
 
+
+	constraint_str = 'log((PR | [X]), (PR | [Y]))'
+	delta = 0.05
+	pt = ParseTree(delta,
+		regime='supervised_learning',
+		sub_regime='classification',
+		columns=['X','Y','Z'])
+	with pytest.raises(RuntimeError) as excinfo:
+		pt.create_from_ast(constraint_str)
+	
+	error_str = ("Please check the syntax of the function: "
+				f"log(). "
+				"It appears you provided more than one argument")
+	assert str(excinfo.value) == error_str
+
 	constraint_str = 'max((PR | [X]))'
 	delta = 0.05
 	pt = ParseTree(delta,
 		regime='supervised_learning',
 		sub_regime='classification',
 		columns=['X','Y','Z'])
 	with pytest.raises(RuntimeError) as excinfo:
@@ -717,14 +760,119 @@
 
 	# Make sure error is raised if we use wrong sub_regime
 	pt = ParseTree(delta,regime='supervised_learning',
 		sub_regime='multiclass_classification',columns=['A'])
 	pt.create_from_ast(constraint_str)
 	assert pt.root.right.measure_function_name == 'ACC'
 
+def test_rl_alt_reward_string():
+	delta = 0.05
+	constraint_str = 'J_pi_new_[1] - 0.5'
+
+	pt = ParseTree(delta,regime='reinforcement_learning',
+		sub_regime='all')
+	pt.create_from_ast(constraint_str)
+	assert pt.root.left.measure_function_name == 'J_pi_new'
+	assert pt.root.left.name == 'J_pi_new_[1]'
+	assert pt.root.left.alt_reward_number == 1
+
+
+	constraint_str = '(J_pi_new_[2] | [A,B]) - 0.5'
+	pt = ParseTree(delta,regime='reinforcement_learning',
+		sub_regime='all',columns=['A','B'])
+	pt.create_from_ast(constraint_str)
+	assert pt.root.left.measure_function_name == 'J_pi_new'
+	assert pt.root.left.name == 'J_pi_new_[2] | [A,B]'
+	assert pt.root.left.alt_reward_number == 2
+
+	constraint_str = 'J_pi_new_PDIS_[1] - 0.5'
+
+	pt = ParseTree(delta,regime='reinforcement_learning',
+		sub_regime='all')
+	pt.create_from_ast(constraint_str)
+	assert pt.root.left.measure_function_name == 'J_pi_new_PDIS'
+	assert pt.root.left.name == 'J_pi_new_PDIS_[1]'
+	assert pt.root.left.alt_reward_number == 1
+
+def test_rl_alt_reward_precalc_return():
+	np.random.seed(0)
+	
+	from seldonian.RL.RL_model import RL_model
+	from seldonian.RL.Agents.Policies.Softmax import DiscreteSoftmax
+	from seldonian.RL.Env_Description import Spaces, Env_Description
+	data_pth = 'static/datasets/RL/gridworld/gridworld_100episodes_2altrewards.pkl'
+	loader = DataSetLoader(regime="reinforcement_learning")
+	dataset = loader.load_RL_dataset_from_episode_file(data_pth)
+	
+	# Initialize policy
+	num_states = 9
+	observation_space = Spaces.Discrete_Space(0, num_states-1)
+	action_space = Spaces.Discrete_Space(0, 3)
+	env_description =  Env_Description.Env_Description(observation_space, action_space)
+	policy = DiscreteSoftmax(hyperparam_and_setting_dict={},
+		env_description=env_description)
+	env_kwargs={'gamma':0.9}
+	model = RL_model(policy=policy,env_kwargs=env_kwargs)
+
+	IS_constraint_strs = ['J_pi_new_[1] >= -0.25']
+	IS_deltas=[0.05]
+
+	IS_pt = ParseTree(delta=IS_deltas[0],
+		regime='reinforcement_learning',
+		sub_regime='all',
+		columns=[])
+	
+	IS_pt.create_from_ast(IS_constraint_strs[0])
+	IS_pt.assign_deltas(weight_method='equal')
+
+	# propagate the bounds with example theta value
+	theta = np.random.uniform(-0.05,0.05,(9,4))
+	IS_pt.propagate_bounds(theta=theta,dataset=dataset,
+		model=model,branch='candidate_selection',
+		regime='reinforcement_learning',
+		n_safety=150)
+	assert IS_pt.root.lower == pytest.approx(-0.92395544668)
+	assert IS_pt.root.upper == pytest.approx(8.01612852017466)
+	IS_pt.reset_base_node_dict(reset_data=True)
+	IS_pt.evaluate_constraint(theta=theta,dataset=dataset,
+		model=model,regime='reinforcement_learning',
+		branch='safety_test')
+	assert IS_pt.root.value == pytest.approx(3.5460865367462726)
+
+	weighted_returns_alt_reward = IS_pt.base_node_dict["J_pi_new_[1]"]['data_dict']['weighted_returns']
+	assert weighted_returns_alt_reward[0] == pytest.approx(7.563782445399999)
+
+	PDIS_constraint_strs = ['J_pi_new_PDIS_[1] >= -0.25']
+	PDIS_deltas=[0.05]
+
+	PDIS_pt = ParseTree(delta=PDIS_deltas[0],
+		regime='reinforcement_learning',
+		sub_regime='all',
+		columns=[])
+	
+	PDIS_pt.create_from_ast(PDIS_constraint_strs[0])
+	PDIS_pt.assign_deltas(weight_method='equal')
+
+	# propagate the bounds with example theta value
+	PDIS_pt.propagate_bounds(theta=theta,dataset=dataset,
+		model=model,branch='candidate_selection',
+		regime='reinforcement_learning',
+		n_safety=150)
+	assert PDIS_pt.root.lower == pytest.approx(-0.14631012356483214)
+	assert PDIS_pt.root.upper == pytest.approx(0.3068278441442427)
+	PDIS_pt.reset_base_node_dict(reset_data=True)
+	PDIS_pt.evaluate_constraint(theta=theta,dataset=dataset,
+		model=model,regime='reinforcement_learning',
+		branch='safety_test')
+	assert PDIS_pt.root.value == pytest.approx(0.08025886028)
+
+	weighted_returns_alt_reward = PDIS_pt.base_node_dict["J_pi_new_PDIS_[1]"]['data_dict']['weighted_returns']
+	assert weighted_returns_alt_reward[0] == pytest.approx(7.563782445399999)
+
+
 def test_measure_function_with_conditional_bad_syntax_captured():
 	delta=0.05
 	error_str = ("Error parsing your expression."
 				" The issue is most likely due to"
 				" missing/mismatched parentheses or square brackets"
 				" in a conditional expression involving '|'.")
 
@@ -893,24 +1041,15 @@
 		sub_regime='regression',columns=['M'])
 	with pytest.raises(NotImplementedError) as excinfo:
 		pt.create_from_ast(constraint_str)
 	error_str = ("Error parsing your expression."
 					" A unary operator was used which we do not support: "
 					f"+")
 	assert str(excinfo.value) == error_str
-	# assert pt.root.name == 'sub'
-	# assert pt.root.right.value == 10
-	# assert pt.root.left.name == 'mult'
-	# assert pt.root.left.left.value == -1
-	# assert pt.root.left.right.name == 'abs'
-	# assert pt.root.left.right.left.name == 'Mean_Error | [M]'
-	# assert pt.n_nodes == 6
-	# assert pt.n_base_nodes == 1
-	# assert len(pt.base_node_dict) == 1
-
+	
 def test_raise_error_on_excluded_operators():
 
 	constraint_str = 'FPR^4'
 	delta = 0.05
 	pt = ParseTree(delta,regime='supervised_learning',
 		sub_regime='classification')
 	with pytest.raises(NotImplementedError) as excinfo:
@@ -1000,28 +1139,46 @@
 
 	model_instance = LinearRegressionModel()
 
 	constraint_str = 'exp(FPR - 0.5)'
 	delta = 0.05
 	pt = ParseTree(delta,regime='supervised_learning',
 		sub_regime='classification',
-		columns=dataset.meta_information['sensitive_col_names'])
+		columns=dataset.meta.sensitive_col_names)
 	
 	pt.create_from_ast(constraint_str)
 	pt.assign_deltas(weight_method='equal')
 
 	# propagate the bounds with example theta value
 	# theta = np.hstack([np.array([0.0,0.0]),np.random.uniform(-0.05,0.05,10)])
 	theta = np.random.uniform(-0.05,0.05,10)
 	pt.propagate_bounds(theta=theta,dataset=dataset,
 		model=model_instance,branch='safety_test',
 		regime='supervised_learning')
 	assert pt.root.lower == pytest.approx(0.5990300)
 	assert pt.root.upper == pytest.approx(0.5999346)
 
+	constraint_str = '1+log(FPR)'
+	delta = 0.05
+	pt = ParseTree(delta,regime='supervised_learning',
+		sub_regime='classification',
+		columns=dataset.meta.sensitive_col_names)
+	# pt.build_tree(constraint_str)
+	
+	pt.create_from_ast(constraint_str)
+	pt.assign_deltas(weight_method='equal')
+
+	# propagate the bounds with example theta value
+	theta = np.random.uniform(-0.05,0.05,10)
+	pt.propagate_bounds(theta=theta,dataset=dataset,
+		model=model_instance,branch='safety_test',
+		regime='supervised_learning')
+	assert pt.root.lower == pytest.approx(-2.5187904943528903)
+	assert pt.root.upper == pytest.approx(-2.470509955060809)
+
 def test_deltas_assigned_equally():
 	constraint_str = 'abs((Mean_Error|[M]) - (Mean_Error|[F])) - 0.1'
 	delta = 0.05 
 
 	pt = ParseTree(delta,regime='supervised_learning',
 		sub_regime='regression',columns=['M','F'])
 	pt.create_from_ast(constraint_str)
@@ -1222,22 +1379,22 @@
 			features, labels,test_size=frac_data_in_safety, shuffle=False)
 	
 	candidate_dataset = SupervisedDataSet(
 		features=candidate_features,
 		labels=candidate_labels,
 		sensitive_attrs=[],
 		num_datapoints=len(candidate_features),
-		meta_information=dataset.meta_information)
+		meta=dataset.meta)
 
 	safety_dataset = SupervisedDataSet(
 		features=safety_features,
 		labels=safety_labels,
 		sensitive_attrs=[],
 		num_datapoints=len(safety_features),
-		meta_information=dataset.meta_information)
+		meta=dataset.meta)
 
 	pt = ParseTree(deltas[0],regime='supervised_learning',
 		sub_regime='regression')
 	pt.create_from_ast(constraint_strs[0])
 	pt.assign_deltas(weight_method='equal')
 	pt.assign_bounds_needed()
 	
@@ -1321,22 +1478,22 @@
 	safety_labels = labels[n_candidate:] 
 	
 	candidate_dataset = SupervisedDataSet(
 		features=candidate_features,
 		labels=candidate_labels,
 		sensitive_attrs=[],
 		num_datapoints=len(candidate_features),
-		meta_information=dataset.meta_information)
+		meta=dataset.meta)
 
 	safety_dataset = SupervisedDataSet(
 		features=safety_features,
 		labels=safety_labels,
 		sensitive_attrs=[],
 		num_datapoints=len(safety_features),
-		meta_information=dataset.meta_information)
+		meta=dataset.meta)
 
 	pt = ParseTree(deltas[0],regime='supervised_learning',
 		sub_regime='regression')
 	pt.create_from_ast(constraint_strs[0])
 	pt.assign_deltas(weight_method='equal')
 	pt.assign_bounds_needed()
 	
@@ -1387,22 +1544,22 @@
 			features, labels,test_size=frac_data_in_safety, shuffle=False)
 	
 	candidate_dataset = SupervisedDataSet(
 		features=candidate_features,
 		labels=candidate_labels,
 		sensitive_attrs=[],
 		num_datapoints=len(candidate_features),
-		meta_information=dataset.meta_information)
+		meta=dataset.meta)
 
 	safety_dataset = SupervisedDataSet(
 		features=safety_features,
 		labels=safety_labels,
 		sensitive_attrs=[],
 		num_datapoints=len(safety_features),
-		meta_information=dataset.meta_information)
+		meta=dataset.meta)
 	
 	# First, single sided bound (MSE only needs upper bound)
 
 	pt = ParseTree(deltas[0],regime='supervised_learning',
 		sub_regime='regression')
 	pt.create_from_ast(constraint_strs[0])
 	pt.assign_deltas(weight_method='equal')
@@ -1647,15 +1804,15 @@
 	deltas = [0.05]
 	(dataset,model,
 		primary_objective,parse_trees) = gpa_regression_dataset(
 			constraint_strs,deltas)
 	
 	pt = ParseTree(deltas[0],regime='supervised_learning',
 		sub_regime='regression',
-		columns=dataset.meta_information['sensitive_col_names'])
+		columns=dataset.meta.sensitive_col_names)
 	
 	pt.create_from_ast(constraint_strs[0])
 	pt.assign_deltas(weight_method='equal')
 
 	# propagate the bounds with example theta value
 	# theta = np.hstack([np.array([0.0,0.0]),np.random.uniform(-0.05,0.05,10)])
 	theta = np.random.uniform(-0.05,0.05,10)
@@ -1670,25 +1827,25 @@
 	# Reinforcement learning
 	from seldonian.RL.RL_model import RL_model
 	from seldonian.RL.Agents.Policies.Softmax import DiscreteSoftmax
 	from seldonian.RL.Env_Description import Spaces, Env_Description
 	data_pth = 'static/datasets/RL/gridworld/gridworld_100episodes.pkl'
 
 	episodes = load_pickle(data_pth)
-	RL_meta_information = {
-		'episode_col_names': ['O', 'A', 'R', 'pi_b'],
-		'sensitive_col_names': ['M','F']
-	}
+	RL_meta = RLMetaData(
+		all_col_names=['episode_index','O', 'A', 'R', 'pi_b'],
+		sensitive_col_names=['M','F']
+	)
 	M = np.random.randint(0,2,len(episodes))
 	F = 1-M
 	sensitive_attrs = np.hstack((M.reshape(-1,1),F.reshape(-1,1)))
 	RL_dataset = RLDataSet(
 		episodes=episodes,
 		sensitive_attrs=sensitive_attrs,
-		meta_information=RL_meta_information)
+		meta=RL_meta)
 
 	
 	# Initialize policy
 	num_states = 9
 	observation_space = Spaces.Discrete_Space(0, num_states-1)
 	action_space = Spaces.Discrete_Space(0, 3)
 	env_description =  Env_Description.Env_Description(observation_space, action_space)
@@ -1699,15 +1856,15 @@
 
 	RL_constraint_strs = ['(J_pi_new | [M]) >= -0.25']
 	RL_deltas=[0.05]
 
 	RL_pt = ParseTree(RL_deltas[0],
 		regime='reinforcement_learning',
 		sub_regime='all',
-		columns=RL_dataset.meta_information['sensitive_col_names'])
+		columns=RL_dataset.meta.sensitive_col_names)
 	
 	RL_pt.create_from_ast(RL_constraint_strs[0])
 	RL_pt.assign_deltas(weight_method='equal')
 
 	# propagate the bounds with example theta value
 	# theta = np.hstack([np.array([0.0,0.0]),np.random.uniform(-0.05,0.05,10)])
 	RL_theta = np.random.uniform(-0.05,0.05,(9,4))
@@ -1715,15 +1872,14 @@
 		model=RLmodel,branch='safety_test',
 		regime='reinforcement_learning')
 	assert RL_pt.root.lower == pytest.approx(-0.00556309)
 	assert RL_pt.root.upper == pytest.approx(0.333239520)
 
 	assert len(RL_pt.base_node_dict["J_pi_new | [M]"]['data_dict']['episodes']) == 52
 
-
 def test_build_tree():
 	""" Test the convenience function that builds the tree,
 	weights deltas, and assigns bounds all in one """
 
 	constraint_str = '(FPR + FNR) - 0.5'
 	delta = 0.05
```

### Comparing `seldonian_engine-0.7.9/tests/test_plot_utils.py` & `seldonian_engine-0.8.0/tests/test_plot_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/tests/test_safety_test.py` & `seldonian_engine-0.8.0/tests/test_safety_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
             features, labels,test_size=frac_data_in_safety, shuffle=False)
     
     safety_dataset = SupervisedDataSet(
         features=safety_features,
         labels=safety_labels,
         sensitive_attrs=[],
         num_datapoints=len(safety_features),
-        meta_information=dataset.meta_information)
+        meta=dataset.meta)
 
     # A candidate solution that we know should fail
     candidate_solution = np.array([20,4])
 
     st = SafetyTest(safety_dataset,model,parse_trees)
 
     passed_safety = st.run(candidate_solution)
@@ -82,15 +82,15 @@
             features, labels,test_size=frac_data_in_safety, shuffle=False)
     
     safety_dataset = SupervisedDataSet(
         features=safety_features,
         labels=safety_labels,
         sensitive_attrs=[],
         num_datapoints=len(safety_features),
-        meta_information=dataset.meta_information)
+        meta=dataset.meta)
 
     # A candidate solution that we know is bad
     solution = np.array([20,4])
     st = SafetyTest(safety_dataset,model,parse_trees)
     primary_obj_evl = st.evaluate_primary_objective(solution,primary_objective)
     assert primary_obj_evl == pytest.approx(401.899175)
     
@@ -130,15 +130,15 @@
     candidate_episodes, safety_episodes = train_test_split(
             dataset.episodes,
             test_size=frac_data_in_safety, shuffle=False)
     
     safety_dataset = RLDataSet(
         episodes=safety_episodes,
         num_datapoints=len(safety_episodes),
-        meta_information=dataset.meta_information)
+        meta=dataset.meta)
 
     # A candidate solution that we know is bad
     solution = np.zeros((9,4))
     st = SafetyTest(safety_dataset,model,parse_trees,
         regime=regime)
     primary_obj_evl = st.evaluate_primary_objective(
         solution,primary_objective)
```

### Comparing `seldonian_engine-0.7.9/tests/test_seldonian_algorithm.py` & `seldonian_engine-0.8.0/tests/test_seldonian_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -978,15 +978,15 @@
 		res = SA.get_cs_result()
 	error_str = "Candidate selection has not been run yet, so result is not available."
 	assert error_str in str(excinfo.value)
 	
 	passed_safety,solution = SA.run()
 	res = SA.get_cs_result()
 	res_keys = res.keys()
-	for key in ['candidate_solution', 'best_index', 'best_g', 'best_f', 'theta_vals', 'f_vals', 'g_vals', 'lamb_vals', 'L_vals']:
+	for key in ['candidate_solution', 'best_index', 'best_g', 'best_f', 'f_vals', 'g_vals', 'lamb_vals', 'L_vals']:
 		assert key in res_keys
 
 def test_get_safety_test_result(gpa_regression_dataset):
 	""" Test that the after running the SA on the 
 	gpa regression example, we can get the 
 	dictionary containing the parse trees evaluated 
 	on the safety test. We also test the method
@@ -2093,7 +2093,100 @@
 		passed_safety,solution = SA.run()
 	error_str = (
 				"barrier_function optimization_technique "
 				"is not supported for reinforcement learning. "
 				"Use gradient_descent instead.")
 
 	assert error_str in str(excinfo.value)
+
+def test_RL_gridworld_alt_rewards(RL_gridworld_dataset_alt_rewards):
+	""" Test that we can put constraints on returns that use alternate rewards
+	"""
+	rseed=99
+	np.random.seed(rseed)
+
+	# Vanilla IS first
+	IS_constraint_strs = ['-0.25 - J_pi_new_[1]']
+	deltas = [0.05]
+	
+	IS_parse_trees = make_parse_trees_from_constraints(
+		IS_constraint_strs,
+		deltas,
+		regime='reinforcement_learning',
+		sub_regime='all',
+		columns=[],
+		delta_weight_method='equal')
+	(dataset,policy,
+		env_kwargs,primary_objective) = RL_gridworld_dataset_alt_rewards()
+
+	frac_data_in_safety = 0.6
+	model = RL_model(policy=policy,env_kwargs=env_kwargs)
+	# Create spec object
+	IS_spec = RLSpec(
+		dataset=dataset,
+		model=model,
+		frac_data_in_safety=frac_data_in_safety,
+		use_builtin_primary_gradient_fn=False,
+		primary_objective=primary_objective,
+		initial_solution_fn = None,
+		parse_trees=IS_parse_trees,
+		optimization_technique='gradient_descent',
+		optimizer='adam',
+		optimization_hyperparams={
+			'lambda_init'   : 0.5,
+			'alpha_theta'   : 0.01,
+			'alpha_lamb'    : 0.01,
+			'beta_velocity' : 0.9,
+			'beta_rmsprop'  : 0.95,
+			'num_iters'     : 5,
+			'use_batches'   : False,
+			'gradient_library': "autograd",
+			'hyper_search'  : None,
+			'verbose'       : True,
+		},
+	)
+
+	# # Run seldonian algorithm
+	IS_SA = SeldonianAlgorithm(IS_spec)
+	passed_safety,solution = IS_SA.run()
+
+	## now PDIS
+	PDIS_constraint_strs = ['-0.25 - J_pi_new_PDIS_[1]']
+	deltas = [0.05]
+	
+	PDIS_parse_trees = make_parse_trees_from_constraints(
+		PDIS_constraint_strs,
+		deltas,
+		regime='reinforcement_learning',
+		sub_regime='all',
+		columns=[],
+		delta_weight_method='equal')
+
+	PDIS_spec = RLSpec(
+		dataset=dataset,
+		model=model,
+		frac_data_in_safety=frac_data_in_safety,
+		use_builtin_primary_gradient_fn=False,
+		primary_objective=primary_objective,
+		initial_solution_fn = None,
+		parse_trees=PDIS_parse_trees,
+		optimization_technique='gradient_descent',
+		optimizer='adam',
+		optimization_hyperparams={
+			'lambda_init'   : 0.5,
+			'alpha_theta'   : 0.01,
+			'alpha_lamb'    : 0.01,
+			'beta_velocity' : 0.9,
+			'beta_rmsprop'  : 0.95,
+			'num_iters'     : 5,
+			'use_batches'   : False,
+			'gradient_library': "autograd",
+			'hyper_search'  : None,
+			'verbose'       : True,
+		},
+	)
+
+	# # Run seldonian algorithm
+	PDIS_SA = SeldonianAlgorithm(PDIS_spec)
+	passed_safety,solution = PDIS_SA.run()
+
+
```

### Comparing `seldonian_engine-0.7.9/tests/test_sklearn.py` & `seldonian_engine-0.8.0/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/tests/test_spec.py` & `seldonian_engine-0.8.0/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/tests/test_stats_utils.py` & `seldonian_engine-0.8.0/tests/test_stats_utils.py`

 * *Files identical despite different names*

### Comparing `seldonian_engine-0.7.9/tests/test_tutorial_utils.py` & `seldonian_engine-0.8.0/tests/test_tutorial_utils.py`

 * *Files identical despite different names*

