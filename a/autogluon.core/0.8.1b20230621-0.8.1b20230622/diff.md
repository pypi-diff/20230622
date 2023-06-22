# Comparing `tmp/autogluon.core-0.8.1b20230621.tar.gz` & `tmp/autogluon.core-0.8.1b20230622.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.core-0.8.1b20230621.tar", last modified: Wed Jun 21 09:04:04 2023, max compression
+gzip compressed data, was "autogluon.core-0.8.1b20230622.tar", last modified: Thu Jun 22 09:03:49 2023, max compression
```

## Comparing `autogluon.core-0.8.1b20230621.tar` & `autogluon.core-0.8.1b20230622.tar`

### file list

```diff
@@ -1,122 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.188062 autogluon.core-0.8.1b20230621/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-21 09:04:04.188062 autogluon.core-0.8.1b20230621/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 09:04:04.188062 autogluon.core-0.8.1b20230621/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.176061 autogluon.core-0.8.1b20230621/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.176061 autogluon.core-0.8.1b20230621/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.176061 autogluon.core-0.8.1b20230621/src/autogluon/core/
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/_setup_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.176061 autogluon.core-0.8.1b20230621/src/autogluon/core/augmentation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/augmentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/augmentation/distill_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.180061 autogluon.core-0.8.1b20230621/src/autogluon/core/calibrate/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/calibrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/calibrate/_decision_threshold.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/calibrate/conformity_score.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/calibrate/temperature_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.180061 autogluon.core-0.8.1b20230621/src/autogluon/core/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/data/cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)    14331 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/data/label_cleaner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.180061 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    30240 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/executors.py
--rw-r--r--   0 runner    (1001) docker     (123)    23977 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/ray_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/ray_tune_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/ray_tune_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/ray_tune_searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/space_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.180061 autogluon.core-0.8.1b20230621/src/autogluon/core/learner/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/learner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/learner/abstract_learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.180061 autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)    23214 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18113 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/classification_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/quantile_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/softclass_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.180061 autogluon.core-0.8.1b20230621/src/autogluon/core/models/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.180061 autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    94180 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/abstract_nn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/models/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/dummy/dummy_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59825 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    40465 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4174 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/models/greedy_ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/greedy_ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/problem_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/pseudolabeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/pseudolabeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/pseudolabeling/pseudolabeling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/ray/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/ray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14720 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/ray/resources_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/scheduler/reporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5782 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/scheduler/scheduler_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    15079 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/scheduler/seq_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/dummy_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/local_grid_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/local_random_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9740 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/local_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/searcher_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/task/base/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/task/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6547 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/task/base/base_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.184062 autogluon.core-0.8.1b20230621/src/autogluon/core/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   174249 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/trainer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.188062 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/early_stopping.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    36124 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/feature_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     9624 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/infer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.188062 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/miscs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.188062 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/savers/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/savers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (123)    50798 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-21 09:03:46.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/utils/version_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-21 09:04:04.000000 autogluon.core-0.8.1b20230621/src/autogluon/core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:04:04.176061 autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-21 09:04:04.000000 autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-21 09:04:04.000000 autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:04:04.000000 autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 09:04:04.000000 autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-21 09:04:04.000000 autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-21 09:04:04.000000 autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:04:04.000000 autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.147648 autogluon.core-0.8.1b20230622/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-22 09:03:49.147648 autogluon.core-0.8.1b20230622/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 09:03:49.147648 autogluon.core-0.8.1b20230622/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.135648 autogluon.core-0.8.1b20230622/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.135648 autogluon.core-0.8.1b20230622/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.135648 autogluon.core-0.8.1b20230622/src/autogluon/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/_setup_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/augmentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/augmentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/augmentation/distill_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/calibrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/calibrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/calibrate/_decision_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/calibrate/conformity_score.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/calibrate/temperature_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/data/cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14325 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/data/label_cleaner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29445 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/executors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23387 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/ray_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/ray_tune_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/ray_tune_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/ray_tune_scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/ray_tune_searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/space_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/learner/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/learner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/learner/abstract_learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)    21531 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17849 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/classification_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/quantile_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/softclass_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93846 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/abstract_nn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/models/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/dummy/dummy_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.139648 autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/bagged_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39287 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13377 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/stacker_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/weighted_ensemble_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/models/greedy_ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/greedy_ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/problem_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/pseudolabeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/pseudolabeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/pseudolabeling/pseudolabeling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/ray/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/ray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/ray/resources_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/scheduler/reporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/scheduler/scheduler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14986 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/scheduler/seq_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/dummy_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/local_grid_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/local_random_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9658 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/local_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/searcher_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/task/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/task/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6501 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/task/base/base_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176027 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/trainer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/early_stopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36043 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/feature_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8827 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/infer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/miscs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.143648 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/savers/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/savers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49501 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-06-22 09:03:32.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/utils/version_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-22 09:03:48.000000 autogluon.core-0.8.1b20230622/src/autogluon/core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 09:03:49.135648 autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12720 2023-06-22 09:03:49.000000 autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-22 09:03:49.000000 autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:03:49.000000 autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 09:03:49.000000 autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-22 09:03:49.000000 autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 09:03:49.000000 autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 09:03:49.000000 autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/zip-safe
```

### Comparing `autogluon.core-0.8.1b20230621/PKG-INFO` & `autogluon.core-0.8.1b20230622/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.8.1b20230621
+Version: 0.8.1b20230622
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.8.1b20230621/setup.py` & `autogluon.core-0.8.1b20230622/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,83 +1,86 @@
 #!/usr/bin/env python
 ###########################
 # This code block is a HACK (!), but is necessary to avoid code duplication. Do NOT alter these lines.
+import importlib.util
 import os
+
 from setuptools import setup
-import importlib.util
+
 filepath = os.path.abspath(os.path.dirname(__file__))
-filepath_import = os.path.join(filepath, '..', 'core', 'src', 'autogluon', 'core', '_setup_utils.py')
+filepath_import = os.path.join(filepath, "..", "core", "src", "autogluon", "core", "_setup_utils.py")
 spec = importlib.util.spec_from_file_location("ag_min_dependencies", filepath_import)
 ag = importlib.util.module_from_spec(spec)
 # Identical to `from autogluon.core import _setup_utils as ag`, but works without `autogluon.core` being installed.
 spec.loader.exec_module(ag)
 ###########################
 
 version = ag.load_version_file()
 version = ag.update_version(version)
 
-submodule = 'core'
-install_requires = [
-    # version ranges added in ag.get_dependency_version_ranges()
-    'numpy',
-    'scipy',
-    'scikit-learn',
-    'networkx',
-    'pandas',
-    'tqdm',
-
-    'requests',
-    'matplotlib',
-    'boto3',
-
-    f'autogluon.common=={version}',
-] if not ag.LITE_MODE else [
-    # version ranges added in ag.get_dependency_version_ranges()
-    'numpy',
-    'scipy',
-    'scikit-learn',
-    'pandas',
-    'tqdm',
-    'matplotlib',
-
-    f'{ag.PACKAGE_NAME}.common=={version}',
-]
+submodule = "core"
+install_requires = (
+    [
+        # version ranges added in ag.get_dependency_version_ranges()
+        "numpy",
+        "scipy",
+        "scikit-learn",
+        "networkx",
+        "pandas",
+        "tqdm",
+        "requests",
+        "matplotlib",
+        "boto3",
+        f"autogluon.common=={version}",
+    ]
+    if not ag.LITE_MODE
+    else [
+        # version ranges added in ag.get_dependency_version_ranges()
+        "numpy",
+        "scipy",
+        "scikit-learn",
+        "pandas",
+        "tqdm",
+        "matplotlib",
+        f"{ag.PACKAGE_NAME}.common=={version}",
+    ]
+)
 
 extras_require = {
-    'ray': [
+    "ray": [
         "ray[default]>=2.3,<2.4",
     ],
-    'raytune': [
-        'ray[tune]>=2.3,<2.4',
+    "raytune": [
+        "ray[tune]>=2.3,<2.4",
         # TODO: consider alternatives as hyperopt is not actively maintained.
-        'hyperopt>=0.2.7,<0.2.8',  # This is needed for the bayes search to work.
+        "hyperopt>=0.2.7,<0.2.8",  # This is needed for the bayes search to work.
         # 'GPy>=1.10.0,<1.11.0'  # TODO: Enable this once PBT/PB2 are supported by ray lightning
-    ]
+    ],
 }
 
 tests_require = [
-    'pytest',
-    'types-requests',
-    'types-setuptools',
-    'pytest-mypy',
+    "pytest",
+    "types-requests",
+    "types-setuptools",
+    "pytest-mypy",
     # TODO(Re-enable ray_lightning once it released 0.3.0) 'ray_lightning>=0.2.0,<0.3.0'
 ]
 
 all_requires = []
 
-for extra_package in ['ray', 'raytune']:
+for extra_package in ["ray", "raytune"]:
     all_requires += extras_require[extra_package]
 tests_require = list(set(tests_require))
 all_requires = list(set(all_requires))
-extras_require['tests'] = tests_require
-extras_require['all'] = all_requires
+extras_require["tests"] = tests_require
+extras_require["all"] = all_requires
 
 install_requires = ag.get_dependency_version_ranges(install_requires)
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     ag.create_version_file(version=version, submodule=submodule)
     setup_args = ag.default_setup_args(version=version, submodule=submodule)
     setup(
         install_requires=install_requires,
         extras_require=extras_require,
         **setup_args,
     )
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/__init__.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from  typing import Any
+import warnings
+from typing import Any
+
 from autogluon.common.utils.log_utils import _add_stream_handler
 
+from . import constants, metrics
 from .dataset import TabularDataset
-from . import metrics
-from . import constants
-from .space import Space, Categorical, Real, Int, Bool, spaces
+from .space import Bool, Categorical, Int, Real, Space, spaces
 from .version import __version__
 
 
-import warnings
-
 # TODO: Remove deprecation warning for v1.0
 class DeprecatedSpacesWrapper:
     def __getattr__(self, attr: str) -> Any:
         from autogluon.common import space
 
         if attr in spaces:
             warnings.warn(
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/_setup_utils.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/_setup_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 """Setup utils for autogluon. Only used for installing the code via setup.py, do not import after installation."""
 
 # Refer to https://github.com/scikit-learn/scikit-learn/blob/main/sklearn/_min_dependencies.py for original implementation
 
 import os
 
-AUTOGLUON = 'autogluon'
-PACKAGE_NAME = os.getenv('AUTOGLUON_PACKAGE_NAME', AUTOGLUON)
+AUTOGLUON = "autogluon"
+PACKAGE_NAME = os.getenv("AUTOGLUON_PACKAGE_NAME", AUTOGLUON)
 # TODO: make it more explicit, maybe use another env variable
-LITE_MODE = 'lite' in PACKAGE_NAME
+LITE_MODE = "lite" in PACKAGE_NAME
 
-AUTOGLUON_ROOT_PATH = os.path.abspath(
-    os.path.join(os.path.dirname(os.path.abspath(__file__)), '..', '..', '..', '..')
-)
+AUTOGLUON_ROOT_PATH = os.path.abspath(os.path.join(os.path.dirname(os.path.abspath(__file__)), "..", "..", "..", ".."))
 
-PYTHON_REQUIRES = '>=3.8, <3.11'
+PYTHON_REQUIRES = ">=3.8, <3.11"
 
 
 # Only put packages here that would otherwise appear multiple times across different module's setup.py files.
 DEPENDENT_PACKAGES = {
     # note: if python 3.7 is used, the open CVEs are present: CVE-2021-41496 | CVE-2021-34141; fixes are available in 1.22.x, but python 3.8 only
-    'boto3': '>=1.10,<2',  # <2 because unlikely to introduce breaking changes in minor releases. >=1.10 because 1.10 is 3 years old, no need to support older
-    'numpy': '>=1.21,<1.27',  # "<{N+3}" upper cap, where N is the latest released minor version, assuming no warnings using N
-    'pandas': '>=1.4.1,<1.6',  # "<{N+1}" upper cap
-    'scikit-learn': '>=1.0,<1.3',  # "<{N+1}" upper cap
-    'scipy': '>=1.5.4,<1.12',  # "<{N+2}" upper cap
-    'psutil': '>=5.7.3,<6',  # Major version cap
-    'networkx': '>=3.0,<4',  # Major version cap
-    'tqdm': '>=4.38,<5',  # Major version cap
-    'Pillow': '>=9.3,<9.6',  # "<{N+2}" upper cap
+    "boto3": ">=1.10,<2",  # <2 because unlikely to introduce breaking changes in minor releases. >=1.10 because 1.10 is 3 years old, no need to support older
+    "numpy": ">=1.21,<1.27",  # "<{N+3}" upper cap, where N is the latest released minor version, assuming no warnings using N
+    "pandas": ">=1.4.1,<1.6",  # "<{N+1}" upper cap
+    "scikit-learn": ">=1.0,<1.3",  # "<{N+1}" upper cap
+    "scipy": ">=1.5.4,<1.12",  # "<{N+2}" upper cap
+    "psutil": ">=5.7.3,<6",  # Major version cap
+    "networkx": ">=3.0,<4",  # Major version cap
+    "tqdm": ">=4.38,<5",  # Major version cap
+    "Pillow": ">=9.3,<9.6",  # "<{N+2}" upper cap
 }
 if LITE_MODE:
-    DEPENDENT_PACKAGES = {
-        package: version for package, version in DEPENDENT_PACKAGES.items()
-        if package not in ['psutil', 'Pillow', 'timm']
-    }
+    DEPENDENT_PACKAGES = {package: version for package, version in DEPENDENT_PACKAGES.items() if package not in ["psutil", "Pillow", "timm"]}
 
 DEPENDENT_PACKAGES = {package: package + version for package, version in DEPENDENT_PACKAGES.items()}
 # TODO: Use DOCS_PACKAGES and TEST_PACKAGES
 DOCS_PACKAGES = []
 TEST_PACKAGES = [
-    'flake8',
-    'pytest',
+    "flake8",
+    "pytest",
 ]
 
 
 def load_version_file():
-    with open(os.path.join(AUTOGLUON_ROOT_PATH, 'VERSION')) as version_file:
+    with open(os.path.join(AUTOGLUON_ROOT_PATH, "VERSION")) as version_file:
         version = version_file.read().strip()
     return version
 
 
 def get_dependency_version_ranges(packages: list) -> list:
     return [package if package not in DEPENDENT_PACKAGES else DEPENDENT_PACKAGES[package] for package in packages]
 
@@ -57,96 +52,99 @@
 def update_version(version, use_file_if_exists=True, create_file=False):
     """
     To release a new stable version on PyPi, simply tag the release on github, and the Github CI will automatically publish
     a new stable version to PyPi using the configurations in .github/workflows/pypi_release.yml .
     You need to increase the version number after stable release, so that the nightly pypi can work properly.
     """
     try:
-        if not os.getenv('RELEASE'):
+        if not os.getenv("RELEASE"):
             from datetime import date
-            minor_version_file_path = os.path.join(AUTOGLUON_ROOT_PATH, 'VERSION.minor')
+
+            minor_version_file_path = os.path.join(AUTOGLUON_ROOT_PATH, "VERSION.minor")
             if use_file_if_exists and os.path.isfile(minor_version_file_path):
                 with open(minor_version_file_path) as f:
                     day = f.read().strip()
             else:
                 today = date.today()
                 day = today.strftime("b%Y%m%d")
             version += day
     except Exception:
         pass
-    if create_file and not os.getenv('RELEASE'):
-        with open(os.path.join(AUTOGLUON_ROOT_PATH, 'VERSION.minor'), 'w') as f:
+    if create_file and not os.getenv("RELEASE"):
+        with open(os.path.join(AUTOGLUON_ROOT_PATH, "VERSION.minor"), "w") as f:
             f.write(day)
     return version
 
 
 def create_version_file(*, version, submodule):
-    print('-- Building version ' + version)
+    print("-- Building version " + version)
     if submodule is not None:
-        version_path = os.path.join(AUTOGLUON_ROOT_PATH, submodule, 'src', AUTOGLUON, submodule, 'version.py')
+        version_path = os.path.join(AUTOGLUON_ROOT_PATH, submodule, "src", AUTOGLUON, submodule, "version.py")
     else:
-        version_path = os.path.join(AUTOGLUON_ROOT_PATH, AUTOGLUON, 'src', AUTOGLUON, 'version.py')
-    with open(version_path, 'w') as f:
+        version_path = os.path.join(AUTOGLUON_ROOT_PATH, AUTOGLUON, "src", AUTOGLUON, "version.py")
+    with open(version_path, "w") as f:
         f.write(f'"""This is the {AUTOGLUON} version file."""\n')
         f.write("__version__ = '{}'\n".format(version))
         f.write("__lite__ = {}\n".format(LITE_MODE))
 
 
 def default_setup_args(*, version, submodule):
     from setuptools import find_namespace_packages
-    long_description = open(os.path.join(AUTOGLUON_ROOT_PATH, 'README.md')).read()
+
+    long_description = open(os.path.join(AUTOGLUON_ROOT_PATH, "README.md")).read()
     if submodule is None:
         name = PACKAGE_NAME
     else:
-        name = f'{PACKAGE_NAME}.{submodule}'
+        name = f"{PACKAGE_NAME}.{submodule}"
     setup_args = dict(
         name=name,
         version=version,
-        author='AutoGluon Community',
-        url='https://github.com/autogluon/autogluon',
-        description='AutoML for Image, Text, and Tabular Data',
+        author="AutoGluon Community",
+        url="https://github.com/autogluon/autogluon",
+        description="AutoML for Image, Text, and Tabular Data",
         long_description=long_description,
-        long_description_content_type='text/markdown',
-        license='Apache-2.0',
-        license_files=('../LICENSE', '../NOTICE'),
-
+        long_description_content_type="text/markdown",
+        license="Apache-2.0",
+        license_files=("../LICENSE", "../NOTICE"),
         # Package info
-        packages=find_namespace_packages('src', include=['autogluon.*']),
-        package_dir={'': 'src'},
+        packages=find_namespace_packages("src", include=["autogluon.*"]),
+        package_dir={"": "src"},
         namespace_packages=[AUTOGLUON],
         zip_safe=True,
         include_package_data=True,
         python_requires=PYTHON_REQUIRES,
-        package_data={AUTOGLUON: [
-            'LICENSE',
-        ]},
+        package_data={
+            AUTOGLUON: [
+                "LICENSE",
+            ]
+        },
         classifiers=[
             "Development Status :: 4 - Beta",
             "Intended Audience :: Education",
             "Intended Audience :: Developers",
             "Intended Audience :: Science/Research",
             "Intended Audience :: Customer Service",
             "Intended Audience :: Financial and Insurance Industry",
             "Intended Audience :: Healthcare Industry",
             "Intended Audience :: Telecommunications Industry",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: MacOS",
             "Operating System :: Microsoft :: Windows",
             "Operating System :: POSIX",
             "Operating System :: Unix",
-            'Programming Language :: Python :: 3',
+            "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Topic :: Software Development",
             "Topic :: Scientific/Engineering :: Artificial Intelligence",
             "Topic :: Scientific/Engineering :: Information Analysis",
             "Topic :: Scientific/Engineering :: Image Recognition",
         ],
         project_urls={
-            'Documentation': 'https://auto.gluon.ai',
-            'Bug Reports': 'https://github.com/autogluon/autogluon/issues',
-            'Source': 'https://github.com/autogluon/autogluon/',
-            'Contribute!': 'https://github.com/autogluon/autogluon/blob/master/CONTRIBUTING.md',
+            "Documentation": "https://auto.gluon.ai",
+            "Bug Reports": "https://github.com/autogluon/autogluon/issues",
+            "Source": "https://github.com/autogluon/autogluon/",
+            "Contribute!": "https://github.com/autogluon/autogluon/blob/master/CONTRIBUTING.md",
         },
     )
     return setup_args
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/augmentation/distill_utils.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/augmentation/distill_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,172 +11,180 @@
 from ..constants import BINARY, MULTICLASS, REGRESSION
 from ..metrics import mean_squared_error
 
 logger = logging.getLogger(__name__)
 
 
 def format_distillation_labels(y, problem_type, num_classes=None, eps_labelsmooth=0.01):
-    """ Transforms train/test label objects (y) to the correct type for distillation (smoothed regression targets for binary, one-hot labels for multiclass).
-        eps_labelsmooth : truncates labels to [EPS, 1-EPS], eg. when converting binary problems -> regression
+    """Transforms train/test label objects (y) to the correct type for distillation (smoothed regression targets for binary, one-hot labels for multiclass).
+    eps_labelsmooth : truncates labels to [EPS, 1-EPS], eg. when converting binary problems -> regression
     """
     if problem_type == MULTICLASS:
         y_int = y.to_numpy()
         y = np.zeros((y_int.size, num_classes))
-        y[np.arange(y_int.size),y_int] = 1
+        y[np.arange(y_int.size), y_int] = 1
         y = pd.DataFrame(y)
     elif problem_type == BINARY:
         min_pred = 0.0
         max_pred = 1.0
-        y = eps_labelsmooth + ((1-2*eps_labelsmooth)/(max_pred-min_pred)) * (y - min_pred)
+        y = eps_labelsmooth + ((1 - 2 * eps_labelsmooth) / (max_pred - min_pred)) * (y - min_pred)
     return y
 
 
-def augment_data(X, feature_metadata: FeatureMetadata, augmentation_data=None, augment_method='spunge', augment_args=None):
-    """ augment_method options: ['spunge', 'munge']
-    """
+def augment_data(X, feature_metadata: FeatureMetadata, augmentation_data=None, augment_method="spunge", augment_args=None):
+    """augment_method options: ['spunge', 'munge']"""
     if augment_args is None:
         augment_args = {}
     if augmentation_data is not None:
         X_aug = augmentation_data
     else:
-        if 'num_augmented_samples' not in augment_args:
-            if 'max_size' not in augment_args:
-                augment_args['max_size'] = np.inf
-            augment_args['num_augmented_samples'] = int(min(augment_args['max_size'], augment_args['size_factor']*len(X)))
+        if "num_augmented_samples" not in augment_args:
+            if "max_size" not in augment_args:
+                augment_args["max_size"] = np.inf
+            augment_args["num_augmented_samples"] = int(min(augment_args["max_size"], augment_args["size_factor"] * len(X)))
 
-        if augment_method == 'spunge':
+        if augment_method == "spunge":
             X_aug = spunge_augment(X, feature_metadata, **augment_args)
-        elif augment_method == 'munge':
+        elif augment_method == "munge":
             X_aug = munge_augment(X, feature_metadata, **augment_args)
         else:
             raise ValueError(f"unknown augment_method: {augment_method}")
 
     # return postprocess_augmented(X_aug, X)  # TODO: dropping duplicates is much more efficient, but may skew distribution for entirely-categorical data with few categories.
     logger.log(15, f"Augmented training dataset with {len(X_aug)} extra datapoints")
     return X_aug.reset_index(drop=True)
 
 
 def postprocess_augmented(X_aug, X):
-    """ Drops rows from augmented data that are duplicated (including duplicates that appeared in original data X). """
+    """Drops rows from augmented data that are duplicated (including duplicates that appeared in original data X)."""
     X_aug = pd.concat([X, X_aug])
-    X_aug.drop_duplicates(keep='first', inplace=True)
-    X_aug = X_aug.tail(len(X_aug)-len(X))
+    X_aug.drop_duplicates(keep="first", inplace=True)
+    X_aug = X_aug.tail(len(X_aug) - len(X))
     logger.log(15, f"Augmented training dataset with {len(X_aug)} extra datapoints")
     return X_aug.reset_index(drop=True, inplace=False)
 
 
 # TODO: This can easily be optimized heavily
 def spunge_augment(X, feature_metadata: FeatureMetadata, num_augmented_samples=10000, frac_perturb=0.1, continuous_feature_noise=0.1, **kwargs):
-    """ Generates synthetic datapoints for learning to mimic teacher model in distillation
-        via simplified version of MUNGE strategy (that does not require near-neighbor search).
+    """Generates synthetic datapoints for learning to mimic teacher model in distillation
+    via simplified version of MUNGE strategy (that does not require near-neighbor search).
 
-        Args:
-            num_augmented_samples: number of additional augmented data points to return
-            frac_perturb: fraction of features/examples that are perturbed during augmentation. Set near 0 to ensure augmented sample distribution remains closer to real data.
-            continuous_feature_noise: we noise numeric features by this factor times their std-dev. Set near 0 to ensure augmented sample distribution remains closer to real data.
+    Args:
+        num_augmented_samples: number of additional augmented data points to return
+        frac_perturb: fraction of features/examples that are perturbed during augmentation. Set near 0 to ensure augmented sample distribution remains closer to real data.
+        continuous_feature_noise: we noise numeric features by this factor times their std-dev. Set near 0 to ensure augmented sample distribution remains closer to real data.
     """
     if frac_perturb > 1.0:
         raise ValueError("frac_perturb must be <= 1")
     logger.log(20, f"SPUNGE: Augmenting training data with {num_augmented_samples} synthetic samples for distillation...")
 
     X = X.copy()
-    nan_category = '__NaN__'
+    nan_category = "__NaN__"
     category_featnames = feature_metadata.get_features(valid_raw_types=[R_CATEGORY])
     for feature in category_featnames:
         current_categories = X[feature].cat.categories
         if nan_category in current_categories:
             X[feature] = X[feature].fillna(nan_category)
         else:
             X[feature] = X[feature].cat.add_categories(nan_category).fillna(nan_category)
 
-    num_feature_perturb = max(1, int(frac_perturb*len(X.columns)))
-    X_aug = pd.concat([X.iloc[[0]].copy()]*num_augmented_samples)
+    num_feature_perturb = max(1, int(frac_perturb * len(X.columns)))
+    X_aug = pd.concat([X.iloc[[0]].copy()] * num_augmented_samples)
     X_aug.reset_index(drop=True, inplace=True)
     continuous_types = [R_FLOAT, R_INT]
     continuous_featnames = feature_metadata.get_features(valid_raw_types=continuous_types)  # these features will have shuffled values with added noise
 
-    for i in range(num_augmented_samples): # hot-deck sample some features per datapoint
+    for i in range(num_augmented_samples):  # hot-deck sample some features per datapoint
         og_ind = i % len(X)
         augdata_i = X.iloc[og_ind].copy()
-        num_feature_perturb_i = np.random.choice(range(1,num_feature_perturb+1))  # randomly sample number of features to perturb
+        num_feature_perturb_i = np.random.choice(range(1, num_feature_perturb + 1))  # randomly sample number of features to perturb
         cols_toperturb = np.random.choice(list(X.columns), size=num_feature_perturb_i, replace=False)
         for feature in cols_toperturb:
             feature_data = X[feature]
             augdata_i[feature] = feature_data.sample(n=1).values[0]
         X_aug.iloc[i] = augdata_i
 
     for feature in X.columns:
         if feature in continuous_featnames:
             feature_data = X[feature]
             aug_data = X_aug[feature]
-            noise = np.random.normal(scale=np.nanstd(feature_data)*continuous_feature_noise, size=num_augmented_samples)
+            noise = np.random.normal(scale=np.nanstd(feature_data) * continuous_feature_noise, size=num_augmented_samples)
             mask = np.random.binomial(n=1, p=frac_perturb, size=num_augmented_samples)
-            aug_data = aug_data + noise*mask
+            aug_data = aug_data + noise * mask
             X_aug[feature] = pd.Series(aug_data, index=X_aug.index)
 
     for feature in category_featnames:
         X_aug[feature] = X_aug[feature].cat.remove_categories(nan_category)
 
     return X_aug
 
 
 # TODO: Remove or fix, likely doesn't work anymore
 def munge_augment(X, feature_metadata: FeatureMetadata, num_augmented_samples=10000, perturb_prob=0.5, s=1.0, **kwargs):
-    """ Uses MUNGE algorithm to generate synthetic datapoints for learning to mimic teacher model in distillation: https://www.cs.cornell.edu/~caruana/compression.kdd06.pdf
-        Args:
-            num_augmented_samples: number of additional augmented data points to return
-            perturb_prob: probability of perturbing each feature during augmentation. Set near 0 to ensure augmented sample distribution remains closer to real data.
-            s: We noise numeric features by their std-dev divided by this factor (inverse of continuous_feature_noise). Set large to ensure augmented sample distribution remains closer to real data.
+    """Uses MUNGE algorithm to generate synthetic datapoints for learning to mimic teacher model in distillation: https://www.cs.cornell.edu/~caruana/compression.kdd06.pdf
+    Args:
+        num_augmented_samples: number of additional augmented data points to return
+        perturb_prob: probability of perturbing each feature during augmentation. Set near 0 to ensure augmented sample distribution remains closer to real data.
+        s: We noise numeric features by their std-dev divided by this factor (inverse of continuous_feature_noise). Set large to ensure augmented sample distribution remains closer to real data.
     """
     from autogluon.tabular.models.tabular_nn.torch.tabular_nn_torch import TabularNeuralNetTorchModel
-    nn_dummy = TabularNeuralNetTorchModel(path='nn_dummy', name='nn_dummy', problem_type=REGRESSION, eval_metric=mean_squared_error,
-                                          hyperparameters={'num_dataloading_workers': 0, 'proc.embed_min_categories': np.inf},
-                                          features=list(X.columns), feature_metadata=feature_metadata)
-    processed_data = nn_dummy._process_train_data(df=nn_dummy.preprocess(X),
-                                                  labels=pd.Series([1] * len(X)),
-                                                  batch_size=nn_dummy.params['batch_size'],
-                                                  num_dataloading_workers=0,
-                                                  impute_strategy=nn_dummy.params['proc.impute_strategy'],
-                                                  max_category_levels=nn_dummy.params['proc.max_category_levels'],
-                                                  skew_threshold=nn_dummy.params['proc.skew_threshold'],
-                                                  embed_min_categories=nn_dummy.params['proc.embed_min_categories'],
-                                                  use_ngram_features=nn_dummy.params['use_ngram_features'])
+
+    nn_dummy = TabularNeuralNetTorchModel(
+        path="nn_dummy",
+        name="nn_dummy",
+        problem_type=REGRESSION,
+        eval_metric=mean_squared_error,
+        hyperparameters={"num_dataloading_workers": 0, "proc.embed_min_categories": np.inf},
+        features=list(X.columns),
+        feature_metadata=feature_metadata,
+    )
+    processed_data = nn_dummy._process_train_data(
+        df=nn_dummy.preprocess(X),
+        labels=pd.Series([1] * len(X)),
+        batch_size=nn_dummy.params["batch_size"],
+        num_dataloading_workers=0,
+        impute_strategy=nn_dummy.params["proc.impute_strategy"],
+        max_category_levels=nn_dummy.params["proc.max_category_levels"],
+        skew_threshold=nn_dummy.params["proc.skew_threshold"],
+        embed_min_categories=nn_dummy.params["proc.embed_min_categories"],
+        use_ngram_features=nn_dummy.params["use_ngram_features"],
+    )
     X_vector = processed_data.dataset._data[processed_data.vectordata_index].asnumpy()
     processed_data = None
     nn_dummy = None
     gc.collect()
 
     neighbor_finder = NearestNeighbors(n_neighbors=2)
     neighbor_finder.fit(X_vector)
     neigh_dist, neigh_ind = neighbor_finder.kneighbors(X_vector)
-    neigh_ind = neigh_ind[:,1]  # contains indices of nearest neighbors
+    neigh_ind = neigh_ind[:, 1]  # contains indices of nearest neighbors
     neigh_dist = None
     # neigh_dist = neigh_dist[:,1]  # contains distances to nearest neighbors
     neighbor_finder = None
     gc.collect()
 
     if perturb_prob > 1.0:
         raise ValueError("frac_perturb must be <= 1")
     logger.log(20, f"MUNGE: Augmenting training data with {num_augmented_samples} synthetic samples for distillation...")
     X = X.copy()
-    X_aug = pd.concat([X.iloc[[0]].copy()]*num_augmented_samples)
+    X_aug = pd.concat([X.iloc[[0]].copy()] * num_augmented_samples)
     X_aug.reset_index(drop=True, inplace=True)
-    continuous_types = ['float', 'int']
+    continuous_types = ["float", "int"]
     continuous_featnames = feature_metadata.get_features(valid_raw_types=continuous_types)  # these features will have shuffled values with added noise
     for col in continuous_featnames:
         X_aug[col] = X_aug[col].astype(float)
         X[col] = X[col].astype(float)
 
     for i in range(num_augmented_samples):
         og_ind = i % len(X)
         augdata_i = X.iloc[og_ind].copy()
         neighbor_i = X.iloc[neigh_ind[og_ind]].copy()
         # dist_i = neigh_dist[og_ind]
         cols_toperturb = np.random.choice(list(X.columns), size=np.random.binomial(X.shape[1], p=perturb_prob, size=1)[0], replace=False)
         for col in cols_toperturb:
             new_val = neighbor_i[col]
             if col in continuous_featnames:
-                new_val += np.random.normal(scale=np.abs(augdata_i[col]-new_val)/s)
+                new_val += np.random.normal(scale=np.abs(augdata_i[col] - new_val) / s)
             augdata_i[col] = new_val
         X_aug.iloc[i] = augdata_i
 
     return X_aug
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/calibrate/_decision_threshold.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/calibrate/_decision_threshold.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,85 +10,86 @@
 from ..utils import get_pred_from_proba
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: docstring
 # TODO: Can use a smarter search strategy than brute force for faster speed, such as bayes opt.
-def calibrate_decision_threshold(y: np.array,
-                                 y_pred_proba: np.array,
-                                 metric: Union[Callable, Scorer],
-                                 metric_kwargs: dict | None = None,
-                                 decision_thresholds: Union[int, List[float]] = 50,
-                                 metric_name: str | None = None,
-                                 verbose: bool = True) -> float:
+def calibrate_decision_threshold(
+    y: np.array,
+    y_pred_proba: np.array,
+    metric: Union[Callable, Scorer],
+    metric_kwargs: dict | None = None,
+    decision_thresholds: Union[int, List[float]] = 50,
+    metric_name: str | None = None,
+    verbose: bool = True,
+) -> float:
     problem_type = BINARY
     assert len(y_pred_proba.shape) == 1
     assert len(y.shape) == 1
     assert len(y) == len(y_pred_proba)
 
     if metric_kwargs is None:
         metric_kwargs = dict()
 
     if isinstance(metric, Scorer):
         if metric_name is None:
             metric_name = metric.name
         if not metric.needs_pred:
-            logger.warning(f'WARNING: The provided metric "{metric_name}" does not use class predictions for scoring, '
-                           f'and thus is invalid for decision threshold calibration. '
-                           f'Falling back to `decision_threshold=0.5`.')
+            logger.warning(
+                f'WARNING: The provided metric "{metric_name}" does not use class predictions for scoring, '
+                f"and thus is invalid for decision threshold calibration. "
+                f"Falling back to `decision_threshold=0.5`."
+            )
             return 0.5
-    metric_name_log = f' {metric_name}' if metric_name is not None else ''
+    metric_name_log = f" {metric_name}" if metric_name is not None else ""
 
     if isinstance(decision_thresholds, int):
         # Order thresholds by their proximity to 0.5
         num_checks_half = decision_thresholds
         num_checks = num_checks_half * 2
-        decision_thresholds = [[0.5]] + [[0.5 - (i / num_checks), 0.5 + (i / num_checks)] for i in
-                                         range(1, num_checks_half + 1)]
+        decision_thresholds = [[0.5]] + [[0.5 - (i / num_checks), 0.5 + (i / num_checks)] for i in range(1, num_checks_half + 1)]
         decision_thresholds = [item for sublist in decision_thresholds for item in sublist]
     else:
         for decision_threshold in decision_thresholds:
             if decision_threshold > 1 or decision_threshold < 0:
-                raise ValueError(f'Invalid decision_threshold specified: {decision_threshold} |'
-                                 f' Decision thresholds must be between 0 and 1.')
+                raise ValueError(f"Invalid decision_threshold specified: {decision_threshold} |" f" Decision thresholds must be between 0 and 1.")
     best_score_val = None
     best_threshold = None
 
     y_pred_val = get_pred_from_proba(
         y_pred_proba=y_pred_proba,
         problem_type=problem_type,
         decision_threshold=0.5,
     )
     # TODO: Avoid calling like this, re-use logic that works with weights + extra args
     score_val_baseline = metric(y, y_pred_val, **metric_kwargs)
 
     if verbose:
-        logger.log(20, f'Calibrating decision threshold to optimize metric{metric_name_log} '
-                       f'| Checking {len(decision_thresholds)} thresholds...')
+        logger.log(20, f"Calibrating decision threshold to optimize metric{metric_name_log} " f"| Checking {len(decision_thresholds)} thresholds...")
     for decision_threshold in decision_thresholds:
-        extra_log = ''
+        extra_log = ""
         y_pred_val = get_pred_from_proba(
             y_pred_proba=y_pred_proba,
             problem_type=problem_type,
             decision_threshold=decision_threshold,
         )
         # TODO: Avoid calling like this, re-use logic that works with weights + extra args
         score_val = metric(y, y_pred_val, **metric_kwargs)
 
         if best_score_val is None or score_val > best_score_val:
             best_threshold = decision_threshold
             best_score_val = score_val
-            extra_log = '\t| NEW BEST'
+            extra_log = "\t| NEW BEST"
         elif best_score_val == score_val:
             # If the new threshold is closer to 0.5 than the previous threshold, prioritize it.
             if abs(decision_threshold - 0.5) < abs(best_threshold - 0.5):
                 best_threshold = decision_threshold
                 best_score_val = score_val
-                extra_log = '\t| NEW BEST (Tie, using threshold that is closer to 0.5)'
+                extra_log = "\t| NEW BEST (Tie, using threshold that is closer to 0.5)"
 
         if verbose:
-            logger.log(15, f'\tthreshold: {decision_threshold:.3f}\t| val: {score_val:.4f}{extra_log}')
+            logger.log(15, f"\tthreshold: {decision_threshold:.3f}\t| val: {score_val:.4f}{extra_log}")
     if verbose:
-        logger.log(20, f'\tBase Threshold: {0.5:.3f}\t| val: {score_val_baseline:.4f}')
-        logger.log(20, f'\tBest Threshold: {best_threshold:.3f}\t| val: {best_score_val:.4f}')
+        logger.log(20, f"\tBase Threshold: {0.5:.3f}\t| val: {score_val_baseline:.4f}")
+        logger.log(20, f"\tBest Threshold: {best_threshold:.3f}\t| val: {best_score_val:.4f}")
     return best_threshold
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/calibrate/conformity_score.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/calibrate/conformity_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 
 def compute_conformity_score(y_val_pred: np.ndarray, y_val: np.ndarray, quantile_levels: list):
-    '''
+    """
     Compute conformity scores based on validation set. This is only applicable to quantile regression problems.
     The scores are used to conformalize new quantile predictions.
     This is based on the paper 'Conformalized Quantile Regression (https://arxiv.org/abs/1905.03222)',
     and its implementation at 'https://github.com/yromano/cqr'.
 
     Parameters:
     -----------
@@ -16,15 +16,15 @@
     y_val: numpy ndarray
         [num_samples x 1]
         The target values to the validation set
     quantile_levels: list
         List of quantile levels
     Return:
     numpy ndarray: values to conformalize the new quantile predictions
-    '''
+    """
 
     num_samples = y_val.shape[0]
     y_val = y_val.reshape(-1)
     assert y_val_pred.shape[0] == num_samples
     assert y_val_pred.shape[1] == len(quantile_levels)
 
     conformalize_list = []
@@ -36,12 +36,12 @@
             index_high = min(max(index_high, 0), num_samples - 1)
             conformalize = error_high[index_high]
         elif q < 0.5:
             error_low = y_val_pred[:, i] - y_val
             error_low = np.sort(error_low, 0)
             index_low = int(np.ceil((1 - q) * (num_samples + 1))) - 1
             index_low = min(max(index_low, 0), num_samples - 1)
-            conformalize = - error_low[index_low]
+            conformalize = -error_low[index_low]
         else:
             conformalize = 0.0
         conformalize_list.append(conformalize)
     return np.array(conformalize_list)
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/calibrate/temperature_scaling.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/calibrate/temperature_scaling.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import numpy as np
 
 from autogluon.common.utils.try_import import try_import_torch
 
 
-def tune_temperature_scaling(y_val_probs: np.ndarray, y_val: np.ndarray, init_val: float = 1, max_iter: int = 1000,
-                             lr: float = 0.01):
-    '''
+def tune_temperature_scaling(y_val_probs: np.ndarray, y_val: np.ndarray, init_val: float = 1, max_iter: int = 1000, lr: float = 0.01):
+    """
     Tunes a temperature scalar term that divides the logits produced by autogluon model. Logits are generated
     by natural log the predicted probs from model then divides by a temperature scalar, which is tuned
     to minimize cross entropy on validation set.
 
     Parameters:
     -----------
     y_val_probs: numpy ndarray
@@ -21,15 +20,15 @@
     max_iter: int
         The maximum number of iterations to step in tuning
     lr: float
         The initial learning rate
 
     Return:
     float: The temperature scaling term, returns None if infinity found in logits.
-    '''
+    """
     try_import_torch()
     import torch
 
     # This is required to avoid error when passing np.uint16 to torch.tensor. This can occur if >255 classes (Dionis)
     y_val = y_val.astype(np.int64)
 
     y_val_tensor = torch.tensor(y_val)
@@ -44,15 +43,15 @@
     nll_criterion = torch.nn.CrossEntropyLoss()
     optimizer = torch.optim.LBFGS([temperature_param], lr=lr, max_iter=max_iter)
     scheduler = torch.optim.lr_scheduler.ExponentialLR(optimizer, gamma=0.99)
 
     def temperature_scale_step():
         optimizer.zero_grad()
         temp = temperature_param.unsqueeze(1).expand(logits.size(0), logits.size(1))
-        new_logits = (logits / temp)
+        new_logits = logits / temp
         loss = nll_criterion(new_logits, y_val_tensor)
         loss.backward()
         scheduler.step()
         return loss
 
     optimizer.step(temperature_scale_step)
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/constants.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # Do not change these!
-BINARY = 'binary'
-MULTICLASS = 'multiclass'
-REGRESSION = 'regression'
-SOFTCLASS = 'softclass'  # classification with soft-target (rather than classes, labels are probabilities of each class).
-QUANTILE = 'quantile'  # quantile regression (over multiple quantile levels, which are between 0.0 and 1.0)
+BINARY = "binary"
+MULTICLASS = "multiclass"
+REGRESSION = "regression"
+SOFTCLASS = "softclass"  # classification with soft-target (rather than classes, labels are probabilities of each class).
+QUANTILE = "quantile"  # quantile regression (over multiple quantile levels, which are between 0.0 and 1.0)
 
 PROBLEM_TYPES_CLASSIFICATION = [BINARY, MULTICLASS]
 PROBLEM_TYPES_REGRESSION = [REGRESSION]
 PROBLEM_TYPES = PROBLEM_TYPES_CLASSIFICATION + PROBLEM_TYPES_REGRESSION + [SOFTCLASS] + [QUANTILE]
 
 PSEUDO_MODEL_SUFFIX = "_PSEUDO_{iter}"
 
-REFIT_FULL_NAME = 'refit_single_full'  # stack-name used for refit_single_full (aka "compressed") models
+REFIT_FULL_NAME = "refit_single_full"  # stack-name used for refit_single_full (aka "compressed") models
 REFIT_FULL_SUFFIX = "_FULL"  # suffix appended to model name for refit_single_full (aka "compressed") models
 
 # AG_ARGS variables are key names in model hyperparameters to dictionaries of custom AutoGluon arguments.
 # TODO: Have documentation for all AG_ARGS values
-AG_ARGS = 'ag_args'  # Contains arguments to control model name, model priority, and the valid configurations which it can be used in.
-AG_ARGS_FIT = 'ag_args_fit'  # Contains arguments that impact model training, such as early stopping rounds, #cores, #gpus, max time limit, max memory usage  # TODO
-AG_ARGS_ENSEMBLE = 'ag_args_ensemble'  # Contains arguments that impact model ensembling, such as if an ensemble model is allowed to use the original features.  # TODO: v0.1 add to documentation
-AG_ARG_PREFIX = 'ag.'  # Prefix to add to a hyperparameter to indicate it is an aux param for ag_args_fit.
+AG_ARGS = "ag_args"  # Contains arguments to control model name, model priority, and the valid configurations which it can be used in.
+AG_ARGS_FIT = (
+    "ag_args_fit"  # Contains arguments that impact model training, such as early stopping rounds, #cores, #gpus, max time limit, max memory usage  # TODO
+)
+AG_ARGS_ENSEMBLE = "ag_args_ensemble"  # Contains arguments that impact model ensembling, such as if an ensemble model is allowed to use the original features.  # TODO: v0.1 add to documentation
+AG_ARG_PREFIX = "ag."  # Prefix to add to a hyperparameter to indicate it is an aux param for ag_args_fit.
 
-OBJECTIVES_TO_NORMALIZE = ['log_loss', 'pac_score', 'soft_log_loss']  # do not like predicted probabilities = 0
+OBJECTIVES_TO_NORMALIZE = ["log_loss", "pac_score", "soft_log_loss"]  # do not like predicted probabilities = 0
 
-AUTO_WEIGHT = 'auto_weight'
-BALANCE_WEIGHT = 'balance_weight'
+AUTO_WEIGHT = "auto_weight"
+BALANCE_WEIGHT = "balance_weight"
 
 # Constants used to infer problem type
 MULTICLASS_UPPER_LIMIT = 1000  # assume regression if dtype is numeric and unique label count is above this limit
 LARGE_DATA_THRESHOLD = 1000
 REGRESS_THRESHOLD_LARGE_DATA = 0.05
 REGRESS_THRESHOLD_SMALL_DATA = 0.1
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/data/cleaner.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/data/cleaner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
+
 from pandas import DataFrame
 
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION
 
 logger = logging.getLogger(__name__)
 
 
 # Cleaner cleans data prior to entering feature generation
 class Cleaner:
     @staticmethod
@@ -58,17 +59,21 @@
         class_counts = X[label].value_counts()
         class_counts_valid = class_counts[class_counts >= threshold]
         valid_classes = list(class_counts_valid.index)
         sum_prior = sum(class_counts)
         sum_after = sum(class_counts_valid)
         percent = sum_after / sum_prior
         if len(valid_classes) < len(class_counts):
-            logger.log(25, 'Warning: Some classes in the training set have fewer than %s examples. AutoGluon will only keep %s out of %s classes for training and will not try to predict the rare classes. '
-                           'To keep more classes, increase the number of datapoints from these rare classes in the training data or reduce label_count_threshold.' % (threshold, len(valid_classes), len(class_counts)))
+            logger.log(
+                25,
+                "Warning: Some classes in the training set have fewer than %s examples. AutoGluon will only keep %s out of %s classes for training and will not try to predict the rare classes. "
+                "To keep more classes, increase the number of datapoints from these rare classes in the training data or reduce label_count_threshold."
+                % (threshold, len(valid_classes), len(class_counts)),
+            )
         if percent < 1.0:
-            logger.log(25, 'Fraction of data from classes with at least %s examples that will be kept for training models: %s' % (threshold, percent))
+            logger.log(25, "Fraction of data from classes with at least %s examples that will be kept for training models: %s" % (threshold, percent))
         return valid_classes
 
     @staticmethod
     def remove_classes(X, label, valid_classes):
         X = X[X[label].isin(valid_classes)]
         return X
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/data/label_cleaner.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/data/label_cleaner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import copy
 import logging
 from typing import Union
 
 import numpy as np
 from pandas import DataFrame, Series
 
-from autogluon.core.constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, SOFTCLASS
-
+from autogluon.core.constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 from autogluon.core.utils import get_pred_from_proba, get_pred_from_proba_df
 
 logger = logging.getLogger(__name__)
 
 
 # LabelCleaner cleans labels prior to entering feature generation
 class LabelCleaner:
@@ -22,15 +21,17 @@
     problem_type_transform = None
 
     def __init__(self, y: Union[Series, np.ndarray, list, DataFrame]):
         y = self._convert_to_valid_series(y)
         self.original_dtype = y.dtype
 
     @staticmethod
-    def construct(problem_type: str, y: Union[Series, np.ndarray, list, DataFrame], y_uncleaned: Union[Series, np.ndarray, list, DataFrame] = None, positive_class=None):
+    def construct(
+        problem_type: str, y: Union[Series, np.ndarray, list, DataFrame], y_uncleaned: Union[Series, np.ndarray, list, DataFrame] = None, positive_class=None
+    ):
         if problem_type == SOFTCLASS:
             return LabelCleanerSoftclass(y)
         y = LabelCleaner._convert_to_valid_series(y)
         if y_uncleaned is not None:
             y_uncleaned = LabelCleaner._convert_to_valid_series(y_uncleaned)
 
         if problem_type == BINARY:
@@ -51,20 +52,20 @@
     def transformed_dtype(self):
         assert self.num_classes is not None
         max_dtype = np.min_scalar_type(self.num_classes)
         min_dtype = np.min_scalar_type(0)
         return np.promote_types(min_dtype, max_dtype)
 
     def to_transformed_dtype(self, y: Union[Series, np.ndarray, list]) -> Series:
-        if y.dtype.kind in ('i', 'u'):
+        if y.dtype.kind in ("i", "u"):
             return y.astype(self.transformed_dtype)
         return y
 
     def to_original_dtype(self, y: Union[Series, np.ndarray, list]) -> Series:
-        if y.dtype.kind in ('i', 'u'):
+        if y.dtype.kind in ("i", "u"):
             return y.astype(self.original_dtype)
         return y
 
     def transform(self, y: Union[Series, np.ndarray, list]) -> Series:
         y = self._convert_to_valid_series(y)
         y = self._transform(y)
         return self.to_transformed_dtype(y)
@@ -86,16 +87,16 @@
     def inverse_transform_proba(self, y, as_pandas=False, as_pred=False):
         return y
 
     @staticmethod
     def _convert_to_valid_series(y: Union[Series, np.ndarray, list]) -> Series:
         if isinstance(y, np.ndarray) or isinstance(y, list):
             y = Series(y)
-        elif isinstance(y, Series) and y.dtype.name == 'category':
-            y = y.astype('object')
+        elif isinstance(y, Series) and y.dtype.name == "category":
+            y = y.astype("object")
         return y
 
 
 class LabelCleanerMulticlass(LabelCleaner):
     def __init__(self, y: Series, y_uncleaned: Series):
         super().__init__(y)
         self.problem_type_transform = MULTICLASS
@@ -104,16 +105,16 @@
         self.cat_mappings_dependent_var: dict = self._generate_categorical_mapping(y)
         self.inv_map: dict = {v: k for k, v in self.cat_mappings_dependent_var.items()}
 
         self.cat_mappings_dependent_var_uncleaned: dict = self._generate_categorical_mapping(y_uncleaned)
         self.inv_map_uncleaned: dict = {v: k for k, v in self.cat_mappings_dependent_var_uncleaned.items()}
 
         self.num_classes = len(self.cat_mappings_dependent_var.keys())
-        self.ordered_class_labels = list(y_uncleaned.astype('category').cat.categories)
-        self.valid_ordered_class_labels = list(y.astype('category').cat.categories)
+        self.ordered_class_labels = list(y_uncleaned.astype("category").cat.categories)
+        self.valid_ordered_class_labels = list(y.astype("category").cat.categories)
         self.ordered_class_labels_transformed = list(range(len(self.valid_ordered_class_labels)))
         self.invalid_class_count = len(self.ordered_class_labels) - len(self.valid_ordered_class_labels)
         self.labels_to_zero_fill = [1 if label not in self.valid_ordered_class_labels else 0 for label in self.ordered_class_labels]
         self.label_index_to_keep = [i for i, label in enumerate(self.labels_to_zero_fill) if label == 0]
         self.label_index_to_remove = [i for i, label in enumerate(self.labels_to_zero_fill) if label == 1]
 
     def _transform(self, y: Series) -> Series:
@@ -161,56 +162,57 @@
                 y_transformed.index = y_index
         if as_pandas and not as_pred:
             y_transformed = DataFrame(data=y_transformed, index=y_index, columns=self.ordered_class_labels, dtype=np.float32)
         return y_transformed
 
     @staticmethod
     def _generate_categorical_mapping(y: Series) -> dict:
-        categories = y.astype('category')
+        categories = y.astype("category")
         cat_mappings_dependent_var = dict(enumerate(categories.cat.categories))
         return cat_mappings_dependent_var
 
 
 # TODO: Expand print statement to multiclass as well
 class LabelCleanerBinary(LabelCleaner):
     def __init__(self, y: Series, positive_class=None):
         super().__init__(y)
         self.problem_type_transform = BINARY
         y = self._convert_to_valid_series(y)
         self.num_classes = 2
         self.unique_values = list(y.unique())
         if len(self.unique_values) != 2:
-            raise AssertionError('y does not contain exactly 2 unique values:', self.unique_values)
+            raise AssertionError("y does not contain exactly 2 unique values:", self.unique_values)
         try:
             self.unique_values.sort()
         except TypeError:
             # Contains both str and int
             self.unique_values = list(y.unique())
         # TODO: Clean this code, for loop
         pos_class_warning = None
         if positive_class is not None:
             if positive_class not in self.unique_values:
-                raise ValueError(f'positive_class is not a valid class: {self.unique_values} (positive_class={positive_class})')
+                raise ValueError(f"positive_class is not a valid class: {self.unique_values} (positive_class={positive_class})")
             negative_class = [c for c in self.unique_values if c != positive_class][0]
             self.inv_map: dict = {negative_class: 0, positive_class: 1}
-        elif ((str(False) in [str(val) for val in self.unique_values]) and
-              (str(True) in [str(val) for val in self.unique_values])):
+        elif (str(False) in [str(val) for val in self.unique_values]) and (str(True) in [str(val) for val in self.unique_values]):
             false_val = [val for val in self.unique_values if str(val) == str(False)][0]  # may be str or bool
             true_val = [val for val in self.unique_values if str(val) == str(True)][0]  # may be str or bool
             self.inv_map: dict = {false_val: 0, true_val: 1}
         elif (0 in self.unique_values) and (1 in self.unique_values):
             self.inv_map: dict = {0: 0, 1: 1}
         else:
             self.inv_map: dict = {self.unique_values[0]: 0, self.unique_values[1]: 1}
-            pos_class_warning = f'\tNote: For your binary classification, AutoGluon arbitrarily selected which label-value ' \
-                                f'represents positive ({self.unique_values[1]}) vs negative ({self.unique_values[0]}) class.\n'\
-                                '\tTo explicitly set the positive_class, either rename classes to 1 and 0, or specify positive_class in Predictor init.'
+            pos_class_warning = (
+                f"\tNote: For your binary classification, AutoGluon arbitrarily selected which label-value "
+                f"represents positive ({self.unique_values[1]}) vs negative ({self.unique_values[0]}) class.\n"
+                "\tTo explicitly set the positive_class, either rename classes to 1 and 0, or specify positive_class in Predictor init."
+            )
         poslabel = [lbl for lbl in self.inv_map.keys() if self.inv_map[lbl] == 1][0]
         neglabel = [lbl for lbl in self.inv_map.keys() if self.inv_map[lbl] == 0][0]
-        logger.log(20, 'Selected class <--> label mapping:  class 1 = %s, class 0 = %s' % (poslabel, neglabel))
+        logger.log(20, "Selected class <--> label mapping:  class 1 = %s, class 0 = %s" % (poslabel, neglabel))
         if pos_class_warning is not None:
             logger.log(20, pos_class_warning)
         self.cat_mappings_dependent_var: dict = {v: k for k, v in self.inv_map.items()}
         self.ordered_class_labels_transformed = [0, 1]
         self.ordered_class_labels = [self.cat_mappings_dependent_var[label_transformed] for label_transformed in self.ordered_class_labels_transformed]
 
     def inverse_transform_proba(self, y, as_pandas=False, as_pred=False):
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/dataset.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-
 import pandas as pd
 
 from .utils.loaders import load_pd
 
-__all__ = ['TabularDataset']
+__all__ = ["TabularDataset"]
 
 
 class TabularDataset(pd.DataFrame):
     """
-    A dataset in tabular format (with rows = samples, columns = features/variables). 
-    This object is essentially a pandas DataFrame (with some extra attributes) and all existing pandas methods can be applied to it. 
+    A dataset in tabular format (with rows = samples, columns = features/variables).
+    This object is essentially a pandas DataFrame (with some extra attributes) and all existing pandas methods can be applied to it.
     For full list of methods/attributes, see pandas Dataframe documentation: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
 
     Parameters
     ----------
     data : :class:`pd.DataFrame` or str
         If str, path to data file (CSV or Parquet format).
         If you already have your data in a :class:`pd.DataFrame`, you can specify it here.
 
     Attributes
     ----------
     file_path: (str)
         Path to data file from which this `TabularDataset` was created.
         None if `data` was a :class:`pd.DataFrame`.
-    
-    Note: In addition to these attributes, `TabularDataset` also shares all the same attributes and methods of a pandas Dataframe. 
+
+    Note: In addition to these attributes, `TabularDataset` also shares all the same attributes and methods of a pandas Dataframe.
     For a detailed list, see:  https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html
 
     Examples
     --------
     >>> from autogluon.core.dataset import TabularDataset
     >>> train_data = TabularDataset('https://autogluon.s3.amazonaws.com/datasets/Inc/train.csv')
     >>> train_data.head(30)
     >>> train_data.columns
     """
 
-    _metadata = ['file_path']  # preserved properties that will be copied to a new instance of TabularDataset
+    _metadata = ["file_path"]  # preserved properties that will be copied to a new instance of TabularDataset
 
     @property
     def _constructor(self):
         return TabularDataset
 
     @property
     def _constructor_sliced(self):
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/executors.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/executors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,193 +1,179 @@
 from __future__ import annotations
 
 import copy
 import logging
 import math
 import os
-import pandas as pd
 import time
+from abc import ABC, abstractmethod
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
 
-from autogluon.common import space
+import pandas as pd
 
-from abc import ABC, abstractmethod
-from typing import Any, Optional, List, Dict, Union, Callable, Tuple
+from autogluon.common import space
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.s3_utils import is_s3_url
 
-from .constants import RAY_BACKEND, CUSTOM_BACKEND
-from .exceptions import EmptySearchSpace
 from ..ray.resources_calculator import ResourceCalculator
 from ..scheduler.scheduler_factory import scheduler_factory
 from ..utils.savers import save_pkl
-
-from typing import TYPE_CHECKING
+from .constants import CUSTOM_BACKEND, RAY_BACKEND
+from .exceptions import EmptySearchSpace
 
 if TYPE_CHECKING:
     from ..models import AbstractModel
 
 
 logger = logging.getLogger(__name__)
 
 
 class HpoExecutor(ABC):
     """Interface for abstract model to executor HPO runs"""
-    
+
     def __init__(self):
         self.hyperparameter_tune_kwargs = None
         self.resources = None
         self.search_space = None
         self._time_limit = None
-    
+
     @property
     @abstractmethod
     def executor_type(self):
         """Type of the executor"""
         raise NotImplementedError
-    
+
     @property
     def time_limit(self):
         """Time limit for the hpo experiment"""
         return self._time_limit
-    
+
     @time_limit.setter
     def time_limit(self, value):
         self._time_limit = value
 
     @abstractmethod
-    def initialize(
-            self,
-            hyperparameter_tune_kwargs: Union[str, dict],
-            default_num_trials: Optional[int] = None,
-            time_limit: Optional[float] = None
-        ):
+    def initialize(self, hyperparameter_tune_kwargs: Union[str, dict], default_num_trials: Optional[int] = None, time_limit: Optional[float] = None):
         """
         Parse `hyperparameter_tune_kwargs` and initialize the executor
-        
+
         Parameters
         ----------
         hyperparameter_tune_kwargs
             User specified parameters to perform HPO experiment
         default_num_trials
             If user didn't provide `num_trials` in `hyperparameter_tune_kwargs`, will use this value instead.
             If None and user didn't provide `num_trials`, will do 1000 trials when there is no time limit, and 1 trial if there is time limit.
         time_limit
             Time limit provided to the experiment.
         """
         raise NotImplementedError
-    
-    def register_resources(
-        self,
-        initialized_model: AbstractModel,
-        num_cpus: int,
-        num_gpus: Union[int, float],
-        k_fold: Optional[int] = None,
-        **kwargs
-    ):
+
+    def register_resources(self, initialized_model: AbstractModel, num_cpus: int, num_gpus: Union[int, float], k_fold: Optional[int] = None, **kwargs):
         """
         Register total resources used for the experiment, and calculate resources per trial if user specified.
         User specified resources per trial will be validated against total resources and minimum resources required, and respected directly if legit.
         When HPO with bagging, user could specify resources per fold as well as resources per trial.
             Resources per fold will be checked against total resources, minimum resources required, and resources per trial (if specified).
             Resources per fold will have higher priority than resources per trial, and the corresponding resources per trial will be calculated accordingly.
         When no user specified resources present, we try to maximize trials running in parallel while respecting the minimum resources required.
-        
+
         Parameters
         ----------
         initialized_model
             The model that will be performed HPO. This model MUST be initialized.
         num_cpus
             Total number of cpus available for the experiment.
         num_gpus
             Total number of gpus available for the experiment.
         k_fold
             Number of folds if bagging. Used to check if an individual trial is a bagged model.
         kwargs
             Any additional parameters being passed to `AbstractModel.hyperparameter_tune()`
             This function will pass these parameters to initialized model to get estimation of memory usage
         """
-        minimum_model_resources = initialized_model.get_minimum_resources(
-            is_gpu_available=(num_gpus > 0)
-        )
-        minimum_model_num_cpus = minimum_model_resources.get('num_cpus', 1)
-        minimum_model_num_gpus = minimum_model_resources.get('num_gpus', 0)
+        minimum_model_resources = initialized_model.get_minimum_resources(is_gpu_available=(num_gpus > 0))
+        minimum_model_num_cpus = minimum_model_resources.get("num_cpus", 1)
+        minimum_model_num_gpus = minimum_model_resources.get("num_gpus", 0)
         initialized_model_params = initialized_model.get_params()
 
-        if 'hyperparameters' in initialized_model_params and 'ag_args_fit' in initialized_model_params['hyperparameters']:
-            user_specified_trial_num_cpus = initialized_model_params['hyperparameters']['ag_args_fit'].get('num_cpus', None)
-            user_specified_trial_num_gpus = initialized_model_params['hyperparameters']['ag_args_fit'].get('num_gpus', None)
+        if "hyperparameters" in initialized_model_params and "ag_args_fit" in initialized_model_params["hyperparameters"]:
+            user_specified_trial_num_cpus = initialized_model_params["hyperparameters"]["ag_args_fit"].get("num_cpus", None)
+            user_specified_trial_num_gpus = initialized_model_params["hyperparameters"]["ag_args_fit"].get("num_gpus", None)
             if user_specified_trial_num_cpus is not None or user_specified_trial_num_gpus is not None:
                 num_trials_in_parallel_with_gpu = math.inf
                 if user_specified_trial_num_cpus is None:
                     # If user didn't specify cpu per trial, we find the min based on gpu
                     num_trials_in_parallel_with_gpu = num_gpus // user_specified_trial_num_gpus
                     user_specified_trial_num_cpus = num_cpus // num_trials_in_parallel_with_gpu  # keep gpus per trial int to avoid complexity
                 num_trials_in_parallel_with_cpu = math.inf
                 if user_specified_trial_num_gpus is None:
                     # If user didn't specify gpu per trial, we find the min based on cpu
                     num_trials_in_parallel_with_cpu = num_cpus // user_specified_trial_num_cpus
                     user_specified_trial_num_gpus = num_gpus // num_trials_in_parallel_with_cpu  # keep gpus per trial int to avoid complexity
-                assert user_specified_trial_num_cpus <= num_cpus, \
-                    f"Detected trial level cpu requirement = {user_specified_trial_num_cpus} > total cpu granted to AG predictor = {num_cpus}"
-                assert user_specified_trial_num_cpus >= minimum_model_num_cpus, \
-                    f"The trial requires minimum cpu {minimum_model_num_cpus}, but you only specified {user_specified_trial_num_cpus}"
-                assert user_specified_trial_num_gpus <= num_gpus, \
-                    f"Detected trial level gpu requirement = {user_specified_trial_num_gpus} > total gpu granted to AG predictor = {num_gpus}"
-                assert user_specified_trial_num_gpus >= minimum_model_num_gpus, \
-                    f"The trial requires minimum gpu {minimum_model_num_gpus}, but you only specified {user_specified_trial_num_gpus}"
+                assert (
+                    user_specified_trial_num_cpus <= num_cpus
+                ), f"Detected trial level cpu requirement = {user_specified_trial_num_cpus} > total cpu granted to AG predictor = {num_cpus}"
+                assert (
+                    user_specified_trial_num_cpus >= minimum_model_num_cpus
+                ), f"The trial requires minimum cpu {minimum_model_num_cpus}, but you only specified {user_specified_trial_num_cpus}"
+                assert (
+                    user_specified_trial_num_gpus <= num_gpus
+                ), f"Detected trial level gpu requirement = {user_specified_trial_num_gpus} > total gpu granted to AG predictor = {num_gpus}"
+                assert (
+                    user_specified_trial_num_gpus >= minimum_model_num_gpus
+                ), f"The trial requires minimum gpu {minimum_model_num_gpus}, but you only specified {user_specified_trial_num_gpus}"
 
                 # Custom backend should set its total resource to be resources_per_trial
-                self.hyperparameter_tune_kwargs['resources_per_trial'] = {
-                    'num_cpus': user_specified_trial_num_cpus,
-                    'num_gpus': user_specified_trial_num_gpus
-                }
-                
+                self.hyperparameter_tune_kwargs["resources_per_trial"] = {"num_cpus": user_specified_trial_num_cpus, "num_gpus": user_specified_trial_num_gpus}
+
         model_base = initialized_model._get_model_base()
         if model_base != initialized_model:
             # This is an ensemble model
             total_num_cpus_per_trial = num_cpus
             total_num_gpus_per_trial = num_gpus
-            if 'resources_per_trial' in self.hyperparameter_tune_kwargs:
-                resources_per_trial = self.hyperparameter_tune_kwargs['resources_per_trial']
-                total_num_cpus_per_trial = resources_per_trial.get('num_cpus')
-                total_num_gpus_per_trial = resources_per_trial.get('num_gpus')
+            if "resources_per_trial" in self.hyperparameter_tune_kwargs:
+                resources_per_trial = self.hyperparameter_tune_kwargs["resources_per_trial"]
+                total_num_cpus_per_trial = resources_per_trial.get("num_cpus")
+                total_num_gpus_per_trial = resources_per_trial.get("num_gpus")
             user_specified_fold_resources = model_base._user_params_aux
-            user_specified_fold_num_cpus = user_specified_fold_resources.get('num_cpus', None)  # We shouldn't always use it
-            user_specified_fold_num_gpus = user_specified_fold_resources.get('num_gpus', None)
+            user_specified_fold_num_cpus = user_specified_fold_resources.get("num_cpus", None)  # We shouldn't always use it
+            user_specified_fold_num_gpus = user_specified_fold_resources.get("num_gpus", None)
             if user_specified_fold_num_cpus is not None or user_specified_fold_num_gpus is not None:
                 num_folds_in_parallel_with_cpu = math.inf
                 if minimum_model_num_cpus > 0:
                     num_folds_in_parallel_with_cpu = total_num_cpus_per_trial // minimum_model_num_cpus
                 if user_specified_fold_num_cpus is not None:
-                    assert user_specified_fold_num_cpus <= total_num_cpus_per_trial, \
-                        f"Detected fold level cpu requirement = {user_specified_fold_num_cpus} > total cpu granted to AG predictor per trial= {total_num_cpus_per_trial}"
-                    assert user_specified_fold_num_cpus >= minimum_model_num_cpus, \
-                        f"The model requires minimum cpu {minimum_model_num_cpus}, but you only specified {user_specified_fold_num_cpus}"
+                    assert (
+                        user_specified_fold_num_cpus <= total_num_cpus_per_trial
+                    ), f"Detected fold level cpu requirement = {user_specified_fold_num_cpus} > total cpu granted to AG predictor per trial= {total_num_cpus_per_trial}"
+                    assert (
+                        user_specified_fold_num_cpus >= minimum_model_num_cpus
+                    ), f"The model requires minimum cpu {minimum_model_num_cpus}, but you only specified {user_specified_fold_num_cpus}"
                     num_folds_in_parallel_with_cpu = total_num_cpus_per_trial // user_specified_fold_num_cpus
                 num_folds_in_parallel_with_gpu = math.inf
                 if minimum_model_num_gpus > 0:
                     num_folds_in_parallel_with_gpu = total_num_gpus_per_trial // minimum_model_num_gpus
                 if user_specified_fold_num_gpus is not None:
-                    assert user_specified_fold_num_gpus <= total_num_gpus_per_trial, \
-                        f"Detected fold level gpu requirement = {user_specified_fold_num_gpus} > total gpu granted to AG predictor per trial = {total_num_gpus_per_trial}"
-                    assert user_specified_fold_num_gpus >= minimum_model_num_gpus, \
-                        f"The model requires minimum gpu {minimum_model_num_gpus}, but you only specified {user_specified_fold_num_gpus}"
+                    assert (
+                        user_specified_fold_num_gpus <= total_num_gpus_per_trial
+                    ), f"Detected fold level gpu requirement = {user_specified_fold_num_gpus} > total gpu granted to AG predictor per trial = {total_num_gpus_per_trial}"
+                    assert (
+                        user_specified_fold_num_gpus >= minimum_model_num_gpus
+                    ), f"The model requires minimum gpu {minimum_model_num_gpus}, but you only specified {user_specified_fold_num_gpus}"
                     if minimum_model_num_gpus > 0:
                         num_folds_in_parallel_with_gpu = total_num_gpus_per_trial // user_specified_fold_num_gpus
                 num_folds_in_parallel = min(num_folds_in_parallel_with_cpu, num_folds_in_parallel_with_gpu)
 
                 cpu_per_trial = user_specified_fold_num_cpus * min(k_fold, num_folds_in_parallel)
                 gpu_per_trial = user_specified_fold_num_gpus * min(k_fold, num_folds_in_parallel)
 
                 # Custom backend should set its total resource to be resources_per_trial
-                self.hyperparameter_tune_kwargs['resources_per_trial'] = {
-                    'num_cpus': cpu_per_trial,
-                    'num_gpus': gpu_per_trial
-                }
-        if 'resources_per_trial' not in self.hyperparameter_tune_kwargs:
+                self.hyperparameter_tune_kwargs["resources_per_trial"] = {"num_cpus": cpu_per_trial, "num_gpus": gpu_per_trial}
+        if "resources_per_trial" not in self.hyperparameter_tune_kwargs:
             # User didn't provide any requirements
             num_jobs_in_parallel_with_mem = math.inf
 
             if initialized_model.estimate_memory_usage is not None:
                 model_estimate_memory_usage = initialized_model.estimate_memory_usage(**kwargs)
                 total_memory_available = ResourceManager.get_available_virtual_mem()
                 num_jobs_in_parallel_with_mem = total_memory_available // model_estimate_memory_usage
@@ -205,210 +191,192 @@
             if model_base != initialized_model:
                 # bagged model
                 if num_jobs_in_parallel // k_fold < 1:
                     # We can only train 1 trial in parallel
                     num_trials_in_parallel = 1
                 else:
                     num_trials_in_parallel = num_jobs_in_parallel // k_fold
-                if self.executor_type == 'custom':
+                if self.executor_type == "custom":
                     # custom backend runs sequentially
                     num_trials_in_parallel = 1
                 cpu_per_trial = int(num_cpus // num_trials_in_parallel)
                 gpu_per_trial = num_gpus // num_trials_in_parallel
             else:
-                num_trials = self.hyperparameter_tune_kwargs.get('num_trials', math.inf)
-                if self.executor_type == 'custom':
+                num_trials = self.hyperparameter_tune_kwargs.get("num_trials", math.inf)
+                if self.executor_type == "custom":
                     # custom backend runs sequentially
                     num_jobs_in_parallel = 1
                 cpu_per_trial = int(num_cpus // min(num_jobs_in_parallel, num_trials))
                 gpu_per_trial = num_gpus / min(num_jobs_in_parallel, num_trials)
             # In distributed setting, a single trial could be scheduled with resources that's more than a single node causing hanging
             # Force it to be less than the current node. This works under the assumption that all nodes are of the same type
             cpu_per_trial = min(cpu_per_trial, system_num_cpu)
             gpu_per_trial = min(gpu_per_trial, system_num_gpu)
-            
-            self.hyperparameter_tune_kwargs['resources_per_trial'] = {
-                'num_cpus': cpu_per_trial,
-                'num_gpus': gpu_per_trial
-            }
+
+            self.hyperparameter_tune_kwargs["resources_per_trial"] = {"num_cpus": cpu_per_trial, "num_gpus": gpu_per_trial}
 
         self.resources = dict(num_gpus=num_gpus, num_cpus=num_cpus)
 
     @abstractmethod
     def validate_search_space(
-            self,
-            search_space: dict,
-            model_name: str,
-        ):
+        self,
+        search_space: dict,
+        model_name: str,
+    ):
         """
         Validate the search space for the experiment
-        
+
         Parameters
         ----------
         search_space
             Search space provided to the experiment.
         model_name
             The model name of the hpo experiment is tuning. This is only used for logging purpose
         """
         raise NotImplementedError
 
-    def prepare_data(
-        self,
-        X: pd.DataFrame,
-        y: pd.Series,
-        X_val: pd.DataFrame,
-        y_val: pd.Series,
-        path_prefix: str
-    ) -> Tuple[str, str]:
+    def prepare_data(self, X: pd.DataFrame, y: pd.Series, X_val: pd.DataFrame, y_val: pd.Series, path_prefix: str) -> Tuple[str, str]:
         """
         Prepare data as pickle files for hpo trials.
         If path_prefix is a s3 url, will store to s3. Otherwise, store in local disk
-        
+
         Parameters
         ----------
         X: pd.DataFrame
             Training data
         y: pd.Series
             Training label
         X_val: pd.DataFrame
             Validation data
         y_val: pd.Series
             Validation label
         path_prefix: str
             path prefix to store the data artifacts
-        
+
         Return
         ------
         Tuple[str, str]:
             Path to both the training and validation data
         """
+
         def save_data(data: Any, path_prefix: str, filename: str) -> str:
             if is_s3_url(path_prefix):
                 path = path_prefix + filename if path_prefix.endswith("/") else path_prefix + f"/{filename}"
             else:
                 path = os.path.join(path_prefix, filename)
             save_pkl.save(path=path, object=data, verbose=False)
             return path
 
-        dataset_train_filename = 'dataset_train.pkl'
-        dataset_val_filename = 'dataset_val.pkl'
+        dataset_train_filename = "dataset_train.pkl"
+        dataset_val_filename = "dataset_val.pkl"
         train_path = save_data(data=(X, y), path_prefix=path_prefix, filename=dataset_train_filename)
         val_path = save_data(data=(X_val, y_val), path_prefix=path_prefix, filename=dataset_val_filename)
 
         return train_path, val_path
-    
+
     @abstractmethod
     def execute(self, **kwargs):
         """Execute the experiment"""
         raise NotImplementedError
-    
+
     @abstractmethod
-    def report(
-            self,
-            reporter: 'LocalReporter',
-            **kwargs
-        ):
+    def report(self, reporter: "LocalReporter", **kwargs):
         """Report result of the experiment to the reporter. If no reporter needed, pass in None"""
         raise NotImplementedError
-    
+
     @abstractmethod
-    def get_hpo_results(
-            self,
-            model_name: str,
-            model_path_root: str,
-            **kwargs
-        ):
+    def get_hpo_results(self, model_name: str, model_path_root: str, **kwargs):
         """
         Retrieve hpo results
-        
+
         Parameters
         ----------
         model_name
             The model name of the hpo experiment is tuning.
         model_path_root
             Root path of the model
         """
         raise NotImplementedError
 
 
 class RayHpoExecutor(HpoExecutor):
     """Implementation of HpoExecutor Interface, where ray tune is used as the backend"""
-    
+
     custom_to_ray_preset_map = {
-        'auto': {'scheduler': 'FIFO', 'searcher': 'bayes'},
-        'local_random': {'scheduler': 'FIFO', 'searcher': 'random'},
-        'distributed_random': {'scheduler': 'FIFO', 'searcher': 'random'},
-        'random': {'scheduler': 'FIFO', 'searcher': 'random'},
+        "auto": {"scheduler": "FIFO", "searcher": "bayes"},
+        "local_random": {"scheduler": "FIFO", "searcher": "random"},
+        "distributed_random": {"scheduler": "FIFO", "searcher": "random"},
+        "random": {"scheduler": "FIFO", "searcher": "random"},
     }
     custom_to_ray_scheduler_preset_map = {
-        'local': 'FIFO',
-        'distributed': 'FIFO',
+        "local": "FIFO",
+        "distributed": "FIFO",
     }
     custom_to_ray_searcher_preset_map = {
-        'local_random': 'random',
-        'distributed_random': 'random',
-        'random': 'random',
-        'auto': 'bayes',
+        "local_random": "random",
+        "distributed_random": "random",
+        "random": "random",
+        "auto": "bayes",
     }
-    
+
     def __init__(self):
         super().__init__()
         self.analysis = None
-    
+
     @property
     def executor_type(self):
         return RAY_BACKEND
-    
+
     def initialize(self, hyperparameter_tune_kwargs, default_num_trials=None, time_limit=None):
         self.time_limit = time_limit
         if isinstance(hyperparameter_tune_kwargs, dict):
             hyperparameter_tune_kwargs = hyperparameter_tune_kwargs.copy()
         if isinstance(hyperparameter_tune_kwargs, str):
             hyperparameter_tune_kwargs: dict = self.custom_to_ray_preset_map[hyperparameter_tune_kwargs].copy()
-        hyperparameter_tune_kwargs['scheduler'] = self.custom_to_ray_scheduler_preset_map.get(
-            hyperparameter_tune_kwargs['scheduler'],
-            hyperparameter_tune_kwargs['scheduler']
+        hyperparameter_tune_kwargs["scheduler"] = self.custom_to_ray_scheduler_preset_map.get(
+            hyperparameter_tune_kwargs["scheduler"], hyperparameter_tune_kwargs["scheduler"]
         )
-        hyperparameter_tune_kwargs['searcher'] = self.custom_to_ray_searcher_preset_map.get(
-            hyperparameter_tune_kwargs['searcher'],
-            hyperparameter_tune_kwargs['searcher']
+        hyperparameter_tune_kwargs["searcher"] = self.custom_to_ray_searcher_preset_map.get(
+            hyperparameter_tune_kwargs["searcher"], hyperparameter_tune_kwargs["searcher"]
         )
-        if 'num_trials' not in hyperparameter_tune_kwargs and default_num_trials is not None:
-            hyperparameter_tune_kwargs['num_trials'] = default_num_trials
+        if "num_trials" not in hyperparameter_tune_kwargs and default_num_trials is not None:
+            hyperparameter_tune_kwargs["num_trials"] = default_num_trials
         self.hyperparameter_tune_kwargs = copy.deepcopy(hyperparameter_tune_kwargs)
-        
+
     def validate_search_space(self, search_space, model_name):
         from ray.tune.search.sample import Domain
+
         if not any(isinstance(search_space[hyperparam], (space.Space, Domain)) for hyperparam in search_space):
-            logger.warning(f"\tNo hyperparameter search space specified for {model_name}. Skipping HPO. "
-                           f"Will train one model based on the provided hyperparameters.")
+            logger.warning(
+                f"\tNo hyperparameter search space specified for {model_name}. Skipping HPO. " f"Will train one model based on the provided hyperparameters."
+            )
             raise EmptySearchSpace
         self.search_space = search_space
         logger.log(15, f"\tHyperparameter search space for {model_name}: ")
         for hyperparam in search_space:
-                if isinstance(search_space[hyperparam], (space.Space, Domain)):
-                    logger.log(15, f"{hyperparam}:   {search_space[hyperparam]}")
-                    
+            if isinstance(search_space[hyperparam], (space.Space, Domain)):
+                logger.log(15, f"{hyperparam}:   {search_space[hyperparam]}")
+
     def execute(
-            self,
-            *,  # Force kwargs to avoid bugs
-            model_trial: Callable,
-            train_fn_kwargs: dict,
-            directory: str,
-            minimum_cpu_per_trial: int,
-            minimum_gpu_per_trial: float,
-            model_estimate_memory_usage: float,
-            adapter_type: str,
-            trainable_is_parallel: bool = False,
-            tune_config_kwargs: Optional[Dict[str, Any]] = None,
-            run_config_kwargs: Optional[Dict[str, Any]] = None
-        ):
+        self,
+        *,  # Force kwargs to avoid bugs
+        model_trial: Callable,
+        train_fn_kwargs: dict,
+        directory: str,
+        minimum_cpu_per_trial: int,
+        minimum_gpu_per_trial: float,
+        model_estimate_memory_usage: float,
+        adapter_type: str,
+        trainable_is_parallel: bool = False,
+        tune_config_kwargs: Optional[Dict[str, Any]] = None,
+        run_config_kwargs: Optional[Dict[str, Any]] = None,
+    ):
         """
         Execute ray hpo experiment
-        
+
         Parameters
         ----------
         model_trial: Callable
             A function conducting individual trial
         train_fn_kwargs: dict
             A dict containing kwargs passed to model_trial
         directory: str
@@ -428,197 +396,192 @@
         trainable_is_parallel
             Whether the trainable itself will use ray to run parallel job or not.
         tune_config_kwargs
             Additional args being passed to tune.TuneConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.tune.tune_config.TuneConfig
         run_config_kwargs
             Additional args being passed to air.RunConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.air.config.RunConfig
         """
-        from .ray_hpo import (
-            run,
-            RayTuneAdapterFactory
-        )
+        from .ray_hpo import RayTuneAdapterFactory, run
+
         # Disable tensorboard logging to avoid layer warning
         # TODO: remove this when ray tune fix ray tune pass tuple to hyperopt issue
-        os.environ['TUNE_DISABLE_AUTO_CALLBACK_LOGGERS'] = '1'
+        os.environ["TUNE_DISABLE_AUTO_CALLBACK_LOGGERS"] = "1"
         analysis = run(
             trainable=model_trial,
             trainable_args=train_fn_kwargs,
             search_space=self.search_space,
             hyperparameter_tune_kwargs=self.hyperparameter_tune_kwargs,
-            metric='validation_performance',
-            mode='max',
+            metric="validation_performance",
+            mode="max",
             save_dir=directory,
             ray_tune_adapter=RayTuneAdapterFactory.get_adapter(adapter_type)(),
             trainable_is_parallel=trainable_is_parallel,
             total_resources=self.resources,
             minimum_cpu_per_trial=minimum_cpu_per_trial,
             minimum_gpu_per_trial=minimum_gpu_per_trial,
             model_estimate_memory_usage=model_estimate_memory_usage,
             time_budget_s=self.time_limit,
             verbose=0,
             tune_config_kwargs=tune_config_kwargs,
-            run_config_kwargs=run_config_kwargs
+            run_config_kwargs=run_config_kwargs,
         )
-        os.environ.pop('TUNE_DISABLE_AUTO_CALLBACK_LOGGERS', None)
+        os.environ.pop("TUNE_DISABLE_AUTO_CALLBACK_LOGGERS", None)
         self.analysis = analysis
-        
+
     def report(self, reporter, **kwargs):
         from ray.air import session
+
         session.report(kwargs)
-        
+
     def get_hpo_results(self, model_name, model_path_root, **kwargs):
-        assert self.analysis is not None, 'Call `execute()` before `get_hpo_results()`'
+        assert self.analysis is not None, "Call `execute()` before `get_hpo_results()`"
         hpo_models = {}
         for trial, details in self.analysis.results.items():
-            validation_performance = details.get('validation_performance', None)
+            validation_performance = details.get("validation_performance", None)
             # when equals to -inf, trial finished with TimeLimitExceeded exception and didn't finish at least 1 epoch
-            if validation_performance is None or validation_performance == float('-inf'):
+            if validation_performance is None or validation_performance == float("-inf"):
                 continue
-            trial_id = details.get('trial_id')
+            trial_id = details.get("trial_id")
             file_id = trial_id  # unique identifier to files from this trial
             trial_model_name = os.path.join(model_name, file_id)
             trial_model_path = model_path_root + trial_model_name + os.path.sep
-            hpo_models[trial_model_name] = dict(
-                path=trial_model_path
-            )
+            hpo_models[trial_model_name] = dict(path=trial_model_path)
 
             hpo_models[trial_model_name] = dict(
                 path=trial_model_path,
                 val_score=validation_performance,
                 trial=trial,
-                hyperparameters= details['config'],
+                hyperparameters=details["config"],
             )
 
         return hpo_models, self.analysis
 
 
 class CustomHpoExecutor(HpoExecutor):
     """Implementation of HpoExecutor Interface, where our custom logic is used as the backend"""
-    
+
     def __init__(self):
         super().__init__()
         self.scheduler_options = None
         self.scheduler = None
-        
+
     @property
     def executor_type(self):
         return CUSTOM_BACKEND
-    
+
     @property
     def time_limit(self):
         return self._time_limit
-    
+
     @time_limit.setter
     def time_limit(self, value):
         assert self.scheduler_options is not None
-        self.scheduler_options[1]['time_out'] = value
+        self.scheduler_options[1]["time_out"] = value
         self._time_limit = value
-    
+
     def initialize(self, hyperparameter_tune_kwargs, default_num_trials=None, time_limit=None):
         if not isinstance(hyperparameter_tune_kwargs, tuple):
             if isinstance(hyperparameter_tune_kwargs, dict):
                 hyperparameter_tune_kwargs = copy.deepcopy(hyperparameter_tune_kwargs)
                 self.hyperparameter_tune_kwargs = hyperparameter_tune_kwargs
             num_trials = default_num_trials  # This will be ignored if hyperparameter_tune_kwargs contains num_trials
             if default_num_trials is None:
                 num_trials = 1 if time_limit is None else 1000
-            hyperparameter_tune_kwargs = scheduler_factory(hyperparameter_tune_kwargs, num_trials=num_trials, nthreads_per_trial='auto', ngpus_per_trial='auto')
+            hyperparameter_tune_kwargs = scheduler_factory(hyperparameter_tune_kwargs, num_trials=num_trials, nthreads_per_trial="auto", ngpus_per_trial="auto")
             hyperparameter_tune_kwargs = copy.deepcopy(hyperparameter_tune_kwargs)
-            if 'time_out' not in hyperparameter_tune_kwargs[1]:
-                hyperparameter_tune_kwargs[1]['time_out'] = time_limit
-            time_limit = hyperparameter_tune_kwargs[1]['time_out']
+            if "time_out" not in hyperparameter_tune_kwargs[1]:
+                hyperparameter_tune_kwargs[1]["time_out"] = time_limit
+            time_limit = hyperparameter_tune_kwargs[1]["time_out"]
         self.scheduler_options = hyperparameter_tune_kwargs
         self.time_limit = time_limit
         if self.hyperparameter_tune_kwargs is None:
             self.hyperparameter_tune_kwargs = {}
-    
+
     def register_resources(self, initialized_model, **kwargs):
-        assert self.scheduler_options is not None, 'Call `initialize()` before register resources'
+        assert self.scheduler_options is not None, "Call `initialize()` before register resources"
         super().register_resources(initialized_model, **kwargs)
-        if self.hyperparameter_tune_kwargs.get('resources_per_trial', None) is not None:
+        if self.hyperparameter_tune_kwargs.get("resources_per_trial", None) is not None:
             # Custom backend only run trials sequentially
-            self.scheduler_options[1]['resource'] = self.hyperparameter_tune_kwargs['resources_per_trial']
-        logger.debug(f'custom backend resource: {self.resources}, per trial resource: {self.hyperparameter_tune_kwargs}')
-        
+            self.scheduler_options[1]["resource"] = self.hyperparameter_tune_kwargs["resources_per_trial"]
+        logger.debug(f"custom backend resource: {self.resources}, per trial resource: {self.hyperparameter_tune_kwargs}")
+
     def validate_search_space(self, search_space, model_name):
         if not any(isinstance(search_space[hyperparam], space.Space) for hyperparam in search_space):
-            logger.warning(f"\tNo hyperparameter search space specified for {model_name}. Skipping HPO. "
-                           f"Will train one model based on the provided hyperparameters.")
+            logger.warning(
+                f"\tNo hyperparameter search space specified for {model_name}. Skipping HPO. " f"Will train one model based on the provided hyperparameters."
+            )
             raise EmptySearchSpace
         self.search_space = search_space
         logger.log(15, f"\tHyperparameter search space for {model_name}: ")
         for hyperparam in search_space:
-                if isinstance(search_space[hyperparam], space.Space):
-                    logger.log(15, f"{hyperparam}:   {search_space[hyperparam]}")
-                    
+            if isinstance(search_space[hyperparam], space.Space):
+                logger.log(15, f"{hyperparam}:   {search_space[hyperparam]}")
+
     def execute(self, model_trial, train_fn_kwargs, **kwargs):
-        assert self.scheduler_options is not None, 'Call `initialize()` before execute'
+        assert self.scheduler_options is not None, "Call `initialize()` before execute"
         scheduler_cls, scheduler_params = self.scheduler_options  # Unpack tuple
         if scheduler_cls is None or scheduler_params is None:
             raise ValueError("scheduler_cls and scheduler_params cannot be None for hyperparameter tuning")
-        train_fn_kwargs['fit_kwargs'].update(scheduler_params['resource'].copy())
+        train_fn_kwargs["fit_kwargs"].update(scheduler_params["resource"].copy())
         scheduler = scheduler_cls(model_trial, search_space=self.search_space, train_fn_kwargs=train_fn_kwargs, **scheduler_params)
         self.scheduler = scheduler
-        
+
         scheduler.run()
         scheduler.join_jobs()
-    
+
     def report(self, reporter, **kwargs):
         assert reporter is not None
-        reporter(**kwargs)   
-        
+        reporter(**kwargs)
+
     def get_hpo_results(self, model_name, model_path_root, time_start, **kwargs):
-        assert self.scheduler is not None, 'Call `execute()` before `get_hpo_results()`'
+        assert self.scheduler is not None, "Call `execute()` before `get_hpo_results()`"
         # Store results / models from this HPO run:
         best_hp = self.scheduler.get_best_config()  # best_hp only contains searchable stuff
         hpo_results = {
-            'best_reward': self.scheduler.get_best_reward(),
-            'best_config': best_hp,
-            'total_time': time.time() - time_start,
-            'metadata': self.scheduler.metadata,
-            'training_history': self.scheduler.training_history,
-            'config_history': self.scheduler.config_history,
-            'reward_attr': self.scheduler._reward_attr,
+            "best_reward": self.scheduler.get_best_reward(),
+            "best_config": best_hp,
+            "total_time": time.time() - time_start,
+            "metadata": self.scheduler.metadata,
+            "training_history": self.scheduler.training_history,
+            "config_history": self.scheduler.config_history,
+            "reward_attr": self.scheduler._reward_attr,
         }
 
         hpo_models = {}  # stores all the model names and file paths to model objects created during this HPO run.
         hpo_model_performances = {}
-        for trial in sorted(hpo_results['config_history'].keys()):
+        for trial in sorted(hpo_results["config_history"].keys()):
             # TODO: ignore models which were killed early by scheduler (eg. in Hyperband). How to ID these?
             file_id = f"T{trial+1}"  # unique identifier to files from this trial
             trial_model_name = os.path.join(model_name, file_id)
             trial_model_path = model_path_root + trial_model_name + os.path.sep
-            trial_reward = self.scheduler.searcher.get_reward(hpo_results['config_history'][trial])
-            if trial_reward is None or trial_reward == float('-inf'):
+            trial_reward = self.scheduler.searcher.get_reward(hpo_results["config_history"][trial])
+            if trial_reward is None or trial_reward == float("-inf"):
                 continue
             hpo_models[trial_model_name] = dict(
-                path=trial_model_path,
-                val_score=trial_reward,
-                trial=trial,
-                hyperparameters=hpo_results['config_history'][trial]
+                path=trial_model_path, val_score=trial_reward, trial=trial, hyperparameters=hpo_results["config_history"][trial]
             )
 
             hpo_model_performances[trial_model_name] = trial_reward
-        
-        hpo_results['hpo_model_performances'] = hpo_model_performances
 
-        logger.log(15, "Time for %s model HPO: %s" % (model_name, str(hpo_results['total_time'])))
+        hpo_results["hpo_model_performances"] = hpo_model_performances
+
+        logger.log(15, "Time for %s model HPO: %s" % (model_name, str(hpo_results["total_time"])))
         logger.log(15, "Best hyperparameter configuration for %s model: " % model_name)
         logger.log(15, str(best_hp))
 
         return hpo_models, hpo_results
 
 
 class HpoExecutorFactory:
-    
+
     __supported_executors = [
         RayHpoExecutor,
         CustomHpoExecutor,
     ]
-    
+
     __type_to_executor = {cls().executor_type: cls for cls in __supported_executors}
 
     @staticmethod
     def get_hpo_executor(hpo_executor: str) -> HpoExecutor:
         """Return the executor"""
-        assert hpo_executor in HpoExecutorFactory.__type_to_executor, f'{hpo_executor} not supported'
+        assert hpo_executor in HpoExecutorFactory.__type_to_executor, f"{hpo_executor} not supported"
         return HpoExecutorFactory.__type_to_executor[hpo_executor]
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/ray_hpo.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/ray_hpo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 import logging
 import os
 import shutil
 
 from autogluon.common import space as ag_space
-
 from autogluon.common.utils.distribute_utils import DistributedContext
 from autogluon.common.utils.try_import import try_import_ray
+
 try_import_ray()  # try import ray before importing the remaining contents so we can give proper error messages
+from abc import ABC, abstractmethod
+from typing import Callable, List, Optional, Union
+
 import ray
+from ray import air, tune
+from ray.tune import ExperimentAnalysis, PlacementGroupFactory
+from ray.tune.schedulers import TrialScheduler
+from ray.tune.search import SearchAlgorithm, Searcher
+from ray.tune.search.sample import Domain
 
 from autogluon.common.utils.resource_utils import ResourceManager
-from abc import ABC, abstractmethod
-from typing import Optional, Callable, Union, List
 
-from .constants import (
-    MIN,
-    MAX,
-)
-from .ray_tune_constants import (
-    SEARCHER_PRESETS,
-    SCHEDULER_PRESETS
-)
+from ..ray.resources_calculator import ResourceCalculator, ResourceCalculatorFactory
+from .constants import MAX, MIN
 from .exceptions import EmptySearchSpace
+from .ray_tune_constants import SCHEDULER_PRESETS, SEARCHER_PRESETS
 from .ray_tune_scheduler_factory import SchedulerFactory
 from .ray_tune_searcher_factory import SearcherFactory
 from .space_converter import RaySpaceConverterFactory
-from ..ray.resources_calculator import ResourceCalculatorFactory, ResourceCalculator
-
-from ray import tune
-from ray import air
-from ray.tune import PlacementGroupFactory, ExperimentAnalysis
-from ray.tune.search.sample import Domain
-from ray.tune.schedulers import TrialScheduler
-from ray.tune.search import SearchAlgorithm, Searcher
-
 
 logger = logging.getLogger(__name__)
 
 
 class RayTuneAdapter(ABC):
     """
     Abstract class to get module specific resource, and to update module specific arguments
     Instance of this class should be passed to `run` to provide custom behavior
     """
-    
+
     presets = {
-        'auto': {'searcher': 'random', 'scheduler': 'FIFO'},
-        'bayes': {'searcher': 'bayes', 'scheduler': 'FIFO'},
-        'random': {'searcher': 'random', 'scheduler': 'FIFO'}
+        "auto": {"searcher": "random", "scheduler": "FIFO"},
+        "bayes": {"searcher": "bayes", "scheduler": "FIFO"},
+        "random": {"searcher": "random", "scheduler": "FIFO"},
     }
     supported_searchers = []
     supported_schedulers = []
-    
+
     def __init__(self):
         self.num_parallel_jobs = None
         self.cpu_per_job = None
         self.gpu_per_job = None
         self.resources_per_trial = None
-        
+
     @property
     @abstractmethod
     def adapter_type(self):
         raise NotImplementedError
-   
+
     def get_supported_searchers(self) -> list:
         """
         Some searchers requires reporting status within epochs or checkpointing in the middle of training.
         If the trainable doesn't support those functionality, provide supported_searchers here to warn users HPO might not work as expected.
         Returns a list of supported searchers
         """
         return self.supported_searchers
@@ -74,69 +66,73 @@
     def get_supported_schedulers(self) -> list:
         """
         Some schedulers requires reporting status within epochs or checkpointing in the middle of training.
         If the trainable doesn't support those functionality, provide supported_schedulers here to warn users HPO might not work as expected.
         Returns a list of supported schedulers
         """
         return self.supported_schedulers
-    
+
     def check_user_provided_resources_per_trial(self, resources_per_trial: Optional[dict] = None):
         """Do checks or warnings on user provided resources here"""
         pass
-    
+
     @abstractmethod
     def get_resource_calculator(self, **kwargs) -> ResourceCalculator:
         """Get resource calculator"""
         raise NotImplementedError
-    
+
     def update_resource_info(self, resources_info: dict):
         """Get necessary info given resources_info"""
-        self.num_parallel_jobs = resources_info.get('num_parallel_jobs', None)
-        self.cpu_per_job = resources_info.get('cpu_per_job', None)
-        self.gpu_per_job = resources_info.get('gpu_per_job', None)
-        self.resources_per_trial = resources_info.get('resources_per_job', None)
-    
+        self.num_parallel_jobs = resources_info.get("num_parallel_jobs", None)
+        self.cpu_per_job = resources_info.get("cpu_per_job", None)
+        self.gpu_per_job = resources_info.get("gpu_per_job", None)
+        self.resources_per_trial = resources_info.get("resources_per_job", None)
+
     def get_resources_per_trial(
         self,
         total_resources: dict,
         num_samples: int,
         resources_per_trial: Optional[dict] = None,
         minimum_cpu_per_trial: int = 1,
         minimum_gpu_per_trial: float = 0.0,
         model_estimate_memory_usage: Optional[int] = None,
-        **kwargs
+        **kwargs,
     ) -> Union[dict, PlacementGroupFactory]:
         """
         Calculate resources per trial if not specified by the user
         """
         self.check_user_provided_resources_per_trial(resources_per_trial)
-        assert isinstance(minimum_cpu_per_trial, int) and minimum_cpu_per_trial >= 1, 'minimum_cpu_per_trial must be a integer that is larger than 0'
-        assert isinstance(minimum_gpu_per_trial, (int, float)) and minimum_gpu_per_trial >= 0, 'minimum_gpu_per_trial must be an integer or float that is equal to or larger than 0'
-        num_cpus = total_resources.get('num_cpus', ResourceManager.get_cpu_count_psutil())
-        num_gpus = total_resources.get('num_gpus', 0)
-        assert num_gpus >= minimum_gpu_per_trial, f'Total num_gpus available: {num_gpus} must be greater or equal to minimum_gpu_per_trial: {minimum_gpu_per_trial}'
-        
+        assert isinstance(minimum_cpu_per_trial, int) and minimum_cpu_per_trial >= 1, "minimum_cpu_per_trial must be a integer that is larger than 0"
+        assert (
+            isinstance(minimum_gpu_per_trial, (int, float)) and minimum_gpu_per_trial >= 0
+        ), "minimum_gpu_per_trial must be an integer or float that is equal to or larger than 0"
+        num_cpus = total_resources.get("num_cpus", ResourceManager.get_cpu_count_psutil())
+        num_gpus = total_resources.get("num_gpus", 0)
+        assert (
+            num_gpus >= minimum_gpu_per_trial
+        ), f"Total num_gpus available: {num_gpus} must be greater or equal to minimum_gpu_per_trial: {minimum_gpu_per_trial}"
+
         if minimum_gpu_per_trial > 0:
             resources_calculator = self.get_resource_calculator(num_gpus=num_gpus)
         else:
             resources_calculator = self.get_resource_calculator(num_gpus=0)
         resources_info = resources_calculator.get_resources_per_job(
             total_num_cpus=num_cpus,
             total_num_gpus=num_gpus,
             num_jobs=num_samples,
             minimum_cpu_per_job=minimum_cpu_per_trial,
             minimum_gpu_per_job=minimum_gpu_per_trial,
             model_estimate_memory_usage=model_estimate_memory_usage,
             user_resources_per_job=resources_per_trial,
             **kwargs,
         )
-        
+
         self.update_resource_info(resources_info)
         return self.resources_per_trial
-    
+
     @abstractmethod
     def trainable_args_update_method(trainable_args: dict) -> dict:
         """
         Update trainable_args being passed to tune.run with correct information for each trial.
         This can differ in forms for different predictor.
         """
         raise NotImplementedError
@@ -156,15 +152,15 @@
     minimum_cpu_per_trial: int = 1,
     minimum_gpu_per_trial: float = 0.0,
     model_estimate_memory_usage: Optional[int] = None,
     time_budget_s: Optional[float] = None,
     verbose: int = 1,
     tune_config_kwargs: Optional[dict] = None,
     run_config_kwargs: Optional[dict] = None,
-    ) -> tune.ExperimentAnalysis:
+) -> tune.ExperimentAnalysis:
     """
     Parse hyperparameter_tune_kwargs
     Init necessary objects, i.e. searcher, scheduler, and ray
     Translate search space
     Calculate resource per trial and update trainable_args accordingly
     Finally tune.run
 
@@ -210,150 +206,132 @@
     verbose
         0 = silent, 1 = only status updates, 2 = status and brief trial results, 3 = status and detailed trial results.
     tune_config_kwargs
         Additional args being passed to tune.TuneConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.tune.tune_config.TuneConfig
     run_config_kwargs
         Additional args being passed to air.RunConfig https://docs.ray.io/en/latest/ray-air/package-ref.html#ray.air.config.RunConfig
     """
-    assert mode in [MIN, MAX], f'mode {mode} is not a valid option. Options are {[MIN, MAX]}'
+    assert mode in [MIN, MAX], f"mode {mode} is not a valid option. Options are {[MIN, MAX]}"
     if isinstance(hyperparameter_tune_kwargs, str):
-        assert hyperparameter_tune_kwargs in ray_tune_adapter.presets, f'{hyperparameter_tune_kwargs} is not a valid option. Options are {ray_tune_adapter.presets.keys()}'
+        assert (
+            hyperparameter_tune_kwargs in ray_tune_adapter.presets
+        ), f"{hyperparameter_tune_kwargs} is not a valid option. Options are {ray_tune_adapter.presets.keys()}"
         hyperparameter_tune_kwargs = ray_tune_adapter.presets.get(hyperparameter_tune_kwargs)
-    num_samples = hyperparameter_tune_kwargs.get('num_trials', None)
+    num_samples = hyperparameter_tune_kwargs.get("num_trials", None)
     if num_samples is None:
         num_samples = 1 if time_budget_s is None else 1000  # if both num_samples and time_budget_s are None, we only run 1 trial
     if not any(isinstance(search_space[hyperparam], (ag_space.Space, Domain)) for hyperparam in search_space):
         raise EmptySearchSpace
     search_space, default_hyperparameters = _convert_search_space(search_space)
 
     searcher = _get_searcher(
         hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
         metric=metric,
         mode=mode,
         default_hyperparameters=default_hyperparameters,
-        supported_searchers=ray_tune_adapter.get_supported_searchers()
-    )
-    scheduler = _get_scheduler(
-        hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
-        supported_schedulers=ray_tune_adapter.get_supported_schedulers()
+        supported_searchers=ray_tune_adapter.get_supported_searchers(),
     )
+    scheduler = _get_scheduler(hyperparameter_tune_kwargs=hyperparameter_tune_kwargs, supported_schedulers=ray_tune_adapter.get_supported_schedulers())
 
     if not ray.is_initialized():
         if DistributedContext.is_distributed_mode():
             ray.init(address="auto")
         else:
             ray.init(
                 log_to_driver=False,
                 runtime_env={"env_vars": {"PL_DISABLE_FORK": "1"}},  # https://github.com/ray-project/ray/issues/28197
                 logging_level=logging.ERROR,  # https://github.com/ray-project/ray/issues/29216
-                **total_resources
+                **total_resources,
             )
 
-    resources_per_trial = hyperparameter_tune_kwargs.get('resources_per_trial', None)
+    resources_per_trial = hyperparameter_tune_kwargs.get("resources_per_trial", None)
     resources_per_trial = ray_tune_adapter.get_resources_per_trial(
         total_resources=total_resources,
         num_samples=num_samples,
         resources_per_trial=resources_per_trial,
         minimum_gpu_per_trial=minimum_gpu_per_trial,
         minimum_cpu_per_trial=minimum_cpu_per_trial,
         model_estimate_memory_usage=model_estimate_memory_usage,
         wrap_resources_per_job_into_placement_group=trainable_is_parallel,
     )
     resources_per_trial = _validate_resources_per_trial(resources_per_trial)
     logger.debug(f"resources_per_trial to be dispatched by ray tune: {resources_per_trial}")
     ray_tune_adapter.resources_per_trial = resources_per_trial
     trainable_args = ray_tune_adapter.trainable_args_update_method(trainable_args)
-    
+
     original_path = os.getcwd()
     save_dir = os.path.normpath(save_dir)
     if tune_config_kwargs is None:
         tune_config_kwargs = dict()
     if run_config_kwargs is None:
         run_config_kwargs = dict()
     tuner = tune.Tuner(
-        tune.with_resources(
-            tune.with_parameters(trainable, **trainable_args),
-            resources_per_trial
-        ),
+        tune.with_resources(tune.with_parameters(trainable, **trainable_args), resources_per_trial),
         param_space=search_space,
         tune_config=tune.TuneConfig(
-            num_samples=num_samples,
-            search_alg=searcher,
-            scheduler=scheduler,
-            metric=metric,
-            mode=mode,
-            time_budget_s=time_budget_s,
-            **tune_config_kwargs
+            num_samples=num_samples, search_alg=searcher, scheduler=scheduler, metric=metric, mode=mode, time_budget_s=time_budget_s, **tune_config_kwargs
         ),
-        run_config=air.RunConfig(
-            name=os.path.basename(save_dir),
-            local_dir=os.path.dirname(save_dir),
-            verbose=verbose,
-            **run_config_kwargs
-        ),
-        _tuner_kwargs={
-            "trial_name_creator": _trial_name_creator,
-            "trial_dirname_creator": _trial_dirname_creator
-        }
+        run_config=air.RunConfig(name=os.path.basename(save_dir), local_dir=os.path.dirname(save_dir), verbose=verbose, **run_config_kwargs),
+        _tuner_kwargs={"trial_name_creator": _trial_name_creator, "trial_dirname_creator": _trial_dirname_creator},
     )
     results = tuner.fit()
 
     os.chdir(original_path)  # go back to the original directory to avoid relative path being broken
     return results._experiment_analysis
 
 
 def cleanup_trials(save_dir: str, trials_to_keep: Optional[List[str]]):
     """
     Cleanup trial artifacts and keep trials as specified
-    
+
     Parameters
     ----------
     save_dir
         The path to the root of all the saved trials.
         This should be the same `save_dir` as you passed to `run`
     trials_to_keep
         List of trials to keep.
         Provide the dir name to the trial.
         This should be the same as trial_id if you didn't provide custom `trial_dirname_creator`
     """
     directories = [dir for dir in os.listdir(save_dir) if os.path.isdir(os.path.join(save_dir, dir))]
     for directory in directories:
         if directory not in trials_to_keep:
             shutil.rmtree(os.path.join(save_dir, directory))
-            
-            
+
+
 def cleanup_checkpoints(save_dir):
     """
     Cleanup trial artifacts and keep trials as specified
-    
+
     Parameters
     ----------
     save_dir
         The path to the root of all the saved checkpoints.
         This should be the path of a specific trial.
     """
-    directories = [dir for dir in os.listdir(save_dir) if os.path.isdir(os.path.join(save_dir, dir)) and dir.startswith('checkpoint')]
+    directories = [dir for dir in os.listdir(save_dir) if os.path.isdir(os.path.join(save_dir, dir)) and dir.startswith("checkpoint")]
     for directory in directories:
         shutil.rmtree(os.path.join(save_dir, directory))
-        
-        
+
+
 def _trial_name_creator(trial):
     return trial.trial_id
 
 
 def _trial_dirname_creator(trial):
     return trial.trial_id
 
 
 def _validate_resources_per_trial(resources_per_trial):
     if isinstance(resources_per_trial, dict):
-        if 'num_cpus' in resources_per_trial:
-            resources_per_trial['cpu'] = resources_per_trial.pop('num_cpus')
-        if 'num_gpus' in resources_per_trial:
-            resources_per_trial['gpu'] = resources_per_trial.pop('num_gpus')
+        if "num_cpus" in resources_per_trial:
+            resources_per_trial["cpu"] = resources_per_trial.pop("num_cpus")
+        if "num_gpus" in resources_per_trial:
+            resources_per_trial["gpu"] = resources_per_trial.pop("num_gpus")
     return resources_per_trial
 
 
 def _convert_search_space(search_space: dict):
     """Convert the search space to Ray Tune search space if it's AG search space"""
     tune_search_space = search_space.copy()
     default_hyperparameters = dict()
@@ -371,181 +349,182 @@
 
 
 def _get_searcher(
     hyperparameter_tune_kwargs: dict,
     metric: str,
     mode: str,
     default_hyperparameters: Optional[List[dict]] = None,
-    supported_searchers: Optional[List[str]]=None
+    supported_searchers: Optional[List[str]] = None,
 ):
     """Initialize searcher object"""
-    searcher = hyperparameter_tune_kwargs.get('searcher')
-    user_init_args = hyperparameter_tune_kwargs.get('searcher_init_args', dict())
+    searcher = hyperparameter_tune_kwargs.get("searcher")
+    user_init_args = hyperparameter_tune_kwargs.get("searcher_init_args", dict())
     if isinstance(searcher, str):
-        assert searcher in SEARCHER_PRESETS, f'{searcher} is not a valid option. Options are {SEARCHER_PRESETS.keys()}'
+        assert searcher in SEARCHER_PRESETS, f"{searcher} is not a valid option. Options are {SEARCHER_PRESETS.keys()}"
         # Check supported schedulers for str input
         if supported_searchers is not None:
             if searcher not in supported_searchers:
-                logger.warning(f'{searcher} is not supported yet. Using it might behave unexpected. Supported options are {supported_searchers}')
+                logger.warning(f"{searcher} is not supported yet. Using it might behave unexpected. Supported options are {supported_searchers}")
         searcher = SearcherFactory.get_searcher(
             searcher_name=searcher,
             user_init_args=user_init_args,
             metric=metric,
             mode=mode,
             points_to_evaluate=default_hyperparameters,
         )
     assert isinstance(searcher, (SearchAlgorithm, Searcher)) and searcher.__class__ in SEARCHER_PRESETS.values()
     # Check supported schedulers for obj input
     if supported_searchers is not None:
         supported_searchers_cls = [SEARCHER_PRESETS[searchers] for searchers in supported_searchers]
         if searcher.__class__ not in supported_searchers_cls:
-            logger.warning(f'{searcher.__class__} is not supported yet. Using it might behave unexpected. Supported options are {supported_searchers_cls}')
+            logger.warning(f"{searcher.__class__} is not supported yet. Using it might behave unexpected. Supported options are {supported_searchers_cls}")
     return searcher
 
 
-def _get_scheduler(hyperparameter_tune_kwargs: dict, supported_schedulers: Optional[List[str]]=None):
+def _get_scheduler(hyperparameter_tune_kwargs: dict, supported_schedulers: Optional[List[str]] = None):
     """Initialize scheduler object"""
-    scheduler = hyperparameter_tune_kwargs.get('scheduler')
-    user_init_args = hyperparameter_tune_kwargs.get('scheduler_init_args', dict())
+    scheduler = hyperparameter_tune_kwargs.get("scheduler")
+    user_init_args = hyperparameter_tune_kwargs.get("scheduler_init_args", dict())
     if isinstance(scheduler, str):
-        assert scheduler in SCHEDULER_PRESETS, f'{scheduler} is not a valid option. Options are {SCHEDULER_PRESETS.keys()}'
+        assert scheduler in SCHEDULER_PRESETS, f"{scheduler} is not a valid option. Options are {SCHEDULER_PRESETS.keys()}"
         # Check supported schedulers for str input
         if supported_schedulers is not None:
             if scheduler not in supported_schedulers:
-                logger.warning(f'{scheduler} is not supported yet. Using it might behave unexpected. Supported options are {supported_schedulers}')
+                logger.warning(f"{scheduler} is not supported yet. Using it might behave unexpected. Supported options are {supported_schedulers}")
         scheduler = SchedulerFactory.get_scheduler(
             scheduler_name=scheduler,
             user_init_args=user_init_args,
         )
     assert isinstance(scheduler, TrialScheduler) and scheduler.__class__ in SCHEDULER_PRESETS.values()
     # Check supported schedulers for obj input
     if supported_schedulers is not None:
         supported_schedulers_cls = [SCHEDULER_PRESETS[scheduler] for scheduler in supported_schedulers]
         if scheduler.__class__ not in supported_schedulers_cls:
-            logger.warning(f'{scheduler.__class__} is not supported yet. Using it might behave unexpected. Supported options are {supported_schedulers_cls}')
+            logger.warning(f"{scheduler.__class__} is not supported yet. Using it might behave unexpected. Supported options are {supported_schedulers_cls}")
     return scheduler
-    
-    
+
+
 class TabularRayTuneAdapter(RayTuneAdapter):
-    
-    supported_searchers = ['random', 'bayes']
-    supported_schedulers = ['FIFO']
-    
+
+    supported_searchers = ["random", "bayes"]
+    supported_schedulers = ["FIFO"]
+
     @property
     def adapter_type(self):
-        return 'tabular'
-    
+        return "tabular"
+
     def get_resource_calculator(self, num_gpus, **kwargs) -> ResourceCalculator:
-        return ResourceCalculatorFactory.get_resource_calculator(calculator_type='cpu' if num_gpus == 0 else 'gpu')
-    
+        return ResourceCalculatorFactory.get_resource_calculator(calculator_type="cpu" if num_gpus == 0 else "gpu")
+
     def trainable_args_update_method(self, trainable_args: dict) -> dict:
         if isinstance(self.resources_per_trial, dict):
-            trainable_args['fit_kwargs']['num_cpus'] = self.resources_per_trial.get('cpu', 1)
-            trainable_args['fit_kwargs']['num_gpus'] = self.resources_per_trial.get('gpu', 0)
+            trainable_args["fit_kwargs"]["num_cpus"] = self.resources_per_trial.get("cpu", 1)
+            trainable_args["fit_kwargs"]["num_gpus"] = self.resources_per_trial.get("gpu", 0)
         elif isinstance(self.resources_per_trial, tune.PlacementGroupFactory):
             required_resources = self.resources_per_trial.required_resources
-            trainable_args['fit_kwargs']['num_cpus'] = required_resources.get('CPU', 1)
-            trainable_args['fit_kwargs']['num_gpus'] = required_resources.get('GPU', 0)
+            trainable_args["fit_kwargs"]["num_cpus"] = required_resources.get("CPU", 1)
+            trainable_args["fit_kwargs"]["num_gpus"] = required_resources.get("GPU", 0)
         return trainable_args
-    
-    
+
+
 class AutommRayTuneAdapter(RayTuneAdapter):
-    
-    supported_searchers = ['random', 'bayes']
-    supported_schedulers = ['FIFO', 'ASHA']
-    
+
+    supported_searchers = ["random", "bayes"]
+    supported_schedulers = ["FIFO", "ASHA"]
+
     def __init__(self):
         super().__init__()
-        
+
     @property
     def adapter_type(self):
-        return 'automm'
-        
+        return "automm"
+
     def check_user_provided_resources_per_trial(self, resources_per_trial: Optional[dict] = None):
         if resources_per_trial is not None:
             # We do not support a single trial running on multiple GPUs without ray_lightning for now.
-            num_gpus = resources_per_trial.get('num_gpus', None)
+            num_gpus = resources_per_trial.get("num_gpus", None)
             if num_gpus is not None and num_gpus > 1:
-                resources_per_trial['num_gpus'] = 1
-                logger.warning('We do not support a single trial running on multiple GPUs yet')
+                resources_per_trial["num_gpus"] = 1
+                logger.warning("We do not support a single trial running on multiple GPUs yet")
             return resources_per_trial
-        
+
     def get_resource_calculator(self, num_gpus: float):
-        return ResourceCalculatorFactory.get_resource_calculator(calculator_type='cpu' if num_gpus == 0 else 'non_parallel_gpu')
-        
+        return ResourceCalculatorFactory.get_resource_calculator(calculator_type="cpu" if num_gpus == 0 else "non_parallel_gpu")
+
     def trainable_args_update_method(self, trainable_args: dict) -> dict:
-        trainable_args['hyperparameters']['env.num_gpus'] = self.gpu_per_job
-        trainable_args['hyperparameters']['env.num_workers'] = self.cpu_per_job
-        
+        trainable_args["hyperparameters"]["env.num_gpus"] = self.gpu_per_job
+        trainable_args["hyperparameters"]["env.num_workers"] = self.cpu_per_job
+
         return trainable_args
-    
-    
+
+
 class AutommRayTuneLightningAdapter(RayTuneAdapter):
-    
-    supported_searchers = ['random', 'bayes']
-    supported_schedulers = ['FIFO', 'ASHA']
-    
+
+    supported_searchers = ["random", "bayes"]
+    supported_schedulers = ["FIFO", "ASHA"]
+
     def __init__(self):
         super().__init__()
         self.num_workers = None
         self.cpu_per_worker = None
-        
+
     @property
     def adapter_type(self):
-        return 'automm_ray_lightning'
-        
+        return "automm_ray_lightning"
+
     def check_user_provided_resources_per_trial(self, resources_per_trial: Optional[dict] = None):
         if resources_per_trial is not None:
             # Ray Lightning provides a way to get the resources_per_trial because of the complexity of head process and worker process.
             # It's non-trivial to let the user to specify it. Hence we disable such option
-            logger.warning('AutoMM does not support customized resources_per_trial. We will calculate it for you instead.')
+            logger.warning("AutoMM does not support customized resources_per_trial. We will calculate it for you instead.")
 
     def get_resource_calculator(self, num_gpus):
-        return ResourceCalculatorFactory.get_resource_calculator(calculator_type='ray_lightning_cpu' if num_gpus == 0 else 'ray_lightning_gpu')
-    
-    def update_resource_info(self, resources_info: dict): 
-        self.num_parallel_jobs = resources_info.get('num_parallel_jobs', None)
-        self.cpu_per_job = resources_info.get('cpu_per_job', None)
-        self.gpu_per_job = resources_info.get('gpu_per_job', None)
-        self.num_workers = resources_info.get('num_workers', None)
-        self.cpu_per_worker = resources_info.get('cpu_per_worker', None)
-        self.resources_per_trial = resources_info.get('resources_per_job', None)
-        
+        return ResourceCalculatorFactory.get_resource_calculator(calculator_type="ray_lightning_cpu" if num_gpus == 0 else "ray_lightning_gpu")
+
+    def update_resource_info(self, resources_info: dict):
+        self.num_parallel_jobs = resources_info.get("num_parallel_jobs", None)
+        self.cpu_per_job = resources_info.get("cpu_per_job", None)
+        self.gpu_per_job = resources_info.get("gpu_per_job", None)
+        self.num_workers = resources_info.get("num_workers", None)
+        self.cpu_per_worker = resources_info.get("cpu_per_worker", None)
+        self.resources_per_trial = resources_info.get("resources_per_job", None)
+
     def trainable_args_update_method(self, trainable_args: dict) -> dict:
         from ray_lightning import RayPlugin
-        trainable_args['hyperparameters']['env.num_gpus'] = self.gpu_per_job
-        trainable_args['hyperparameters']['env.num_workers'] = self.cpu_per_job
-        trainable_args['hyperparameters']['env.num_nodes'] = 1  # num_nodes is not needed by ray lightning. Setting it to default, which is 1
-        trainable_args['_ray_lightning_plugin'] = RayPlugin(
-                                                    num_workers=self.num_workers,
-                                                    num_cpus_per_worker=self.cpu_per_worker,
-                                                    use_gpu=self.gpu_per_job is not None,
-                                                )
+
+        trainable_args["hyperparameters"]["env.num_gpus"] = self.gpu_per_job
+        trainable_args["hyperparameters"]["env.num_workers"] = self.cpu_per_job
+        trainable_args["hyperparameters"]["env.num_nodes"] = 1  # num_nodes is not needed by ray lightning. Setting it to default, which is 1
+        trainable_args["_ray_lightning_plugin"] = RayPlugin(
+            num_workers=self.num_workers,
+            num_cpus_per_worker=self.cpu_per_worker,
+            use_gpu=self.gpu_per_job is not None,
+        )
         return trainable_args
 
 
 class TimeSeriesRayTuneAdapter(TabularRayTuneAdapter):
-    
-    supported_searchers = ['random', 'bayes']
-    supported_schedulers = ['FIFO']
-    
+
+    supported_searchers = ["random", "bayes"]
+    supported_schedulers = ["FIFO"]
+
     @property
     def adapter_type(self):
-        return 'timeseries'
+        return "timeseries"
 
 
 class RayTuneAdapterFactory:
-    
+
     __supported_adapters = [
         TabularRayTuneAdapter,
         TimeSeriesRayTuneAdapter,
         AutommRayTuneAdapter,
         AutommRayTuneLightningAdapter,
     ]
-    
+
     __type_to_adapter = {cls().adapter_type: cls for cls in __supported_adapters}
 
     @staticmethod
     def get_adapter(adapter_type: str) -> RayTuneAdapter:
         """Return the executor"""
-        assert adapter_type in RayTuneAdapterFactory.__type_to_adapter, f'{adapter_type} not supported'
+        assert adapter_type in RayTuneAdapterFactory.__type_to_adapter, f"{adapter_type} not supported"
         return RayTuneAdapterFactory.__type_to_adapter[adapter_type]
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/ray_tune_scheduler.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/ray_tune_scheduler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 import time
 
 from ray.tune.schedulers import FIFOScheduler
 
 
 class AvgEarlyStopFIFOScheduler(FIFOScheduler):
-    
     def __init__(self, time_limit=None, **kwargs):
         super().__init__(**kwargs)
         self.time_limit = time_limit
         assert self.time_limit is None or self.time_limit > 0
         self.time_start = time.time()
         self.prev_times = []
 
     def on_trial_complete(self, trial_runner, trial, result):
-        time_total = result.get('time_total_s', -1)
+        time_total = result.get("time_total_s", -1)
         if time_total != -1:
             self.prev_times.append(time_total)
         super().on_trial_complete(trial_runner, trial, result)
 
     def choose_trial_to_run(self, trial_runner):
         if self.time_limit is not None:
             time_elapsed = time.time() - self.time_start
             time_left = self.time_limit - time_elapsed
             if self.avg_time > time_left:
                 return None
         return super().choose_trial_to_run(trial_runner)
-            
+
     @property
     def avg_time(self):
         if len(self.prev_times) > 0:
             return sum(self.prev_times) / len(self.prev_times)
-        return float('-inf')
+        return float("-inf")
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/ray_tune_searcher_factory.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/ray_tune_searcher_factory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 from ray.tune.search.basic_variant import BasicVariantGenerator
 from ray.tune.search.hyperopt import HyperOptSearch
 
+
 class SearcherFactory:
-    
+
     searcher_presets = {
-        'random': BasicVariantGenerator,
-        'bayes': HyperOptSearch,
+        "random": BasicVariantGenerator,
+        "bayes": HyperOptSearch,
     }
-    
+
     # These needs to be provided explicitly as searcher init args
     # These should be experiment specified required args
     searcher_required_args = {
-        'random': ['points_to_evaluate'],
-        'bayes': ['metric', 'mode', 'points_to_evaluate'],
+        "random": ["points_to_evaluate"],
+        "bayes": ["metric", "mode", "points_to_evaluate"],
     }
-    
+
     # These are the default values if user not specified
     # These should be non-experiment specific args, which we just pick a default value for the users
     # Can be overridden by the users
     searcher_default_args = {
-        'random': {},
-        'bayes': {},
+        "random": {},
+        "bayes": {},
     }
-    
+
     @staticmethod
     def get_searcher(searcher_name: str, user_init_args, **kwargs):
-        assert searcher_name in SearcherFactory.searcher_presets, f'{searcher_name} is not a valid option. Options are {SearcherFactory.searcher_presets.keys()}'
+        assert (
+            searcher_name in SearcherFactory.searcher_presets
+        ), f"{searcher_name} is not a valid option. Options are {SearcherFactory.searcher_presets.keys()}"
         init_args = {arg: kwargs[arg] for arg in SearcherFactory.searcher_required_args[searcher_name]}
         init_args.update(SearcherFactory.searcher_default_args[searcher_name])
         init_args.update(user_init_args)
-        
+
         return SearcherFactory.searcher_presets[searcher_name](**init_args)
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/hpo/space_converter.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/hpo/space_converter.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,84 +1,80 @@
-from autogluon.common import space as ag_space
-
 from abc import ABC, abstractmethod
+
 from ray import tune
 
+from autogluon.common import space as ag_space
+
 
 class RaySpaceConverter(ABC):
-    
     @property
     @abstractmethod
     def space_type(self):
         """Type of the converter"""
         raise NotImplementedError
-    
+
     @staticmethod
     @abstractmethod
     def convert(space):
         """Convert the search space to ray search space"""
         raise NotImplementedError
-        
-        
+
+
 class RayCategoricalSpaceConverter(RaySpaceConverter):
-    
     @property
     def space_type(self):
         return ag_space.Categorical.__name__
-    
+
     @staticmethod
     def convert(space):
         assert isinstance(space, ag_space.Categorical)
         return tune.choice(space.data)
-    
+
 
 class RayRealSpaceConverter(RaySpaceConverter):
-    
     @property
     def space_type(self):
         return ag_space.Real.__name__
-    
+
     @staticmethod
     def convert(space):
         assert isinstance(space, ag_space.Real)
         if space.log:
             ray_space = tune.loguniform(space.lower, space.upper)
         else:
             ray_space = tune.uniform(space.lower, space.upper)
         return ray_space
-    
-    
+
+
 class RayIntSpaceConverter(RaySpaceConverter):
-    
     @property
     def space_type(self):
         return ag_space.Int.__name__
-    
+
     @staticmethod
     def convert(space):
         assert isinstance(space, ag_space.Int)
-        return tune.randint(space.lower, space.upper+1)
-    
+        return tune.randint(space.lower, space.upper + 1)
+
 
 class RayBoolSpaceConverter(RayIntSpaceConverter):
-    
     @property
     def space_type(self):
         return ag_space.Bool.__name__
 
 
 class RaySpaceConverterFactory:
-    
+
     __supported_converters = [
         RayCategoricalSpaceConverter,
         RayRealSpaceConverter,
         RayIntSpaceConverter,
         RayBoolSpaceConverter,
     ]
-    
+
     __type_to_converter = {cls().space_type: cls for cls in __supported_converters}
 
     @staticmethod
     def get_space_converter(converter_type: str) -> RaySpaceConverter:
         """Return the resource calculator"""
-        assert converter_type in RaySpaceConverterFactory.__type_to_converter, f'{converter_type} not supported'
+        assert converter_type in RaySpaceConverterFactory.__type_to_converter, f"{converter_type} not supported"
         return RaySpaceConverterFactory.__type_to_converter[converter_type]
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/learner/abstract_learner.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/learner/abstract_learner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import random
 import sys
-from typing import Type, Optional
+from typing import Optional, Type
 
 from autogluon.core.trainer import AbstractTrainer
 from autogluon.core.utils.loaders import load_pkl
-from autogluon.core.utils.savers import save_pkl, save_json
+from autogluon.core.utils.savers import save_json, save_pkl
 
 
 class AbstractLearner:
     """Abstract class for autogluon Learners. Learners encompass the learning problem end to end,
     including loading initial data, feature generation, model training, model prediction. Similar
     to Trainers, they implement `fit` and `predict` methods. The abstract method also includes
     concrete implementations of serialization/deserialization methods. Refer to individual
@@ -17,17 +17,15 @@
     """
 
     learner_info_json_name = "info.json"
     learner_info_name = "info.pkl"
     learner_file_name = "learner.pkl"
 
     def __init__(self, path_context: str, random_state: int = 0, **kwargs):
-        self.path, self.model_context, self.save_path = self.create_contexts(
-            path_context
-        )
+        self.path, self.model_context, self.save_path = self.create_contexts(path_context)
 
         self.is_trainer_present: bool = False
         self.trainer: Optional[AbstractTrainer] = None
         self.trainer_type: Optional[Type] = None
         self.trainer_path: Optional[str] = None
         self.reset_paths: bool = False
 
@@ -54,17 +52,15 @@
         model_context = os.path.join(path_context, "models") + os.path.sep
         save_path = os.path.join(path_context, self.learner_file_name)
         return path_context, model_context, save_path
 
     def set_contexts(self, path_context: str):
         """Update the path where model, learner, and trainer objects will be saved.
         Also see `create_contexts`."""
-        self.path, self.model_context, self.save_path = self.create_contexts(
-            path_context
-        )
+        self.path, self.model_context, self.save_path = self.create_contexts(path_context)
 
     @property
     def is_fit(self):
         return self.trainer_path is not None or self.trainer is not None
 
     def fit(self, *args, **kwargs):
         raise NotImplementedError
@@ -113,17 +109,15 @@
 
     def load_trainer(self) -> AbstractTrainer:
         if self.trainer is not None:
             return self.trainer
         else:
             if self.trainer_path is None:
                 raise AssertionError("Trainer does not exist.")
-            return self.trainer_type.load(  # noqa
-                path=self.trainer_path, reset_paths=self.reset_paths
-            )
+            return self.trainer_type.load(path=self.trainer_path, reset_paths=self.reset_paths)  # noqa
 
     # reset_paths=True if the learner files have changed location since fitting.
     # TODO: Potentially set reset_paths=False inside load function if it is the same path to
     # TODO: avoid re-computing paths on all models path_context -> path for v0.1
     @classmethod
     def load_info(cls, path, reset_paths=True, load_model_if_required=True):
         load_path = path + cls.learner_info_name
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/__init__.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+import json
 from abc import ABCMeta, abstractmethod
 from functools import partial
-import json
 
 import numpy as np
 import scipy
 import scipy.stats
 import sklearn.metrics
 
 try:
     from sklearn.metrics._classification import _check_targets, type_of_target
 except:
     from sklearn.metrics.classification import _check_targets, type_of_target
 
-from . import classification_metrics
+from ..constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
+from . import classification_metrics, quantile_metrics
 from .classification_metrics import confusion_matrix
-from . import quantile_metrics
-from ..constants import BINARY, MULTICLASS, REGRESSION, QUANTILE, SOFTCLASS
 
 
 class Scorer(object, metaclass=ABCMeta):
     """
     Scorer wraps an external or custom metric function to align it with AutoGluon's metric logic and API.
     Scorer will alter the returned metric output to ensure higher_is_better and to allow computing metric error. This greatly simplifies downstream logic.
     All metric logic within AutoGluon should use Scorer to ensure consistency whenever possible.
@@ -42,23 +41,24 @@
         The sign of the metric to ensure greater_is_better.
         For score metrics such as accuracy and r2, the sign should be 1.
         For error metrics such as log_loss and mean_squared_error, the sign should be -1.
     kwargs : dict, optional
         kwargs to pass to score_func when called.
         For example, kwargs = {"beta": 2} when using sklearn.metrics.fbeta_score where beta is a required argument.
     """
+
     def __init__(self, name: str, score_func: callable, optimum: float, sign: int, kwargs: dict = None):
         self.name = name
         if kwargs is None:
             kwargs = dict()
         self._kwargs = kwargs
         self._score_func = score_func
         self._optimum = optimum
         if sign != 1 and sign != -1:
-            raise ValueError(f'sign must be one of [1, -1], but was instead {sign}')
+            raise ValueError(f"sign must be one of [1, -1], but was instead {sign}")
         self._sign = sign
         self.alias = set()
 
     def __call__(self, y_true, y_pred, sample_weight=None, **kwargs) -> float:
         """
         Evaluate predicted target values for X relative to y_true.
 
@@ -85,15 +85,15 @@
             k = kwargs
         else:
             k = self._kwargs.copy()
             k.update(kwargs)
         if k is None:
             k = dict()
         if sample_weight is not None:
-            k['sample_weight'] = sample_weight
+            k["sample_weight"] = sample_weight
 
         return self._score(y_true=y_true, y_pred=y_pred, **k)
 
     def error(self, *args, **kwargs) -> float:
         """
         Returns error in lower_is_better format.
         An error of 0 indicates a perfect score.
@@ -121,16 +121,15 @@
 
     def _score(self, y_true, y_pred, **kwargs) -> float:
         y_true, y_pred, kwargs = self._preprocess(y_true=y_true, y_pred=y_pred, **kwargs)
         return self._sign * self._score_func(y_true, y_pred, **kwargs)
 
     def add_alias(self, alias):
         if alias == self.name:
-            raise ValueError(f'The alias "{alias}" is the same as the original name "{self.name}". '
-                             f'This is not allowed.')
+            raise ValueError(f'The alias "{alias}" is the same as the original name "{self.name}". ' f"This is not allowed.")
         self.alias.add(alias)
 
     @property
     def greater_is_better(self) -> bool:
         """
         Return whether the score returned by scorer(...) is in greater_is_better format.
         By default, all Scorers are in greater_is_better format.
@@ -198,19 +197,19 @@
         if isinstance(y_pred, list):
             y_pred = np.array(y_pred)
 
         if len(y_pred.shape) == 1 or y_pred.shape[1] == 1:
             pass  # must be regression, all other task types would return at least two probabilities
         else:
             type_true = type_of_target(y_true)
-            if type_true == 'continuous':
+            if type_true == "continuous":
                 pass
-            elif type_true in ['binary', 'multiclass']:
+            elif type_true in ["binary", "multiclass"]:
                 y_pred = np.argmax(y_pred, axis=1)
-            elif type_true == 'multilabel-indicator':
+            elif type_true == "multilabel-indicator":
                 y_pred[y_pred > 0.5] = 1.0
                 y_pred[y_pred <= 0.5] = 0.0
             else:
                 raise ValueError(type_true)
         return y_true, y_pred, kwargs
 
     @property
@@ -287,22 +286,22 @@
 
 class _QuantileScorer(Scorer):
     def _preprocess(self, y_true, y_pred, **kwargs):
         if isinstance(y_true, list):
             y_true = np.array(y_true)
         if isinstance(y_pred, list):
             y_pred = np.array(y_pred)
-        if 'quantile_levels' not in kwargs:
-            raise AssertionError('quantile_levels is required to score quantile metrics')
-        if isinstance(kwargs['quantile_levels'], list):
-            kwargs['quantile_levels'] = np.array(kwargs['quantile_levels'])
+        if "quantile_levels" not in kwargs:
+            raise AssertionError("quantile_levels is required to score quantile metrics")
+        if isinstance(kwargs["quantile_levels"], list):
+            kwargs["quantile_levels"] = np.array(kwargs["quantile_levels"])
 
         type_true = type_of_target(y_true)
 
-        if len(y_pred.shape) == 2 or y_pred.shape[1] >= 1 or type_true == 'continuous':
+        if len(y_pred.shape) == 2 or y_pred.shape[1] >= 1 or type_true == "continuous":
             pass  # must be quantile regression, all other task types would return at least two probabilities
         else:
             raise ValueError(type_true)
         return y_true, y_pred, kwargs
 
     @property
     def needs_pred(self):
@@ -319,34 +318,25 @@
     @property
     def needs_quantile(self):
         return True
 
 
 def _add_scorer_to_metric_dict(metric_dict, scorer):
     if scorer.name in metric_dict:
-        raise ValueError(f'Duplicated score name found! scorer={scorer}, name={scorer.name}. '
-                         f'Consider to register with a different name.')
+        raise ValueError(f"Duplicated score name found! scorer={scorer}, name={scorer.name}. " f"Consider to register with a different name.")
     metric_dict[scorer.name] = scorer
     for alias in scorer.alias:
         if alias in metric_dict:
-            raise ValueError(f'Duplicated alias found! scorer={scorer}, alias={alias}. '
-                             f'Consider to use a different alias.')
+            raise ValueError(f"Duplicated alias found! scorer={scorer}, alias={alias}. " f"Consider to use a different alias.")
         metric_dict[alias] = scorer
 
 
-def make_scorer(name,
-                score_func,
-                *,
-                optimum=1,
-                greater_is_better=True,
-                needs_proba=False,
-                needs_threshold=False,
-                needs_quantile=False,
-                metric_kwargs: dict = None,
-                **kwargs) -> Scorer:
+def make_scorer(
+    name, score_func, *, optimum=1, greater_is_better=True, needs_proba=False, needs_threshold=False, needs_quantile=False, metric_kwargs: dict = None, **kwargs
+) -> Scorer:
     """Make a scorer from a performance metric or loss function.
 
     Factory inspired by scikit-learn which wraps scikit-learn scoring functions
     to be used in auto-sklearn.
 
     Parameters
     ----------
@@ -404,115 +394,80 @@
         optimum=optimum,
         sign=sign,
         kwargs=kwargs,
     )
 
 
 # Standard regression scores
-r2 = make_scorer('r2',
-                 sklearn.metrics.r2_score)
-mean_squared_error = make_scorer('mean_squared_error',
-                                 sklearn.metrics.mean_squared_error,
-                                 optimum=0,
-                                 greater_is_better=False)
-mean_squared_error.add_alias('mse')
-
-mean_absolute_error = make_scorer('mean_absolute_error',
-                                  sklearn.metrics.mean_absolute_error,
-                                  optimum=0,
-                                  greater_is_better=False)
-mean_absolute_error.add_alias('mae')
-
-median_absolute_error = make_scorer('median_absolute_error',
-                                    sklearn.metrics.median_absolute_error,
-                                    optimum=0,
-                                    greater_is_better=False)
-
-mean_absolute_percentage_error = make_scorer('mean_absolute_percentage_error',
-                                    sklearn.metrics.mean_absolute_percentage_error,
-                                    optimum=0,
-                                    greater_is_better=False)
-mean_absolute_percentage_error.add_alias('mape')
+r2 = make_scorer("r2", sklearn.metrics.r2_score)
+mean_squared_error = make_scorer("mean_squared_error", sklearn.metrics.mean_squared_error, optimum=0, greater_is_better=False)
+mean_squared_error.add_alias("mse")
+
+mean_absolute_error = make_scorer("mean_absolute_error", sklearn.metrics.mean_absolute_error, optimum=0, greater_is_better=False)
+mean_absolute_error.add_alias("mae")
+
+median_absolute_error = make_scorer("median_absolute_error", sklearn.metrics.median_absolute_error, optimum=0, greater_is_better=False)
+
+mean_absolute_percentage_error = make_scorer(
+    "mean_absolute_percentage_error", sklearn.metrics.mean_absolute_percentage_error, optimum=0, greater_is_better=False
+)
+mean_absolute_percentage_error.add_alias("mape")
 
 
 def local_spearmanr(y_true, y_pred):
     return float(scipy.stats.spearmanr(y_true, y_pred)[0])
 
 
-spearmanr = make_scorer('spearmanr',
-                        local_spearmanr,
-                        optimum=1.0,
-                        greater_is_better=True)
+spearmanr = make_scorer("spearmanr", local_spearmanr, optimum=1.0, greater_is_better=True)
 
 
 def local_pearsonr(y_true, y_pred):
     return float(scipy.stats.pearsonr(y_true, y_pred)[0])
 
 
-pearsonr = make_scorer('pearsonr',
-                       local_pearsonr,
-                       optimum=1.0,
-                       greater_is_better=True)
+pearsonr = make_scorer("pearsonr", local_pearsonr, optimum=1.0, greater_is_better=True)
 
 
 def rmse_func(y_true, y_pred, **kwargs):
     if kwargs:
         return sklearn.metrics.mean_squared_error(y_true, y_pred, squared=False, **kwargs)
     else:
         return np.sqrt(((y_true - y_pred) ** 2).mean())
 
 
-root_mean_squared_error = make_scorer('root_mean_squared_error',
-                                      rmse_func,
-                                      optimum=0,
-                                      greater_is_better=False)
-root_mean_squared_error.add_alias('rmse')
+root_mean_squared_error = make_scorer("root_mean_squared_error", rmse_func, optimum=0, greater_is_better=False)
+root_mean_squared_error.add_alias("rmse")
 
 # Quantile pinball loss
-pinball_loss = make_scorer('pinball_loss',
-                           quantile_metrics.pinball_loss,
-                           needs_quantile=True,
-                           optimum=0.0,
-                           greater_is_better=False)
-pinball_loss.add_alias('pinball')
+pinball_loss = make_scorer("pinball_loss", quantile_metrics.pinball_loss, needs_quantile=True, optimum=0.0, greater_is_better=False)
+pinball_loss.add_alias("pinball")
 
 
 # Standard Classification Scores
-accuracy = make_scorer('accuracy', sklearn.metrics.accuracy_score)
-accuracy.add_alias('acc')
+accuracy = make_scorer("accuracy", sklearn.metrics.accuracy_score)
+accuracy.add_alias("acc")
 
-balanced_accuracy = make_scorer('balanced_accuracy', classification_metrics.balanced_accuracy)
-f1 = make_scorer('f1', sklearn.metrics.f1_score)
-mcc = make_scorer('mcc', sklearn.metrics.matthews_corrcoef)
+balanced_accuracy = make_scorer("balanced_accuracy", classification_metrics.balanced_accuracy)
+f1 = make_scorer("f1", sklearn.metrics.f1_score)
+mcc = make_scorer("mcc", sklearn.metrics.matthews_corrcoef)
 
 
 # Score functions that need decision values
-roc_auc = make_scorer('roc_auc',
-                      classification_metrics.customized_binary_roc_auc_score,
-                      greater_is_better=True,
-                      needs_threshold=True)
-
-roc_auc_ovo_macro = make_scorer('roc_auc_ovo_macro',
-                                sklearn.metrics.roc_auc_score,
-                                multi_class='ovo',
-                                average='macro',
-                                greater_is_better=True,
-                                needs_proba=True,
-                                needs_threshold=False)
-
-average_precision = make_scorer('average_precision',
-                                sklearn.metrics.average_precision_score,
-                                needs_threshold=True)
-precision = make_scorer('precision',
-                        sklearn.metrics.precision_score)
-recall = make_scorer('recall',
-                     sklearn.metrics.recall_score)
+roc_auc = make_scorer("roc_auc", classification_metrics.customized_binary_roc_auc_score, greater_is_better=True, needs_threshold=True)
+
+roc_auc_ovo_macro = make_scorer(
+    "roc_auc_ovo_macro", sklearn.metrics.roc_auc_score, multi_class="ovo", average="macro", greater_is_better=True, needs_proba=True, needs_threshold=False
+)
+
+average_precision = make_scorer("average_precision", sklearn.metrics.average_precision_score, needs_threshold=True)
+precision = make_scorer("precision", sklearn.metrics.precision_score)
+recall = make_scorer("recall", sklearn.metrics.recall_score)
 
 # Register other metrics
-quadratic_kappa = make_scorer('quadratic_kappa', classification_metrics.quadratic_kappa, needs_proba=False)
+quadratic_kappa = make_scorer("quadratic_kappa", classification_metrics.quadratic_kappa, needs_proba=False)
 
 
 def customized_log_loss(y_true, y_pred, eps=1e-15):
     """
 
     Parameters
     ----------
@@ -531,36 +486,27 @@
         The negative log-likelihood
     """
     assert y_true.ndim == 1
     if y_pred.ndim == 1:
         # First clip the y_pred which is also used in sklearn
         # Convert to float64 to avoid rounding error on the clip operation with epsilon
         y_pred = np.clip(y_pred.astype(float), eps, 1 - eps)
-        return - (y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred)).mean()
+        return -(y_true * np.log(y_pred) + (1 - y_true) * np.log(1 - y_pred)).mean()
     else:
-        assert y_pred.ndim == 2, 'Only ndim=2 is supported'
+        assert y_pred.ndim == 2, "Only ndim=2 is supported"
         labels = np.arange(y_pred.shape[1], dtype=np.int32)
-        return sklearn.metrics.log_loss(y_true.astype(np.int32), y_pred,
-                                        labels=labels,
-                                        eps=eps)
+        return sklearn.metrics.log_loss(y_true.astype(np.int32), y_pred, labels=labels, eps=eps)
 
 
 # Score function for probabilistic classification
-log_loss = make_scorer('log_loss',
-                       customized_log_loss,
-                       optimum=0,
-                       greater_is_better=False,
-                       needs_proba=True)
-log_loss.add_alias('nll')
-
-pac = make_scorer('pac',
-                  classification_metrics.pac,
-                  greater_is_better=True,
-                  needs_proba=True)
-pac.add_alias('pac_score')
+log_loss = make_scorer("log_loss", customized_log_loss, optimum=0, greater_is_better=False, needs_proba=True)
+log_loss.add_alias("nll")
+
+pac = make_scorer("pac", classification_metrics.pac, greater_is_better=True, needs_proba=True)
+pac.add_alias("pac_score")
 
 REGRESSION_METRICS = dict()
 for scorer in [
     r2,
     mean_squared_error,
     root_mean_squared_error,
     mean_absolute_error,
@@ -592,23 +538,20 @@
 for scorer in [
     roc_auc,
     average_precision,
 ]:
     _add_scorer_to_metric_dict(metric_dict=BINARY_METRICS, scorer=scorer)
 
 
-for name, metric in [('precision', sklearn.metrics.precision_score),
-                     ('recall', sklearn.metrics.recall_score),
-                     ('f1', sklearn.metrics.f1_score)]:
+for name, metric in [("precision", sklearn.metrics.precision_score), ("recall", sklearn.metrics.recall_score), ("f1", sklearn.metrics.f1_score)]:
     globals()[name] = make_scorer(name, metric)
     _add_scorer_to_metric_dict(metric_dict=BINARY_METRICS, scorer=globals()[name])
-    for average in ['macro', 'micro', 'weighted']:
-        qualified_name = '{0}_{1}'.format(name, average)
-        globals()[qualified_name] = make_scorer(qualified_name,
-                                                partial(metric, pos_label=None, average=average))
+    for average in ["macro", "micro", "weighted"]:
+        qualified_name = "{0}_{1}".format(name, average)
+        globals()[qualified_name] = make_scorer(qualified_name, partial(metric, pos_label=None, average=average))
         _add_scorer_to_metric_dict(metric_dict=BINARY_METRICS, scorer=globals()[qualified_name])
         _add_scorer_to_metric_dict(metric_dict=MULTICLASS_METRICS, scorer=globals()[qualified_name])
 
 METRICS = {
     BINARY: BINARY_METRICS,
     MULTICLASS: MULTICLASS_METRICS,
     REGRESSION: REGRESSION_METRICS,
@@ -625,38 +568,41 @@
 
 
 def get_metric(metric, problem_type=None, metric_type=None) -> Scorer:
     """Returns metric function by using its name if the metric is str.
     Performs basic check for metric compatibility with given problem type."""
 
     if metric is not None and isinstance(metric, str):
-        if metric == 'soft_log_loss':
+        if metric == "soft_log_loss":
             if problem_type == QUANTILE:
                 raise ValueError(f"{metric_type}={metric} can not be used for quantile problems")
             from .softclass_metrics import soft_log_loss
+
             return soft_log_loss
         if problem_type is not None:
             if problem_type not in METRICS:
                 raise ValueError(f"Invalid problem_type '{problem_type}'. Valid problem types: {list(METRICS.keys())}")
             if metric not in METRICS[problem_type]:
                 valid_problem_types = _get_valid_metric_problem_types(metric)
                 if valid_problem_types:
-                    raise ValueError(f"{metric_type}='{metric}' is not a valid metric for problem_type='{problem_type}'. Valid problem_types for this metric: {valid_problem_types}")
+                    raise ValueError(
+                        f"{metric_type}='{metric}' is not a valid metric for problem_type='{problem_type}'. Valid problem_types for this metric: {valid_problem_types}"
+                    )
                 else:
-                    raise ValueError(f"Unknown metric '{metric}'. "
-                                     f"Valid metrics for problem_type='{problem_type}':\n"
-                                     f"{list(METRICS[problem_type].keys())}")
+                    raise ValueError(
+                        f"Unknown metric '{metric}'. " f"Valid metrics for problem_type='{problem_type}':\n" f"{list(METRICS[problem_type].keys())}"
+                    )
             return METRICS[problem_type][metric]
         for pt in METRICS:
             if metric in METRICS[pt]:
                 return METRICS[pt][metric]
         all_available_metrics = dict()
         for pt in METRICS:
             all_available_metrics[pt] = list(METRICS[pt].keys())
-        all_available_metrics[SOFTCLASS] = ['soft_log_loss']
+        all_available_metrics[SOFTCLASS] = ["soft_log_loss"]
 
         raise ValueError(
             f"{metric_type}='{metric}' is an unknown metric, all available metrics by problem_type are:\n"
             f"{json.dumps(all_available_metrics, indent=2)}\n"
             f"You can also refer to "
             f"autogluon.core.metrics to see how to define your own {metric_type} function"
         )
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/classification_metrics.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/classification_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,79 +1,73 @@
 import logging
 from typing import Union
 
 import numpy as np
 import pandas as pd
-from scipy.sparse import coo_matrix
 import sklearn
-from sklearn.utils.multiclass import unique_labels
-from sklearn.utils import check_consistent_length
+from scipy.sparse import coo_matrix
 from sklearn.metrics import cohen_kappa_score
+from sklearn.utils import check_consistent_length
+from sklearn.utils.multiclass import unique_labels
 
 try:
     from sklearn.metrics._classification import _check_targets, type_of_target
 except:
     from sklearn.metrics.classification import _check_targets, type_of_target
 
 logger = logging.getLogger(__name__)
 
 
 def balanced_accuracy(solution, prediction):
     y_type, solution, prediction = _check_targets(solution, prediction)
 
-    if y_type not in ["binary", "multiclass", 'multilabel-indicator']:
+    if y_type not in ["binary", "multiclass", "multilabel-indicator"]:
         raise ValueError(f"{y_type} is not supported")
 
-    if y_type == 'binary':
+    if y_type == "binary":
         # Do not transform into any multiclass representation
         pass
 
-    elif y_type == 'multiclass':
+    elif y_type == "multiclass":
         n = len(solution)
         unique_sol, encoded_sol = np.unique(solution, return_inverse=True)
         unique_pred, encoded_pred = np.unique(prediction, return_inverse=True)
         classes = np.unique(np.concatenate((unique_sol, unique_pred)))
-        map_sol = np.array([np.where(classes==c)[0][0] for c in unique_sol])
-        map_pred = np.array([np.where(classes==c)[0][0] for c in unique_pred])
+        map_sol = np.array([np.where(classes == c)[0][0] for c in unique_sol])
+        map_pred = np.array([np.where(classes == c)[0][0] for c in unique_pred])
         # one hot encoding
         sol_ohe = np.zeros((n, len(classes)))
         pred_ohe = np.zeros((n, len(classes)))
         sol_ohe[np.arange(n), map_sol[encoded_sol]] = 1
         pred_ohe[np.arange(n), map_pred[encoded_pred]] = 1
         solution = sol_ohe
         prediction = pred_ohe
 
-    elif y_type == 'multilabel-indicator':
+    elif y_type == "multilabel-indicator":
         solution = solution.toarray()
         prediction = prediction.toarray()
     else:
-        raise NotImplementedError(f'bac_metric does not support task type {y_type}')
+        raise NotImplementedError(f"bac_metric does not support task type {y_type}")
 
     fn = np.sum(np.multiply(solution, (1 - prediction)), axis=0, dtype=float)
     tp = np.sum(np.multiply(solution, prediction), axis=0, dtype=float)
     # Bounding to avoid division by 0
     eps = 1e-15
     tp = np.maximum(eps, tp)
     pos_num = np.maximum(eps, tp + fn)
     tpr = tp / pos_num  # true positive rate (sensitivity)
 
-    if y_type in ('binary', 'multilabel-indicator'):
-        tn = np.sum(
-            np.multiply((1 - solution), (1 - prediction)),
-            axis=0, dtype=float
-        )
-        fp = np.sum(
-            np.multiply((1 - solution), prediction),
-            axis=0, dtype=float
-        )
+    if y_type in ("binary", "multilabel-indicator"):
+        tn = np.sum(np.multiply((1 - solution), (1 - prediction)), axis=0, dtype=float)
+        fp = np.sum(np.multiply((1 - solution), prediction), axis=0, dtype=float)
         tn = np.maximum(eps, tn)
         neg_num = np.maximum(eps, tn + fp)
         tnr = tn / neg_num  # true negative rate (specificity)
         bac = 0.5 * (tpr + tnr)
-    elif y_type == 'multiclass':
+    elif y_type == "multiclass":
         bac = tpr
     else:
         raise ValueError(y_type)
 
     return np.mean(bac)  # average over all classes
 
 
@@ -100,18 +94,18 @@
         :return:
         """
         # Binarize solution
         sol = np.ravel(solution)  # convert to 1-d array
         maxi = np.nanmax(sol[np.isfinite(sol)])
         mini = np.nanmin(sol[np.isfinite(sol)])
         if maxi == mini:
-            logger.debug('Warning: cannot normalize array')
+            logger.debug("Warning: cannot normalize array")
             return [solution, prediction]
         diff = maxi - mini
-        mid = (maxi + mini) / 2.
+        mid = (maxi + mini) / 2.0
 
         solution[solution >= mid] = 1
         solution[solution < mid] = 0
         # Normalize and threshold predictions (takes effect only if solution not
         # in {0, 1})
 
         prediction -= float(mini)
@@ -127,15 +121,15 @@
 
     def log_loss(solution, prediction, task):
         """Log loss for binary and multiclass."""
         [sample_num, label_num] = solution.shape
         # Lower gives problems with float32!
         eps = 0.00000003
 
-        if (task == 'multiclass') and (label_num > 1):
+        if (task == "multiclass") and (label_num > 1):
             # Make sure the lines add up to one for multi-class classification
             norma = np.sum(prediction, axis=1)
             for k in range(sample_num):
                 prediction[k, :] /= np.maximum(norma[k], eps)
 
             sample_num = solution.shape[0]
             for i in range(sample_num):
@@ -147,21 +141,18 @@
             # For the base prediction, this solution is ridiculous in the
             # multi-label case
 
             # Bounding of predictions to avoid log(0),1/0,...
         prediction = np.minimum(1 - eps, np.maximum(eps, prediction))
         # Compute the log loss
         pos_class_log_loss = -np.mean(solution * np.log(prediction), axis=0)
-        if (task != 'multiclass') or (label_num == 1):
+        if (task != "multiclass") or (label_num == 1):
             # The multi-label case is a bunch of binary problems.
             # The second class is the negative class for each column.
-            neg_class_log_loss = -np.mean(
-                (1 - solution) * np.log(1 - prediction),
-                axis=0
-            )
+            neg_class_log_loss = -np.mean((1 - solution) * np.log(1 - prediction), axis=0)
             log_loss = pos_class_log_loss + neg_class_log_loss
             # Each column is an independent problem, so we average.
             # The probabilities in one line do not add up to one.
             # log_loss = mvmean(log_loss)
             # print('binary {}'.format(log_loss))
             # In the multilabel case, the right thing i to AVERAGE not sum
             # We return all the scores so we can normalize correctly later on
@@ -175,15 +166,15 @@
 
     def prior_log_loss(frac_pos, task):
         """Baseline log loss.
         For multiple classes or labels return the values for each column
         """
         eps = 1e-15
         frac_pos_ = np.maximum(eps, frac_pos)
-        if task != 'multiclass':  # binary case
+        if task != "multiclass":  # binary case
             frac_neg = 1 - frac_pos
             frac_neg_ = np.maximum(eps, frac_neg)
             pos_class_log_loss_ = -frac_pos * np.log(frac_pos_)
             neg_class_log_loss_ = -frac_neg * np.log(frac_neg_)
             base_log_loss = pos_class_log_loss_ + neg_class_log_loss_
             # base_log_loss = mvmean(base_log_loss)
             # print('binary {}'.format(base_log_loss))
@@ -199,59 +190,56 @@
     y_type = type_of_target(solution)
 
     if isinstance(solution, pd.Series):
         solution = solution.values
     if isinstance(prediction, pd.Series):
         prediction = prediction.values
 
-    if y_type == 'binary':
+    if y_type == "binary":
         if len(solution.shape) == 1:
             solution = solution.reshape((-1, 1))
         if len(prediction.shape) == 1:
             prediction = prediction.reshape((-1, 1))
         if len(prediction.shape) == 2:
             if prediction.shape[1] > 2:
-                raise ValueError(f'A prediction array with probability values '
-                                 f'for {prediction.shape[1]} classes is not a binary '
-                                 f'classification problem')
+                raise ValueError(f"A prediction array with probability values " f"for {prediction.shape[1]} classes is not a binary " f"classification problem")
             # Prediction will be copied into a new binary array - no copy
             prediction = prediction.reshape((-1, 1))
         else:
-            raise ValueError(f'Invalid prediction shape {prediction.shape}')
+            raise ValueError(f"Invalid prediction shape {prediction.shape}")
 
-    elif y_type == 'multiclass':
+    elif y_type == "multiclass":
         if len(solution.shape) == 2:
             if solution.shape[1] > 1:
-                raise ValueError(f'Solution array must only contain one class '
-                                 f'label, but contains {solution.shape[1]}')
+                raise ValueError(f"Solution array must only contain one class " f"label, but contains {solution.shape[1]}")
         elif len(solution.shape) == 1:
             pass
         else:
-            raise ValueError('Solution.shape %s' % solution.shape)
+            raise ValueError("Solution.shape %s" % solution.shape)
 
         # Need to create a multiclass solution and a multiclass predictions
         max_class = prediction.shape[1] - 1
         solution_binary = np.zeros((len(solution), max_class + 1))
         for i in range(len(solution)):
             solution_binary[i, int(solution[i])] = 1
         solution = solution_binary
 
-    elif y_type == 'multilabel-indicator':
+    elif y_type == "multilabel-indicator":
         solution = solution.copy()
 
     else:
-        raise NotImplementedError(f'pac_score does not support task {y_type}')
+        raise NotImplementedError(f"pac_score does not support task {y_type}")
 
     solution, prediction = normalize_array(solution, prediction.copy())
 
     sample_num, _ = solution.shape
 
     eps = 1e-7
     # Compute the base log loss (using the prior probabilities)
-    pos_num = 1. * np.sum(solution, axis=0, dtype=float)  # float conversion!
+    pos_num = 1.0 * np.sum(solution, axis=0, dtype=float)  # float conversion!
     frac_pos = pos_num / sample_num  # prior proba of positive class
     the_base_log_loss = prior_log_loss(frac_pos, y_type)
     the_log_loss = log_loss(solution, prediction, y_type)
 
     # Exponentiate to turn into an accuracy-like score.
     # In the multi-label case, we need to average AFTER taking the exp
     # because it is an NL operation
@@ -259,47 +247,47 @@
     base_pac = np.mean(np.exp(-the_base_log_loss))
     # Normalize: 0 for random, 1 for perfect
     score = (pac - base_pac) / np.maximum(eps, (1 - base_pac))
 
     return score
 
 
-def confusion_matrix(solution, prediction, labels=None, weights=None, normalize=None, output_format='numpy_array'):
+def confusion_matrix(solution, prediction, labels=None, weights=None, normalize=None, output_format="numpy_array"):
     """
-        Computes confusion matrix for a given true and predicted targets
-        Parameters:
-            solution - true targets
-            prediction - predicted targets
-            labels - list of labels for which confusion matrix should be calculated
-            weights - list of weights of each target
-            normalize - should the output be normalized. Can take values {'true', 'pred', 'all'}
-            output_format - output format of the matrix. Can take values {'python_list', 'numpy_array', 'pandas_dataframe'}
-        TODO : Add dedicated confusion_matrix function to AbstractLearner
+    Computes confusion matrix for a given true and predicted targets
+    Parameters:
+        solution - true targets
+        prediction - predicted targets
+        labels - list of labels for which confusion matrix should be calculated
+        weights - list of weights of each target
+        normalize - should the output be normalized. Can take values {'true', 'pred', 'all'}
+        output_format - output format of the matrix. Can take values {'python_list', 'numpy_array', 'pandas_dataframe'}
+    TODO : Add dedicated confusion_matrix function to AbstractLearner
     """
     y_type, solution, prediction = _check_targets(solution, prediction)
     # Only binary and multiclass data is supported
     if y_type not in ("binary", "multiclass"):
-        raise ValueError(f'{y_type} dataset is not currently supported')
+        raise ValueError(f"{y_type} dataset is not currently supported")
 
     if labels is None:
         labels = unique_labels(solution, prediction)
     else:
         # Ensure that label contains only 1-D binary or multi-class array
         labels_type = type_of_target(labels)
         if labels_type not in ("binary", "multiclass"):
-            raise ValueError(f'{labels_type} labels are not supported')
+            raise ValueError(f"{labels_type} labels are not supported")
         labels = np.array(labels)
 
     if weights is None:
         weights = np.ones(solution.size, dtype=int)
     else:
         # Ensure that weights contains only 1-D integer or float array
         weights_type = type_of_target(weights)
         if weights_type not in ("binary", "multiclass", "continuous"):
-            raise ValueError(f'{weights_type} weights are not supported')
+            raise ValueError(f"{weights_type} weights are not supported")
         weights = np.array(weights)
 
     n_labels = labels.size
     if n_labels == 0:
         raise ValueError("Labels cannot be empty")
     elif (np.unique(labels)).size != n_labels:
         raise ValueError("Labels cannot have duplicates")
@@ -313,34 +301,35 @@
 
     # Invalidate indexes with target labels outside the accepted set of labels
     valid_indexes = np.logical_and(np.in1d(solution, labels), np.in1d(prediction, labels))
     solution = np.array([label_to_index.get(i) for i in solution[valid_indexes]])
     prediction = np.array([label_to_index.get(i) for i in prediction[valid_indexes]])
     weights = weights[valid_indexes]
     # For high precision
-    matrix_dtype = np.int64 if weights.dtype.kind in {'i', 'u', 'b'} else np.float64
+    matrix_dtype = np.int64 if weights.dtype.kind in {"i", "u", "b"} else np.float64
     cm = coo_matrix((weights, (solution, prediction)), shape=(n_labels, n_labels), dtype=matrix_dtype).toarray()
-    with np.errstate(all='ignore'):
-        if normalize == 'true':
+    with np.errstate(all="ignore"):
+        if normalize == "true":
             cm = cm / cm.sum(axis=1, keepdims=True)
-        elif normalize == 'pred':
+        elif normalize == "pred":
             cm = cm / cm.sum(axis=0, keepdims=True)
-        elif normalize == 'all':
+        elif normalize == "all":
             cm = cm / cm.sum()
         cm = np.nan_to_num(cm)
-    if output_format == 'python_list':
+    if output_format == "python_list":
         return cm.tolist()
-    elif output_format == 'numpy_array':
+    elif output_format == "numpy_array":
         return cm
-    elif output_format == 'pandas_dataframe':
+    elif output_format == "pandas_dataframe":
         cm_df = pd.DataFrame(data=cm, index=labels, columns=labels)
         return cm_df
     else:
         return cm
 
+
 # TODO Add the "labels" option to metrics that will require the label map.
 #  We will need to update how we use those metrics accordingly.
 def quadratic_kappa(y_true, y_pred):
     """Calculate the cohen kappa score with quadratic weighting scheme.
 
     This is also known as "quadratic kappa" in the Kaggle competitions
     such as petfinder: https://www.kaggle.com/c/petfinder-adoption-prediction/overview/evaluation
@@ -363,15 +352,15 @@
     labels = None
     if y_pred.ndim > 1:
         if labels is not None:
             assert len(labels) == y_pred.shape[1]
         else:
             labels = np.arange(y_pred.shape[1])
         y_pred = np.argmax(y_pred, axis=-1)
-    return cohen_kappa_score(y_true, y_pred, labels=labels, weights='quadratic')
+    return cohen_kappa_score(y_true, y_pred, labels=labels, weights="quadratic")
 
 
 # Refer to https://github.com/scikit-learn/scikit-learn/blame/f3f51f9b611bf873bd5836748647221480071a87/sklearn/metrics/_ranking.py#L985-L1000
 #  for the original logic and full explanation of what this does. This number has no impact on the score calculated, and is purely for speed.
 #  This value was chosen as having a lower value simply slows down the majority of function calls more than it speeds them up.
 #  It was observed that function calls were sped up by 25% by increasing this from 2 to 100000.
 #  Values greater than this were not tested but would be marginal difference as large samples get less speed up.
@@ -420,17 +409,15 @@
     # keep track of how many true positives and false positives have occurred at each threshold
     tps = np.cumsum(y_true)[threshold_idxs]
     fps = 1 + threshold_idxs - tps
 
     if tps.size > _OPTIMIZE_INDICES_THRESHOLD:
         # optimize indices only when there is enough size to justify
         # this has no impact on the final score
-        optimal_idxs = np.where(
-            np.r_[True, np.logical_or(np.diff(fps, 2), np.diff(tps, 2)), True]
-        )[0]
+        optimal_idxs = np.where(np.r_[True, np.logical_or(np.diff(fps, 2), np.diff(tps, 2)), True])[0]
         fps = fps[optimal_idxs]
         tps = tps[optimal_idxs]
 
     # Add an extra threshold position
     # to make sure that the curve starts at (0, 0)
     tps = np.r_[0, tps]
     fps = np.r_[0, fps]
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/quantile_metrics.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/quantile_metrics.py`

 * *Files identical despite different names*

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/metrics/softclass_metrics.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/metrics/softclass_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 logger = logging.getLogger(__name__)
 
 EPS = 1e-10  # clipping threshold to prevent NaN
 
 
 def _soft_log_loss(true_probs, predicted_probs):
-    """ Both args must be 2D pandas/numpy arrays """
+    """Both args must be 2D pandas/numpy arrays"""
     true_probs = np.array(true_probs)
     predicted_probs = np.array(predicted_probs)
     if len(true_probs.shape) != 2 or len(predicted_probs.shape) != 2:
         raise ValueError("both truth and prediction must be 2D numpy arrays")
     if true_probs.shape != predicted_probs.shape:
         raise ValueError("truth and prediction must be 2D numpy arrays with the same shape")
 
@@ -25,9 +25,8 @@
     true_probs = true_probs / true_probs.sum(axis=1, keepdims=1)  # renormalize
     predicted_probs = predicted_probs / predicted_probs.sum(axis=1, keepdims=1)
     loss = -(np.log(predicted_probs) * true_probs).sum(axis=1).mean()
     return loss
 
 
 # Score for soft-classification (with soft, probabilistic labels):
-soft_log_loss = make_scorer('soft_log_loss', _soft_log_loss,
-                            greater_is_better=False, needs_proba=True)
+soft_log_loss = make_scorer("soft_log_loss", _soft_log_loss, greater_is_better=False, needs_proba=True)
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/_utils.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-
-from autogluon.core.utils.early_stopping import AdaptiveES, ES_CLASS_MAP
+from autogluon.core.utils.early_stopping import ES_CLASS_MAP, AdaptiveES
 
 
 # TODO: Add more strategies
-def get_early_stopping_rounds(num_rows_train, strategy='auto', min_patience=20, max_patience=300, min_rows=10000):
+def get_early_stopping_rounds(num_rows_train, strategy="auto", min_patience=20, max_patience=300, min_rows=10000):
     if isinstance(strategy, (tuple, list)):
         strategy = list(strategy)
         if isinstance(strategy[0], str):
             if strategy[0] in ES_CLASS_MAP:
                 strategy[0] = ES_CLASS_MAP[strategy[0]]
             else:
-                raise AssertionError(f'unknown early stopping strategy: {strategy}')
+                raise AssertionError(f"unknown early stopping strategy: {strategy}")
         return strategy
 
     """Gets early stopping rounds"""
-    if strategy == 'auto':
-        strategy = 'simple'
+    if strategy == "auto":
+        strategy = "simple"
 
     modifier = 1 if num_rows_train <= min_rows else min_rows / num_rows_train
     simple_early_stopping_rounds = max(
         round(modifier * max_patience),
         min_patience,
     )
-    if strategy == 'simple':
+    if strategy == "simple":
         return simple_early_stopping_rounds
-    elif strategy == 'adaptive':
+    elif strategy == "adaptive":
         return AdaptiveES, dict(adaptive_offset=min_patience, min_patience=simple_early_stopping_rounds)
     else:
-        raise AssertionError(f'unknown early stopping strategy: {strategy}')
+        raise AssertionError(f"unknown early stopping strategy: {strategy}")
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/_tags.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-
 _DEFAULT_TAGS = {
     # Whether the model can produce out-of-fold (or similar) predictions of the training data without being significantly overfit.
-    'valid_oof': False,
+    "valid_oof": False,
     # Whether the model can be refit using the combined train and val data as training and no validation data without issue.
     #  TL;DR: Keep value as False unless you know what you are doing. This is advanced functionality.
     #  If False, when calling predictor.refit_full(), this model will simply be duplicated (if non-bag) or will have the first fold model duplicated (if bag).
     #  This will result in a slightly worse refit model than an optimally implemented refit_full, but is a simple fallback that is still effective.
     #  If True (Advanced), when calling predictor.refit_full(), this model will be fit again on 100% of the data as training data (no validation data)
     #  using hyperparameters defined by this model's implementation.
     #  If a model does not use validation data in any way during training, then it is safe to set `can_infer_full` to True without additional work.
@@ -16,16 +15,16 @@
     #  we want the refit_full model to stop training on epoch 10 (trusting that its performance will mimic the original model).
     #  This can be implemented via passing epoch=10 (best epoch) at end of `_fit` by setting (example): `self.params_trained['epochs'] = self.model.best_epoch`
     #  If the model has even more complex functionality associated with the `epochs` value itself (such as cyclic learning rate),
     #  a solution is to pass epochs=100 and
     #  implement a new parameter `final_epoch=10` that forces the model to stop at `final_epoch` (while maintaining the same LR schedule).
     #  This can get very complex to implement correctly for refit_full.
     #  It is recommended in these scenarios to set `can_refit_full` to False until a correct implementation is added.
-    'can_refit_full': False,
+    "can_refit_full": False,
 }
 
 
 _DEFAULT_CLASS_TAGS = {
     # Whether the model can handle raw text input features.
     #  Used for informing the global feature preprocessor on if it should keep raw text features.
-    'handles_text': False,
+    "handles_text": False,
 }
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/abstract_model.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/abstract_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,43 +9,54 @@
 import time
 from typing import Any, Dict, Optional, Union
 
 import numpy as np
 import pandas as pd
 import scipy
 
-from autogluon.common.utils.distribute_utils import DistributedContext
 from autogluon.common.features.feature_metadata import FeatureMetadata
-from autogluon.common.utils.try_import import try_import_ray
+from autogluon.common.utils.distribute_utils import DistributedContext
+from autogluon.common.utils.lite import disable_if_lite_mode
+from autogluon.common.utils.log_utils import DuplicateFilter
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.path_converter import PathConverter
+from autogluon.common.utils.resource_utils import RayResourceManager, ResourceManager, get_resource_manager
+from autogluon.common.utils.try_import import try_import_ray
 from autogluon.common.utils.utils import setup_outputdir
-from autogluon.common.utils.lite import disable_if_lite_mode
-from autogluon.common.utils.log_utils import DuplicateFilter
-from autogluon.common.utils.resource_utils import ResourceManager, RayResourceManager
-from autogluon.common.utils.resource_utils import get_resource_manager
-from autogluon.common.utils.distribute_utils import DistributedContext
 
-from .model_trial import model_trial, skip_hpo
-from ._tags import _DEFAULT_CLASS_TAGS, _DEFAULT_TAGS
 from ... import metrics
-from ...constants import AG_ARG_PREFIX, AG_ARGS_FIT, BINARY, REGRESSION, QUANTILE, REFIT_FULL_SUFFIX, OBJECTIVES_TO_NORMALIZE
+from ...constants import (
+    AG_ARG_PREFIX,
+    AG_ARGS_FIT,
+    BINARY,
+    OBJECTIVES_TO_NORMALIZE,
+    QUANTILE,
+    REFIT_FULL_SUFFIX,
+    REGRESSION,
+)
 from ...data.label_cleaner import LabelCleaner, LabelCleanerMulticlassToBinary
+from ...hpo.constants import CUSTOM_BACKEND, RAY_BACKEND
 from ...hpo.exceptions import EmptySearchSpace
-from ...hpo.constants import RAY_BACKEND, CUSTOM_BACKEND
 from ...hpo.executors import HpoExecutor, HpoExecutorFactory
 from ...ray.resources_calculator import ResourceCalculator
 from ...scheduler import LocalSequentialScheduler
-from ...utils import get_pred_from_proba, normalize_pred_probas, infer_eval_metric, infer_problem_type, \
-    compute_permutation_feature_importance, compute_weighted_metric
-from ...utils.exceptions import TimeLimitExceeded, NoValidFeatures, NotEnoughMemoryError
+from ...utils import (
+    compute_permutation_feature_importance,
+    compute_weighted_metric,
+    get_pred_from_proba,
+    infer_eval_metric,
+    infer_problem_type,
+    normalize_pred_probas,
+)
+from ...utils.exceptions import NotEnoughMemoryError, NoValidFeatures, TimeLimitExceeded
 from ...utils.loaders import load_pkl
 from ...utils.savers import save_json, save_pkl
 from ...utils.time import sample_df_for_time_func, time_func
-
+from ._tags import _DEFAULT_CLASS_TAGS, _DEFAULT_TAGS
+from .model_trial import model_trial, skip_hpo
 
 logger = logging.getLogger(__name__)
 dup_filter = DuplicateFilter()
 logger.addFilter(dup_filter)
 
 
 class AbstractModel:
@@ -82,56 +93,51 @@
 
         You can also pass your own evaluation function here as long as it follows formatting of the functions defined in folder `autogluon.core.metrics`.
     hyperparameters : dict, default = None
         Hyperparameters that will be used by the model (can be search spaces instead of fixed values).
         If None, model defaults are used. This is identical to passing an empty dictionary.
     """
 
-    model_file_name = 'model.pkl'
-    model_info_name = 'info.pkl'
-    model_info_json_name = 'info.json'
-
-    def __init__(self,
-                 path: str = None,
-                 name: str = None,
-                 problem_type: str = None,
-                 eval_metric: Union[str, metrics.Scorer] = None,
-                 hyperparameters=None):
+    model_file_name = "model.pkl"
+    model_info_name = "info.pkl"
+    model_info_json_name = "info.json"
+
+    def __init__(self, path: str = None, name: str = None, problem_type: str = None, eval_metric: Union[str, metrics.Scorer] = None, hyperparameters=None):
 
         if name is None:
             self.name = self.__class__.__name__
-            logger.log(20, f'Warning: No name was specified for model, defaulting to class name: {self.name}')
+            logger.log(20, f"Warning: No name was specified for model, defaulting to class name: {self.name}")
         else:
             self.name = name  # TODO: v0.1 Consider setting to self._name and having self.name be a property so self.name can't be set outside of self.rename()
 
         self.path_root = path
         if self.path_root is None:
             path_suffix = self.name
             if len(self.name) > 0:
                 if self.name[0] != os.path.sep:
                     path_suffix = os.path.sep + path_suffix
             # TODO: Would be ideal to not create dir, but still track that it is unique. However, this isn't possible to do without a global list of used dirs or using UUID.
             path_cur = setup_outputdir(path=None, create_dir=True, path_suffix=path_suffix)
             self.path_root = path_cur.rsplit(self.path_suffix, 1)[0]
-            logger.log(20, f'Warning: No path was specified for model, defaulting to: {self.path_root}')
+            logger.log(20, f"Warning: No path was specified for model, defaulting to: {self.path_root}")
 
         # v0.9 FIXME: This is a hack, change so we aren't vulnerable to self.path_root breaking things
         self.path_root = PathConverter.to_relative(self.path_root)
 
         self.path = self.create_contexts(self.path_root + self.path_suffix)  # TODO: Make this path a function for consistency.
 
         self.num_classes = None
         self.model = None
         self.problem_type = problem_type
 
         # whether to calibrate predictions via conformal methods
         self.conformalize = None
 
         if eval_metric is not None:
-            self.eval_metric = metrics.get_metric(eval_metric, self.problem_type, 'eval_metric')  # Note: we require higher values = better performance
+            self.eval_metric = metrics.get_metric(eval_metric, self.problem_type, "eval_metric")  # Note: we require higher values = better performance
         else:
             self.eval_metric = None
         self.normalize_pred_probas = None
 
         self.features = None  # External features, do not use internally
         self.feature_metadata = None  # External feature metadata, do not use internally
         self._features_internal = None  # Internal features, safe to use internally via the `_features` property
@@ -152,15 +158,17 @@
         self._is_initialized = False
         self._is_fit_metadata_registered = False
         self._fit_metadata = dict()
 
         self._compiler = None
 
     @classmethod
-    def _init_user_params(cls, params: Optional[Dict[str, Any]] = None, ag_args_fit: str = AG_ARGS_FIT, ag_arg_prefix: str = AG_ARG_PREFIX) -> (Dict[str, Any], Dict[str, Any]):
+    def _init_user_params(
+        cls, params: Optional[Dict[str, Any]] = None, ag_args_fit: str = AG_ARGS_FIT, ag_arg_prefix: str = AG_ARG_PREFIX
+    ) -> (Dict[str, Any], Dict[str, Any]):
         """
         Given the user-specified hyperparameters, split into `params` and `params_aux`.
 
         Parameters
         ----------
         params : Optional[Dict[str, Any]], default = None
             The model hyperparameters dictionary
@@ -187,39 +195,45 @@
             params will contain the native model hyperparameters
             params_aux will contain special auxiliary hyperparameters
         """
         params = copy.deepcopy(params) if params is not None else dict()
         assert isinstance(params, dict), f"Invalid dtype of params! Expected dict, but got {type(params)}"
         for k in params.keys():
             if not isinstance(k, str):
-                logger.warning(f'Warning: Specified {cls.__name__} hyperparameter key is not of type str: {k} (type={type(k)}). '
-                               f'There might be a bug in your configuration.')
+                logger.warning(
+                    f"Warning: Specified {cls.__name__} hyperparameter key is not of type str: {k} (type={type(k)}). "
+                    f"There might be a bug in your configuration."
+                )
 
         params_aux = params.pop(ag_args_fit, dict())
         if params_aux is None:
             params_aux = dict()
         assert isinstance(params_aux, dict), f"Invalid dtype of params_aux! Expected dict, but got {type(params_aux)}"
         if ag_arg_prefix is not None:
             param_aux_keys = list(params_aux.keys())
             for k in param_aux_keys:
                 if isinstance(k, str) and k.startswith(ag_arg_prefix):
-                    k_no_prefix = k[len(ag_arg_prefix):]
+                    k_no_prefix = k[len(ag_arg_prefix) :]
                     if k_no_prefix in params_aux:
-                        logger.warning(f'Warning: {cls.__name__} hyperparameter "{k}" is present '
-                                       f'in `ag_args_fit` as both "{k}" and "{k_no_prefix}". '
-                                       f'Will use "{k}" and ignore "{k_no_prefix}".')
+                        logger.warning(
+                            f'Warning: {cls.__name__} hyperparameter "{k}" is present '
+                            f'in `ag_args_fit` as both "{k}" and "{k_no_prefix}". '
+                            f'Will use "{k}" and ignore "{k_no_prefix}".'
+                        )
                     params_aux[k_no_prefix] = params_aux.pop(k)
             param_keys = list(params.keys())
             for k in param_keys:
                 if isinstance(k, str) and k.startswith(ag_arg_prefix):
-                    k_no_prefix = k[len(ag_arg_prefix):]
+                    k_no_prefix = k[len(ag_arg_prefix) :]
                     if k_no_prefix in params_aux:
-                        logger.warning(f'Warning: {cls.__name__} hyperparameter "{k}" is present '
-                                       f'in both `ag_args_fit` and `hyperparameters`. '
-                                       f'Will use `hyperparameters` value.')
+                        logger.warning(
+                            f'Warning: {cls.__name__} hyperparameter "{k}" is present '
+                            f"in both `ag_args_fit` and `hyperparameters`. "
+                            f"Will use `hyperparameters` value."
+                        )
                     params_aux[k_no_prefix] = params.pop(k)
         return params, params_aux
 
     def _init_params(self):
         """Initializes model hyperparameters"""
         hyperparameters = self._user_params
         self._set_default_params()
@@ -332,16 +346,16 @@
         Returns
         -------
         dict of hyperparameter search spaces.
         """
         return {}
 
     def _get_search_space(self):
-        """ Sets up default search space for HPO. Each hyperparameter which user did not specify is converted from
-            default fixed value to default search space.
+        """Sets up default search space for HPO. Each hyperparameter which user did not specify is converted from
+        default fixed value to default search space.
         """
         def_search_space = self._get_default_searchspace().copy()
         # Note: when subclassing AbstractModel, you must define or import get_default_searchspace() from the appropriate location.
         for key in self.nondefault_params:  # delete all user-specified hyperparams from the default search space
             def_search_space.pop(key, None)
         params = self._get_params()
         params.update(def_search_space)
@@ -355,15 +369,15 @@
     @staticmethod
     def create_contexts(path_context):
         path = path_context
         return path
 
     def rename(self, name: str):
         """Renames the model and updates self.path to reflect the updated name."""
-        self.path = self.path[:-len(self.name) - 1] + name + os.path.sep
+        self.path = self.path[: -len(self.name) - 1] + name + os.path.sep
         self.name = name
 
     def preprocess(self, X, preprocess_nonadaptive=True, preprocess_stateful=True, **kwargs):
         """
         Preprocesses the input data into internal form ready for fitting or inference.
         It is not recommended to override this method, as it is closely tied to multi-layer stacking logic. Instead, override `_preprocess`.
         """
@@ -414,333 +428,335 @@
         if self.features is None:
             self.features = list(X.columns)
         # TODO: Consider changing how this works or where it is done
         if feature_metadata is None:
             feature_metadata = FeatureMetadata.from_df(X)
         else:
             feature_metadata = copy.deepcopy(feature_metadata)
-        get_features_kwargs = self.params_aux.get('get_features_kwargs', None)
+        get_features_kwargs = self.params_aux.get("get_features_kwargs", None)
         if get_features_kwargs is not None:
             valid_features = feature_metadata.get_features(**get_features_kwargs)
         else:
-            valid_raw_types = self.params_aux.get('valid_raw_types', None)
-            valid_special_types = self.params_aux.get('valid_special_types', None)
-            ignored_type_group_raw = self.params_aux.get('ignored_type_group_raw', None)
-            ignored_type_group_special = self.params_aux.get('ignored_type_group_special', None)
+            valid_raw_types = self.params_aux.get("valid_raw_types", None)
+            valid_special_types = self.params_aux.get("valid_special_types", None)
+            ignored_type_group_raw = self.params_aux.get("ignored_type_group_raw", None)
+            ignored_type_group_special = self.params_aux.get("ignored_type_group_special", None)
             valid_features = feature_metadata.get_features(
                 valid_raw_types=valid_raw_types,
                 valid_special_types=valid_special_types,
                 invalid_raw_types=ignored_type_group_raw,
-                invalid_special_types=ignored_type_group_special
+                invalid_special_types=ignored_type_group_special,
             )
-        get_features_kwargs_extra = self.params_aux.get('get_features_kwargs_extra', None)
+        get_features_kwargs_extra = self.params_aux.get("get_features_kwargs_extra", None)
         if get_features_kwargs_extra is not None:
             valid_features_extra = feature_metadata.get_features(**get_features_kwargs_extra)
             valid_features = [feature for feature in valid_features if feature in valid_features_extra]
         dropped_features = [feature for feature in self.features if feature not in valid_features]
-        logger.log(10, f'\tDropped {len(dropped_features)} of {len(self.features)} features.')
+        logger.log(10, f"\tDropped {len(dropped_features)} of {len(self.features)} features.")
         self.features = [feature for feature in self.features if feature in valid_features]
         self.feature_metadata = feature_metadata.keep_features(self.features)
-        error_if_no_features = self.params_aux.get('error_if_no_features', True)
+        error_if_no_features = self.params_aux.get("error_if_no_features", True)
         if error_if_no_features and not self.features:
             raise NoValidFeatures
         # TODO: If unique_counts == 2 (including NaN), then treat as boolean
-        if self.params_aux.get('drop_unique', True):
+        if self.params_aux.get("drop_unique", True):
             # TODO: Could this be optimized to be faster? This might be a bit slow for large data.
             unique_counts = X[self.features].nunique(axis=0, dropna=False)
             columns_to_drop = list(unique_counts[unique_counts < 2].index)
             features_to_drop_internal = columns_to_drop
             if not features_to_drop_internal:
                 features_to_drop_internal = None
         else:
             features_to_drop_internal = None
         if features_to_drop_internal is not None:
-            logger.log(10, f'\tDropped {len(features_to_drop_internal)} of {len(self.features)} internal features: {features_to_drop_internal}')
+            logger.log(10, f"\tDropped {len(features_to_drop_internal)} of {len(self.features)} internal features: {features_to_drop_internal}")
             self._features_internal = [feature for feature in self.features if feature not in features_to_drop_internal]
             self._feature_metadata = self.feature_metadata.keep_features(self._features_internal)
             self._is_features_in_same_as_ex = False
         else:
             self._features_internal = self.features
             self._feature_metadata = self.feature_metadata
             self._is_features_in_same_as_ex = True
         if error_if_no_features and not self._features_internal:
             raise NoValidFeatures
 
     def _preprocess_fit_args(self, **kwargs):
-        sample_weight = kwargs.get('sample_weight', None)
+        sample_weight = kwargs.get("sample_weight", None)
         if sample_weight is not None and isinstance(sample_weight, str):
             raise ValueError("In model.fit(), sample_weight should be array of sample weight values, not string.")
-        time_limit = kwargs.get('time_limit', None)
-        max_time_limit_ratio = self.params_aux.get('max_time_limit_ratio', 1)
+        time_limit = kwargs.get("time_limit", None)
+        max_time_limit_ratio = self.params_aux.get("max_time_limit_ratio", 1)
         if time_limit is not None:
             time_limit *= max_time_limit_ratio
-        max_time_limit = self.params_aux.get('max_time_limit', None)
+        max_time_limit = self.params_aux.get("max_time_limit", None)
         if max_time_limit is not None:
             if time_limit is None:
                 time_limit = max_time_limit
             else:
                 time_limit = min(time_limit, max_time_limit)
-        min_time_limit = self.params_aux.get('min_time_limit', 0)
+        min_time_limit = self.params_aux.get("min_time_limit", 0)
         if min_time_limit is None:
             time_limit = min_time_limit
         elif time_limit is not None:
             time_limit = max(time_limit, min_time_limit)
-        kwargs['time_limit'] = time_limit
+        kwargs["time_limit"] = time_limit
         kwargs = self._preprocess_fit_resources(**kwargs)
         return kwargs
 
     def initialize(self, **kwargs):
         if not self._is_initialized:
             self._initialize(**kwargs)
             self._is_initialized = True
 
-        kwargs.pop('feature_metadata', None)
-        kwargs.pop('num_classes', None)
+        kwargs.pop("feature_metadata", None)
+        kwargs.pop("num_classes", None)
         return kwargs
 
     def _initialize(self, X=None, y=None, feature_metadata=None, num_classes=None, **kwargs):
         if num_classes is not None:
             self.num_classes = num_classes
         if y is not None:
             if self.problem_type is None:
                 self.problem_type = infer_problem_type(y=y)
             if self.num_classes is None:
                 label_cleaner = LabelCleaner.construct(problem_type=self.problem_type, y=y)
                 self.num_classes = label_cleaner.num_classes
 
         self._init_params_aux()
 
-        self._init_misc(
-            X=X,
-            y=y,
-            feature_metadata=feature_metadata,
-            num_classes=num_classes,
-            **kwargs
-        )
+        self._init_misc(X=X, y=y, feature_metadata=feature_metadata, num_classes=num_classes, **kwargs)
 
         if X is not None:
             self._preprocess_set_features(X=X, feature_metadata=feature_metadata)
 
         self._init_params()
 
     def _init_misc(self, **kwargs):
         """Initialize parameters that depend on self.params_aux being initialized"""
         if self.eval_metric is None:
             self.eval_metric = infer_eval_metric(problem_type=self.problem_type)
-            logger.log(20, f"Model {self.name}'s eval_metric inferred to be '{self.eval_metric.name}' because problem_type='{self.problem_type}' and eval_metric was not specified during init.")
-        self.eval_metric = metrics.get_metric(self.eval_metric, self.problem_type, 'eval_metric')  # Note: we require higher values = better performance
+            logger.log(
+                20,
+                f"Model {self.name}'s eval_metric inferred to be '{self.eval_metric.name}' because problem_type='{self.problem_type}' and eval_metric was not specified during init.",
+            )
+        self.eval_metric = metrics.get_metric(self.eval_metric, self.problem_type, "eval_metric")  # Note: we require higher values = better performance
 
-        self.stopping_metric = self.params_aux.get('stopping_metric', self._get_default_stopping_metric())
-        self.stopping_metric = metrics.get_metric(self.stopping_metric, self.problem_type, 'stopping_metric')
+        self.stopping_metric = self.params_aux.get("stopping_metric", self._get_default_stopping_metric())
+        self.stopping_metric = metrics.get_metric(self.stopping_metric, self.problem_type, "stopping_metric")
 
-        self.quantile_levels = self.params_aux.get('quantile_levels', None)
+        self.quantile_levels = self.params_aux.get("quantile_levels", None)
 
         if self.eval_metric.name in OBJECTIVES_TO_NORMALIZE:
             self.normalize_pred_probas = True
             logger.debug(f"{self.name} predicted probabilities will be transformed to never =0 since eval_metric='{self.eval_metric.name}'")
         else:
             self.normalize_pred_probas = False
-            
-    def _process_user_provided_resource_requirement_to_calculate_total_resource_when_ensemble(self, system_resource, user_specified_total_resource, user_specified_ensemble_resource, resource_type, k_fold):
-        if user_specified_total_resource == 'auto':
+
+    def _process_user_provided_resource_requirement_to_calculate_total_resource_when_ensemble(
+        self, system_resource, user_specified_total_resource, user_specified_ensemble_resource, resource_type, k_fold
+    ):
+        if user_specified_total_resource == "auto":
             user_specified_total_resource = math.inf
-        
+
         # retrieve model level requirement when self is bagged model
         user_specified_model_level_resource = self._get_child_aux_val(key=resource_type, default=None)
         if user_specified_model_level_resource is not None:
-            assert user_specified_model_level_resource <= system_resource, f'Specified {resource_type} per model base is more than the total: {system_resource}'
+            assert user_specified_model_level_resource <= system_resource, f"Specified {resource_type} per model base is more than the total: {system_resource}"
         user_specified_lower_level_resource = user_specified_ensemble_resource
         if user_specified_ensemble_resource is not None:
             if user_specified_model_level_resource is not None:
-                user_specified_lower_level_resource = min(user_specified_model_level_resource * k_fold, user_specified_ensemble_resource, system_resource, user_specified_total_resource)
+                user_specified_lower_level_resource = min(
+                    user_specified_model_level_resource * k_fold, user_specified_ensemble_resource, system_resource, user_specified_total_resource
+                )
         else:
             if user_specified_model_level_resource is not None:
                 user_specified_lower_level_resource = min(user_specified_model_level_resource * k_fold, system_resource, user_specified_total_resource)
         return user_specified_lower_level_resource
-    
+
     def _calculate_total_resources(
-        self,
-        silent: bool = False,
-        total_resources: Optional[Dict[str, Union[int, float]]] = None,
-        parallel_hpo: bool = False,
-        **kwargs
+        self, silent: bool = False, total_resources: Optional[Dict[str, Union[int, float]]] = None, parallel_hpo: bool = False, **kwargs
     ) -> Dict[str, Any]:
         """
         Process user-specified total resources.
         Sanity checks will be done to user-specified total resources to make sure it's legit.
         When user-specified resources are not defined, will instead look at model's default resource requirements.
-        
+
         Will set the calculated total resources in kwargs and return it
         """
         resource_manager = get_resource_manager()
         system_num_cpus = resource_manager.get_cpu_count()
         system_num_gpus = resource_manager.get_gpu_count_all()
         if total_resources is None:
             total_resources = {}
-        num_cpus = total_resources.get('num_cpus', 'auto')
-        num_gpus = total_resources.get('num_gpus', 'auto')
+        num_cpus = total_resources.get("num_cpus", "auto")
+        num_gpus = total_resources.get("num_gpus", "auto")
         default_num_cpus, default_num_gpus = self._get_default_resources()
         # This could be resource requirement for bagged model or individual model
-        user_specified_lower_level_num_cpus = self._user_params_aux.get('num_cpus', None)
-        user_specified_lower_level_num_gpus = self._user_params_aux.get('num_gpus', None)
+        user_specified_lower_level_num_cpus = self._user_params_aux.get("num_cpus", None)
+        user_specified_lower_level_num_gpus = self._user_params_aux.get("num_gpus", None)
         if user_specified_lower_level_num_cpus is not None:
-            assert user_specified_lower_level_num_cpus <= system_num_cpus, f'Specified num_cpus per {self.__class__.__name__} is more than the total: {system_num_cpus}'
+            assert (
+                user_specified_lower_level_num_cpus <= system_num_cpus
+            ), f"Specified num_cpus per {self.__class__.__name__} is more than the total: {system_num_cpus}"
         if user_specified_lower_level_num_gpus is not None:
-            assert user_specified_lower_level_num_gpus <= system_num_cpus, f'Specified num_gpus per {self.__class__.__name__} is more than the total: {system_num_cpus}'
-        k_fold = kwargs.get('k_fold', None)
+            assert (
+                user_specified_lower_level_num_gpus <= system_num_cpus
+            ), f"Specified num_gpus per {self.__class__.__name__} is more than the total: {system_num_cpus}"
+        k_fold = kwargs.get("k_fold", None)
         if k_fold is not None and k_fold > 0:
             # bagged model will look ag_args_ensemble and ag_args_fit internally to determine resources
             # pass all resources here by default
             default_num_cpus = system_num_cpus
             default_num_gpus = system_num_gpus if default_num_gpus > 0 else 0
             user_specified_lower_level_num_cpus = self._process_user_provided_resource_requirement_to_calculate_total_resource_when_ensemble(
                 system_resource=system_num_cpus,
                 user_specified_total_resource=num_cpus,
                 user_specified_ensemble_resource=user_specified_lower_level_num_cpus,
-                resource_type='num_cpus',
-                k_fold=k_fold
+                resource_type="num_cpus",
+                k_fold=k_fold,
             )
             user_specified_lower_level_num_gpus = self._process_user_provided_resource_requirement_to_calculate_total_resource_when_ensemble(
                 system_resource=system_num_gpus,
                 user_specified_total_resource=num_gpus,
                 user_specified_ensemble_resource=user_specified_lower_level_num_gpus,
-                resource_type='num_gpus',
-                k_fold=k_fold
+                resource_type="num_gpus",
+                k_fold=k_fold,
             )
-        if num_cpus != 'auto' and num_cpus > system_num_cpus:
-            logger.warning(f'Specified total num_cpus: {num_cpus}, but only {system_num_cpus} are available. Will use {system_num_cpus} instead')
+        if num_cpus != "auto" and num_cpus > system_num_cpus:
+            logger.warning(f"Specified total num_cpus: {num_cpus}, but only {system_num_cpus} are available. Will use {system_num_cpus} instead")
             num_cpus = system_num_cpus
-        if num_gpus != 'auto' and num_gpus > system_num_gpus:
-            logger.warning(f'Specified total num_gpus: {num_gpus}, but only {system_num_gpus} are available. Will use {system_num_gpus} instead')
+        if num_gpus != "auto" and num_gpus > system_num_gpus:
+            logger.warning(f"Specified total num_gpus: {num_gpus}, but only {system_num_gpus} are available. Will use {system_num_gpus} instead")
             num_gpus = system_num_gpus
-        if num_cpus == 'auto':
+        if num_cpus == "auto":
             if user_specified_lower_level_num_cpus is not None:
                 if not parallel_hpo:
                     num_cpus = user_specified_lower_level_num_cpus
                 else:
                     num_cpus = system_num_cpus
             else:
                 if not parallel_hpo:
                     num_cpus = default_num_cpus
                 else:
                     num_cpus = system_num_cpus
         else:
             if not parallel_hpo:
                 if user_specified_lower_level_num_cpus is not None:
-                    assert user_specified_lower_level_num_cpus <= num_cpus, f'Specified num_cpus per {self.__class__.__name__} is more than the total specified: {num_cpus}'
+                    assert (
+                        user_specified_lower_level_num_cpus <= num_cpus
+                    ), f"Specified num_cpus per {self.__class__.__name__} is more than the total specified: {num_cpus}"
                     num_cpus = user_specified_lower_level_num_cpus
-        if num_gpus == 'auto':
+        if num_gpus == "auto":
             if user_specified_lower_level_num_gpus is not None:
                 if not parallel_hpo:
                     num_gpus = user_specified_lower_level_num_gpus
                 else:
                     num_gpus = system_num_gpus if user_specified_lower_level_num_gpus > 0 else 0
             else:
                 if not parallel_hpo:
                     num_gpus = default_num_gpus
                 else:
                     num_gpus = system_num_gpus if default_num_gpus > 0 else 0
         else:
             if not parallel_hpo:
                 if user_specified_lower_level_num_gpus is not None:
-                    assert user_specified_lower_level_num_gpus <= num_gpus, f'Specified num_gpus per {self.__class__.__name__} is more than the total specified: {num_gpus}'
+                    assert (
+                        user_specified_lower_level_num_gpus <= num_gpus
+                    ), f"Specified num_gpus per {self.__class__.__name__} is more than the total specified: {num_gpus}"
                     num_gpus = user_specified_lower_level_num_gpus
 
-        minimum_model_resources = self.get_minimum_resources(
-            is_gpu_available=(num_gpus > 0)
-        )
-        minimum_model_num_cpus = minimum_model_resources.get('num_cpus', 1)
-        minimum_model_num_gpus = minimum_model_resources.get('num_gpus', 0)
+        minimum_model_resources = self.get_minimum_resources(is_gpu_available=(num_gpus > 0))
+        minimum_model_num_cpus = minimum_model_resources.get("num_cpus", 1)
+        minimum_model_num_gpus = minimum_model_resources.get("num_gpus", 0)
 
         assert system_num_cpus >= num_cpus
         assert system_num_gpus >= num_gpus
 
-        assert system_num_cpus >= minimum_model_num_cpus, f'The total system num_cpus={system_num_cpus} is less than minimum num_cpus={minimum_model_num_cpus} to fit {self.__class__.__name__}. Consider using a machine with more CPUs.'
-        assert system_num_gpus >= minimum_model_num_gpus, f'The total system num_gpus={system_num_gpus} is less than minimum num_gpus={minimum_model_num_gpus} to fit {self.__class__.__name__}. Consider using a machine with more GPUs.'
+        assert (
+            system_num_cpus >= minimum_model_num_cpus
+        ), f"The total system num_cpus={system_num_cpus} is less than minimum num_cpus={minimum_model_num_cpus} to fit {self.__class__.__name__}. Consider using a machine with more CPUs."
+        assert (
+            system_num_gpus >= minimum_model_num_gpus
+        ), f"The total system num_gpus={system_num_gpus} is less than minimum num_gpus={minimum_model_num_gpus} to fit {self.__class__.__name__}. Consider using a machine with more GPUs."
+
+        assert (
+            num_cpus >= minimum_model_num_cpus
+        ), f"Specified num_cpus={num_cpus} per {self.__class__.__name__} is less than minimum num_cpus={minimum_model_num_cpus}"
+        assert (
+            num_gpus >= minimum_model_num_gpus
+        ), f"Specified num_gpus={num_gpus} per {self.__class__.__name__} is less than minimum num_gpus={minimum_model_num_gpus}"
 
-        assert num_cpus >= minimum_model_num_cpus, f'Specified num_cpus={num_cpus} per {self.__class__.__name__} is less than minimum num_cpus={minimum_model_num_cpus}'
-        assert num_gpus >= minimum_model_num_gpus, f'Specified num_gpus={num_gpus} per {self.__class__.__name__} is less than minimum num_gpus={minimum_model_num_gpus}'
-        
-        kwargs['num_cpus'] = num_cpus
-        kwargs['num_gpus'] = num_gpus
+        kwargs["num_cpus"] = num_cpus
+        kwargs["num_gpus"] = num_gpus
         if not silent:
             logger.log(15, f"\tFitting {self.name} with 'num_gpus': {kwargs['num_gpus']}, 'num_cpus': {kwargs['num_cpus']}")
-        
+
         return kwargs
 
     def _preprocess_fit_resources(
-        self,
-        silent: bool = False,
-        total_resources: Optional[Dict[str, Union[int, float]]] = None,
-        parallel_hpo: bool = False,
-        **kwargs
+        self, silent: bool = False, total_resources: Optional[Dict[str, Union[int, float]]] = None, parallel_hpo: bool = False, **kwargs
     ) -> Dict[str, Any]:
         """
         This function should be called to process user-specified total resources.
         Sanity checks will be done to user-specified total resources to make sure it's legit.
         When user-specified resources are not defined, will instead look at model's default resource requirements.
-        
+
         When kwargs contains `num_cpus` and `num_gpus` means this total resources has been calculated by previous layers(i.e. bagged model to model base).
         Will respect this value and check if there's specific maximum resource requirements and enforce those
-        
+
         Will set the calculated resources in kwargs and return it
         """
-        if 'num_cpus' in kwargs and 'num_gpus' in kwargs:
+        if "num_cpus" in kwargs and "num_gpus" in kwargs:
             # This value will only be passed by autogluon through previous layers(i.e. bagged model to model base).
             # We respect this value with highest priority
             # They should always be set to valid values
-            enforced_num_cpus = kwargs.get('num_cpus', None)
-            enforced_num_gpus = kwargs.get('num_gpus', None)
-            assert enforced_num_cpus is not None and enforced_num_cpus != 'auto' and enforced_num_gpus is not None and enforced_num_gpus != 'auto'
+            enforced_num_cpus = kwargs.get("num_cpus", None)
+            enforced_num_gpus = kwargs.get("num_gpus", None)
+            assert enforced_num_cpus is not None and enforced_num_cpus != "auto" and enforced_num_gpus is not None and enforced_num_gpus != "auto"
             # The logic below is needed because ray cluster is running some process in the backend even when it's ready to be used
             # Trying to use all cores on the machine could lead to resource contention situation
             # TODO: remove this logic if ray team can identify what's going on underneath and how to workaround
             max_resources = self._get_maximum_resources()
             max_num_cpus = max_resources.get("num_cpus", None)
             max_num_gpus = max_resources.get("num_gpus", None)
             if max_num_gpus is not None:
                 enforced_num_gpus = min(max_num_gpus, enforced_num_gpus)
             if DistributedContext.is_distributed_mode():
-                minimum_model_resources = self.get_minimum_resources(
-                    is_gpu_available=(enforced_num_gpus > 0)
-                )
-                minimum_model_num_cpus = minimum_model_resources.get('num_cpus', 1)
+                minimum_model_resources = self.get_minimum_resources(is_gpu_available=(enforced_num_gpus > 0))
+                minimum_model_num_cpus = minimum_model_resources.get("num_cpus", 1)
                 enforced_num_cpus = max(minimum_model_num_cpus, enforced_num_cpus - 2)  # leave some cpu resources for process running by cluster nodes
             if max_num_cpus is not None:
                 enforced_num_cpus = min(max_num_cpus, enforced_num_cpus)
             kwargs["num_cpus"] = enforced_num_cpus
             kwargs["num_gpus"] = enforced_num_gpus
             return kwargs
-        
+
         return self._calculate_total_resources(silent=silent, total_resources=total_resources, parallel_hpo=parallel_hpo, **kwargs)
 
     def _register_fit_metadata(self, **kwargs):
         """
         Used to track properties of the inputs received during fit, such as if validation data was present.
         """
         if not self._is_fit_metadata_registered:
             self._fit_metadata = self._compute_fit_metadata(**kwargs)
             self._is_fit_metadata_registered = True
 
     def _compute_fit_metadata(self, X_val=None, X_unlabeled=None, **kwargs):
-        fit_metadata = dict(
-            val_in_fit=X_val is not None,
-            unlabeled_in_fit=X_unlabeled is not None
-        )
+        fit_metadata = dict(val_in_fit=X_val is not None, unlabeled_in_fit=X_unlabeled is not None)
         return fit_metadata
 
     def get_fit_metadata(self) -> dict:
         """
         Returns dictionary of metadata related to model fit that isn't related to hyperparameters.
         Must be called after model has been fit.
         """
-        assert self._is_fit_metadata_registered, 'fit_metadata must be registered before calling get_fit_metadata()!'
+        assert self._is_fit_metadata_registered, "fit_metadata must be registered before calling get_fit_metadata()!"
         fit_metadata = dict()
         fit_metadata.update(self._fit_metadata)
-        fit_metadata['predict_1_batch_size'] = self._get_child_aux_val(key='predict_1_batch_size', default=None)
+        fit_metadata["predict_1_batch_size"] = self._get_child_aux_val(key="predict_1_batch_size", default=None)
         return fit_metadata
 
     def _get_child_aux_val(self, key: str, default=None):
         """
         Get aux val of child model (or self if no child)
         This is necessary to get a parameter value that is constant across all children without having to load the children after fitting.
         """
@@ -795,17 +811,19 @@
             verbosity 3: logs training iterations periodically, and logs more detailed information.
             verbosity 2: logs only important information.
             verbosity 1: logs only warnings and exceptions.
             verbosity 0: logs only exceptions.
         **kwargs :
             Any additional fit arguments a model supports.
         """
-        kwargs = self.initialize(**kwargs)  # FIXME: This might have to go before self._preprocess_fit_args, but then time_limit might be incorrect in **kwargs init to initialize
+        kwargs = self.initialize(
+            **kwargs
+        )  # FIXME: This might have to go before self._preprocess_fit_args, but then time_limit might be incorrect in **kwargs init to initialize
         kwargs = self._preprocess_fit_args(**kwargs)
-        if 'time_limit' in kwargs and kwargs['time_limit'] is not None and kwargs['time_limit'] <= 0:
+        if "time_limit" in kwargs and kwargs["time_limit"] is not None and kwargs["time_limit"] <= 0:
             logger.warning(f'\tWarning: Model has no time left to train, skipping model... (Time Left = {kwargs["time_limit"]:.1f}s)')
             raise TimeLimitExceeded
 
         self._register_fit_metadata(**kwargs)
         self.validate_fit_resources(**kwargs)
         self._validate_fit_memory_usage(**kwargs)
         out = self._fit(**kwargs)
@@ -820,40 +838,42 @@
         This should be focused around computing and saving metadata that is only possible post-fit.
         Parameters are identical to those passed to `self._fit(...)`.
 
         Returns
         -------
         Returns self
         """
-        predict_1_batch_size = self.params_aux.get('predict_1_batch_size', None)
-        if self.predict_1_time is None and predict_1_batch_size is not None and 'X' in kwargs and kwargs['X'] is not None:
-            X_1 = sample_df_for_time_func(df=kwargs['X'], sample_size=predict_1_batch_size)
+        predict_1_batch_size = self.params_aux.get("predict_1_batch_size", None)
+        if self.predict_1_time is None and predict_1_batch_size is not None and "X" in kwargs and kwargs["X"] is not None:
+            X_1 = sample_df_for_time_func(df=kwargs["X"], sample_size=predict_1_batch_size)
             self.predict_1_time = time_func(f=self.predict, args=[X_1]) / len(X_1)
         return self
 
     def get_features(self):
         assert self.is_fit(), "The model must be fit before calling the get_features method."
         if self.feature_metadata:
             return self.feature_metadata.get_features()
         else:
             return self.features
 
-    def _fit(self,
-             X,
-             y,
-             X_val=None,
-             y_val=None,
-             X_unlabeled=None,
-             time_limit=None,
-             sample_weight=None,
-             sample_weight_val=None,
-             num_cpus=None,
-             num_gpus=None,
-             verbosity=2,
-             **kwargs):
+    def _fit(
+        self,
+        X,
+        y,
+        X_val=None,
+        y_val=None,
+        X_unlabeled=None,
+        time_limit=None,
+        sample_weight=None,
+        sample_weight_val=None,
+        num_cpus=None,
+        num_gpus=None,
+        verbosity=2,
+        **kwargs,
+    ):
         """
         Fit model to predict values in y based on X.
 
         Models should override this method with their custom model fit logic.
         X should not be assumed to be in a state ready for fitting to the inner model, and models may require special preprocessing in this method.
         It is very important that `X = self.preprocess(X)` is called within `_fit`, or else `predict` and `predict_proba` may not work as intended.
         It is also important that `_preprocess` is overwritten to properly clean the data.
@@ -1030,61 +1050,55 @@
         model : cls
             Loaded model object.
         """
         file_path = path + cls.model_file_name
         model = load_pkl.load(path=file_path, verbose=verbose)
         if reset_paths:
             model.set_contexts(path)
-        if hasattr(model, '_compiler'):
+        if hasattr(model, "_compiler"):
             if model._compiler is not None and not model._compiler.save_in_pkl:
                 model.model = model._compiler.load(path=path)
         return model
 
-    def compute_feature_importance(self,
-                                   X,
-                                   y,
-                                   features=None,
-                                   silent=False,
-                                   importance_as_list=False,
-                                   **kwargs) -> pd.DataFrame:
+    def compute_feature_importance(self, X, y, features=None, silent=False, importance_as_list=False, **kwargs) -> pd.DataFrame:
         if self.features is not None:
             X = X[self.features]
 
         if not features:
             features = self.features
         else:
             features = list(features)
 
         # NOTE: Needed as bagged models 'features' attribute is not the same as childrens' 'features' attributes
         banned_features = [feature for feature in features if feature not in self.get_features()]
         features_to_check = [feature for feature in features if feature not in banned_features]
 
         if features_to_check:
             fi_df = self._compute_permutation_importance(X=X, y=y, features=features_to_check, silent=silent, importance_as_list=importance_as_list, **kwargs)
-            n = fi_df.iloc[0]['n'] if len(fi_df) > 0 else 1
+            n = fi_df.iloc[0]["n"] if len(fi_df) > 0 else 1
         else:
             fi_df = None
-            n = kwargs.get('num_shuffle_sets', 1)
+            n = kwargs.get("num_shuffle_sets", 1)
 
         if importance_as_list:
             banned_importance = [0] * n
-            results_banned = pd.Series(data=[banned_importance for _ in range(len(banned_features))], index=banned_features, dtype='object')
+            results_banned = pd.Series(data=[banned_importance for _ in range(len(banned_features))], index=banned_features, dtype="object")
         else:
             banned_importance = 0
-            results_banned = pd.Series(data=[banned_importance for _ in range(len(banned_features))], index=banned_features, dtype='float64')
+            results_banned = pd.Series(data=[banned_importance for _ in range(len(banned_features))], index=banned_features, dtype="float64")
 
-        results_banned_df = results_banned.to_frame(name='importance')
-        results_banned_df['stddev'] = 0
-        results_banned_df['n'] = n
-        results_banned_df['n'] = results_banned_df['n'].astype('int64')
+        results_banned_df = results_banned.to_frame(name="importance")
+        results_banned_df["stddev"] = 0
+        results_banned_df["n"] = n
+        results_banned_df["n"] = results_banned_df["n"].astype("int64")
         if fi_df is not None:
             fi_df = pd.concat([fi_df, results_banned_df])
         else:
             fi_df = results_banned_df
-        fi_df = fi_df.sort_values(ascending=False, by='importance')
+        fi_df = fi_df.sort_values(ascending=False, by="importance")
 
         return fi_df
 
     # Compute feature importance via permutation importance
     # Note: Expensive to compute
     #  Time to compute is O(predict_time*num_features)
     def _compute_permutation_importance(self, X, y, features: list, eval_metric=None, silent=False, **kwargs) -> pd.DataFrame:
@@ -1095,16 +1109,24 @@
             predict_func = self.predict
         else:
             predict_func = self.predict_proba
         transform_func_kwargs = dict(preprocess_stateful=False)
         predict_func_kwargs = dict(preprocess_nonadaptive=False)
 
         return compute_permutation_feature_importance(
-            X=X, y=y, features=features, eval_metric=self.eval_metric, predict_func=predict_func, predict_func_kwargs=predict_func_kwargs,
-            transform_func=transform_func, transform_func_kwargs=transform_func_kwargs, silent=silent, **kwargs
+            X=X,
+            y=y,
+            features=features,
+            eval_metric=self.eval_metric,
+            predict_func=predict_func,
+            predict_func_kwargs=predict_func_kwargs,
+            transform_func=transform_func,
+            transform_func_kwargs=transform_func_kwargs,
+            silent=silent,
+            **kwargs,
         )
 
     def can_compile(self, compiler_configs=None):
         """
         Verify whether the model can be compiled with the compiler configuration.
 
         Parameters
@@ -1113,15 +1135,15 @@
             Model specific compiler options.
             This can be useful to specify the compiler backend for a specific model,
             e.g. {"RandomForest": {"compiler": "onnx"}}
         """
         if not self.is_fit():
             return False
         compiler = compiler_configs.get("compiler", "native")
-        compiler_fallback_to_native = compiler_configs.get('compiler_fallback_to_native', False)
+        compiler_fallback_to_native = compiler_configs.get("compiler_fallback_to_native", False)
 
         compilers = self._valid_compilers()
         compiler_names = {c.name: c for c in compilers}
         if compiler is not None and compiler not in compiler_names:
             return False
         compiler_cls = compiler_names[compiler]
         if not compiler_cls.can_compile():
@@ -1145,25 +1167,24 @@
             e.g. {"RandomForest": {"compiler": "onnx"}}
         """
         assert self.is_fit(), "The model must be fit before calling the compile method."
         if compiler_configs is None:
             compiler_configs = {}
         compiler = compiler_configs.get("compiler", "native")
         batch_size = compiler_configs.get("batch_size", None)
-        compiler_fallback_to_native = compiler_configs.get('compiler_fallback_to_native', False)
+        compiler_fallback_to_native = compiler_configs.get("compiler_fallback_to_native", False)
 
-        self._compiler = self._get_compiler(compiler=compiler,
-                                            compiler_fallback_to_native=compiler_fallback_to_native)
+        self._compiler = self._get_compiler(compiler=compiler, compiler_fallback_to_native=compiler_fallback_to_native)
         if self._compiler is not None:
             input_types = self._get_input_types(batch_size=batch_size)
             self._compile(input_types=input_types)
 
     def _compile(self, **kwargs):
         """Take the compiler to perform actual compilation."""
-        input_types = kwargs.get('input_types', self._get_input_types(batch_size=None))
+        input_types = kwargs.get("input_types", self._get_input_types(batch_size=None))
         self.model = self._compiler.compile(model=self.model, path=self.path, input_types=input_types)
 
     # FIXME: This won't work for all models, and self._features is not
     # a trustworthy variable for final input shape
     def _get_input_types(self, batch_size=None) -> list:
         """
         Get input types as a list of tuples, containing shape and dtype.
@@ -1207,31 +1228,32 @@
             If this is True, the method would return native compiler when
             dependencies of the specified compiler is not installed. The fallback
             strategy won't be used by default.
         """
         compilers = self._valid_compilers()
         compiler_names = {c.name: c for c in compilers}
         if compiler is not None and compiler not in compiler_names:
-            raise AssertionError(f'Unknown compiler: {compiler}. Valid compilers: {compiler_names}')
+            raise AssertionError(f"Unknown compiler: {compiler}. Valid compilers: {compiler_names}")
         if compiler is None:
             return self._default_compiler()
         compiler_cls = compiler_names[compiler]
         if not compiler_cls.can_compile():
             if not compiler_fallback_to_native:
-                raise AssertionError(f'Specified compiler ({compiler}) is unable to compile'
-                                     ' (potentially lacking dependencies) and "compiler_fallback_to_native==False"')
+                raise AssertionError(
+                    f"Specified compiler ({compiler}) is unable to compile" ' (potentially lacking dependencies) and "compiler_fallback_to_native==False"'
+                )
             compiler_cls = self._default_compiler()
         return compiler_cls
 
     def get_compiler_name(self) -> str:
         assert self.is_fit(), "The model must be fit before calling the get_compiler_name method."
         if self._compiler is not None:
             return self._compiler.name
         else:
-            return 'native'
+            return "native"
 
     def get_trained_params(self) -> dict:
         """
         Returns the hyperparameters of the trained model.
         If the model early stopped, this will contain the epoch/iteration the model uses during inference, instead of the epoch/iteration specified during fit.
         This is used for generating a model template to refit on all of the data (no validation set).
         """
@@ -1281,25 +1303,21 @@
         template = self.__class__(**params)
 
         return template
 
     def convert_to_refit_full_template(self):
         """After calling this function, returned model should be able to be fit without X_val, y_val using the iterations trained by the original model."""
         params = copy.deepcopy(self.get_params())
-        params['hyperparameters'].update(self.params_trained)
-        params['name'] = params['name'] + REFIT_FULL_SUFFIX
+        params["hyperparameters"].update(self.params_trained)
+        params["name"] = params["name"] + REFIT_FULL_SUFFIX
         template = self.__class__(**params)
 
         return template
 
-    def hyperparameter_tune(self,
-                            hyperparameter_tune_kwargs = 'auto',
-                            hpo_executor: HpoExecutor = None,
-                            time_limit: float = None,
-                            **kwargs):
+    def hyperparameter_tune(self, hyperparameter_tune_kwargs="auto", hpo_executor: HpoExecutor = None, time_limit: float = None, **kwargs):
         """
         Perform hyperparameter tuning of the model, fitting multiple variants of the model based on the search space provided in `hyperparameters` during init.
 
         Parameters
         ----------
         hyperparameter_tune_kwargs : str or dict, default='auto'
             Hyperparameter tuning strategy and kwargs (for example, how many HPO trials to run).
@@ -1350,35 +1368,35 @@
         hpo_info: Any
             Advanced output with scheduler specific logic, primarily for debugging.
             In case of Ray Tune backend, this will be an Analysis object: https://docs.ray.io/en/latest/tune/api_docs/analysis.html
         """
         # if hpo_executor is not None, ensemble has already created the hpo_executor
         if hpo_executor is None:
             hpo_executor = self._get_default_hpo_executor()
-            default_num_trials = kwargs.pop('default_num_trials', None)
+            default_num_trials = kwargs.pop("default_num_trials", None)
             hpo_executor.initialize(hyperparameter_tune_kwargs, default_num_trials=default_num_trials, time_limit=time_limit)
         kwargs = self.initialize(time_limit=time_limit, **kwargs)
         self._register_fit_metadata(**kwargs)
         self._validate_fit_memory_usage(**kwargs)
-        kwargs = self._preprocess_fit_resources(parallel_hpo=hpo_executor.executor_type=='ray', **kwargs)
+        kwargs = self._preprocess_fit_resources(parallel_hpo=hpo_executor.executor_type == "ray", **kwargs)
         self.validate_fit_resources(**kwargs)
         hpo_executor.register_resources(self, **kwargs)
         return self._hyperparameter_tune(hpo_executor=hpo_executor, **kwargs)
 
     def _hyperparameter_tune(self, X, y, X_val, y_val, hpo_executor, **kwargs):
         """
         Hyperparameter tune the model.
 
         This usually does not need to be overwritten by models.
         """
         # verbosity = kwargs.get('verbosity', 2)
         time_start = time.time()
         logger.log(15, "Starting generic AbstractModel hyperparameter tuning for %s model..." % self.name)
         search_space = self._get_search_space()
-        
+
         try:
             hpo_executor.validate_search_space(search_space, self.name)
         except EmptySearchSpace:
             return skip_hpo(self, X=X, y=y, X_val=X_val, y_val=y_val, **kwargs)
 
         directory = self.path
         os.makedirs(directory, exist_ok=True)
@@ -1391,73 +1409,71 @@
         init_params = self.get_params()
         # We set soft time limit to avoid trials being terminated directly by ray tune
         trial_soft_time_limit = None
         if hpo_executor.time_limit is not None:
             trial_soft_time_limit = max(hpo_executor.time_limit * 0.9, hpo_executor.time_limit - 5)  # 5 seconds max for buffer
 
         fit_kwargs = dict()
-        fit_kwargs['feature_metadata'] = self.feature_metadata
-        fit_kwargs['num_classes'] = self.num_classes
-        fit_kwargs['sample_weight'] = kwargs.get('sample_weight', None)
-        fit_kwargs['sample_weight_val'] = kwargs.get('sample_weight_val', None)
+        fit_kwargs["feature_metadata"] = self.feature_metadata
+        fit_kwargs["num_classes"] = self.num_classes
+        fit_kwargs["sample_weight"] = kwargs.get("sample_weight", None)
+        fit_kwargs["sample_weight_val"] = kwargs.get("sample_weight_val", None)
         train_fn_kwargs = dict(
             model_cls=model_cls,
             init_params=init_params,
             time_start=time_start,
             time_limit=trial_soft_time_limit,
             fit_kwargs=fit_kwargs,
             train_path=train_path,
             val_path=val_path,
             hpo_executor=hpo_executor,
         )
         model_estimate_memory_usage = None
         if self.estimate_memory_usage is not None:
             model_estimate_memory_usage = self.estimate_memory_usage(X=X, **kwargs)
-        minimum_resources = self.get_minimum_resources(
-            is_gpu_available=(hpo_executor.resources.get('num_gpus', 0) > 0)
-        )
+        minimum_resources = self.get_minimum_resources(is_gpu_available=(hpo_executor.resources.get("num_gpus", 0) > 0))
         hpo_executor.execute(
             model_trial=model_trial,
             train_fn_kwargs=train_fn_kwargs,
             directory=directory,
-            minimum_cpu_per_trial=minimum_resources.get('num_cpus', 1),
-            minimum_gpu_per_trial=minimum_resources.get('num_gpus', 0),
+            minimum_cpu_per_trial=minimum_resources.get("num_cpus", 1),
+            minimum_gpu_per_trial=minimum_resources.get("num_gpus", 0),
             model_estimate_memory_usage=model_estimate_memory_usage,
-            adapter_type='tabular',
-            tune_config_kwargs={'chdir_to_trial_dir': False}
+            adapter_type="tabular",
+            tune_config_kwargs={"chdir_to_trial_dir": False},
         )
 
         hpo_results = hpo_executor.get_hpo_results(
             model_name=self.name,
             model_path_root=self.path_root,
             time_start=time_start,
         )
-        
+
         # cleanup artifacts
         for data_file in [train_path, val_path]:
             try:
                 os.remove(data_file)
             except FileNotFoundError:
                 pass
 
         return hpo_results
-    
+
     def _get_hpo_backend(self):
         """Choose which backend(Ray or Custom) to use for hpo"""
         if DistributedContext.is_distributed_mode():
             return RAY_BACKEND
         return CUSTOM_BACKEND
 
     def _get_default_hpo_executor(self) -> HpoExecutor:
         backend = self._get_model_base()._get_hpo_backend()  # If ensemble, will use the base model to determine backend
         if backend == RAY_BACKEND:
             try:
                 try_import_ray()
             except Exception as e:
-                warning_msg = f'Will use custom hpo logic because ray import failed. Reason: {str(e)}'
+                warning_msg = f"Will use custom hpo logic because ray import failed. Reason: {str(e)}"
                 dup_filter.attach_filter_targets(warning_msg)
                 logger.warning(warning_msg)
                 backend = CUSTOM_BACKEND
         hpo_executor = HpoExecutorFactory.get_hpo_executor(backend)()
         return hpo_executor
 
     @property
@@ -1476,16 +1492,17 @@
     # TODO: Experimental, currently unused
     #  Has not been tested on Windows
     #  Does not work if model is located in S3
     #  Does not work if called before model was saved to disk (Will output 0)
     def get_disk_size(self) -> int:
         # Taken from https://stackoverflow.com/a/1392549
         from pathlib import Path
+
         model_path = Path(self.path)
-        model_disk_size = sum(f.stat().st_size for f in model_path.glob('**/*') if f.is_file())
+        model_disk_size = sum(f.stat().st_size for f in model_path.glob("**/*") if f.is_file())
         return model_disk_size
 
     # TODO: This results in a doubling of memory usage of the model to calculate its size.
     #  If the model takes ~40%+ of memory, this may result in an OOM error.
     #  This is generally not an issue because the model already needed to do this when being saved to disk, so the error would have been triggered earlier.
     #  Consider using Pympler package for memory efficiency: https://pympler.readthedocs.io/en/latest/asizeof.html#asizeof
     def get_memory_size(self) -> int:
@@ -1498,35 +1515,35 @@
         Returns
         -------
             int: number of bytes will be used during training
         """
         assert self.is_initialized(), "Only estimate memory usage after the model is initialized."
         return self._estimate_memory_usage(**kwargs)
 
-    def validate_fit_resources(self, num_cpus='auto', num_gpus='auto', total_resources=None, **kwargs):
+    def validate_fit_resources(self, num_cpus="auto", num_gpus="auto", total_resources=None, **kwargs):
         """
         Verifies that the provided num_cpus and num_gpus (or defaults if not provided) are sufficient to train the model.
         Raises an AssertionError if not sufficient.
         """
         resources = self._preprocess_fit_resources(num_cpus=num_cpus, num_gpus=num_gpus, total_resources=total_resources, silent=True)
         self._validate_fit_resources(**resources)
 
     def _validate_fit_resources(self, **resources):
         res_min = self.get_minimum_resources()
         for resource_name in res_min:
             if resource_name not in resources:
-                raise AssertionError(f'Model requires {res_min[resource_name]} {resource_name} to fit, but no available amount was defined.')
+                raise AssertionError(f"Model requires {res_min[resource_name]} {resource_name} to fit, but no available amount was defined.")
             elif res_min[resource_name] > resources[resource_name]:
-                raise AssertionError(f'Model requires {res_min[resource_name]} {resource_name} to fit, but {resources[resource_name]} are available.')
-        total_resources = resources.get('total_resources', None)
+                raise AssertionError(f"Model requires {res_min[resource_name]} {resource_name} to fit, but {resources[resource_name]} are available.")
+        total_resources = resources.get("total_resources", None)
         if total_resources is None:
             total_resources = {}
         for resource_name, resource_value in total_resources.items():
             if resources[resource_name] > resource_value:
-                raise AssertionError(f'Specified {resources[resource_name]} {resource_name} to fit, but only {resource_value} are available in total.')
+                raise AssertionError(f"Specified {resources[resource_name]} {resource_name} to fit, but only {resource_value} are available in total.")
 
     def get_minimum_resources(self, is_gpu_available=False) -> Dict[str, Union[int, float]]:
         """
         Parameters
         ----------
         is_gpu_available
             Whether gpu is available in the system.
@@ -1534,15 +1551,15 @@
 
         Returns a dictionary of minimum resource requirements to fit the model.
         Subclass should consider overriding this method if it requires more resources to train.
         If a resource is not part of the output dictionary, it is considered unnecessary.
         Valid keys: 'num_cpus', 'num_gpus'.
         """
         return {
-            'num_cpus': 1,
+            "num_cpus": 1,
         }
 
     def _estimate_memory_usage(self, X: pd.DataFrame, **kwargs) -> int:
         """
         Estimates the peak memory usage during model fitting.
         This method simply provides a default implementation. Each model should consider implementing custom memory estimation logic.
 
@@ -1581,15 +1598,15 @@
         mem_size_threshold : int, default = None
             If not None, skips checking available memory if the expected model size is less than `mem_size_threshold` bytes.
             This is used to speed-up training by avoiding the check in cases where the machine almost certainly has sufficient memory.
         **kwargs : dict,
             Fit time kwargs, including X, y, X_val, and y_val.
             Can be used to customize estimation of memory usage.
         """
-        max_memory_usage_ratio = self.params_aux['max_memory_usage_ratio']
+        max_memory_usage_ratio = self.params_aux["max_memory_usage_ratio"]
         if max_memory_usage_ratio is None:
             return  # Skip memory check
 
         approx_mem_size_req = self.estimate_memory_usage(**kwargs)
         if mem_size_threshold is not None and approx_mem_size_req < (mem_size_threshold * min(max_memory_usage_ratio, 1)):
             return  # Model is smaller than the min threshold to check available mem
 
@@ -1597,36 +1614,46 @@
         ratio = approx_mem_size_req / available_mem
         min_error_memory_ratio = ratio / mem_error_threshold
         min_warning_memory_ratio = ratio / mem_warning_threshold
         max_memory_usage_error_ratio = mem_error_threshold * max_memory_usage_ratio
         max_memory_usage_warning_ratio = mem_warning_threshold * max_memory_usage_ratio
 
         log_ag_args_fit_example = '`predictor.fit(..., ag_args_fit={"ag.max_memory_usage_ratio": VALUE})`'
-        log_ag_args_fit_example = f'\n\t\tTo set the same value for all models, do the following when calling predictor.fit: {log_ag_args_fit_example}'
+        log_ag_args_fit_example = f"\n\t\tTo set the same value for all models, do the following when calling predictor.fit: {log_ag_args_fit_example}"
 
-        log_user_guideline = f'Estimated to require {approx_mem_size_req / 1e9:.3f} GB ' \
-                             f'out of {available_mem / 1e9:.3f} GB available memory ({min_error_memory_ratio*100:.3f}%)... ' \
-                             f'({max_memory_usage_error_ratio*100:.3f}% of avail memory is the max safe size)'
+        log_user_guideline = (
+            f"Estimated to require {approx_mem_size_req / 1e9:.3f} GB "
+            f"out of {available_mem / 1e9:.3f} GB available memory ({min_error_memory_ratio*100:.3f}%)... "
+            f"({max_memory_usage_error_ratio*100:.3f}% of avail memory is the max safe size)"
+        )
         if min_error_memory_ratio > max_memory_usage_error_ratio:
-            log_user_guideline += f'\n\tTo force training the model, specify the model hyperparameter "ag.max_memory_usage_ratio" to a larger value ' \
-                                  f'(currently {max_memory_usage_ratio}, set to >={min_error_memory_ratio + 0.05:.2f} to avoid the error)' \
-                                  f'{log_ag_args_fit_example}'
+            log_user_guideline += (
+                f'\n\tTo force training the model, specify the model hyperparameter "ag.max_memory_usage_ratio" to a larger value '
+                f"(currently {max_memory_usage_ratio}, set to >={min_error_memory_ratio + 0.05:.2f} to avoid the error)"
+                f"{log_ag_args_fit_example}"
+            )
             if min_error_memory_ratio >= 1:
-                log_user_guideline += f'\n\t\tSetting "ag.max_memory_usage_ratio" to values above 1 may result in out-of-memory errors. ' \
-                                      f'You may consider using a machine with more memory as a safer alternative.'
-            logger.warning(f'\tWarning: Not enough memory to safely train model. {log_user_guideline}')
+                log_user_guideline += (
+                    f'\n\t\tSetting "ag.max_memory_usage_ratio" to values above 1 may result in out-of-memory errors. '
+                    f"You may consider using a machine with more memory as a safer alternative."
+                )
+            logger.warning(f"\tWarning: Not enough memory to safely train model. {log_user_guideline}")
             raise NotEnoughMemoryError
         elif min_warning_memory_ratio > max_memory_usage_warning_ratio:
-            log_user_guideline += f'\n\tTo avoid this warning, specify the model hyperparameter "ag.max_memory_usage_ratio" to a larger value ' \
-                                  f'(currently {max_memory_usage_ratio}, set to >={min_warning_memory_ratio + 0.05:.2f} to avoid the warning)' \
-                                  f'{log_ag_args_fit_example}'
+            log_user_guideline += (
+                f'\n\tTo avoid this warning, specify the model hyperparameter "ag.max_memory_usage_ratio" to a larger value '
+                f"(currently {max_memory_usage_ratio}, set to >={min_warning_memory_ratio + 0.05:.2f} to avoid the warning)"
+                f"{log_ag_args_fit_example}"
+            )
             if min_warning_memory_ratio >= 1:
-                log_user_guideline += f'\n\t\tSetting "ag.max_memory_usage_ratio" to values above 1 may result in out-of-memory errors. ' \
-                                      f'You may consider using a machine with more memory as a safer alternative.'
-            logger.warning(f'\tWarning: Potentially not enough memory to safely train model. {log_user_guideline}')
+                log_user_guideline += (
+                    f'\n\t\tSetting "ag.max_memory_usage_ratio" to values above 1 may result in out-of-memory errors. '
+                    f"You may consider using a machine with more memory as a safer alternative."
+                )
+            logger.warning(f"\tWarning: Potentially not enough memory to safely train model. {log_user_guideline}")
 
     def reduce_memory_size(self, remove_fit=True, remove_info=False, requires_save=True, **kwargs):
         """
         Removes non-essential objects from the model to reduce memory and disk footprint.
         If `remove_fit=True`, enables the removal of variables which are required for fitting the model. If the model is already fully trained, then it is safe to remove these.
         If `remove_info=True`, enables the removal of variables which are used during model.get_info(). The values will be None when calling model.get_info().
         If `requires_save=True`, enables the removal of variables which are part of the model.pkl object, requiring an overwrite of the model to disk if it was previously persisted.
@@ -1639,46 +1666,47 @@
         """
         Deletes the model from disk.
 
         WARNING: This will DELETE ALL FILES in the self.path directory, regardless if they were created by AutoGluon or not.
         DO NOT STORE FILES INSIDE OF THE MODEL DIRECTORY THAT ARE UNRELATED TO AUTOGLUON.
         """
         if not silent:
-            logger.log(30, f'Deleting model {self.name}. All files under {self.path} will be removed.')
-        from pathlib import Path
+            logger.log(30, f"Deleting model {self.name}. All files under {self.path} will be removed.")
         import shutil
+        from pathlib import Path
+
         model_path = Path(self.path)
         # TODO: Report errors?
         shutil.rmtree(path=model_path, ignore_errors=True)
 
     def get_info(self) -> dict:
         """
         Returns a dictionary of numerous fields describing the model.
         """
         info = {
-            'name': self.name,
-            'model_type': type(self).__name__,
-            'problem_type': self.problem_type,
-            'eval_metric': self.eval_metric.name,
-            'stopping_metric': self.stopping_metric.name,
-            'fit_time': self.fit_time,
-            'num_classes': self.num_classes,
-            'quantile_levels': self.quantile_levels,
-            'predict_time': self.predict_time,
-            'val_score': self.val_score,
-            'hyperparameters': self.params,
-            'hyperparameters_fit': self.params_trained,  # TODO: Explain in docs that this is for hyperparameters that differ in final model from original hyperparameters, such as epochs (from early stopping)
-            'hyperparameters_nondefault': self.nondefault_params,
+            "name": self.name,
+            "model_type": type(self).__name__,
+            "problem_type": self.problem_type,
+            "eval_metric": self.eval_metric.name,
+            "stopping_metric": self.stopping_metric.name,
+            "fit_time": self.fit_time,
+            "num_classes": self.num_classes,
+            "quantile_levels": self.quantile_levels,
+            "predict_time": self.predict_time,
+            "val_score": self.val_score,
+            "hyperparameters": self.params,
+            "hyperparameters_fit": self.params_trained,  # TODO: Explain in docs that this is for hyperparameters that differ in final model from original hyperparameters, such as epochs (from early stopping)
+            "hyperparameters_nondefault": self.nondefault_params,
             AG_ARGS_FIT: self.params_aux,
-            'num_features': len(self.features) if self.features else None,
-            'features': self.features,
-            'feature_metadata': self.feature_metadata,
+            "num_features": len(self.features) if self.features else None,
+            "features": self.features,
+            "feature_metadata": self.feature_metadata,
             # 'disk_size': self.get_disk_size(),
-            'memory_size': self.get_memory_size(),  # Memory usage of model in bytes
-            'compile_time': self.compile_time if hasattr(self, 'compile_time') else None,
+            "memory_size": self.get_memory_size(),  # Memory usage of model in bytes
+            "compile_time": self.compile_time if hasattr(self, "compile_time") else None,
         }
         return info
 
     @classmethod
     def load_info(cls, path, load_model_if_required=True) -> dict:
         load_path = path + cls.model_info_name
         try:
@@ -1693,29 +1721,28 @@
     def save_info(self) -> dict:
         info = self.get_info()
 
         save_pkl.save(path=self.path + self.model_info_name, object=info)
         json_path = self.path + self.model_info_json_name
         save_json.save(path=json_path, obj=info)
         return info
-    
+
     def _get_maximum_resources(self) -> Dict[str, Union[int, float]]:
         """
         Get the maximum resources allowed to use for this model.
         This can be useful when model not scale well with resources, i.e. cpu cores.
         Return empty dict if no maximum resources needed
-        
+
         Return
         ------
         Dict[str, Union[int, float]]
             key, name of the resource, i.e. `num_cpus`, `num_gpus`
             value, maximum amount of resources
         """
         return {}
-        
 
     def _get_default_resources(self):
         """
         Determines the default resource usage of the model during fit.
 
         Models may want to override this if they depend heavily on GPUs, as the default sets num_gpus to 0.
         """
@@ -1741,19 +1768,19 @@
 
     def _get_default_stopping_metric(self):
         """
         Returns the default stopping metric to use for early stopping.
         This is used if stopping_metric was not explicitly specified.
         Models may wish to override this in case a more suitable stopping_metric exists for a given eval_metric.
         """
-        if self.eval_metric.name == 'roc_auc':
-            stopping_metric = 'log_loss'
+        if self.eval_metric.name == "roc_auc":
+            stopping_metric = "log_loss"
         else:
             stopping_metric = self.eval_metric
-        stopping_metric = metrics.get_metric(stopping_metric, self.problem_type, 'stopping_metric')
+        stopping_metric = metrics.get_metric(stopping_metric, self.problem_type, "stopping_metric")
         return stopping_metric
 
     # TODO: v1.0 Move params_aux to params, separate logic as in _get_ag_params, keep `ag.` prefix for ag_args_fit params
     #  This will allow to hyperparameter tune ag_args_fit hyperparameters.
     #  Also delete `self.params_aux` entirely, make it a method instead.
     def _get_params(self) -> dict:
         """Gets all params."""
@@ -1803,15 +1830,15 @@
         Tags are key-value pairs assigned to an object.
         These can be accessed after initializing an object.
         Tags are used for identifying if an object supports certain functionality.
         """
         # first get class tags, which are overwritten by any object tags
         collected_tags = self._get_class_tags()
         for base_class in reversed(inspect.getmro(self.__class__)):
-            if hasattr(base_class, '_more_tags'):
+            if hasattr(base_class, "_more_tags"):
                 # need the if because mixins might not have _more_tags
                 # but might do redundant work in estimators
                 # (i.e. calling more tags on BaseEstimator multiple times)
                 more_tags = base_class._more_tags(self)
                 collected_tags.update(more_tags)
         return collected_tags
 
@@ -1820,15 +1847,15 @@
         """
         Class tags are tags assigned to a class that are fixed.
         These can be accessed prior to initializing an object.
         Tags are used for identifying if an object supports certain functionality.
         """
         collected_tags = {}
         for base_class in reversed(inspect.getmro(cls)):
-            if hasattr(base_class, '_class_tags'):
+            if hasattr(base_class, "_class_tags"):
                 # need the if because mixins might not have _class_tags
                 # but might do redundant work in estimators
                 # (i.e. calling more tags on BaseEstimator multiple times)
                 more_tags = base_class._class_tags()
                 collected_tags.update(more_tags)
         return collected_tags
 
@@ -1837,10 +1864,10 @@
         """
         [Advanced] Optional tags used to communicate model capabilities to AutoML systems, such as if the model supports text features.
         """
         return _DEFAULT_CLASS_TAGS
 
     def _more_tags(self) -> dict:
         return _DEFAULT_TAGS
-    
+
     def _get_model_base(self):
         return self
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/abstract_nn_model.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/abstract_nn_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,83 @@
 import logging
+
 import numpy as np
 
-from autogluon.common.features.types import R_CATEGORY, R_OBJECT, R_FLOAT, R_INT, S_BOOL
+from autogluon.common.features.types import R_CATEGORY, R_FLOAT, R_INT, R_OBJECT, S_BOOL
 
 from .abstract_model import AbstractModel
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractNeuralNetworkModel(AbstractModel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._types_of_features = None
 
     # TODO: v0.1 clean method
     def _get_types_of_features(self, df, skew_threshold=None, embed_min_categories=None, use_ngram_features=None, needs_extra_types=True):
-        """ Returns dict with keys: : 'continuous', 'skewed', 'onehot', 'embed', 'language', values = ordered list of feature-names falling into each category.
-            Each value is a list of feature-names corresponding to columns in original dataframe.
-            TODO: ensure features with zero variance have already been removed before this function is called.
+        """Returns dict with keys: : 'continuous', 'skewed', 'onehot', 'embed', 'language', values = ordered list of feature-names falling into each category.
+        Each value is a list of feature-names corresponding to columns in original dataframe.
+        TODO: ensure features with zero variance have already been removed before this function is called.
         """
         if self._types_of_features is not None:
             Warning("Attempting to _get_types_of_features for Model, but previously already did this.")
 
         continuous_featnames = self._feature_metadata.get_features(valid_raw_types=[R_INT, R_FLOAT], invalid_special_types=[S_BOOL])
         categorical_featnames = self._feature_metadata.get_features(valid_raw_types=[R_CATEGORY, R_OBJECT])
         bool_featnames = self._feature_metadata.get_features(required_special_types=[S_BOOL])
 
-        language_featnames = [] # TODO: not implemented. This should fetch text features present in the data
+        language_featnames = []  # TODO: not implemented. This should fetch text features present in the data
         valid_features = categorical_featnames + continuous_featnames + bool_featnames + language_featnames
 
         if len(valid_features) < df.shape[1]:
             unknown_features = [feature for feature in df.columns if feature not in valid_features]
             logger.log(15, f"Model will additionally ignore the following columns: {unknown_features}")
             df = df.drop(columns=unknown_features)
             self._features_internal = list(df.columns)
 
         self.features_to_drop = df.columns[df.isna().all()].tolist()  # drop entirely NA columns which may arise after train/val split
         if self.features_to_drop:
             logger.log(15, f"Model will additionally ignore the following columns: {self.features_to_drop}")
             df = df.drop(columns=self.features_to_drop)
 
         if needs_extra_types is True:
-            types_of_features = {'continuous': [], 'skewed': [], 'onehot': [], 'embed': [], 'language': [], 'bool': []}
+            types_of_features = {"continuous": [], "skewed": [], "onehot": [], "embed": [], "language": [], "bool": []}
             # continuous = numeric features to rescale
             # skewed = features to which we will apply power (ie. log / box-cox) transform before normalization
             # onehot = features to one-hot encode (unknown categories for these features encountered at test-time are encoded as all zeros). We one-hot encode any features encountered that only have two unique values.
             features_to_consider = [feat for feat in self._features_internal if feat not in self.features_to_drop]
             for feature in features_to_consider:
                 feature_data = df[feature]  # pd.Series
                 num_unique_vals = len(feature_data.unique())
                 if feature in bool_featnames:
-                    types_of_features['bool'].append(feature)
+                    types_of_features["bool"].append(feature)
                 elif num_unique_vals == 2:  # will be onehot encoded regardless of proc.embed_min_categories value
-                    types_of_features['onehot'].append(feature)
+                    types_of_features["onehot"].append(feature)
                 elif feature in continuous_featnames:
                     if np.abs(feature_data.skew()) > skew_threshold:
-                        types_of_features['skewed'].append(feature)
+                        types_of_features["skewed"].append(feature)
                     else:
-                        types_of_features['continuous'].append(feature)
+                        types_of_features["continuous"].append(feature)
                 elif feature in categorical_featnames:
                     if num_unique_vals >= embed_min_categories:  # sufficiently many categories to warrant learned embedding dedicated to this feature
-                        types_of_features['embed'].append(feature)
+                        types_of_features["embed"].append(feature)
                     else:
-                        types_of_features['onehot'].append(feature)
+                        types_of_features["onehot"].append(feature)
                 elif feature in language_featnames:
-                    types_of_features['language'].append(feature)
+                    types_of_features["language"].append(feature)
         else:
             types_of_features = []
             for feature in valid_features:
                 if feature in categorical_featnames:
-                    feature_type = 'CATEGORICAL'
+                    feature_type = "CATEGORICAL"
                 elif feature in continuous_featnames or feature in bool_featnames:
-                    feature_type = 'SCALAR'
+                    feature_type = "SCALAR"
                 elif feature in language_featnames:
-                    feature_type = 'TEXT'
+                    feature_type = "TEXT"
                 else:
-                    raise ValueError(f'Invalid feature: {feature}')
+                    raise ValueError(f"Invalid feature: {feature}")
 
                 types_of_features.append({"name": feature, "type": feature_type})
 
         return types_of_features, df
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/abstract/model_trial.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/abstract/model_trial.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+import logging
 import os
 import time
-import logging
 
-from ...hpo.constants import RAY_BACKEND, CUSTOM_BACKEND, VALID_BACKEND
-from ...utils.loaders import load_pkl
+from ...hpo.constants import CUSTOM_BACKEND, RAY_BACKEND, VALID_BACKEND
 from ...utils.exceptions import TimeLimitExceeded
+from ...utils.loaders import load_pkl
 
 logger = logging.getLogger(__name__)
 
 
 def model_trial(
     args,
     model_cls,
@@ -18,75 +18,70 @@
     time_start,
     hpo_executor,
     is_bagged_model=False,
     reporter=None,  # reporter only used by custom strategy, hence optional
     time_limit=None,
     fit_kwargs=None,
 ):
-    """ Training script for hyperparameter evaluation of an arbitrary model that subclasses AbstractModel."""
+    """Training script for hyperparameter evaluation of an arbitrary model that subclasses AbstractModel."""
     try:
         if fit_kwargs is None:
             fit_kwargs = dict()
 
-        model = init_model(
-            args=args,
-            model_cls=model_cls,
-            init_params=init_params,
-            backend=hpo_executor.executor_type,
-            is_bagged_model=is_bagged_model
-        )
+        model = init_model(args=args, model_cls=model_cls, init_params=init_params, backend=hpo_executor.executor_type, is_bagged_model=is_bagged_model)
 
         X, y = load_pkl.load(train_path)
         X_val, y_val = load_pkl.load(val_path)
 
         fit_model_args = dict(X=X, y=y, X_val=X_val, y_val=y_val, **fit_kwargs)
         predict_proba_args = dict(X=X_val)
         model = fit_and_save_model(
             model=model,
             fit_args=fit_model_args,
             predict_proba_args=predict_proba_args,
             y_val=y_val,
             time_start=time_start,
             time_limit=time_limit,
-        )   
+        )
     except Exception as e:
         if not isinstance(e, TimeLimitExceeded):
             logger.exception(e, exc_info=True)
         # In case of TimeLimitExceed, val_score could be None
-        hpo_executor.report(reporter=reporter, epoch=1, validation_performance=model.val_score if model.val_score is not None else float('-inf'))
+        hpo_executor.report(reporter=reporter, epoch=1, validation_performance=model.val_score if model.val_score is not None else float("-inf"))
         if reporter is not None:
             reporter.terminate()
     else:
         hpo_executor.report(reporter=reporter, epoch=1, validation_performance=model.val_score)
 
 
 def init_model(args, model_cls, init_params, backend, is_bagged_model=False):
     args = args.copy()
 
     if backend == CUSTOM_BACKEND:
-        task_id = args.pop('task_id')
+        task_id = args.pop("task_id")
         file_prefix = f"T{task_id+1}"  # append to all file names created during this trial. Do NOT change!
     elif backend == RAY_BACKEND:
         from ray import tune
+
         task_id = tune.get_trial_id()
         file_prefix = task_id
     else:
         raise ValueError(f"Invalid backend: {backend}. Valid options are [{CUSTOM_BACKEND}, {RAY_BACKEND}]")
 
     if is_bagged_model:
-        if 'model_base_kwargs' not in init_params:
-            init_params['model_base_kwargs'] = {}
-        if 'hyperparameters' not in init_params['model_base_kwargs']:
-            init_params['model_base_kwargs']['hyperparameters'] = {}
-        init_params['model_base_kwargs']['hyperparameters'].update(args)
+        if "model_base_kwargs" not in init_params:
+            init_params["model_base_kwargs"] = {}
+        if "hyperparameters" not in init_params["model_base_kwargs"]:
+            init_params["model_base_kwargs"]["hyperparameters"] = {}
+        init_params["model_base_kwargs"]["hyperparameters"].update(args)
     else:
-        if 'hyperparameters' not in init_params:
-            init_params['hyperparameters'] = {}
-        init_params['hyperparameters'].update(args)
-    init_params['name'] = init_params['name'] + os.path.sep + file_prefix
+        if "hyperparameters" not in init_params:
+            init_params["hyperparameters"] = {}
+        init_params["hyperparameters"].update(args)
+    init_params["name"] = init_params["name"] + os.path.sep + file_prefix
 
     return model_cls(**init_params)
 
 
 def fit_and_save_model(model, fit_args, predict_proba_args, y_val, time_start, time_limit=None):
     time_current = time.time()
     time_elapsed = time_current - time_start
@@ -97,42 +92,35 @@
     else:
         time_left = None
 
     time_fit_start = time.time()
     model.fit(**fit_args, time_limit=time_left)
     time_fit_end = time.time()
 
-    if model._get_tags().get('valid_oof', False):
-        oof_pred_proba = model.get_oof_pred_proba(X=fit_args['X'], y=fit_args['y'])
+    if model._get_tags().get("valid_oof", False):
+        oof_pred_proba = model.get_oof_pred_proba(X=fit_args["X"], y=fit_args["y"])
         time_pred_end = time.time()
         # TODO: use sample_weight?
         # sample_weight = fit_args.get('sample_weight', None)
-        model.val_score = model.score_with_y_pred_proba(y=fit_args['y'], y_pred_proba=oof_pred_proba)
+        model.val_score = model.score_with_y_pred_proba(y=fit_args["y"], y_pred_proba=oof_pred_proba)
     else:
         y_pred_proba = model.predict_proba(**predict_proba_args)
         time_pred_end = time.time()
-        sample_weight_val = fit_args.get('sample_weight_val', None)
+        sample_weight_val = fit_args.get("sample_weight_val", None)
         model.val_score = model.score_with_y_pred_proba(y=y_val, y_pred_proba=y_pred_proba, sample_weight=sample_weight_val)
 
     model.fit_time = time_fit_end - time_fit_start
     model.predict_time = time_pred_end - time_fit_end
     model.save()
     return model
 
 
 def skip_hpo(model, X, y, X_val, y_val, time_limit=None, **kwargs):
     """Skips HPO and simply trains the model once with the provided HPO time budget. Returns model artifacts as if from HPO."""
     fit_model_args = dict(X=X, y=y, **kwargs)
     predict_proba_args = dict(X=X_val)
-    fit_and_save_model(
-        model=model,
-        fit_args=fit_model_args,
-        predict_proba_args=predict_proba_args,
-        y_val=y_val,
-        time_start=time.time(),
-        time_limit=time_limit
-    )
-    hpo_results = {'total_time': model.fit_time}
+    fit_and_save_model(model=model, fit_args=fit_model_args, predict_proba_args=predict_proba_args, y_val=y_val, time_start=time.time(), time_limit=time_limit)
+    hpo_results = {"total_time": model.fit_time}
     hpo_model_performances = {model.name: model.val_score}
-    hpo_results['hpo_model_performances'] = hpo_model_performances
-    hpo_models = {model.name: {'path': model.path}}
+    hpo_results["hpo_model_performances"] = hpo_model_performances
+    hpo_models = {model.name: {"path": model.path}}
     return hpo_models, hpo_results
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/dummy/_dummy_quantile_regressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import numpy as np
 
 
 class DummyQuantileRegressor:
     """Adds support for quantile regression to dummy models"""
+
     def __init__(self, quantile_levels: list):
         self.quantile_levels = quantile_levels
         self.models = []
 
     def fit(self, X, y):
         from sklearn.dummy import DummyRegressor
+
         for quantile in self.quantile_levels:
             m = DummyRegressor(quantile=quantile)
             m.fit(X, y)
             self.models.append(m)
 
     def predict(self, X):
         predictions = []
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/dummy/dummy_model.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/dummy/dummy_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import pandas as pd
 
-from ._dummy_quantile_regressor import DummyQuantileRegressor
+from ...constants import BINARY, MULTICLASS, QUANTILE, REGRESSION
 from .. import AbstractModel
-from ...constants import BINARY, MULTICLASS, REGRESSION, QUANTILE
+from ._dummy_quantile_regressor import DummyQuantileRegressor
 
 
 class DummyModel(AbstractModel):
     """
     A dummy model that ignores input features and predicts only a constant value.
     Useful for tests and calculating worst-case performance.
     """
+
     def _get_model_type(self):
         from sklearn.dummy import DummyClassifier, DummyRegressor
+
         if self.problem_type == REGRESSION:
             return DummyRegressor
         elif self.problem_type == QUANTILE:
             return DummyQuantileRegressor
         elif self.problem_type in [BINARY, MULTICLASS]:
             return DummyClassifier
         else:
-            raise ValueError(f'DummyModel does not support problem_type={self.problem_type}')
+            raise ValueError(f"DummyModel does not support problem_type={self.problem_type}")
 
     def preprocess(self, X: pd.DataFrame, **kwargs):
         return X
 
     def _fit(self, X, y, **kwargs):
         X = self.preprocess(X)
         model_cls = self._get_model_type()
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/bagged_ensemble_model.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/bagged_ensemble_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,27 +8,33 @@
 from collections import Counter
 from statistics import mean
 from typing import Dict, Type, Union
 
 import numpy as np
 import pandas as pd
 
-from autogluon.common.utils.try_import import try_import_ray
 from autogluon.common.utils.distribute_utils import DistributedContext
 from autogluon.common.utils.log_utils import DuplicateFilter
-from .fold_fitting_strategy import FoldFittingStrategy, SequentialLocalFoldFittingStrategy, ParallelFoldFittingStrategy, ParallelLocalFoldFittingStrategy, ParallelDistributedFoldFittingStrategy
-from ..abstract.abstract_model import AbstractModel
-from ..abstract.model_trial import model_trial, skip_hpo
-from ...constants import MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE, REFIT_FULL_SUFFIX
+from autogluon.common.utils.try_import import try_import_ray
+
+from ...constants import MULTICLASS, QUANTILE, REFIT_FULL_SUFFIX, REGRESSION, SOFTCLASS
 from ...hpo.exceptions import EmptySearchSpace
 from ...utils.exceptions import TimeLimitExceeded
 from ...utils.loaders import load_pkl
 from ...utils.savers import save_pkl
 from ...utils.utils import CVSplitter, _compute_fi_with_stddev
-
+from ..abstract.abstract_model import AbstractModel
+from ..abstract.model_trial import model_trial, skip_hpo
+from .fold_fitting_strategy import (
+    FoldFittingStrategy,
+    ParallelDistributedFoldFittingStrategy,
+    ParallelFoldFittingStrategy,
+    ParallelLocalFoldFittingStrategy,
+    SequentialLocalFoldFittingStrategy,
+)
 
 logger = logging.getLogger(__name__)
 dup_filter = DuplicateFilter()
 logger.addFilter(dup_filter)
 
 
 # TODO: Add metadata object with info like score on each model, train time on each model, etc.
@@ -46,24 +52,26 @@
     model_base_kwargs : Dict[str, any], default = None
         kwargs used to initialize model_base if model_base is a class.
     random_state : int, default = 0
         Random state used to split the data into cross-validation folds during fit.
     **kwargs
         Refer to AbstractModel documentation
     """
-    _oof_filename = 'oof.pkl'
+
+    _oof_filename = "oof.pkl"
 
     def __init__(self, model_base: Union[AbstractModel, Type[AbstractModel]], model_base_kwargs: Dict[str, any] = None, random_state: int = 0, **kwargs):
         if inspect.isclass(model_base):
             if model_base_kwargs is None:
                 model_base_kwargs = dict()
             self.model_base: AbstractModel = model_base(**model_base_kwargs)
         elif model_base_kwargs is not None:
-            raise AssertionError(f'model_base_kwargs must be None if model_base was passed as an object! '
-                                 f'(model_base: {model_base}, model_base_kwargs: {model_base_kwargs})')
+            raise AssertionError(
+                f"model_base_kwargs must be None if model_base was passed as an object! " f"(model_base: {model_base}, model_base_kwargs: {model_base_kwargs})"
+            )
         else:
             self.model_base: AbstractModel = model_base
         self._child_type = type(self.model_base)
         self.models = []
         self._oof_pred_proba = None
         self._oof_pred_model_repeats = None
         self._n_repeats = 0  # Number of n_repeats with at least 1 model fit, if kfold=5 and 8 models have been fit, _n_repeats is 2
@@ -82,15 +90,15 @@
         self._params_aux_child = None  # aux params of child model
 
         super().__init__(problem_type=self.model_base.problem_type, eval_metric=self.model_base.eval_metric, **kwargs)
 
     def _set_default_params(self):
         default_params = {
             # 'use_child_oof': False,  # [Advanced] Whether to defer to child model for OOF preds and only train a single child.
-            'save_bag_folds': True,
+            "save_bag_folds": True,
             # 'refit_folds': False,  # [Advanced, Experimental] Whether to refit bags immediately to a refit_full model in a single .fit call.
             # 'num_folds' None,  # Number of bagged folds per set. If specified, overrides .fit `k_fold` value.
             # 'max_sets': None,  # Maximum bagged repeats to allow, if specified, will set `self.can_fit()` to `self._n_repeats_finished < max_repeats`
         }
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
         super()._set_default_params()
@@ -103,15 +111,15 @@
         default_auxiliary_params.update(extra_auxiliary_params)
         return default_auxiliary_params
 
     def is_valid(self):
         return self.is_fit() and (self._n_repeats == self._n_repeats_finished)
 
     def can_infer(self):
-        return self.is_fit() and self.params.get('save_bag_folds', True)
+        return self.is_fit() and self.params.get("save_bag_folds", True)
 
     def is_stratified(self):
         if self.problem_type in [REGRESSION, QUANTILE, SOFTCLASS]:
             return False
         else:
             return True
 
@@ -120,15 +128,15 @@
 
     def can_fit(self) -> bool:
         if not self.is_fit():
             return True
         if not self._bagged_mode:
             return False
         # If max_sets is specified and the model has already fit >=max_sets, return False
-        return self._get_model_params().get('max_sets', None) is None or self._get_model_params().get('max_sets') > self._n_repeats_finished
+        return self._get_model_params().get("max_sets", None) is None or self._get_model_params().get("max_sets") > self._n_repeats_finished
 
     def is_valid_oof(self):
         return self.is_fit() and (self._child_oof or self._bagged_mode)
 
     def get_oof_pred_proba(self, **kwargs):
         # TODO: Require is_valid == True (add option param to ignore is_valid)
         return self._oof_pred_proba_func(self._oof_pred_proba, self._oof_pred_model_repeats)
@@ -159,30 +167,32 @@
             return model.preprocess(X, preprocess_stateful=False)
         else:
             return X
 
     def _get_cv_splitter(self, n_splits, n_repeats, groups=None):
         return CVSplitter(n_splits=n_splits, n_repeats=n_repeats, groups=groups, stratified=self.is_stratified(), random_state=self._random_state)
 
-    def _fit(self,
-             X,
-             y,
-             X_val=None,
-             y_val=None,
-             X_pseudo=None,
-             y_pseudo=None,
-             k_fold=None,
-             k_fold_start=0,
-             k_fold_end=None,
-             n_repeats=1,
-             n_repeat_start=0,
-             groups=None,
-             _skip_oof=False,
-             **kwargs):
-        use_child_oof = self.params.get('use_child_oof', False)
+    def _fit(
+        self,
+        X,
+        y,
+        X_val=None,
+        y_val=None,
+        X_pseudo=None,
+        y_pseudo=None,
+        k_fold=None,
+        k_fold_start=0,
+        k_fold_end=None,
+        n_repeats=1,
+        n_repeat_start=0,
+        groups=None,
+        _skip_oof=False,
+        **kwargs,
+    ):
+        use_child_oof = self.params.get("use_child_oof", False)
         if use_child_oof:
             if self.is_fit():
                 # TODO: We may want to throw an exception instead and avoid calling fit more than once
                 return self
             k_fold = 1
             k_fold_end = None
             groups = None
@@ -190,15 +200,15 @@
             k_fold, k_fold_end = self._update_k_fold(k_fold=k_fold, k_fold_end=k_fold_end)
         if k_fold is None and groups is None:
             k_fold = 5
         if k_fold is not None and k_fold < 1:
             k_fold = 1
         if k_fold is None or k_fold > 1:
             k_fold = self._get_cv_splitter(n_splits=k_fold, n_repeats=n_repeats, groups=groups).n_splits
-        max_sets = self._get_model_params().get('max_sets', None)
+        max_sets = self._get_model_params().get("max_sets", None)
         if max_sets is not None:
             if n_repeats > max_sets:
                 n_repeats = max_sets
         self._validate_bag_kwargs(
             k_fold=k_fold,
             k_fold_start=k_fold_start,
             k_fold_end=k_fold_end,
@@ -206,127 +216,133 @@
             n_repeat_start=n_repeat_start,
             groups=groups,
         )
         if k_fold_end is None:
             k_fold_end = k_fold
 
         model_base = self._get_model_base()
-        model_base.rename(name='')
-        kwargs['feature_metadata'] = self.feature_metadata
-        kwargs['num_classes'] = self.num_classes  # TODO: maybe don't pass num_classes to children
+        model_base.rename(name="")
+        kwargs["feature_metadata"] = self.feature_metadata
+        kwargs["num_classes"] = self.num_classes  # TODO: maybe don't pass num_classes to children
 
         if self.model_base is not None:
             self.save_model_base(self.model_base)
             self.model_base = None
 
         if self._oof_pred_proba is None and self.is_fit():
             self._load_oof()
 
-        can_refit_full = self._get_tags_child().get('can_refit_full', False)
+        can_refit_full = self._get_tags_child().get("can_refit_full", False)
 
-        if (not can_refit_full or k_fold == 1) and not self.params.get('save_bag_folds', True):
+        if (not can_refit_full or k_fold == 1) and not self.params.get("save_bag_folds", True):
             # TODO: This is a hack to avoid a very challenging situation:
             #  in high_quality preset we don't save fold models, but for models that don't support refit_full,
             #  they must copy the first fold model instead of fitting again.
             #  Therefore we must override save_bag_folds for these unsupported models so that the refit versions have a fold model to copy.
             #  This could be implemented better by only keeping the first fold model artifact and avoid saving the other fold model artifacts (lower disk usage)
             #  However, this is complex to code accounting for the fitting strategies and would be prone to difficult to diagnose bugs.
-            self.params['save_bag_folds'] = True
+            self.params["save_bag_folds"] = True
             if k_fold != 1:
                 # Only log in the situation where functionality is currently suboptimal
-                logger.log(20, '\tForcing `save_bag_folds=True` because child model does not support `refit_full`.')
+                logger.log(20, "\tForcing `save_bag_folds=True` because child model does not support `refit_full`.")
 
-        save_bag_folds = self.params.get('save_bag_folds', True)
+        save_bag_folds = self.params.get("save_bag_folds", True)
         if k_fold == 1:
             self._fit_single(X=X, y=y, model_base=model_base, use_child_oof=use_child_oof, skip_oof=_skip_oof, **kwargs)
             return self
         else:
-            refit_folds = self.params.get('refit_folds', False)
+            refit_folds = self.params.get("refit_folds", False)
             if refit_folds:
                 if n_repeat_start != 0 or k_fold_start != 0:
-                    raise AssertionError(f'n_repeat_start and k_fold_start must be 0 with refit_folds=True, values: ({n_repeat_start}, {k_fold_start})')
+                    raise AssertionError(f"n_repeat_start and k_fold_start must be 0 with refit_folds=True, values: ({n_repeat_start}, {k_fold_start})")
                 if k_fold_end != k_fold:
-                    raise AssertionError(f'k_fold_end and k_fold must be equal with refit_folds=True, values: ({k_fold_end}, {k_fold})')
+                    raise AssertionError(f"k_fold_end and k_fold must be equal with refit_folds=True, values: ({k_fold_end}, {k_fold})")
                 save_bag_folds = False
-                if kwargs.get('time_limit', None) is not None:
+                if kwargs.get("time_limit", None) is not None:
                     fold_start = n_repeat_start * k_fold + k_fold_start
                     fold_end = (n_repeats - 1) * k_fold + k_fold_end
                     folds_to_fit = fold_end - fold_start
                     # Reserve time for final refit model
-                    kwargs['time_limit'] = kwargs['time_limit'] * folds_to_fit / (folds_to_fit + 1.2)
-            self._fit_folds(X=X, y=y, model_base=model_base, X_pseudo=X_pseudo, y_pseudo=y_pseudo,
-                            k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold_end,
-                            n_repeats=n_repeats, n_repeat_start=n_repeat_start, save_folds=save_bag_folds, groups=groups, **kwargs)
+                    kwargs["time_limit"] = kwargs["time_limit"] * folds_to_fit / (folds_to_fit + 1.2)
+            self._fit_folds(
+                X=X,
+                y=y,
+                model_base=model_base,
+                X_pseudo=X_pseudo,
+                y_pseudo=y_pseudo,
+                k_fold=k_fold,
+                k_fold_start=k_fold_start,
+                k_fold_end=k_fold_end,
+                n_repeats=n_repeats,
+                n_repeat_start=n_repeat_start,
+                save_folds=save_bag_folds,
+                groups=groups,
+                **kwargs,
+            )
             # FIXME: Cleanup self
             # FIXME: Support `can_refit_full=False` models
             if refit_folds:
                 refit_template = self.convert_to_refit_full_template(name_suffix=None)
-                refit_template.params['use_child_oof'] = False
-                kwargs['time_limit'] = None
+                refit_template.params["use_child_oof"] = False
+                kwargs["time_limit"] = None
                 # _skip_oof=True to avoid inferring on training data needlessly.
                 refit_template.fit(X=X, y=y, k_fold=1, _skip_oof=True, **kwargs)
                 refit_template._oof_pred_proba = self._oof_pred_proba
                 refit_template._oof_pred_model_repeats = self._oof_pred_model_repeats
                 refit_template._child_oof = True
                 refit_template.fit_time += self.fit_time + self.predict_time
                 refit_template.predict_time = self.predict_time
                 return refit_template
             else:
                 return self
 
     def _update_k_fold(self, k_fold, k_fold_end=None, verbose=True):
         """Update k_fold and k_fold_end in case num_folds was specified"""
-        k_fold_override = self.params.get('num_folds', None)
+        k_fold_override = self.params.get("num_folds", None)
         if k_fold_override is not None:
             if k_fold is not None:
                 if k_fold != k_fold_override and verbose:
-                    logger.log(20, f'\tSetting folds to {k_fold_override}. Ignoring `k_fold={k_fold}` because `num_folds={k_fold_override}` overrides.')
+                    logger.log(20, f"\tSetting folds to {k_fold_override}. Ignoring `k_fold={k_fold}` because `num_folds={k_fold_override}` overrides.")
                 if k_fold_end is not None and k_fold_end == k_fold:
                     k_fold_end = k_fold_override
             k_fold = k_fold_override
         return k_fold, k_fold_end
 
     def _get_child_aux_val(self, key: str, default=None):
         assert self.is_initialized(), "Model must be initialized before calling self._get_child_aux_val!"
         return self._params_aux_child.get(key, default)
 
-    def _validate_bag_kwargs(self, *,
-                             k_fold,
-                             k_fold_start,
-                             k_fold_end,
-                             n_repeats,
-                             n_repeat_start,
-                             groups):
+    def _validate_bag_kwargs(self, *, k_fold, k_fold_start, k_fold_end, n_repeats, n_repeat_start, groups):
         if groups is not None:
             if self._n_repeats_finished != 0:
-                raise AssertionError('Bagged models cannot call fit with `groups` specified when a full k-fold set has already been fit.')
+                raise AssertionError("Bagged models cannot call fit with `groups` specified when a full k-fold set has already been fit.")
             if n_repeats > 1:
-                raise AssertionError('Cannot perform repeated bagging with `groups` specified.')
+                raise AssertionError("Cannot perform repeated bagging with `groups` specified.")
             return
 
         if k_fold_end is None:
             k_fold_end = k_fold
         if k_fold is None:
-            raise ValueError('k_fold cannot be None.')
+            raise ValueError("k_fold cannot be None.")
         if k_fold < 1:
-            raise ValueError(f'k_fold must be equal or greater than 1, value: ({k_fold})')
+            raise ValueError(f"k_fold must be equal or greater than 1, value: ({k_fold})")
         if n_repeat_start != self._n_repeats_finished:
-            raise ValueError(f'n_repeat_start must equal self._n_repeats_finished, values: ({n_repeat_start}, {self._n_repeats_finished})')
+            raise ValueError(f"n_repeat_start must equal self._n_repeats_finished, values: ({n_repeat_start}, {self._n_repeats_finished})")
         if n_repeats <= n_repeat_start:
-            raise ValueError(f'n_repeats must be greater than n_repeat_start, values: ({n_repeats}, {n_repeat_start})')
+            raise ValueError(f"n_repeats must be greater than n_repeat_start, values: ({n_repeats}, {n_repeat_start})")
         if k_fold_start != self._k_fold_end:
-            raise ValueError(f'k_fold_start must equal previous k_fold_end, values: ({k_fold_start}, {self._k_fold_end})')
+            raise ValueError(f"k_fold_start must equal previous k_fold_end, values: ({k_fold_start}, {self._k_fold_end})")
         if k_fold_start >= k_fold_end:
             # TODO: Remove this limitation if n_repeats > 1
-            raise ValueError(f'k_fold_end must be greater than k_fold_start, values: ({k_fold_end}, {k_fold_start})')
+            raise ValueError(f"k_fold_end must be greater than k_fold_start, values: ({k_fold_end}, {k_fold_start})")
         if (n_repeats - n_repeat_start) > 1 and k_fold_end != k_fold:
             # TODO: Remove this limitation
-            raise ValueError(f'k_fold_end must equal k_fold when (n_repeats - n_repeat_start) > 1, values: ({k_fold_end}, {k_fold})')
+            raise ValueError(f"k_fold_end must equal k_fold when (n_repeats - n_repeat_start) > 1, values: ({k_fold_end}, {k_fold})")
         if self._k is not None and self._k != k_fold:
-            raise ValueError(f'k_fold must equal previously fit k_fold value for the current n_repeat, values: (({k_fold}, {self._k})')
+            raise ValueError(f"k_fold must equal previously fit k_fold value for the current n_repeat, values: (({k_fold}, {self._k})")
 
     def predict_proba(self, X, normalize=None, **kwargs):
         model = self.load_child(self.models[0])
         X = self.preprocess(X, model=model, **kwargs)
         pred_proba = model.predict_proba(X=X, preprocess_nonadaptive=False, normalize=normalize)
         for model in self.models[1:]:
             model = self.load_child(model)
@@ -350,18 +366,18 @@
         y_pred_proba = self.get_oof_pred_proba()[valid_indices]
         if sample_weight is not None:
             sample_weight = sample_weight[valid_indices]
         return self.score_with_y_pred_proba(y=y, y_pred_proba=y_pred_proba, sample_weight=sample_weight)
 
     def _fit_single(self, X, y, model_base, use_child_oof, time_limit=None, skip_oof=False, **kwargs):
         if self.is_fit():
-            raise AssertionError('Model is already fit.')
+            raise AssertionError("Model is already fit.")
         if self._n_repeats != 0:
-            raise ValueError(f'n_repeats must equal 0 when fitting a single model with k_fold == 1, value: {self._n_repeats}')
-        model_base.name = f'{model_base.name}S1F1'
+            raise ValueError(f"n_repeats must equal 0 when fitting a single model with k_fold == 1, value: {self._n_repeats}")
+        model_base.name = f"{model_base.name}S1F1"
         model_base.set_contexts(path_context=self.path + model_base.name + os.path.sep)
         time_start_fit = time.time()
         model_base.fit(X=X, y=y, time_limit=time_limit, **kwargs)
         model_base.fit_time = time.time() - time_start_fit
         model_base.predict_time = None
         if not skip_oof:
             X_len = len(X)
@@ -380,42 +396,51 @@
                 n_sample = min(500, round(X_len * 0.1))
                 frac = n_sample / X_len
                 X_sample = X.sample(n=n_sample)
                 time_start_predict = time.time()
                 model_base.predict_proba(X_sample)
                 time_predict_frac = time.time() - time_start_predict
                 time_predict_estimate = time_predict_frac / frac
-                logger.log(15, f'\t{round(time_predict_estimate, 2)}s\t= Estimated out-of-fold prediction time...')
+                logger.log(15, f"\t{round(time_predict_estimate, 2)}s\t= Estimated out-of-fold prediction time...")
                 if time_predict_estimate > time_left:
-                    logger.warning(f'\tNot enough time to generate out-of-fold predictions for model. Estimated time required was {round(time_predict_estimate, 2)}s compared to {round(time_left, 2)}s of available time.')
+                    logger.warning(
+                        f"\tNot enough time to generate out-of-fold predictions for model. Estimated time required was {round(time_predict_estimate, 2)}s compared to {round(time_left, 2)}s of available time."
+                    )
                     raise TimeLimitExceeded
 
             if use_child_oof:
-                logger.log(15, '\t`use_child_oof` was specified for this model. It will function similarly to a bagged model, but will only fit one child model.')
+                logger.log(
+                    15, "\t`use_child_oof` was specified for this model. It will function similarly to a bagged model, but will only fit one child model."
+                )
                 time_start_predict = time.time()
-                if model_base._get_tags().get('valid_oof', False):
+                if model_base._get_tags().get("valid_oof", False):
                     self._oof_pred_proba = model_base.get_oof_pred_proba(X=X, y=y)
                 else:
-                    logger.warning('\tWARNING: `use_child_oof` was specified but child model does not have a dedicated `get_oof_pred_proba` method. This model may have heavily overfit validation scores.')
+                    logger.warning(
+                        "\tWARNING: `use_child_oof` was specified but child model does not have a dedicated `get_oof_pred_proba` method. This model may have heavily overfit validation scores."
+                    )
                     self._oof_pred_proba = model_base.predict_proba(X=X)
                 self._child_oof = True
                 model_base.predict_time = time.time() - time_start_predict
                 model_base.val_score = model_base.score_with_y_pred_proba(y=y, y_pred_proba=self._oof_pred_proba)
             else:
-                can_get_oof_from_train = self._get_tags().get('can_get_oof_from_train', False)
+                can_get_oof_from_train = self._get_tags().get("can_get_oof_from_train", False)
                 if not can_get_oof_from_train:
                     # TODO: Consider raising an exception in v1.0 release, we don't want this happening when not intended.
-                    logger.log(30, f'\tWARNING: Setting `self._oof_pred_proba` by predicting on train directly! '
-                                   f'This is probably a bug and should be investigated...\n'
-                                   f'\tIf this is intended, set the model tag "can_get_oof_from_train" to True '
-                                   f'in `{self.__class__.__name__}._more_tags` to avoid this warning.')
+                    logger.log(
+                        30,
+                        f"\tWARNING: Setting `self._oof_pred_proba` by predicting on train directly! "
+                        f"This is probably a bug and should be investigated...\n"
+                        f'\tIf this is intended, set the model tag "can_get_oof_from_train" to True '
+                        f"in `{self.__class__.__name__}._more_tags` to avoid this warning.",
+                    )
                 self._oof_pred_proba = model_base.predict_proba(X=X)  # TODO: Cheater value, will be overfit to valid set
             self._oof_pred_model_repeats = np.ones(shape=len(X), dtype=np.uint8)
         model_base.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
-        if not self.params.get('save_bag_folds', True):
+        if not self.params.get("save_bag_folds", True):
             model_base.model = None
         if self.low_memory:
             self.save_child(model_base)
         self.add_child(model=model_base, add_child_times=True)
         self._set_n_repeat_single()
 
     def _set_n_repeat_single(self):
@@ -426,67 +451,68 @@
         self._bagged_mode = False
 
     def _get_default_fold_fitting_strategy(self):
         try:
             try_import_ray()
             fold_fitting_strategy = "parallel_distributed" if DistributedContext.is_distributed_mode() else "parallel_local"
         except Exception as e:
-            warning_msg = f'Will use sequential fold fitting strategy because import of ray failed. Reason: {str(e)}'
+            warning_msg = f"Will use sequential fold fitting strategy because import of ray failed. Reason: {str(e)}"
             dup_filter.attach_filter_targets(warning_msg)
             logger.warning(warning_msg)
-            fold_fitting_strategy = 'sequential_local'
-        assert fold_fitting_strategy in ['parallel_distributed', 'parallel_local', 'sequential_local']
+            fold_fitting_strategy = "sequential_local"
+        assert fold_fitting_strategy in ["parallel_distributed", "parallel_local", "sequential_local"]
         return fold_fitting_strategy
-    
+
     def _get_fold_fitting_strategy(self, model_base, num_gpus):
-        fold_fitting_strategy = self.params.get('fold_fitting_strategy', 'auto')
+        fold_fitting_strategy = self.params.get("fold_fitting_strategy", "auto")
         if num_gpus is not None and not isinstance(num_gpus, str):
             # Use a specialized fitting strategy for CPU or GPU models if specified.
             if num_gpus > 0:
-                fold_fitting_strategy = self.params.get('fold_fitting_strategy_gpu', fold_fitting_strategy)
+                fold_fitting_strategy = self.params.get("fold_fitting_strategy_gpu", fold_fitting_strategy)
             else:
-                fold_fitting_strategy = self.params.get('fold_fitting_strategy_cpu', fold_fitting_strategy)
-        if fold_fitting_strategy == 'auto':
+                fold_fitting_strategy = self.params.get("fold_fitting_strategy_cpu", fold_fitting_strategy)
+        if fold_fitting_strategy == "auto":
             fold_fitting_strategy = self._get_default_fold_fitting_strategy()
-        disable_parallel_fitting = self.params.get('_disable_parallel_fitting', False)
-        if fold_fitting_strategy in ['parallel_local', "parallel_distributed"]:
+        disable_parallel_fitting = self.params.get("_disable_parallel_fitting", False)
+        if fold_fitting_strategy in ["parallel_local", "parallel_distributed"]:
             if fold_fitting_strategy == "parallel_local":
                 fold_fitting_strategy = ParallelLocalFoldFittingStrategy
             else:
                 fold_fitting_strategy = ParallelDistributedFoldFittingStrategy
             if disable_parallel_fitting:
                 fold_fitting_strategy = SequentialLocalFoldFittingStrategy
-                logger.log(20, f'\t{model_base.__class__.__name__} does not support parallel folding yet. Will use sequential folding instead')
-        elif fold_fitting_strategy == 'sequential_local':
+                logger.log(20, f"\t{model_base.__class__.__name__} does not support parallel folding yet. Will use sequential folding instead")
+        elif fold_fitting_strategy == "sequential_local":
             fold_fitting_strategy = SequentialLocalFoldFittingStrategy
         else:
             raise ValueError(
-                f'{fold_fitting_strategy} is not a valid option for fold_fitting_strategy'
-                'Valid options are: parallel_local and sequential_local'
+                f"{fold_fitting_strategy} is not a valid option for fold_fitting_strategy" "Valid options are: parallel_local and sequential_local"
             )
         return fold_fitting_strategy
 
-    def _fit_folds(self,
-                   X,
-                   y,
-                   model_base,
-                   X_pseudo=None,
-                   y_pseudo=None,
-                   k_fold=None,
-                   k_fold_start=0,
-                   k_fold_end=None,
-                   n_repeats=1,
-                   n_repeat_start=0,
-                   time_limit=None,
-                   sample_weight=None,
-                   save_folds=True,
-                   groups=None,
-                   num_cpus=None,
-                   num_gpus=None,
-                   **kwargs):
+    def _fit_folds(
+        self,
+        X,
+        y,
+        model_base,
+        X_pseudo=None,
+        y_pseudo=None,
+        k_fold=None,
+        k_fold_start=0,
+        k_fold_end=None,
+        n_repeats=1,
+        n_repeat_start=0,
+        time_limit=None,
+        sample_weight=None,
+        save_folds=True,
+        groups=None,
+        num_cpus=None,
+        num_gpus=None,
+        **kwargs,
+    ):
         fold_fitting_strategy_cls = self._get_fold_fitting_strategy(model_base=model_base, num_gpus=num_gpus)
         # TODO: Preprocess data here instead of repeatedly
         # FIXME: Raise exception if multiclass/binary and a single val fold contains all instances of a class. (Can happen if custom groups is specified)
         time_start = time.time()
         if k_fold_start != 0:
             cv_splitter = self._cv_splitters[n_repeat_start]
         else:
@@ -511,41 +537,58 @@
 
         fold_fit_args_list = [dict(fold_ctx=fold_ctx) for fold_ctx in fold_fit_args_list]
 
         oof_pred_proba, oof_pred_model_repeats = self._construct_empty_oof(X=X, y=y)
         models = []
 
         num_folds = len(fold_fit_args_list)
-        num_folds_parallel = self.params.get('num_folds_parallel', 'auto')
-        if num_folds_parallel == 'auto':
+        num_folds_parallel = self.params.get("num_folds_parallel", "auto")
+        if num_folds_parallel == "auto":
             num_folds_parallel = num_folds
         fold_fitting_strategy_args = dict(
-            model_base=model_base, model_base_kwargs=kwargs,
-            bagged_ensemble_model=self, X=X, y=y, X_pseudo=X_pseudo, y_pseudo=y_pseudo, sample_weight=sample_weight,
-            time_limit=time_limit, time_start=time_start, models=models,
-            oof_pred_proba=oof_pred_proba, oof_pred_model_repeats=oof_pred_model_repeats,
-            save_folds=save_folds, num_cpus=num_cpus, num_gpus=num_gpus
+            model_base=model_base,
+            model_base_kwargs=kwargs,
+            bagged_ensemble_model=self,
+            X=X,
+            y=y,
+            X_pseudo=X_pseudo,
+            y_pseudo=y_pseudo,
+            sample_weight=sample_weight,
+            time_limit=time_limit,
+            time_start=time_start,
+            models=models,
+            oof_pred_proba=oof_pred_proba,
+            oof_pred_model_repeats=oof_pred_model_repeats,
+            save_folds=save_folds,
+            num_cpus=num_cpus,
+            num_gpus=num_gpus,
         )
         # noinspection PyCallingNonCallable
         if issubclass(fold_fitting_strategy_cls, ParallelFoldFittingStrategy):
-            fold_fitting_strategy_args['num_jobs'] = num_folds
-            fold_fitting_strategy_args['num_folds_parallel'] = num_folds_parallel
+            fold_fitting_strategy_args["num_jobs"] = num_folds
+            fold_fitting_strategy_args["num_folds_parallel"] = num_folds_parallel
         if fold_fitting_strategy_cls == ParallelDistributedFoldFittingStrategy:
-            fold_fitting_strategy_args['model_sync_path'] = DistributedContext.get_model_sync_path()
+            fold_fitting_strategy_args["model_sync_path"] = DistributedContext.get_model_sync_path()
         fold_fitting_strategy: FoldFittingStrategy = fold_fitting_strategy_cls(**fold_fitting_strategy_args)
 
         if type(fold_fitting_strategy) == ParallelLocalFoldFittingStrategy and not fold_fitting_strategy.is_mem_sufficient():
             # If memory is not sufficient, fall back to sequential fold strategy
             fold_fitting_strategy: FoldFittingStrategy = SequentialLocalFoldFittingStrategy(**fold_fitting_strategy_args)
-            logger.log(30, f'\tMemory not enough to fit {model_base.__class__.__name__} folds in parallel. Will do sequential fitting instead. '
-                           f'\tConsider decreasing folds trained in parallel by passing num_folds_parallel to ag_args_ensemble when calling predictor.fit')
+            logger.log(
+                30,
+                f"\tMemory not enough to fit {model_base.__class__.__name__} folds in parallel. Will do sequential fitting instead. "
+                f"\tConsider decreasing folds trained in parallel by passing num_folds_parallel to ag_args_ensemble when calling predictor.fit",
+            )
 
-        logger.log(20, f'\tFitting {len(fold_fit_args_list)} child models '
-                       f'({fold_fit_args_list[0]["fold_ctx"]["model_name_suffix"]} - {fold_fit_args_list[-1]["fold_ctx"]["model_name_suffix"]}) | '
-                       f'Fitting with {fold_fitting_strategy.__class__.__name__}')
+        logger.log(
+            20,
+            f"\tFitting {len(fold_fit_args_list)} child models "
+            f'({fold_fit_args_list[0]["fold_ctx"]["model_name_suffix"]} - {fold_fit_args_list[-1]["fold_ctx"]["model_name_suffix"]}) | '
+            f"Fitting with {fold_fitting_strategy.__class__.__name__}",
+        )
 
         # noinspection PyCallingNonCallable
         for fold_fit_args in fold_fit_args_list:
             fold_fitting_strategy.schedule_fold_model_fit(**fold_fit_args)
         fold_fitting_strategy.after_all_folds_scheduled()
 
         for model in models:
@@ -569,22 +612,15 @@
             self._n_repeats_finished = self._n_repeats
         else:
             self._k = k_fold
             self._k_fold_end = k_fold_end
             self._n_repeats_finished = self._n_repeats - 1
 
     @staticmethod
-    def _generate_fold_configs(*,
-                               X,
-                               y,
-                               cv_splitter,
-                               k_fold_start,
-                               k_fold_end,
-                               n_repeat_start,
-                               n_repeat_end) -> (list, int, int):
+    def _generate_fold_configs(*, X, y, cv_splitter, k_fold_start, k_fold_end, n_repeat_start, n_repeat_end) -> (list, int, int):
         """
         Generates fold configs given a cv_splitter, k_fold start-end and n_repeat start-end.
         Fold configs are used by inheritors of FoldFittingStrategy when fitting fold models.
 
         Returns a list of fold configs, the number of started repeats, and the number of finished repeats.
         """
         k_fold = cv_splitter.n_splits
@@ -605,15 +641,15 @@
 
             fold_in_set_start = k_fold_start if repeat == n_repeat_start else 0
             fold_in_set_end = k_fold_end if is_last_set else k_fold
 
             for fold_in_set in range(fold_in_set_start, fold_in_set_end):  # For each fold
                 fold = fold_in_set + (repeat * k_fold)
                 fold_ctx = dict(
-                    model_name_suffix=f'S{repeat + 1}F{fold_in_set + 1}',  # S5F3 = 3rd fold of the 5th repeat set
+                    model_name_suffix=f"S{repeat + 1}F{fold_in_set + 1}",  # S5F3 = 3rd fold of the 5th repeat set
                     fold=kfolds[fold],
                     is_last_fold=fold == (fold_end - 1),
                     folds_to_fit=folds_to_fit,
                     folds_finished=fold - fold_start,
                     folds_left=fold_end - fold,
                 )
 
@@ -624,83 +660,89 @@
         assert len(fold_fit_args_list) == folds_to_fit, "fold_fit_args_list is not the expected length!"
 
         return fold_fit_args_list, n_repeats_started, n_repeats_finished
 
     # TODO: Augment to generate OOF after shuffling each column in X (Batching), this is the fastest way.
     # TODO: Reduce logging clutter during OOF importance calculation (Currently logs separately for each child)
     # Generates OOF predictions from pre-trained bagged models, assuming X and y are in the same row order as used in .fit(X, y)
-    def compute_feature_importance(self,
-                                   X,
-                                   y,
-                                   features=None,
-                                   silent=False,
-                                   time_limit=None,
-                                   is_oof=False,
-                                   **kwargs) -> pd.DataFrame:
+    def compute_feature_importance(self, X, y, features=None, silent=False, time_limit=None, is_oof=False, **kwargs) -> pd.DataFrame:
         if features is None:
             # FIXME: use FULL features (children can have different features)
             features = self.load_child(model=self.models[0]).features
         if not is_oof:
             return super().compute_feature_importance(X, y, features=features, time_limit=time_limit, silent=silent, **kwargs)
         fi_fold_list = []
         model_index = 0
         num_children = len(self.models)
         if time_limit is not None:
             time_limit_per_child = time_limit / num_children
         else:
             time_limit_per_child = None
         if not silent:
-            logging_message = f'Computing feature importance via permutation shuffling for {len(features)} features using out-of-fold (OOF) data aggregated across {num_children} child models...'
+            logging_message = f"Computing feature importance via permutation shuffling for {len(features)} features using out-of-fold (OOF) data aggregated across {num_children} child models..."
             if time_limit is not None:
-                logging_message = f'{logging_message} Time limit: {time_limit}s...'
+                logging_message = f"{logging_message} Time limit: {time_limit}s..."
             logger.log(20, logging_message)
 
         time_start = time.time()
         early_stop = False
         children_completed = 0
-        log_final_suffix = ''
+        log_final_suffix = ""
         for n_repeat, k in enumerate(self._k_per_n_repeat):
             if is_oof:
                 if self._child_oof or not self._bagged_mode:
-                    raise AssertionError('Model trained with no validation data cannot get feature importance on training data, please specify new test data to compute feature importances (model=%s)' % self.name)
+                    raise AssertionError(
+                        "Model trained with no validation data cannot get feature importance on training data, please specify new test data to compute feature importances (model=%s)"
+                        % self.name
+                    )
                 kfolds = self._cv_splitters[n_repeat].split(X=X, y=y)
-                cur_kfolds = kfolds[n_repeat * k:(n_repeat + 1) * k]
+                cur_kfolds = kfolds[n_repeat * k : (n_repeat + 1) * k]
             else:
                 cur_kfolds = [(None, list(range(len(X))))] * k
             for i, fold in enumerate(cur_kfolds):
                 _, test_index = fold
                 model = self.load_child(self.models[model_index + i])
-                fi_fold = model.compute_feature_importance(X=X.iloc[test_index, :], y=y.iloc[test_index], features=features, time_limit=time_limit_per_child,
-                                                           silent=silent, log_prefix='\t', importance_as_list=True, **kwargs)
+                fi_fold = model.compute_feature_importance(
+                    X=X.iloc[test_index, :],
+                    y=y.iloc[test_index],
+                    features=features,
+                    time_limit=time_limit_per_child,
+                    silent=silent,
+                    log_prefix="\t",
+                    importance_as_list=True,
+                    **kwargs,
+                )
                 fi_fold_list.append(fi_fold)
 
                 children_completed += 1
                 if time_limit is not None and children_completed != num_children:
                     time_now = time.time()
                     time_left = time_limit - (time_now - time_start)
                     time_child_average = (time_now - time_start) / children_completed
                     if time_left < (time_child_average * 1.1):
-                        log_final_suffix = f' (Early stopping due to lack of time...)'
+                        log_final_suffix = f" (Early stopping due to lack of time...)"
                         early_stop = True
                         break
             if early_stop:
                 break
             model_index += k
         # TODO: DON'T THROW AWAY SAMPLES! USE LARGER N
         fi_list_dict = dict()
         for val in fi_fold_list:
-            val = val['importance'].to_dict()  # TODO: Don't throw away stddev information of children
+            val = val["importance"].to_dict()  # TODO: Don't throw away stddev information of children
             for key in val:
                 if key not in fi_list_dict:
                     fi_list_dict[key] = []
                 fi_list_dict[key] += val[key]
         fi_df = _compute_fi_with_stddev(fi_list_dict)
 
         if not silent:
-            logger.log(20, f'\t{round(time.time() - time_start, 2)}s\t= Actual runtime (Completed {children_completed} of {num_children} children){log_final_suffix}')
+            logger.log(
+                20, f"\t{round(time.time() - time_start, 2)}s\t= Actual runtime (Completed {children_completed} of {num_children} children){log_final_suffix}"
+            )
 
         return fi_df
 
     def get_features(self):
         assert self.is_fit(), "The model must be fit before calling the get_features method."
         return self.load_child(self.models[0]).get_features()
 
@@ -780,36 +822,36 @@
 
         Returns
         -------
         model_full_template : AbstractModel
             Unfit model capable of being fit without X_val, y_val. Hyperparameters are based on post-fit self hyperparameters.
         """
         init_args = self.get_params()
-        init_args['hyperparameters']['save_bag_folds'] = True  # refit full models must save folds
-        init_args['model_base'] = self.convert_to_refit_full_template_child()
+        init_args["hyperparameters"]["save_bag_folds"] = True  # refit full models must save folds
+        init_args["model_base"] = self.convert_to_refit_full_template_child()
         if name_suffix:
-            init_args['name'] = init_args['name'] + name_suffix
+            init_args["name"] = init_args["name"] + name_suffix
         model_full_template = self.__class__(**init_args)
         return model_full_template
 
     def convert_to_refit_full_template_child(self) -> AbstractModel:
         refit_params_trained = self._get_compressed_params_trained()
         refit_params = copy.deepcopy(self._get_model_base().get_params())
-        refit_params['hyperparameters'].update(refit_params_trained)
+        refit_params["hyperparameters"].update(refit_params_trained)
         refit_child_template = self._child_type(**refit_params)
 
         return refit_child_template
 
     def convert_to_refit_full_via_copy(self) -> AbstractModel:
         """
         Creates a new refit_full variant of the model, but instead of training it simply copies `self` while keeping only the first fold model.
         This method is for compatibility with models that have not implemented refit_full support as a fallback.
         """
-        if not self.params.get('save_bag_folds', True):
-            raise AssertionError('Cannot perform copy-based refit_full when save_bag_folds is False!')
+        if not self.params.get("save_bag_folds", True):
+            raise AssertionError("Cannot perform copy-based refit_full when save_bag_folds is False!")
         __models = self.models
         self.models = []
         model_full = copy.deepcopy(self)
         self.models = __models
         child_0 = self.load_child(self.models[0])
         model_full.fit_time = None
         model_full.predict_time = None
@@ -824,27 +866,24 @@
 
     def get_params(self):
         init_args = dict(
             model_base=self._get_model_base(),
             random_state=self._random_state,
         )
         init_args.update(super().get_params())
-        init_args.pop('eval_metric')
-        init_args.pop('problem_type')
+        init_args.pop("eval_metric")
+        init_args.pop("problem_type")
         return init_args
 
     def convert_to_template_child(self):
         return self._get_model_base().convert_to_template()
 
     def _get_compressed_params(self, model_params_list=None):
         if model_params_list is None:
-            model_params_list = [
-                self.load_child(child).get_trained_params()
-                for child in self.models
-            ]
+            model_params_list = [self.load_child(child).get_trained_params() for child in self.models]
 
         model_params_compressed = dict()
         for param in model_params_list[0].keys():
             model_param_vals = [model_params[param] for model_params in model_params_list]
             if all(isinstance(val, bool) for val in model_param_vals):
                 counter = Counter(model_param_vals)
                 compressed_val = counter.most_common(1)[0][0]
@@ -858,18 +897,15 @@
                     compressed_val = counter.most_common(1)[0][0]
                 except TypeError:
                     compressed_val = model_param_vals[0]
             model_params_compressed[param] = compressed_val
         return model_params_compressed
 
     def _get_compressed_params_trained(self):
-        model_params_list = [
-            self.load_child(child).params_trained
-            for child in self.models
-        ]
+        model_params_list = [self.load_child(child).params_trained for child in self.models]
         return self._get_compressed_params(model_params_list=model_params_list)
 
     def _get_model_base(self):
         if self.model_base is None:
             return self.load_model_base()
         else:
             return self.model_base
@@ -914,31 +950,31 @@
         if load_oof:
             model._load_oof()
         return model
 
     @classmethod
     def load_oof(cls, path, verbose=True):
         try:
-            oof = load_pkl.load(path=os.path.join(path + 'utils', cls._oof_filename), verbose=verbose)
-            oof_pred_proba = oof['_oof_pred_proba']
-            oof_pred_model_repeats = oof['_oof_pred_model_repeats']
+            oof = load_pkl.load(path=os.path.join(path + "utils", cls._oof_filename), verbose=verbose)
+            oof_pred_proba = oof["_oof_pred_proba"]
+            oof_pred_model_repeats = oof["_oof_pred_model_repeats"]
         except FileNotFoundError:
             model = cls.load(path=path, reset_paths=True, verbose=verbose)
             model._load_oof()
             oof_pred_proba = model._oof_pred_proba
             oof_pred_model_repeats = model._oof_pred_model_repeats
         return cls._oof_pred_proba_func(oof_pred_proba=oof_pred_proba, oof_pred_model_repeats=oof_pred_model_repeats)
 
     def _load_oof(self):
         if self._oof_pred_proba is not None:
             pass
         else:
-            oof = load_pkl.load(path=os.path.join(self.path + 'utils', self._oof_filename))
-            self._oof_pred_proba = oof['_oof_pred_proba']
-            self._oof_pred_model_repeats = oof['_oof_pred_model_repeats']
+            oof = load_pkl.load(path=os.path.join(self.path + "utils", self._oof_filename))
+            self._oof_pred_proba = oof["_oof_pred_proba"]
+            self._oof_pred_model_repeats = oof["_oof_pred_model_repeats"]
 
     def persist_child_models(self, reset_paths=True):
         for i, model_name in enumerate(self.models):
             if isinstance(model_name, str):
                 child_path = self.create_contexts(self.path + model_name + os.path.sep)
                 child_model = self._child_type.load(path=child_path, reset_paths=reset_paths, verbose=True)
                 self.models[i] = child_model
@@ -952,32 +988,35 @@
             if isinstance(model, str):
                 model_names.append(model)
             else:
                 model_names.append(model.name)
         return model_names
 
     def load_model_base(self):
-        return load_pkl.load(path=os.path.join(self.path + 'utils', 'model_template.pkl'))
+        return load_pkl.load(path=os.path.join(self.path + "utils", "model_template.pkl"))
 
     def save_model_base(self, model_base):
-        save_pkl.save(path=os.path.join(self.path + 'utils', 'model_template.pkl'), object=model_base)
+        save_pkl.save(path=os.path.join(self.path + "utils", "model_template.pkl"), object=model_base)
 
     def save(self, path=None, verbose=True, save_oof=True, save_children=False) -> str:
         if path is None:
             path = self.path
 
         if save_children:
             for child in self.models:
                 self.save_child(model=child, path=path, verbose=False)
 
         if save_oof and self._oof_pred_proba is not None:
-            save_pkl.save(path=os.path.join(path + 'utils', self._oof_filename), object={
-                '_oof_pred_proba': self._oof_pred_proba,
-                '_oof_pred_model_repeats': self._oof_pred_model_repeats,
-            })
+            save_pkl.save(
+                path=os.path.join(path + "utils", self._oof_filename),
+                object={
+                    "_oof_pred_proba": self._oof_pred_proba,
+                    "_oof_pred_model_repeats": self._oof_pred_model_repeats,
+                },
+            )
             self._oof_pred_proba = None
             self._oof_pred_model_repeats = None
 
         _models = self.models
         if self.low_memory:
             self.models = self._get_child_model_names(self.models)
         path = super().save(path=path, verbose=verbose)
@@ -986,28 +1025,28 @@
 
     # If `remove_fit_stack=True`, variables will be removed that are required to fit more folds and to fit new stacker models which use this model as a base model.
     #  This includes OOF variables.
     def reduce_memory_size(self, remove_fit_stack=False, remove_fit=True, remove_info=False, requires_save=True, reduce_children=False, **kwargs):
         super().reduce_memory_size(remove_fit=remove_fit, remove_info=remove_info, requires_save=requires_save, **kwargs)
         if remove_fit_stack:
             try:
-                os.remove(os.path.join(self.path + 'utils', self._oof_filename))
+                os.remove(os.path.join(self.path + "utils", self._oof_filename))
             except FileNotFoundError:
                 pass
             if requires_save:
                 self._oof_pred_proba = None
                 self._oof_pred_model_repeats = None
             try:
-                os.remove(os.path.join(self.path + 'utils', 'model_template.pkl'))
+                os.remove(os.path.join(self.path + "utils", "model_template.pkl"))
             except FileNotFoundError:
                 pass
             if requires_save:
                 self.model_base = None
             try:
-                os.rmdir(self.path + 'utils')
+                os.rmdir(self.path + "utils")
             except OSError:
                 pass
         if reduce_children:
             for model in self.models:
                 model = self.load_child(model)
                 model.reduce_memory_size(remove_fit=remove_fit, remove_info=remove_info, requires_save=requires_save, **kwargs)
                 if requires_save and self.low_memory:
@@ -1021,26 +1060,26 @@
             else:
                 model_names.append(model.name)
         return model_names
 
     def get_info(self):
         info = super().get_info()
         children_info = self._get_child_info()
-        child_memory_sizes = [child['memory_size'] for child in children_info.values()]
+        child_memory_sizes = [child["memory_size"] for child in children_info.values()]
         sum_memory_size_child = sum(child_memory_sizes)
         if child_memory_sizes:
             max_memory_size_child = max(child_memory_sizes)
         else:
             max_memory_size_child = 0
         if self.low_memory:
-            max_memory_size = info['memory_size'] + sum_memory_size_child
-            min_memory_size = info['memory_size'] + max_memory_size_child
+            max_memory_size = info["memory_size"] + sum_memory_size_child
+            min_memory_size = info["memory_size"] + max_memory_size_child
         else:
-            max_memory_size = info['memory_size']
-            min_memory_size = info['memory_size'] - sum_memory_size_child + max_memory_size_child
+            max_memory_size = info["memory_size"]
+            min_memory_size = info["memory_size"] - sum_memory_size_child + max_memory_size_child
 
         # Necessary if save_space is used as save_space deletes model_base.
         if len(self.models) > 0:
             child_model = self.load_child(self.models[0])
         else:
             child_model = self._get_model_base()
         child_hyperparameters = child_model.params
@@ -1060,20 +1099,20 @@
             bagged_mode=self._bagged_mode,
             max_memory_size=max_memory_size,  # Memory used when all children are loaded into memory at once.
             min_memory_size=min_memory_size,  # Memory used when only the largest child is loaded into memory.
             child_hyperparameters=child_hyperparameters,
             child_hyperparameters_fit=self._get_compressed_params_trained(),
             child_ag_args_fit=child_ag_args_fit,
         )
-        info['bagged_info'] = bagged_info
-        info['children_info'] = children_info
+        info["bagged_info"] = bagged_info
+        info["children_info"] = children_info
 
-        child_features_full = list(set().union(*[child['features'] for child in children_info.values()]))
-        info['features'] = child_features_full
-        info['num_features'] = len(child_features_full)
+        child_features_full = list(set().union(*[child["features"] for child in children_info.values()]))
+        info["features"] = child_features_full
+        info["num_features"] = len(child_features_full)
 
         return info
 
     def get_memory_size(self):
         models = self.models
         self.models = None
         memory_size = super().get_memory_size()
@@ -1111,33 +1150,23 @@
         elif self.problem_type == QUANTILE:
             oof_pred_proba = np.zeros(shape=(len(X), len(self.quantile_levels)), dtype=np.float32)
         else:
             oof_pred_proba = np.zeros(shape=len(X), dtype=np.float32)
         oof_pred_model_repeats = np.zeros(shape=len(X), dtype=np.uint8)
         return oof_pred_proba, oof_pred_model_repeats
 
-    def _hyperparameter_tune(
-        self,
-        X,
-        y,
-        X_val,
-        y_val,
-        hpo_executor,
-        k_fold=None,
-        k_fold_end=None,
-        **kwargs
-    ):
+    def _hyperparameter_tune(self, X, y, X_val, y_val, hpo_executor, k_fold=None, k_fold_end=None, **kwargs):
         time_start = time.time()
         logger.log(15, "Starting generic AbstractModel hyperparameter tuning for %s model..." % self.name)
         k_fold, k_fold_end = self._update_k_fold(k_fold=k_fold, k_fold_end=k_fold_end)
         # initialize the model base to get necessary info for search space and estimating memory usage
         initialized_model_base = copy.deepcopy(self.model_base)
         model_init_args = self.model_base.get_params()
-        model_init_args['feature_metadata'] = self.feature_metadata
-        model_init_args['num_classes'] = self.num_classes
+        model_init_args["feature_metadata"] = self.feature_metadata
+        model_init_args["num_classes"] = self.num_classes
         initialized_model_base.initialize(X=X, y=y, **model_init_args)
         search_space = initialized_model_base._get_search_space()
 
         try:
             hpo_executor.validate_search_space(search_space, self.name)
         except EmptySearchSpace:
             return skip_hpo(X=X, y=y, X_val=X_val, y_val=y_val, **kwargs)
@@ -1150,75 +1179,73 @@
         train_path, val_path = hpo_executor.prepare_data(X=X, y=y, X_val=X_val, y_val=y_val, path_prefix=data_path)
 
         model_cls = self.__class__
         init_params = copy.deepcopy(self.get_params())
         model_base = self._get_model_base()
 
         if not inspect.isclass(model_base):
-            init_params['model_base'] = init_params['model_base'].__class__
-            init_params['model_base_kwargs'] = model_base.get_params()
+            init_params["model_base"] = init_params["model_base"].__class__
+            init_params["model_base_kwargs"] = model_base.get_params()
         # Here the hyperparameters are unprocessed search space.
         # HPO Executor will handle passing in the correct parameters.
         # But we need to keep the ag_args_fit being passed to the base model
-        if 'hyperparameters' in init_params['model_base_kwargs']:
-            model_base_ag_args_fit = init_params['model_base_kwargs']['hyperparameters'].get('ag_args_fit', {})
-            init_params['model_base_kwargs']['hyperparameters'] = {'ag_args_fit': model_base_ag_args_fit}
+        if "hyperparameters" in init_params["model_base_kwargs"]:
+            model_base_ag_args_fit = init_params["model_base_kwargs"]["hyperparameters"].get("ag_args_fit", {})
+            init_params["model_base_kwargs"]["hyperparameters"] = {"ag_args_fit": model_base_ag_args_fit}
         # We set soft time limit to avoid trials being terminated directly by ray tune
         trial_soft_time_limit = None
         if hpo_executor.time_limit is not None:
             trial_soft_time_limit = max(hpo_executor.time_limit * 0.9, hpo_executor.time_limit - 5)  # 5 seconds max for buffer
 
         fit_kwargs = copy.deepcopy(kwargs)
-        fit_kwargs['k_fold'] = k_fold
-        fit_kwargs['k_fold_end'] = k_fold_end
-        fit_kwargs['feature_metadata'] = self.feature_metadata
-        fit_kwargs['num_classes'] = self.num_classes
-        fit_kwargs['sample_weight'] = kwargs.get('sample_weight', None)
-        fit_kwargs['sample_weight_val'] = kwargs.get('sample_weight_val', None)
-        fit_kwargs.pop('time_limit', None)  # time_limit already set in hpo_executor
+        fit_kwargs["k_fold"] = k_fold
+        fit_kwargs["k_fold_end"] = k_fold_end
+        fit_kwargs["feature_metadata"] = self.feature_metadata
+        fit_kwargs["num_classes"] = self.num_classes
+        fit_kwargs["sample_weight"] = kwargs.get("sample_weight", None)
+        fit_kwargs["sample_weight_val"] = kwargs.get("sample_weight_val", None)
+        fit_kwargs.pop("time_limit", None)  # time_limit already set in hpo_executor
         train_fn_kwargs = dict(
             model_cls=model_cls,
             init_params=init_params,
             time_start=time_start,
             time_limit=trial_soft_time_limit,
             fit_kwargs=fit_kwargs,
             train_path=train_path,
             val_path=val_path,
             hpo_executor=hpo_executor,
             is_bagged_model=True,
         )
-            
-        minimum_resources_per_fold = self.get_minimum_resources(
-            is_gpu_available=(hpo_executor.resources.get('num_gpus', 0) > 0)
-        )
-        minimum_cpu_per_fold = minimum_resources_per_fold.get('num_cpus', 1)
-        minimum_gpu_per_fold = minimum_resources_per_fold.get('num_gpus', 0)
+
+        minimum_resources_per_fold = self.get_minimum_resources(is_gpu_available=(hpo_executor.resources.get("num_gpus", 0) > 0))
+        minimum_cpu_per_fold = minimum_resources_per_fold.get("num_cpus", 1)
+        minimum_gpu_per_fold = minimum_resources_per_fold.get("num_gpus", 0)
 
         hpo_executor.execute(
             model_trial=model_trial,
             train_fn_kwargs=train_fn_kwargs,
             directory=directory,
             minimum_cpu_per_trial=minimum_cpu_per_fold,
             minimum_gpu_per_trial=minimum_gpu_per_fold,
             model_estimate_memory_usage=None,  # Not needed as we've already calculated it above
-            adapter_type='tabular',
+            adapter_type="tabular",
             trainable_is_parallel=True,
-            tune_config_kwargs={'chdir_to_trial_dir': False}
+            tune_config_kwargs={"chdir_to_trial_dir": False},
         )
 
         hpo_results = hpo_executor.get_hpo_results(
             model_name=self.name,
             model_path_root=self.path_root,
             time_start=time_start,
         )
 
         return hpo_results
 
     def _more_tags(self):
         return {
-            'valid_oof': True,
-            'can_refit_full': True,
+            "valid_oof": True,
+            "can_refit_full": True,
         }
 
     def _get_tags_child(self):
         """Gets the tags of the child model."""
         return self._get_model_base()._get_tags()
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/fold_fitting_strategy.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/fold_fitting_strategy.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 import copy
 import logging
 import math
 import os
-import time
-import pandas as pd
 import pickle
+import time
 from abc import abstractmethod
+from typing import Any, Dict, Optional, Union
 
+import pandas as pd
 from numpy import ndarray
 from pandas import DataFrame, Series
-from typing import Any, Dict, Union, Optional
 
 from autogluon.common.utils.lite import disable_if_lite_mode
 from autogluon.common.utils.pandas_utils import get_approximate_df_mem_usage
 from autogluon.common.utils.resource_utils import ResourceManager
+from autogluon.common.utils.s3_utils import download_s3_folder, s3_path_to_bucket_prefix, upload_s3_folder
 from autogluon.common.utils.try_import import try_import_ray
-from autogluon.common.utils.s3_utils import download_s3_folder, upload_s3_folder, s3_path_to_bucket_prefix
 
-from ..abstract.abstract_model import AbstractModel
 from ...ray.resources_calculator import ResourceCalculatorFactory
-from ...utils.exceptions import TimeLimitExceeded, NotEnoughMemoryError, NotEnoughCudaMemoryError
+from ...utils.exceptions import NotEnoughCudaMemoryError, NotEnoughMemoryError, TimeLimitExceeded
+from ..abstract.abstract_model import AbstractModel
 
 logger = logging.getLogger(__name__)
 
-TEXT_MODEL = 'TextPredictorModel'
-IMAGE_MODEL = 'ImagePredictorModel'
-TABULAR_TORCH_MODEL = 'TabularNeuralNetModel'
-TABULAR_FASTAI_MODEL = 'NNFastAiTabularModel'
-
+TEXT_MODEL = "TextPredictorModel"
+IMAGE_MODEL = "ImagePredictorModel"
+TABULAR_TORCH_MODEL = "TabularNeuralNetModel"
+TABULAR_FASTAI_MODEL = "NNFastAiTabularModel"
 
-class AbstractFoldFittingStrategy():
 
+class AbstractFoldFittingStrategy:
     @abstractmethod
     def schedule_fold_model_fit(self, fold_ctx):
         """
         Schedule fold model training.
         By design this part is supposed to be 'lazy' evaluator,
         no actual training is performed here.
         Distributed fitters will handle jobs scheduling here.
@@ -49,16 +48,16 @@
         """
 
     @abstractmethod
     def _fit(self, model_base, time_start_fold, time_limit_fold, fold_ctx, kwargs):
         """
         Method is called when a fold is ready to be fit
         """
-        
-        
+
+
 class FoldFittingStrategy(AbstractFoldFittingStrategy):
     """
     Provides some default implementation for AbstractFoldFittingStrategy
 
     Parameters
     ----------
         model_base: AbstractModel
@@ -70,40 +69,40 @@
         X : DataFrame
             The training data the model will be trained on.
         y: Series
             The labels of the training data.
         sample_weight:
             The sample weight of the training data.
         time_limit: float
-            Approximately how long(in seconds) the fold fitting should be run for. 
-            If None, no time-constraint will be enforced allowing the folds to fully train.        
+            Approximately how long(in seconds) the fold fitting should be run for.
+            If None, no time-constraint will be enforced allowing the folds to fully train.
         time_start: float
             Time starts to fit the BaggedEnsembleModel.
         models: list
             List of models that will be trained.
         oof_pred_proba: ndarray
             Out of folds predict probabilities that are already calculated.
         oof_pred_model_repeats: ndarray,
             Number of repeats the out of folds predict probabilities has been done.
-        save_folds: bool, 
+        save_folds: bool,
             Whether to save the folds to disk.
         time_limit_fold_ratio: float, default=0.8
             The ratio of max time limit for each fold.
             If the estimated time required exceeds this ratio, will raise TimeLimitExceed error
     Attributes
     ----------
         X : DataFrame
             The training data the model will be trained on.
         y: Series
             The labels of the training data.
         sample_weight:
             The sample weight of the training data.
         time_limit: float
-            Approximately how long(in seconds) the fold fitting should be run for. 
-            If None, no time-constraint will be enforced allowing the folds to fully train.        
+            Approximately how long(in seconds) the fold fitting should be run for.
+            If None, no time-constraint will be enforced allowing the folds to fully train.
         time_start: float
             Time starts to fit the BaggedEnsembleModel.
         models: list
             List of models that will be trained.
         oof_pred_proba: ndarray
             Out of folds predict probabilities that are already calculated.
         oof_pred_model_repeats: ndarray,
@@ -112,19 +111,35 @@
             List of jobs that will be scheduled.
         save_folds: bool,
             Whether to save the folds to disk.
         time_limit_fold_ratio: float
             The ratio of max time limit for each fold.
     """
 
-    def __init__(self, model_base, model_base_kwargs, bagged_ensemble_model,
-                 X: DataFrame, y: Series, X_pseudo: DataFrame, y_pseudo: Series,
-                 sample_weight, time_limit: float, time_start: float,
-                 models: list, oof_pred_proba: ndarray, oof_pred_model_repeats: ndarray,
-                 save_folds: bool, num_cpus: int, num_gpus: Union[int, float], time_limit_fold_ratio=0.8, **kwargs):
+    def __init__(
+        self,
+        model_base,
+        model_base_kwargs,
+        bagged_ensemble_model,
+        X: DataFrame,
+        y: Series,
+        X_pseudo: DataFrame,
+        y_pseudo: Series,
+        sample_weight,
+        time_limit: float,
+        time_start: float,
+        models: list,
+        oof_pred_proba: ndarray,
+        oof_pred_model_repeats: ndarray,
+        save_folds: bool,
+        num_cpus: int,
+        num_gpus: Union[int, float],
+        time_limit_fold_ratio=0.8,
+        **kwargs,
+    ):
         self.model_base = model_base
         self.model_base_kwargs = model_base_kwargs
         self.X = X
         self.y = y
         self.X_pseudo = X_pseudo
         self.y_pseudo = y_pseudo
         self.sample_weight = sample_weight
@@ -135,72 +150,76 @@
         self.oof_pred_model_repeats = oof_pred_model_repeats
         self.bagged_ensemble_model = bagged_ensemble_model
         self.jobs = []
         self.save_folds = save_folds
         self.time_limit_fold_ratio = time_limit_fold_ratio
         self.num_cpus = num_cpus
         self.num_gpus = num_gpus
-        logger.debug(f'Upper level total_num_cpus, num_gpus {self.num_cpus} | {self.num_gpus}')
+        logger.debug(f"Upper level total_num_cpus, num_gpus {self.num_cpus} | {self.num_gpus}")
         self._validate_user_specified_resources()
 
     def schedule_fold_model_fit(self, fold_ctx):
         raise NotImplementedError
 
     def after_all_folds_scheduled(self):
         raise NotImplementedError
-    
+
     def _validate_user_specified_resources(self):
         # User specified value through ag_args_fit means they want this individual model to use this amount of resources
         user_ensemble_resources = None
         user_resources_per_job = None
         # initialize the model base to get necessary info for estimating memory usage and getting resources
         self._initialized_model_base = copy.deepcopy(self.model_base)
         self._initialized_model_base.initialize(X=self.X, y=self.y, **self.model_base_kwargs)
-        user_cpu_per_job = self._initialized_model_base._get_child_aux_val(key='num_cpus', default=None)
-        user_gpu_per_job = self._initialized_model_base._get_child_aux_val(key='num_gpus', default=None)
+        user_cpu_per_job = self._initialized_model_base._get_child_aux_val(key="num_cpus", default=None)
+        user_gpu_per_job = self._initialized_model_base._get_child_aux_val(key="num_gpus", default=None)
         minimum_model_resources = self._initialized_model_base.get_minimum_resources(
             is_gpu_available=(self.num_gpus > 0),
         )
-        minimum_model_num_cpus = minimum_model_resources.get('num_cpus', 1)
-        minimum_model_num_gpus = minimum_model_resources.get('num_gpus', 0)
-        logger.debug(f'minimum_model_resources: {minimum_model_resources}')
-        logger.debug(f'user_cpu_per_job, user_gpu_per_job {user_cpu_per_job} | {user_gpu_per_job}')
-        user_ensemble_cpu = self.bagged_ensemble_model._user_params_aux.get('num_cpus', None)
-        user_ensemble_gpu = self.bagged_ensemble_model._user_params_aux.get('num_gpus', None)
-        logger.debug(f'user_ensemble_cpu, user_ensemble_gpu {user_ensemble_cpu} | {user_ensemble_gpu}')
+        minimum_model_num_cpus = minimum_model_resources.get("num_cpus", 1)
+        minimum_model_num_gpus = minimum_model_resources.get("num_gpus", 0)
+        logger.debug(f"minimum_model_resources: {minimum_model_resources}")
+        logger.debug(f"user_cpu_per_job, user_gpu_per_job {user_cpu_per_job} | {user_gpu_per_job}")
+        user_ensemble_cpu = self.bagged_ensemble_model._user_params_aux.get("num_cpus", None)
+        user_ensemble_gpu = self.bagged_ensemble_model._user_params_aux.get("num_gpus", None)
+        logger.debug(f"user_ensemble_cpu, user_ensemble_gpu {user_ensemble_cpu} | {user_ensemble_gpu}")
         if user_ensemble_cpu is not None or user_ensemble_gpu is not None:
             user_ensemble_resources = dict()
         if user_ensemble_cpu is not None:
-            assert user_ensemble_cpu <= self.num_cpus, \
-                f"Detected ensemble cpu requirement = {user_ensemble_cpu} > total cpu granted = {self.num_cpus}"
-            assert user_ensemble_cpu >= minimum_model_num_cpus, \
-                f"Detected ensenble cpu requirement = {user_ensemble_cpu} < minimum cpu required by the model = {minimum_model_num_cpus}"
-            user_ensemble_resources['num_cpus'] = user_ensemble_cpu
+            assert user_ensemble_cpu <= self.num_cpus, f"Detected ensemble cpu requirement = {user_ensemble_cpu} > total cpu granted = {self.num_cpus}"
+            assert (
+                user_ensemble_cpu >= minimum_model_num_cpus
+            ), f"Detected ensenble cpu requirement = {user_ensemble_cpu} < minimum cpu required by the model = {minimum_model_num_cpus}"
+            user_ensemble_resources["num_cpus"] = user_ensemble_cpu
             self.num_cpus = user_ensemble_cpu
         if user_ensemble_gpu is not None:
-            assert user_ensemble_gpu <= self.num_gpus, \
-                f"Detected ensemble gpu requirement = {user_ensemble_gpu} > total gpu granted = {self.num_gpus}"
-            assert user_ensemble_gpu >= minimum_model_num_gpus, \
-                f"Detected ensenble gpu requirement = {user_ensemble_cpu} < minimum gpu required by the model = {minimum_model_num_gpus}"
-            user_ensemble_resources['num_gpus'] = user_ensemble_gpu
+            assert user_ensemble_gpu <= self.num_gpus, f"Detected ensemble gpu requirement = {user_ensemble_gpu} > total gpu granted = {self.num_gpus}"
+            assert (
+                user_ensemble_gpu >= minimum_model_num_gpus
+            ), f"Detected ensenble gpu requirement = {user_ensemble_cpu} < minimum gpu required by the model = {minimum_model_num_gpus}"
+            user_ensemble_resources["num_gpus"] = user_ensemble_gpu
             self.num_gpus = user_ensemble_gpu
         if user_cpu_per_job is not None or user_gpu_per_job is not None:
             user_resources_per_job = dict()
         if user_cpu_per_job is not None:
-            assert user_cpu_per_job <= self.num_cpus, \
-                f"Detected model level cpu requirement = {user_cpu_per_job} > total cpu granted to the bagged model = {self.num_cpus}"
-            assert user_cpu_per_job >= minimum_model_num_cpus, \
-                f"Detected model level cpu requirement = {user_cpu_per_job} < minimum cpu required by the model = {minimum_model_num_cpus}"
-            user_resources_per_job['num_cpus'] = user_cpu_per_job
-        if user_gpu_per_job is not None: 
-            assert user_gpu_per_job <= self.num_gpus, \
-                f"Detected model level gpu requirement = {user_gpu_per_job} > total gpu granted to the bagged model = {self.num_gpus}"
-            assert user_gpu_per_job >= minimum_model_num_gpus, \
-                f"Detected model level gpu requirement = {user_gpu_per_job} < minimum gpu required by the model = {minimum_model_num_gpus}"
-            user_resources_per_job['num_gpus'] = user_gpu_per_job
+            assert (
+                user_cpu_per_job <= self.num_cpus
+            ), f"Detected model level cpu requirement = {user_cpu_per_job} > total cpu granted to the bagged model = {self.num_cpus}"
+            assert (
+                user_cpu_per_job >= minimum_model_num_cpus
+            ), f"Detected model level cpu requirement = {user_cpu_per_job} < minimum cpu required by the model = {minimum_model_num_cpus}"
+            user_resources_per_job["num_cpus"] = user_cpu_per_job
+        if user_gpu_per_job is not None:
+            assert (
+                user_gpu_per_job <= self.num_gpus
+            ), f"Detected model level gpu requirement = {user_gpu_per_job} > total gpu granted to the bagged model = {self.num_gpus}"
+            assert (
+                user_gpu_per_job >= minimum_model_num_gpus
+            ), f"Detected model level gpu requirement = {user_gpu_per_job} < minimum gpu required by the model = {minimum_model_num_gpus}"
+            user_resources_per_job["num_gpus"] = user_gpu_per_job
         self.user_ensemble_resources = user_ensemble_resources
         self.user_resources_per_job = user_resources_per_job
 
     def _get_fold_time_limit(self, fold_ctx):
         _, folds_finished, folds_left, folds_to_fit, _, _ = self._get_fold_properties(fold_ctx)
         time_elapsed = time.time() - self.time_start
         if self.time_limit is not None:
@@ -215,30 +234,29 @@
             if time_left <= 0:
                 raise TimeLimitExceeded
         else:
             time_limit_fold = None
         return time_limit_fold
 
     def _update_bagged_ensemble(self, fold_model, pred_proba, fold_ctx):
-        _, val_index = fold_ctx['fold']
+        _, val_index = fold_ctx["fold"]
         model_to_append = fold_model
         if not self.save_folds:
             fold_model.model = None
         if self.bagged_ensemble_model.low_memory:
             self.bagged_ensemble_model.save_child(fold_model, verbose=False)
             model_to_append = fold_model.name
         self.models.append(model_to_append)
         self.oof_pred_proba[val_index] += pred_proba
         self.oof_pred_model_repeats[val_index] += 1
         self.bagged_ensemble_model._add_child_times_to_bag(model=fold_model)
 
     def _predict_oof(self, fold_model, fold_ctx):
         time_train_end_fold = time.time()
-        fold, folds_finished, folds_left, \
-            folds_to_fit, is_last_fold, model_name_suffix = self._get_fold_properties(fold_ctx)
+        fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = self._get_fold_properties(fold_ctx)
         _, val_index = fold
         X_val_fold = self.X.iloc[val_index, :]
         y_val_fold = self.y.iloc[val_index]
         # Check to avoid unnecessarily predicting and saving a model
         # when an Exception is going to be raised later
         if self.time_limit is not None:
             if not is_last_fold:
@@ -246,47 +264,47 @@
                 time_left = self.time_limit - time_elapsed
                 expected_time_required = time_elapsed * folds_to_fit / (folds_finished + 1)
                 expected_remaining_time_required = expected_time_required * (folds_left - 1) / folds_to_fit
                 if expected_remaining_time_required > time_left:
                     raise TimeLimitExceeded
         pred_proba = fold_model.predict_proba(X_val_fold)
         fold_model.predict_time = time.time() - time_train_end_fold
-        fold_model.val_score = fold_model.score_with_y_pred_proba(y=y_val_fold,
-                                                                  y_pred_proba=pred_proba)
+        fold_model.val_score = fold_model.score_with_y_pred_proba(y=y_val_fold, y_pred_proba=pred_proba)
         fold_model.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
-        if not self.bagged_ensemble_model.params.get('save_bag_folds', True):
+        if not self.bagged_ensemble_model.params.get("save_bag_folds", True):
             fold_model.model = None
         return fold_model, pred_proba
 
     @staticmethod
     def _get_fold_properties(fold_ctx):
-        fold, folds_finished, folds_left, \
-            folds_to_fit, is_last_fold, model_name_suffix = [
-                fold_ctx[f] for f in ['fold', 'folds_finished', 'folds_left', 'folds_to_fit', 'is_last_fold', 'model_name_suffix']]
+        fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = [
+            fold_ctx[f] for f in ["fold", "folds_finished", "folds_left", "folds_to_fit", "is_last_fold", "model_name_suffix"]
+        ]
         return fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix
 
 
 class SequentialLocalFoldFittingStrategy(FoldFittingStrategy):
     """
     This strategy fits the folds locally in a sequence.
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         if self.user_ensemble_resources is None:
             if self.user_resources_per_job is None:
                 self.num_cpus, self.num_gpus = self.model_base._get_default_resources()
             else:
-                self.num_cpus = self.user_resources_per_job.get('num_cpus', self.num_cpus)
-                self.num_gpus = self.user_resources_per_job.get('num_gpus', self.num_gpus)
+                self.num_cpus = self.user_resources_per_job.get("num_cpus", self.num_cpus)
+                self.num_gpus = self.user_resources_per_job.get("num_gpus", self.num_gpus)
         else:
             if self.user_resources_per_job is not None:
-                self.num_cpus = self.user_resources_per_job.get('num_cpus', self.num_cpus)
-                self.num_gpus = self.user_resources_per_job.get('num_gpus', self.num_gpus)
-        self.resources = {'num_cpus': self.num_cpus, 'num_gpus': self.num_gpus}
-        
+                self.num_cpus = self.user_resources_per_job.get("num_cpus", self.num_cpus)
+                self.num_gpus = self.user_resources_per_job.get("num_gpus", self.num_gpus)
+        self.resources = {"num_cpus": self.num_cpus, "num_gpus": self.num_gpus}
+
     def schedule_fold_model_fit(self, fold_ctx):
         self.jobs.append(fold_ctx)
 
     def after_all_folds_scheduled(self):
         for job in self.jobs:
             self._fit_fold_model(job)
 
@@ -299,139 +317,119 @@
 
     def _fit(self, model_base, time_start_fold, time_limit_fold, fold_ctx, kwargs):
         fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = self._get_fold_properties(fold_ctx)
         train_index, val_index = fold
         X_fold, X_val_fold = self.X.iloc[train_index, :], self.X.iloc[val_index, :]
         y_fold, y_val_fold = self.y.iloc[train_index], self.y.iloc[val_index]
         fold_model = copy.deepcopy(model_base)
-        fold_model.name = f'{fold_model.name}{model_name_suffix}'
+        fold_model.name = f"{fold_model.name}{model_name_suffix}"
         fold_model.set_contexts(self.bagged_ensemble_model.path + fold_model.name + os.path.sep)
         kwargs_fold = kwargs.copy()
         is_pseudo = self.X_pseudo is not None and self.y_pseudo is not None
         if self.sample_weight is not None:
-            kwargs_fold['sample_weight'] = self.sample_weight[train_index]
-            kwargs_fold['sample_weight_val'] = self.sample_weight[val_index]
+            kwargs_fold["sample_weight"] = self.sample_weight[train_index]
+            kwargs_fold["sample_weight_val"] = self.sample_weight[val_index]
 
             if is_pseudo:
                 # TODO: Add support for sample_weight when pseudo is present
-                raise Exception('Sample weights given, but not used due to pseudo labelled data being given.')
+                raise Exception("Sample weights given, but not used due to pseudo labelled data being given.")
             else:
-                kwargs_fold['sample_weight'] = self.sample_weight[train_index]
-                kwargs_fold['sample_weight_val'] = self.sample_weight[val_index]
+                kwargs_fold["sample_weight"] = self.sample_weight[train_index]
+                kwargs_fold["sample_weight_val"] = self.sample_weight[val_index]
 
         if is_pseudo:
-            logger.log(15, f'{len(self.X_pseudo)} extra rows of pseudolabeled data added to training set for {fold_model.name}')
+            logger.log(15, f"{len(self.X_pseudo)} extra rows of pseudolabeled data added to training set for {fold_model.name}")
             X_fold = pd.concat([X_fold, self.X_pseudo], axis=0, ignore_index=True)
             y_fold = pd.concat([y_fold, self.y_pseudo], axis=0, ignore_index=True)
 
         num_cpus = self.num_cpus
         num_gpus = self.num_gpus
         if self.user_resources_per_job is not None:
-            num_cpus = min(self.num_cpus, self.user_resources_per_job.get('num_cpus', math.inf))
-            num_gpus = min(self.num_gpus, self.user_resources_per_job.get('num_gpus', math.inf))
-        fold_model.fit(
-            X=X_fold,
-            y=y_fold,
-            X_val=X_val_fold,
-            y_val=y_val_fold,
-            time_limit=time_limit_fold,
-            num_cpus=num_cpus,
-            num_gpus=num_gpus,
-            **kwargs_fold
-        )
+            num_cpus = min(self.num_cpus, self.user_resources_per_job.get("num_cpus", math.inf))
+            num_gpus = min(self.num_gpus, self.user_resources_per_job.get("num_gpus", math.inf))
+        fold_model.fit(X=X_fold, y=y_fold, X_val=X_val_fold, y_val=y_val_fold, time_limit=time_limit_fold, num_cpus=num_cpus, num_gpus=num_gpus, **kwargs_fold)
         fold_model.fit_time = time.time() - time_start_fold
         return fold_model
 
 
 def _ray_fit(
     *,
     model_base: AbstractModel,
     bagged_ensemble_model_path: str,
     X: Union[str, pd.DataFrame],
     y: Union[str, pd.DataFrame],
     X_pseudo: Union[str, pd.DataFrame],
     y_pseudo: Union[str, pd.DataFrame],
     fold_ctx: Dict[str, Any],
     time_limit_fold: float,
-    save_bag_folds: bool, 
+    save_bag_folds: bool,
     resources: Dict[str, Any],
     kwargs_fold: Dict[str, Any],
     head_node_id: str,
-    model_sync_path: Optional[str] = None
+    model_sync_path: Optional[str] = None,
 ):
     import ray  # ray must be present
+
     node_id = ray.get_runtime_context().get_node_id()
     is_head_node = node_id == head_node_id
     logger.debug(f"head node: {is_head_node}")
     logger.debug(f"executing fold on node {node_id}")
-    logger.log(10, 'ray worker training')
+    logger.log(10, "ray worker training")
     time_start_fold = time.time()
-    fold, folds_finished, folds_left, \
-        folds_to_fit, is_last_fold, \
-        model_name_suffix = FoldFittingStrategy._get_fold_properties(fold_ctx)
+    fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = FoldFittingStrategy._get_fold_properties(fold_ctx)
     train_index, val_index = fold
     fold_model = copy.deepcopy(model_base)
-    fold_model.name = f'{fold_model.name}{model_name_suffix}'
+    fold_model.name = f"{fold_model.name}{model_name_suffix}"
     fold_model_local_save_path = bagged_ensemble_model_path + fold_model.name + os.path.sep
     fold_model.set_contexts(fold_model_local_save_path)
     if type(X) == str and type(y) == str:
-        with open(X, 'rb') as X_f, open(y, 'rb') as y_f:
+        with open(X, "rb") as X_f, open(y, "rb") as y_f:
             X = pickle.load(X_f)
             y = pickle.load(y_f)
     is_pseudo = False
     if X_pseudo is not None and y_pseudo is not None:
         if type(X_pseudo) == str and type(y_pseudo) == str:
-            with open(X_pseudo, 'rb') as X_pseudo_f, open(y_pseudo, 'rb') as y_pseudo_f:
+            with open(X_pseudo, "rb") as X_pseudo_f, open(y_pseudo, "rb") as y_pseudo_f:
                 X_pseudo = pickle.load(X_pseudo_f)
                 y_pseudo = pickle.load(y_pseudo_f)
         is_pseudo = True
 
     X_fold, X_val_fold = X.iloc[train_index, :], X.iloc[val_index, :]
     y_fold, y_val_fold = y.iloc[train_index], y.iloc[val_index]
     if is_pseudo:
-            logger.log(15, f'{len(X_pseudo)} extra rows of pseudolabeled data added to training set for {fold_model.name}')
-            X_fold = pd.concat([X_fold, X_pseudo], axis=0, ignore_index=True)
-            y_fold = pd.concat([y_fold, y_pseudo], axis=0, ignore_index=True)
-    fold_model.fit(X=X_fold, y=y_fold, X_val=X_val_fold, y_val=y_val_fold,
-                   time_limit=time_limit_fold, **resources, **kwargs_fold)
+        logger.log(15, f"{len(X_pseudo)} extra rows of pseudolabeled data added to training set for {fold_model.name}")
+        X_fold = pd.concat([X_fold, X_pseudo], axis=0, ignore_index=True)
+        y_fold = pd.concat([y_fold, y_pseudo], axis=0, ignore_index=True)
+    fold_model.fit(X=X_fold, y=y_fold, X_val=X_val_fold, y_val=y_val_fold, time_limit=time_limit_fold, **resources, **kwargs_fold)
     time_train_end_fold = time.time()
     fold_model.fit_time = time_train_end_fold - time_start_fold
-    fold_model, pred_proba = _ray_predict_oof(fold_model, X_val_fold, y_val_fold,
-                                              time_train_end_fold, resources['num_cpus'], save_bag_folds)
+    fold_model, pred_proba = _ray_predict_oof(fold_model, X_val_fold, y_val_fold, time_train_end_fold, resources["num_cpus"], save_bag_folds)
     save_path = fold_model.save()
     if model_sync_path is not None and not is_head_node:
         model_sync_path = model_sync_path + f"{fold_model.name}/"  # s3 path hence need "/" as the saperator
         bucket, prefix = s3_path_to_bucket_prefix(model_sync_path)
-        upload_s3_folder(
-            bucket=bucket,
-            prefix=prefix,
-            folder_to_upload=save_path,
-            verbose=False
-        )
-    return fold_model.name, pred_proba, time_start_fold, \
-        time_train_end_fold, fold_model.predict_time, fold_model.predict_1_time
+        upload_s3_folder(bucket=bucket, prefix=prefix, folder_to_upload=save_path, verbose=False)
+    return fold_model.name, pred_proba, time_start_fold, time_train_end_fold, fold_model.predict_time, fold_model.predict_1_time
 
 
-def _ray_predict_oof(fold_model, X_val_fold, y_val_fold, time_train_end_fold,
-                     num_cpus=-1, save_bag_folds=True):
+def _ray_predict_oof(fold_model, X_val_fold, y_val_fold, time_train_end_fold, num_cpus=-1, save_bag_folds=True):
     pred_proba = fold_model.predict_proba(X_val_fold, num_cpus=num_cpus)
     time_pred_end_fold = time.time()
     fold_model.predict_time = time_pred_end_fold - time_train_end_fold
-    fold_model.val_score = fold_model.score_with_y_pred_proba(y=y_val_fold,
-                                                              y_pred_proba=pred_proba)
+    fold_model.val_score = fold_model.score_with_y_pred_proba(y=y_val_fold, y_pred_proba=pred_proba)
     fold_model.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
     if not save_bag_folds:
         fold_model.model = None
     return fold_model, pred_proba
 
 
 class ParallelFoldFittingStrategy(FoldFittingStrategy):
     """
     An implementation of FoldFittingStrategy to train multiple folds in parallel.
-    Folds are spread to cpu/gpu cores by ray tasks. 
+    Folds are spread to cpu/gpu cores by ray tasks.
     Large data are stored in ray object store, which minimizes memory usage and unessary serializations.
     Trained models are saved to disk within each ray task.
 
     Parameters
     ----------
         num_folds_parallel: int
             Number of folds to train in parallel at once.
@@ -458,68 +456,55 @@
         time_end_fit: float
             The time of the last model finishes training.
         fit_time: float
             The amount of time used to fit all folds.
         predict_time: float
             The amount of time used to do out of folds predictions for all folds.
     """
-    def __init__(
-        self,
-        *,
-        num_jobs: int,
-        num_folds_parallel: int,
-        max_memory_usage_ratio: float = 0.8,
-        model_sync_path: Optional[str] = None,
-        **kwargs
-    ):
+
+    def __init__(self, *, num_jobs: int, num_folds_parallel: int, max_memory_usage_ratio: float = 0.8, model_sync_path: Optional[str] = None, **kwargs):
         super().__init__(**kwargs)
         self.ray = try_import_ray()
         self.max_memory_usage_ratio = min(max_memory_usage_ratio, 1.0)
         self.model_sync_path = model_sync_path
         self.time_start_fit = None
         self.time_end_fit = None
         self.fit_time = 0
         self.predict_time = 0
         self.predict_1_time = None
         # max_calls to guarantee release of gpu resource
         self._ray_fit = self.ray.remote(max_calls=1)(_ray_fit)
         self.resources, self.batches, self.num_parallel_jobs = self._get_resource_suggestions(
-            num_jobs=num_jobs,
-            user_specified_num_folds_parallel=num_folds_parallel,
-            user_resources_per_job=self.user_resources_per_job
+            num_jobs=num_jobs, user_specified_num_folds_parallel=num_folds_parallel, user_resources_per_job=self.user_resources_per_job
         )
 
     @disable_if_lite_mode(ret=True)
     def is_mem_sufficient(self):
-        '''Check if the memory is sufficient to do parallel training'''
+        """Check if the memory is sufficient to do parallel training"""
         model_mem_est = self._initialized_model_base.estimate_memory_usage(X=self.X)
         total_model_mem_est = self.num_parallel_jobs * model_mem_est
         data_mem_est = self._estimate_data_memory_usage()
         total_data_mem_est = self.num_parallel_jobs * data_mem_est
         mem_available = ResourceManager.get_available_virtual_mem()
         return (mem_available * self.max_memory_usage_ratio) > (total_model_mem_est + total_data_mem_est)
 
     def _estimate_data_memory_usage(self):
         X_mem = get_approximate_df_mem_usage(self.X).sum()
         y_mem = get_approximate_df_mem_usage(self.y.to_frame()).sum()
         return X_mem + y_mem
 
     def schedule_fold_model_fit(self, fold_ctx):
         self.jobs.append(fold_ctx)
-        
+
     def _get_ray_init_args(self) -> Dict[str, Any]:
         """
         Get the arguments needed to init ray runtime.
         This could differ in different context, i.e. distributed vs local
         """
-        return dict(
-            address="auto",
-            logging_level=logging.ERROR,
-            log_to_driver=False
-        )
+        return dict(address="auto", logging_level=logging.ERROR, log_to_driver=False)
 
     def after_all_folds_scheduled(self):
         if not self.ray.is_initialized():
             ray_init_args = self._get_ray_init_args()
             self.ray.init(**ray_init_args)
         head_node_id = self.ray.get_runtime_context().get_node_id()
         logger.debug(f"Dispatching folds on node {head_node_id}")
@@ -538,59 +523,57 @@
                 y_ref=y,
                 X_pseudo_ref=X_pseudo,
                 y_pseudo_ref=y_pseudo,
                 time_limit_fold=time_limit_fold,
                 fold_ctx=fold_ctx,
                 resources=self.resources,
                 head_node_id=head_node_id,
-                kwargs=self.model_base_kwargs
+                kwargs=self.model_base_kwargs,
             )
             job_fold_map[ref] = fold_ctx
             job_refs.append(ref)
 
         # update ensemble whenever a model return
         unfinished = job_refs
         while unfinished:
             finished, unfinished = self.ray.wait(unfinished, num_returns=1)
             finished = finished[0]
             try:
-                fold_model, pred_proba, time_start_fit, \
-                    time_end_fit, predict_time, predict_1_time = self.ray.get(finished)
+                fold_model, pred_proba, time_start_fit, time_end_fit, predict_time, predict_1_time = self.ray.get(finished)
                 fold_ctx = job_fold_map.get(finished, None)
                 assert fold_ctx is not None
-                self._update_bagged_ensemble(fold_model=fold_model,
-                                             pred_proba=pred_proba,
-                                             time_start_fit=time_start_fit,
-                                             time_end_fit=time_end_fit,
-                                             predict_time=predict_time,
-                                             predict_1_time=predict_1_time,
-                                             fold_ctx=fold_ctx)
+                self._update_bagged_ensemble(
+                    fold_model=fold_model,
+                    pred_proba=pred_proba,
+                    time_start_fit=time_start_fit,
+                    time_end_fit=time_end_fit,
+                    predict_time=predict_time,
+                    predict_1_time=predict_1_time,
+                    fold_ctx=fold_ctx,
+                )
                 model_sync_path = None
                 if self.model_sync_path is not None:
                     model_sync_path: str = self.model_sync_path + fold_model
                     if not model_sync_path.endswith("/"):
                         model_sync_path += "/"
-                self.sync_model_artifact(
-                    local_path=os.path.join(self.bagged_ensemble_model.path + fold_model),
-                    model_sync_path=model_sync_path
-                )
+                self.sync_model_artifact(local_path=os.path.join(self.bagged_ensemble_model.path + fold_model), model_sync_path=model_sync_path)
             except TimeLimitExceeded:
                 # Terminate all ray tasks because a fold failed
                 self.terminate_all_unfinished_tasks(unfinished)
                 raise TimeLimitExceeded
             # NotEnoughMemoryError is an autogluon custom error,
             # it predict memory usage before hand
             # MemoryError is the actual python memory error if the process failed
             except (NotEnoughMemoryError, MemoryError):
-                error_msg = 'Consider decrease folds trained in parallel \
+                error_msg = "Consider decrease folds trained in parallel \
                              by passing num_fold_parallel to ag_args_ensemble \
                              when calling tabular.fit.\n\
                              If none working, use sequential folding by passing \
                              SequentialLocalFoldFittingStrategy to ag_args_ensemble \
-                             when calling tabular.fit and try again.'
+                             when calling tabular.fit and try again."
                 logger.warning(error_msg)
                 # Terminate all ray tasks because a fold failed
                 self.terminate_all_unfinished_tasks(unfinished)
                 raise NotEnoughMemoryError
             except Exception as e:
                 processed_exception = self._parse_ray_error(e)
                 # Terminate all ray tasks because a fold failed
@@ -601,68 +584,50 @@
             self.fit_time = self.time_end_fit - self.time_start_fit
         self.bagged_ensemble_model._add_parallel_child_times(fit_time=self.fit_time, predict_time=self.predict_time, predict_1_time=self.predict_1_time)
 
     def terminate_all_unfinished_tasks(self, unfinished_tasks):
         for task in unfinished_tasks:
             self.ray.cancel(task, force=True)
 
-    def _fit(
-        self,
-        *,
-        model_base_ref,
-        X_ref,
-        y_ref,
-        X_pseudo_ref,
-        y_pseudo_ref,
-        time_limit_fold,
-        fold_ctx,
-        resources,
-        head_node_id,
-        kwargs
-    ):
-        fold, folds_finished, folds_left, \
-            folds_to_fit, is_last_fold, \
-            model_name_suffix = self._get_fold_properties(fold_ctx)
-        logger.debug(f'Folding resources per job {resources}')
+    def _fit(self, *, model_base_ref, X_ref, y_ref, X_pseudo_ref, y_pseudo_ref, time_limit_fold, fold_ctx, resources, head_node_id, kwargs):
+        fold, folds_finished, folds_left, folds_to_fit, is_last_fold, model_name_suffix = self._get_fold_properties(fold_ctx)
+        logger.debug(f"Folding resources per job {resources}")
         train_index, val_index = fold
         fold_ctx_ref = self.ray.put(fold_ctx)
         save_bag_folds = self.save_folds
         kwargs_fold = kwargs.copy()
         is_pseudo = X_pseudo_ref is not None and y_pseudo_ref is not None
         if self.sample_weight is not None:
             if is_pseudo:
                 # TODO: Add support for sample_weight when pseudo is present
-                raise Exception('Sample weights given, but not used due to pseudo labelled data being given.')
+                raise Exception("Sample weights given, but not used due to pseudo labelled data being given.")
             else:
-                kwargs_fold['sample_weight'] = self.sample_weight[train_index]
-                kwargs_fold['sample_weight_val'] = self.sample_weight[val_index]
+                kwargs_fold["sample_weight"] = self.sample_weight[train_index]
+                kwargs_fold["sample_weight_val"] = self.sample_weight[val_index]
         pg = self.ray.util.get_current_placement_group()
         return self._ray_fit.options(
-            **resources,
-            scheduling_strategy=self.ray.util.scheduling_strategies.PlacementGroupSchedulingStrategy(
-                placement_group=pg
-            )).remote(
-                model_base=model_base_ref,
-                bagged_ensemble_model_path=self.bagged_ensemble_model.path,
-                X=X_ref,
-                y=y_ref,
-                X_pseudo=X_pseudo_ref,
-                y_pseudo=y_pseudo_ref,
-                fold_ctx=fold_ctx_ref,
-                time_limit_fold=time_limit_fold,
-                save_bag_folds=save_bag_folds,
-                resources=resources,
-                kwargs_fold=kwargs_fold,
-                head_node_id=head_node_id,
-                model_sync_path=self.model_sync_path
-            )
+            **resources, scheduling_strategy=self.ray.util.scheduling_strategies.PlacementGroupSchedulingStrategy(placement_group=pg)
+        ).remote(
+            model_base=model_base_ref,
+            bagged_ensemble_model_path=self.bagged_ensemble_model.path,
+            X=X_ref,
+            y=y_ref,
+            X_pseudo=X_pseudo_ref,
+            y_pseudo=y_pseudo_ref,
+            fold_ctx=fold_ctx_ref,
+            time_limit_fold=time_limit_fold,
+            save_bag_folds=save_bag_folds,
+            resources=resources,
+            kwargs_fold=kwargs_fold,
+            head_node_id=head_node_id,
+            model_sync_path=self.model_sync_path,
+        )
 
-    def _update_bagged_ensemble(self, fold_model, pred_proba, time_start_fit,
-                                time_end_fit, predict_time, predict_1_time, fold_ctx):
-        _, val_index = fold_ctx['fold']
+    def _update_bagged_ensemble(self, fold_model, pred_proba, time_start_fit, time_end_fit, predict_time, predict_1_time, fold_ctx):
+        _, val_index = fold_ctx["fold"]
         self.models.append(fold_model)
         self.oof_pred_proba[val_index] += pred_proba
         self.oof_pred_model_repeats[val_index] += 1
         if self.time_start_fit:
             self.time_start_fit = min(time_start_fit, self.time_start_fit)
         else:
             self.time_start_fit = time_start_fit
@@ -684,165 +649,144 @@
             time_limit_fold = required_time_per_fold * self.time_limit_fold_ratio
             if time_left <= 0:
                 raise TimeLimitExceeded
         else:
             time_limit_fold = None
         return time_limit_fold
 
-    def _get_resource_suggestions(
-        self,
-        num_jobs,
-        user_specified_num_folds_parallel,
-        user_resources_per_job
-    ):  
+    def _get_resource_suggestions(self, num_jobs, user_specified_num_folds_parallel, user_resources_per_job):
         """
         Get resources per job, number of total batches, and number of jobs running in parallel for a single batch
         based on total number of jobs, user specified number of jobs to be run in parallel, and user specified resources per job.
         When user specified resources per job, will validate and force this value if legit.
         Otherwise, will try to run as many jobs in parallel as possible respecting the minimum resources required per job.
         """
         user_specified_num_folds_parallel = min(num_jobs, user_specified_num_folds_parallel)
-        model_min_resources = self._initialized_model_base.get_minimum_resources(
-            is_gpu_available=(self.num_gpus > 0)
-        )
-        resources_calculator = ResourceCalculatorFactory.get_resource_calculator(calculator_type='cpu' if self.num_gpus == 0 else 'gpu')
+        model_min_resources = self._initialized_model_base.get_minimum_resources(is_gpu_available=(self.num_gpus > 0))
+        resources_calculator = ResourceCalculatorFactory.get_resource_calculator(calculator_type="cpu" if self.num_gpus == 0 else "gpu")
         # use minimum resource to control number of jobs running in parallel
         min_cpu_per_job_based_on_num_folds_parallel = self.num_cpus // user_specified_num_folds_parallel
         min_gpu_per_job_based_on_num_folds_parallel = self.num_gpus / user_specified_num_folds_parallel
-        min_cpu_based_on_model = model_min_resources.get('num_cpus', 1)
-        min_gpu_based_on_model = model_min_resources.get('num_gpus', 0)
-        
+        min_cpu_based_on_model = model_min_resources.get("num_cpus", 1)
+        min_gpu_based_on_model = model_min_resources.get("num_gpus", 0)
+
         get_resources_per_job_args = dict(
             total_num_cpus=self.num_cpus,
             total_num_gpus=self.num_gpus,
             num_jobs=num_jobs,
             minimum_cpu_per_job=max(min_cpu_per_job_based_on_num_folds_parallel, min_cpu_based_on_model),
             minimum_gpu_per_job=max(min_gpu_per_job_based_on_num_folds_parallel, min_gpu_based_on_model),
-            user_resources_per_job=user_resources_per_job
+            user_resources_per_job=user_resources_per_job,
         )
         if user_resources_per_job is not None:
-            get_resources_per_job_args['minimum_cpu_per_job'] = min_cpu_based_on_model
-            get_resources_per_job_args['minimum_gpu_per_job'] = min_gpu_based_on_model
+            get_resources_per_job_args["minimum_cpu_per_job"] = min_cpu_based_on_model
+            get_resources_per_job_args["minimum_gpu_per_job"] = min_gpu_based_on_model
 
-        resources_info = resources_calculator.get_resources_per_job(
-            **get_resources_per_job_args
-        )
-        resources = resources_info.get('resources_per_job')
-        if 'num_gpus' not in resources:
-            resources['num_gpus'] = 0
-        num_parallel_jobs = resources_info.get('num_parallel_jobs')
-        batches = resources_info.get('batches')
+        resources_info = resources_calculator.get_resources_per_job(**get_resources_per_job_args)
+        resources = resources_info.get("resources_per_job")
+        if "num_gpus" not in resources:
+            resources["num_gpus"] = 0
+        num_parallel_jobs = resources_info.get("num_parallel_jobs")
+        batches = resources_info.get("batches")
 
         # renname key to match ray job requirement
-        resources['num_cpus'] = resources.pop('cpu')
-        num_gpus = resources.pop('gpu', None)
+        resources["num_cpus"] = resources.pop("cpu")
+        num_gpus = resources.pop("gpu", None)
         if num_gpus is not None and num_gpus > 0:
-            resources['num_gpus'] = num_gpus
+            resources["num_gpus"] = num_gpus
 
         return resources, batches, num_parallel_jobs
 
     def _prepare_data(self, in_mem=True):
         X_pseudo = None
         y_pseudo = None
         if in_mem:
             X = self.ray.put(self.X)
             y = self.ray.put(self.y)
             if self.X_pseudo is not None and self.y_pseudo is not None:
                 X_pseudo = self.ray.put(self.X_pseudo)
                 y_pseudo = self.ray.put(self.y_pseudo)
         else:
-            X = 'X.pkl'
-            y = 'y.pkl'
-            utils = 'utils'
+            X = "X.pkl"
+            y = "y.pkl"
+            utils = "utils"
             X = os.path.join(self.bagged_ensemble_model.path, utils, X)
             y = os.path.join(self.bagged_ensemble_model.path, utils, y)
-            with open(X, 'wb') as X_f, open(y, 'wb') as y_f:
+            with open(X, "wb") as X_f, open(y, "wb") as y_f:
                 pickle.dump(self.X, X_f)
                 pickle.dump(self.y, y_f)
             if self.X_pseudo is not None and self.y_pseudo is not None:
-                X_pseudo = 'X_pseudo.pkl'
-                y_pseudo = 'y_pseudo.pkl'
+                X_pseudo = "X_pseudo.pkl"
+                y_pseudo = "y_pseudo.pkl"
                 X_pseudo = os.path.join(self.bagged_ensemble_model.path, utils, X_pseudo)
                 y_pseudo = os.path.join(self.bagged_ensemble_model.path, utils, y_pseudo)
         return X, y, X_pseudo, y_pseudo
 
     def _parse_ray_error(self, e):
         error = str(e).lower()
-        if 'cuda' in error and ('out of memory' in error or 'alloc' in error):
-            default_error_msg = 'If none working, use sequential folding by passing \
+        if "cuda" in error and ("out of memory" in error or "alloc" in error):
+            default_error_msg = "If none working, use sequential folding by passing \
                          SequentialLocalFoldFittingStrategy to ag_args_ensemble \
-                         when calling tabular.fit and try again.'
+                         when calling tabular.fit and try again."
             # FIXME: Avoid hardcoding model names.
             if self.model_base.__class__.__name__ in [TEXT_MODEL, IMAGE_MODEL]:
-                error_msg = f'Out of CUDA memory while training \
+                error_msg = f"Out of CUDA memory while training \
                             {self.model_base.__class__.__name__}. \
                             Consider decrease batch size in hyperparameter and try again.\n\
                             Or decrease folds trained in parallel by passing num_fold_parallel \
                             to ag_args_ensemble when calling tabular.fit if you have multiple \
-                            gpus and try again'
+                            gpus and try again"
                 logger.warning(error_msg)
             # FIXME: Avoid hardcoding model names.
             elif self.model_base.__class__.__name__ in [TABULAR_TORCH_MODEL, TABULAR_FASTAI_MODEL]:
-                error_msg = f'Out of CUDA memory while training \
+                error_msg = f"Out of CUDA memory while training \
                             {self.model_base.__class__.__name__}. \
                             Consider decrease batch size in hyperparameter and try again.\n\
                             Or decrease folds trained in parallel by passing num_fold_parallel \
-                            to ag_args_ensemble when calling tabular.fit and try again'
+                            to ag_args_ensemble when calling tabular.fit and try again"
                 logger.warning(error_msg)
             else:
-                error_msg = f'Out of CUDA memory while training \
+                error_msg = f"Out of CUDA memory while training \
                             {self.model_base.__class__.__name__}. \
                             Consider decrease folds trained in parallel by passing \
                             num_fold_parallel to ag_args_ensemble when calling tabular.fit \
-                            and try again'
+                            and try again"
                 logger.warning(error_msg)
             logger.warning(default_error_msg)
             e = NotEnoughCudaMemoryError
         return e
-    
+
     def sync_model_artifact(self, local_path: str, model_sync_path: str):
         """
         Sync model artifacts being uploaded to `model_sync_path` to `local_path`
         This method is expected to be called on the head node in the cluster to collect model artifacts after training
-        
+
         Parameters
         ----------
         local_path: str
             local path to download artifacts
         model_sync_path: str
             remote path to download model artifacts from
         """
         self._sync_model_artifact(local_path=local_path, model_sync_path=model_sync_path)
-    
+
     def _sync_model_artifact(self, **kwargs):
         pass
-    
-    
+
+
 class ParallelLocalFoldFittingStrategy(ParallelFoldFittingStrategy):
-    
     def _get_ray_init_args(self):
-        ray_init_args = dict(
-            log_to_driver=False,
-            logging_level=logging.ERROR,
-            num_cpus=self.num_cpus
-        )
+        ray_init_args = dict(log_to_driver=False, logging_level=logging.ERROR, num_cpus=self.num_cpus)
         if self.num_gpus > 0:
-            ray_init_args['num_gpus'] = self.num_gpus
+            ray_init_args["num_gpus"] = self.num_gpus
         return ray_init_args
 
-    
+
 class ParallelDistributedFoldFittingStrategy(ParallelFoldFittingStrategy):
-    
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         # Append bag model name in the path
         self.model_sync_path = self.model_sync_path + os.path.basename(os.path.normpath(self.bagged_ensemble_model.path)) + "/"
 
     def _sync_model_artifact(self, local_path, model_sync_path):
         bucket, path = s3_path_to_bucket_prefix(model_sync_path)
-        download_s3_folder(
-            bucket=bucket,
-            prefix=path,
-            local_path=local_path,
-            error_if_exists=False,
-            verbose=False
-        )
+        download_s3_folder(bucket=bucket, prefix=path, local_path=local_path, error_if_exists=False, verbose=False)
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/ray_parallel_fold_fitting_strategy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,56 @@
+import time
+
 import ray
 from numpy import ndarray
 from pandas import DataFrame, Series
 from ray.util import placement_group, placement_group_table
-import time
 
 from autogluon.core.models.ensemble.fold_fitting_strategy import SequentialLocalFoldFittingStrategy
 
 
 @ray.remote
 def model_fit_task_ray(X_fold, X_val_fold, fold_model, kwargs_fold, time_limit_fold, y_fold, y_val_fold):
     fold_model.fit(X=X_fold, y=y_fold, X_val=X_val_fold, y_val=y_val_fold, time_limit=time_limit_fold, **kwargs_fold)
     time_train_end_fold = time.time()
     return fold_model, time_train_end_fold
 
-class RayParallelFitter(SequentialLocalFoldFittingStrategy):
 
-    def __init__(self, bagged_ensemble_model, X: DataFrame, y: Series, sample_weight, time_limit: float, time_start: float, models: list, oof_pred_proba: ndarray, oof_pred_model_repeats: ndarray, save_folds: bool):
+class RayParallelFitter(SequentialLocalFoldFittingStrategy):
+    def __init__(
+        self,
+        bagged_ensemble_model,
+        X: DataFrame,
+        y: Series,
+        sample_weight,
+        time_limit: float,
+        time_start: float,
+        models: list,
+        oof_pred_proba: ndarray,
+        oof_pred_model_repeats: ndarray,
+        save_folds: bool,
+    ):
         super().__init__(bagged_ensemble_model, X, y, sample_weight, time_limit, time_start, models, oof_pred_proba, oof_pred_model_repeats, save_folds)
         # ray.util.connect("localhost:10001")
         # ray.init(address='auto')
-        print('init')
+        print("init")
         ray.init()
 
     def schedule_fold_model_fit(self, model_base, fold_ctx, kwargs):
         args = [model_base, fold_ctx, kwargs]
         args_refs = [ray.put(arg) for arg in args]
-        print('...model_fit')
+        print("...model_fit")
 
         pg = placement_group([{"CPU": 2}], strategy="STRICT_SPREAD")
         ray.get(pg.ready())
         print(placement_group_table(pg))
         results_ref = model_fit_task_ray.options(placement_group=pg).remote(*args_refs)
         self.jobs.append((results_ref, time_start_fold, on_fit_end_fn))
 
     def wait_for_completion(self):
-        print('...wait')
+        print("...wait")
         for (results_ref, time_start_fold, on_fit_end_fn) in self.jobs:
             fold_model, time_train_end_fold = ray.get(results_ref)
-            print(f'{fold_model} | {time_train_end_fold}')
+            print(f"{fold_model} | {time_train_end_fold}")
             on_fit_end_fn(fold_model, time_train_end_fold, time_start_fold)
 
         ray.shutdown()
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/stacker_ensemble_model.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/stacker_ensemble_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import copy
 import logging
 import os
 import time
-from typing import Dict
-
 from collections import defaultdict
+from typing import Dict
 
 import numpy as np
 import pandas as pd
 
 from autogluon.common.features.feature_metadata import FeatureMetadata
 from autogluon.common.features.types import R_FLOAT, S_STACK
 from autogluon.common.utils.path_converter import PathConverter
 
-from .bagged_ensemble_model import BaggedEnsembleModel
+from ...constants import MULTICLASS, QUANTILE, SOFTCLASS
 from ..abstract.abstract_model import AbstractModel
-from ...constants import MULTICLASS, SOFTCLASS, QUANTILE
+from .bagged_ensemble_model import BaggedEnsembleModel
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: Currently, if this is a stacker above level 1, it will be very slow taking raw input due to each stacker needing to repeat computation on the base models.
 #  To solve this, this model must know full context of stacker, and only get preds once for each required model
 #  This is already done in trainer, but could be moved internally.
@@ -29,63 +28,73 @@
 
     By specifying base models during init, stacker models can use the base model predictions as features during training and inference.
 
     This property allows for significantly improved model quality in many situations compared to non-stacking alternatives.
 
     Stacker models can act as base models to other stacker models, enabling multi-layer stack ensembling.
     """
-    def __init__(self,
-                 base_model_names=None,
-                 base_models_dict=None,
-                 base_model_paths_dict=None,
-                 base_model_types_dict=None,
-                 base_model_types_inner_dict=None,
-                 base_model_performances_dict=None,
-                 **kwargs):
+
+    def __init__(
+        self,
+        base_model_names=None,
+        base_models_dict=None,
+        base_model_paths_dict=None,
+        base_model_types_dict=None,
+        base_model_types_inner_dict=None,
+        base_model_performances_dict=None,
+        **kwargs,
+    ):
         super().__init__(**kwargs)
         if base_model_names is None:
             base_model_names = []
         if base_models_dict is None:
             base_models_dict = {}
         if base_model_paths_dict is None:
             base_model_paths_dict = {}
         if base_model_types_dict is None:
             base_model_types_dict = {}
         self.base_model_names = base_model_names
         self.base_models_dict: Dict[str, AbstractModel] = base_models_dict  # String name -> Model objects
         self.base_model_paths_dict = base_model_paths_dict
 
         # FIXME: DO NOT DO THIS, FIX ASAP
-        self.base_model_paths_dict = {
-            k: PathConverter.to_relative(v) for k, v in self.base_model_paths_dict.items()
-        }
+        self.base_model_paths_dict = {k: PathConverter.to_relative(v) for k, v in self.base_model_paths_dict.items()}
 
         self.base_model_types_dict = base_model_types_dict
 
         # TODO: Consider deleting these variables after initialization
         self._base_model_performances_dict = base_model_performances_dict
         self._base_model_types_inner_dict = base_model_types_inner_dict
 
     def _initialize(self, **kwargs):
         super()._initialize(**kwargs)
         base_model_performances_dict = self._base_model_performances_dict
         base_model_types_inner_dict = self._base_model_types_inner_dict
         if (base_model_performances_dict is not None) and (base_model_types_inner_dict is not None):
-            if self.params['max_base_models_per_type'] > 0:
-                self.base_model_names = self.limit_models_per_type(models=self.base_model_names, model_types=base_model_types_inner_dict, model_scores=base_model_performances_dict, max_base_models_per_type=self.params['max_base_models_per_type'])
-            if self.params['max_base_models'] > 0:
-                self.base_model_names = self.limit_models(models=self.base_model_names, model_scores=base_model_performances_dict, max_base_models=self.params['max_base_models'])
+            if self.params["max_base_models_per_type"] > 0:
+                self.base_model_names = self.limit_models_per_type(
+                    models=self.base_model_names,
+                    model_types=base_model_types_inner_dict,
+                    model_scores=base_model_performances_dict,
+                    max_base_models_per_type=self.params["max_base_models_per_type"],
+                )
+            if self.params["max_base_models"] > 0:
+                self.base_model_names = self.limit_models(
+                    models=self.base_model_names, model_scores=base_model_performances_dict, max_base_models=self.params["max_base_models"]
+                )
 
         for model_name, model in self.base_models_dict.items():
             if model_name not in self.base_model_names:
                 self.base_models_dict.pop(model_name)
 
         self.stack_column_prefix_lst = copy.deepcopy(self.base_model_names)
         self.stack_columns, self.num_pred_cols_per_model = self.set_stack_columns(stack_column_prefix_lst=self.stack_column_prefix_lst)
-        self.stack_column_prefix_to_model_map = {stack_column_prefix: self.base_model_names[i] for i, stack_column_prefix in enumerate(self.stack_column_prefix_lst)}
+        self.stack_column_prefix_to_model_map = {
+            stack_column_prefix: self.base_model_names[i] for i, stack_column_prefix in enumerate(self.stack_column_prefix_lst)
+        }
 
         self._add_stack_to_feature_metadata()
 
     @staticmethod
     def limit_models_per_type(models, model_types, model_scores, max_base_models_per_type):
         model_type_groups = defaultdict(list)
         for model in models:
@@ -95,68 +104,67 @@
             models_remain += sorted(model_type_groups[key], key=lambda x: x[1], reverse=True)[:max_base_models_per_type]
         models_valid_set = set([model for model, score in models_remain])
         # Important: Ensure ordering of `models_valid` is the same as `models`
         models_valid = [model for model in models if model in models_valid_set]
         return models_valid
 
     def limit_models(self, models, model_scores, max_base_models):
-        model_types = {model: '' for model in models}
+        model_types = {model: "" for model in models}
         return self.limit_models_per_type(models=models, model_types=model_types, model_scores=model_scores, max_base_models_per_type=max_base_models)
 
     def _set_default_params(self):
-        default_params = {'use_orig_features': True, 'max_base_models': 25, 'max_base_models_per_type': 5}
+        default_params = {"use_orig_features": True, "max_base_models": 25, "max_base_models_per_type": 5}
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
         super()._set_default_params()
 
     def preprocess(self, X, fit=False, compute_base_preds=True, infer=True, model_pred_proba_dict=None, **kwargs):
         if self.stack_column_prefix_lst:
             if infer:
                 if set(self.stack_columns).issubset(set(list(X.columns))):
-                    compute_base_preds = False  # TODO: Consider removing, this can be dangerous but the code to make this work otherwise is complex (must rewrite predict_proba)
+                    compute_base_preds = (
+                        False  # TODO: Consider removing, this can be dangerous but the code to make this work otherwise is complex (must rewrite predict_proba)
+                    )
             if compute_base_preds:
                 X_stacker = []
                 for stack_column_prefix in self.stack_column_prefix_lst:
                     base_model_name = self.stack_column_prefix_to_model_map[stack_column_prefix]
                     if fit:
                         base_model_type = self.base_model_types_dict[base_model_name]
                         base_model_path = self.base_model_paths_dict[base_model_name]
                         y_pred_proba = base_model_type.load_oof(path=base_model_path)
                     elif model_pred_proba_dict and base_model_name in model_pred_proba_dict:
                         y_pred_proba = model_pred_proba_dict[base_model_name]
                     else:
                         base_model = self.load_base_model(base_model_name)
                         y_pred_proba = base_model.predict_proba(X)
-                    X_stacker.append(y_pred_proba)  # TODO: This could get very large on a high class count problem. Consider capping to top N most frequent classes and merging least frequent
+                    X_stacker.append(
+                        y_pred_proba
+                    )  # TODO: This could get very large on a high class count problem. Consider capping to top N most frequent classes and merging least frequent
                 X_stacker = self.pred_probas_to_df(X_stacker, index=X.index)
-                if self.params['use_orig_features']:
+                if self.params["use_orig_features"]:
                     X = pd.concat([X_stacker, X], axis=1)
                 else:
                     X = X_stacker
-            elif not self.params['use_orig_features']:
+            elif not self.params["use_orig_features"]:
                 X = X[self.stack_columns]
         X = super().preprocess(X, **kwargs)
         return X
 
     def pred_probas_to_df(self, pred_proba: list, index=None) -> pd.DataFrame:
         if self.problem_type in [MULTICLASS, SOFTCLASS, QUANTILE]:
             pred_proba = np.concatenate(pred_proba, axis=1)
             pred_proba = pd.DataFrame(pred_proba, columns=self.stack_columns)
         else:
             pred_proba = pd.DataFrame(data=np.asarray(pred_proba).T, columns=self.stack_columns)
         if index is not None:
             pred_proba.set_index(index, inplace=True)
         return pred_proba
 
-    def _fit(self,
-             X,
-             y,
-             compute_base_preds=True,
-             time_limit=None,
-             **kwargs):
+    def _fit(self, X, y, compute_base_preds=True, time_limit=None, **kwargs):
         start_time = time.time()
         # TODO: This could be preprocess_nonadaptive=True in general, just have preprocess_nonadaptive=False for child models
         X = self.preprocess(X=X, preprocess_nonadaptive=False, fit=True, compute_base_preds=compute_base_preds)
         if time_limit is not None:
             time_limit = time_limit - (time.time() - start_time)
         return super()._fit(X=X, y=y, time_limit=time_limit, **kwargs)
 
@@ -170,29 +178,29 @@
         for model, model_path in self.base_model_paths_dict.items():
             model_path = os.path.abspath(model_path) + os.path.sep
             model_local_path = model_path.split(abs_path_root_orig, 1)[1]
             self.base_model_paths_dict[model] = self.path_root + model_local_path
 
     def set_stack_columns(self, stack_column_prefix_lst):
         if self.problem_type in [MULTICLASS, SOFTCLASS]:
-            stack_columns = [stack_column_prefix + '_' + str(cls) for stack_column_prefix in stack_column_prefix_lst for cls in range(self.num_classes)]
+            stack_columns = [stack_column_prefix + "_" + str(cls) for stack_column_prefix in stack_column_prefix_lst for cls in range(self.num_classes)]
             num_pred_cols_per_model = self.num_classes
         elif self.problem_type == QUANTILE:
-            stack_columns = [stack_column_prefix + '_' + str(q) for stack_column_prefix in stack_column_prefix_lst for q in self.quantile_levels]
+            stack_columns = [stack_column_prefix + "_" + str(q) for stack_column_prefix in stack_column_prefix_lst for q in self.quantile_levels]
             num_pred_cols_per_model = len(self.quantile_levels)
         else:
             stack_columns = stack_column_prefix_lst
             num_pred_cols_per_model = 1
         return stack_columns, num_pred_cols_per_model
 
     def _hyperparameter_tune(self, X, y, k_fold, hpo_executor, compute_base_preds=True, **kwargs):
         if len(self.models) != 0:
-            raise ValueError('self.models must be empty to call hyperparameter_tune, value: %s' % self.models)
+            raise ValueError("self.models must be empty to call hyperparameter_tune, value: %s" % self.models)
 
-        preprocess_kwargs = {'compute_base_preds': compute_base_preds}
+        preprocess_kwargs = {"compute_base_preds": compute_base_preds}
         return super()._hyperparameter_tune(X=X, y=y, k_fold=k_fold, hpo_executor=hpo_executor, preprocess_kwargs=preprocess_kwargs, **kwargs)
 
     def get_params(self):
         init_args = dict(
             base_model_names=self.base_model_names,
             base_models_dict=self.base_models_dict,
             base_model_paths_dict=self.base_model_paths_dict,
@@ -214,17 +222,17 @@
 
     def get_info(self):
         info = super().get_info()
         stacker_info = dict(
             num_base_models=len(self.base_model_names),
             base_model_names=self.base_model_names,
         )
-        children_info = info.pop('children_info')
-        info['stacker_info'] = stacker_info
-        info['children_info'] = children_info  # Ensure children_info is last in order
+        children_info = info.pop("children_info")
+        info["stacker_info"] = stacker_info
+        info["children_info"] = children_info  # Ensure children_info is last in order
         return info
 
     def _add_stack_to_feature_metadata(self):
         if len(self.models) == 0:
             type_map_raw = {column: R_FLOAT for column in self.stack_columns}
             type_group_map_special = {S_STACK: self.stack_columns}
             stacker_feature_metadata = FeatureMetadata(type_map_raw=type_map_raw, type_group_map_special=type_group_map_special)
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/ensemble/weighted_ensemble_model.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/ensemble/weighted_ensemble_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 import logging
 from collections import defaultdict
 
 import numpy as np
 import pandas as pd
 
-from .stacker_ensemble_model import StackerEnsembleModel
 from ..greedy_ensemble.greedy_weighted_ensemble_model import GreedyWeightedEnsembleModel
+from .stacker_ensemble_model import StackerEnsembleModel
 
 logger = logging.getLogger(__name__)
 
 
 # TODO: v0.1 see if this can be removed and logic moved to greedy weighted ensemble model -> Use StackerEnsembleModel as stacker instead
 # TODO: Optimize predict speed when fit on kfold, can simply sum weights
 class WeightedEnsembleModel(StackerEnsembleModel):
     """
     Weighted ensemble meta-model that implements Ensemble Selection: https://www.cs.cornell.edu/~alexn/papers/shotgun.icml04.revised.rev2.pdf
 
     A :class:`autogluon.core.models.GreedyWeightedEnsembleModel` must be specified as the `model_base` to properly function.
     """
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.low_memory = False
 
-    def _fit(self,
-             X,
-             y,
-             **kwargs):
+    def _fit(self, X, y, **kwargs):
         super()._fit(X, y, **kwargs)
         stack_columns = []
         for model in self.models:
             model = self.load_child(model, verbose=False)
             stack_columns = stack_columns + [stack_column for stack_column in model.base_model_names if stack_column not in stack_columns]
         self.stack_column_prefix_lst = [stack_column for stack_column in self.stack_column_prefix_lst if stack_column in stack_columns]
         self.stack_columns, self.num_pred_cols_per_model = self.set_stack_columns(stack_column_prefix_lst=self.stack_column_prefix_lst)
         min_stack_column_prefix_to_model_map = {k: v for k, v in self.stack_column_prefix_to_model_map.items() if k in self.stack_column_prefix_lst}
-        self.base_model_names = [base_model_name for base_model_name in self.base_model_names if base_model_name in min_stack_column_prefix_to_model_map.values()]
+        self.base_model_names = [
+            base_model_name for base_model_name in self.base_model_names if base_model_name in min_stack_column_prefix_to_model_map.values()
+        ]
         self.stack_column_prefix_to_model_map = min_stack_column_prefix_to_model_map
         return self
 
     def _get_model_weights(self):
         weights_dict = defaultdict(int)
         num_models = len(self.models)
         for model in self.models:
@@ -47,36 +47,40 @@
             for key in model_weight_dict.keys():
                 weights_dict[key] += model_weight_dict[key]
         for key in weights_dict:
             weights_dict[key] = weights_dict[key] / num_models
         return weights_dict
 
     def compute_feature_importance(self, X, y, features=None, is_oof=True, **kwargs) -> pd.DataFrame:
-        logger.warning('Warning: non-raw feature importance calculation is not valid for weighted ensemble since it does not have features, returning ensemble weights instead...')
+        logger.warning(
+            "Warning: non-raw feature importance calculation is not valid for weighted ensemble since it does not have features, returning ensemble weights instead..."
+        )
         if is_oof:
             fi = pd.Series(self._get_model_weights()).sort_values(ascending=False)
         else:
-            logger.warning('Warning: Feature importance calculation is not yet implemented for WeightedEnsembleModel on unseen data, returning generic feature importance...')
+            logger.warning(
+                "Warning: Feature importance calculation is not yet implemented for WeightedEnsembleModel on unseen data, returning generic feature importance..."
+            )
             fi = pd.Series(self._get_model_weights()).sort_values(ascending=False)
 
-        fi_df = fi.to_frame(name='importance')
-        fi_df['stddev'] = np.nan
-        fi_df['p_score'] = np.nan
-        fi_df['n'] = np.nan
+        fi_df = fi.to_frame(name="importance")
+        fi_df["stddev"] = np.nan
+        fi_df["p_score"] = np.nan
+        fi_df["n"] = np.nan
 
         # TODO: Rewrite preprocess() in greedy_weighted_ensemble_model to enable
         # fi_df = super().compute_feature_importance(X=X, y=y, features_to_use=features_to_use, preprocess=preprocess, is_oof=is_oof, **kwargs)
         return fi_df
 
     def _set_default_params(self):
-        default_params = {'use_orig_features': False}
+        default_params = {"use_orig_features": False}
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
         super()._set_default_params()
 
     def _more_tags(self):
         """
         This model can generate out-of-fold (oof) predictions by predicting directly on the training data.
         This will make the result slightly overfit, but the weighted ensemble has limited degrees of freedom intentionally, making the overfitting negligible.
         """
-        tags = {'can_get_oof_from_train': True}
+        tags = {"can_get_oof_from_train": True}
         return tags
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/greedy_ensemble/ensemble_selection.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time
 from collections import Counter
 
 import numpy as np
 
 from ...constants import PROBLEM_TYPES
 from ...metrics import log_loss
-from ...utils import get_pred_from_proba, compute_weighted_metric
+from ...utils import compute_weighted_metric, get_pred_from_proba
 
 logger = logging.getLogger(__name__)
 
 
 class AbstractWeightedEnsemble:
     def predict(self, X):
         y_pred_proba = self.predict_proba(X)
@@ -24,51 +24,51 @@
         preds_norm = [pred * weight for pred, weight in zip(pred_probas, weights)]
         preds_ensemble = np.sum(preds_norm, axis=0)
         return preds_ensemble
 
 
 class EnsembleSelection(AbstractWeightedEnsemble):
     def __init__(
-            self,
-            ensemble_size: int,
-            problem_type: str,
-            metric,
-            sorted_initialization: bool = False,
-            bagging: bool = False,
-            tie_breaker: str = 'random',
-            random_state: np.random.RandomState = None,
-            **kwargs,
+        self,
+        ensemble_size: int,
+        problem_type: str,
+        metric,
+        sorted_initialization: bool = False,
+        bagging: bool = False,
+        tie_breaker: str = "random",
+        random_state: np.random.RandomState = None,
+        **kwargs,
     ):
         self.ensemble_size = ensemble_size
         self.problem_type = problem_type
         self.metric = metric
         self.sorted_initialization = sorted_initialization
         self.bagging = bagging
         self.use_best = True
-        if tie_breaker not in ['random', 'second_metric']:
+        if tie_breaker not in ["random", "second_metric"]:
             raise ValueError(f"Unknown tie_breaker value: {tie_breaker}. Must be one of: ['random', 'second_metric']")
         self.tie_breaker = tie_breaker
         if random_state is not None:
             self.random_state = random_state
         else:
             self.random_state = np.random.RandomState(seed=0)
-        self.quantile_levels = kwargs.get('quantile_levels', None)
+        self.quantile_levels = kwargs.get("quantile_levels", None)
 
     def fit(self, predictions, labels, time_limit=None, identifiers=None, sample_weight=None):
         self.ensemble_size = int(self.ensemble_size)
         if self.ensemble_size < 1:
-            raise ValueError('Ensemble size cannot be less than one!')
+            raise ValueError("Ensemble size cannot be less than one!")
         if not self.problem_type in PROBLEM_TYPES:
-            raise ValueError('Unknown problem type %s.' % self.problem_type)
+            raise ValueError("Unknown problem type %s." % self.problem_type)
         # if not isinstance(self.metric, Scorer):
         #     raise ValueError('Metric must be of type scorer')
 
         self._fit(predictions=predictions, labels=labels, time_limit=time_limit, sample_weight=sample_weight)
         self._calculate_weights()
-        logger.log(15, 'Ensemble weights: ')
+        logger.log(15, "Ensemble weights: ")
         logger.log(15, self.weights_)
         return self
 
     # TODO: Consider having a removal stage, remove each model and see if score is affected, if improves or not effected, remove it.
     def _fit(self, predictions, labels, time_limit=None, sample_weight=None):
         ensemble_size = self.ensemble_size
         self.num_input_models_ = len(predictions)
@@ -105,15 +105,15 @@
                 for pred in ensemble:
                     ensemble_prediction += pred
                 ensemble_prediction /= s
 
                 weighted_ensemble_prediction = (s / float(s + 1)) * ensemble_prediction
             fant_ensemble_prediction = np.zeros(weighted_ensemble_prediction.shape)
             for j, pred in enumerate(predictions):
-                fant_ensemble_prediction[:] = weighted_ensemble_prediction + (1. / float(s + 1)) * pred
+                fant_ensemble_prediction[:] = weighted_ensemble_prediction + (1.0 / float(s + 1)) * pred
                 scores[j] = self._calculate_regret(y_true=labels, y_pred_proba=fant_ensemble_prediction, metric=self.metric, sample_weight=sample_weight)
                 if round_scores:
                     scores[j] = scores[j].round(round_decimals)
 
             all_best = np.argwhere(scores == np.nanmin(scores)).flatten()
 
             if (len(all_best) > 1) and used_models:
@@ -122,25 +122,25 @@
                 for m in all_best:
                     if m in used_models:
                         new_all_best.append(m)
                 if new_all_best:
                     all_best = new_all_best
 
             if len(all_best) > 1:
-                if self.tie_breaker == 'second_metric':
-                    if self.problem_type in ['binary', 'multiclass']:
+                if self.tie_breaker == "second_metric":
+                    if self.problem_type in ["binary", "multiclass"]:
                         # Tiebreak with log_loss
                         scores_tiebreak = np.zeros((len(all_best)))
                         secondary_metric = log_loss
                         fant_ensemble_prediction = np.zeros(weighted_ensemble_prediction.shape)
                         index_map = {}
                         for k, j in enumerate(all_best):
                             index_map[k] = j
                             pred = predictions[j]
-                            fant_ensemble_prediction[:] = weighted_ensemble_prediction + (1. / float(s + 1)) * pred
+                            fant_ensemble_prediction[:] = weighted_ensemble_prediction + (1.0 / float(s + 1)) * pred
                             scores_tiebreak[k] = self._calculate_regret(y_true=labels, y_pred_proba=fant_ensemble_prediction, metric=secondary_metric)
                         all_best_tiebreak = np.argwhere(scores_tiebreak == np.nanmin(scores_tiebreak)).flatten()
                         all_best = [index_map[index] for index in all_best_tiebreak]
 
             best = self.random_state.choice(all_best)
             best_score = scores[best]
 
@@ -161,32 +161,35 @@
             if len(predictions) == 1:
                 break
 
             if time_limit is not None:
                 time_elapsed = time.time() - time_start
                 time_left = time_limit - time_elapsed
                 if time_left <= 0:
-                    logger.warning('Warning: Ensemble Selection ran out of time, early stopping at iteration %s. This may mean that the time_limit specified is very small for this problem.' % (i+1))
+                    logger.warning(
+                        "Warning: Ensemble Selection ran out of time, early stopping at iteration %s. This may mean that the time_limit specified is very small for this problem."
+                        % (i + 1)
+                    )
                     break
 
         min_score = np.min(trajectory)
         first_index_of_best = trajectory.index(min_score)
 
         if self.use_best:
-            self.indices_ = order[:first_index_of_best+1]
-            self.trajectory_ = trajectory[:first_index_of_best+1]
+            self.indices_ = order[: first_index_of_best + 1]
+            self.trajectory_ = trajectory[: first_index_of_best + 1]
             self.train_score_ = trajectory[first_index_of_best]
             self.ensemble_size = first_index_of_best + 1
-            logger.log(15, 'Ensemble size: %s' % self.ensemble_size)
+            logger.log(15, "Ensemble size: %s" % self.ensemble_size)
         else:
             self.indices_ = order
             self.trajectory_ = trajectory
             self.train_score_ = trajectory[-1]
 
-        logger.debug("Ensemble indices: "+str(self.indices_))
+        logger.debug("Ensemble indices: " + str(self.indices_))
 
     def _calculate_regret(self, y_true, y_pred_proba, metric, sample_weight=None):
         if metric.needs_pred or metric.needs_quantile:
             preds = get_pred_from_proba(y_pred_proba=y_pred_proba, problem_type=self.problem_type)
         else:
             preds = y_pred_proba
         score = compute_weighted_metric(y_true, preds, metric, sample_weight, quantile_levels=self.quantile_levels)
@@ -203,14 +206,15 @@
             weights = weights / np.sum(weights)
 
         self.weights_ = weights
 
 
 class SimpleWeightedEnsemble(AbstractWeightedEnsemble):
     """Predefined user-weights ensemble"""
+
     def __init__(self, weights, problem_type, **kwargs):
         self.weights_ = weights
         self.problem_type = problem_type
 
     @property
     def ensemble_size(self):
         return len(self.weights_)
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/models/greedy_ensemble/greedy_weighted_ensemble_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import logging
 
 from autogluon.common.features.types import S_STACK
 
-from .ensemble_selection import EnsembleSelection, SimpleWeightedEnsemble
+from ...constants import MULTICLASS, QUANTILE, SOFTCLASS
 from ..abstract.abstract_model import AbstractModel
-from ...constants import MULTICLASS, SOFTCLASS, QUANTILE
+from .ensemble_selection import EnsembleSelection, SimpleWeightedEnsemble
 
 logger = logging.getLogger(__name__)
 
 
 class GreedyWeightedEnsembleModel(AbstractModel):
     def __init__(self, base_model_names=None, model_base=EnsembleSelection, **kwargs):
         super().__init__(**kwargs)
         self.model_base = model_base
         self.num_pred_cols_per_model = None
         self.base_model_names = base_model_names
         self.weights_ = None
 
     def _set_default_params(self):
-        default_params = {'ensemble_size': 100}
+        default_params = {"ensemble_size": 100}
         for param, val in default_params.items():
             self._set_default_param_value(param, val)
 
     def _get_default_auxiliary_params(self) -> dict:
         default_auxiliary_params = super()._get_default_auxiliary_params()
         extra_auxiliary_params = dict(
             drop_unique=False,
@@ -44,30 +44,23 @@
         elif self.problem_type == QUANTILE:
             self.num_pred_cols_per_model = len(self.quantile_levels)
         if self.base_model_names is None:
             self.base_model_names = self._infer_base_model_names()
         self.features = self._set_stack_columns(base_model_names=self.base_model_names)
 
     # TODO: Check memory after loading best model predictions, only load top X model predictions that fit in memory
-    def _fit(self,
-             X,
-             y,
-             X_val=None,
-             y_val=None,
-             time_limit=None,
-             sample_weight=None,
-             **kwargs):
+    def _fit(self, X, y, X_val=None, y_val=None, time_limit=None, sample_weight=None, **kwargs):
         params = self._get_model_params()
         if self.model is None:
             X = self.preprocess(X)
             self.model = self.model_base(problem_type=self.problem_type, quantile_levels=self.quantile_levels, metric=self.stopping_metric, **params)
             self.model = self.model.fit(X, y, time_limit=time_limit, sample_weight=sample_weight)
             self.base_model_names, self.model.weights_ = self.remove_zero_weight_models(self.base_model_names, self.model.weights_)
         self.features = self._set_stack_columns(base_model_names=self.base_model_names)
-        self.params_trained['ensemble_size'] = self.model.ensemble_size
+        self.params_trained["ensemble_size"] = self.model.ensemble_size
         self.weights_ = self.model.weights_
 
     def convert_pred_probas_df_to_list(self, pred_probas_df) -> list:
         pred_probas = []
         for i, model in enumerate(self.base_model_names):
             index_start = i * self.num_pred_cols_per_model
             index_end = (i + 1) * self.num_pred_cols_per_model
@@ -86,65 +79,64 @@
             if weight != 0:
                 base_models_to_keep.append(base_model_names[i])
                 base_model_weights_to_keep.append(weight)
         return base_models_to_keep, base_model_weights_to_keep
 
     def _set_stack_columns(self, base_model_names):
         if self.problem_type in [MULTICLASS, SOFTCLASS]:
-            stack_columns = [model_name + '_' + str(cls) for model_name in base_model_names for cls in range(self.num_classes)]
+            stack_columns = [model_name + "_" + str(cls) for model_name in base_model_names for cls in range(self.num_classes)]
         elif self.problem_type == QUANTILE:
-            stack_columns = [model_name + '_' + str(q) for model_name in base_model_names for q in self.quantile_levels]
+            stack_columns = [model_name + "_" + str(q) for model_name in base_model_names for q in self.quantile_levels]
         else:
             stack_columns = base_model_names
         return stack_columns
 
     def _infer_base_model_names(self):
         stack_column_names = self.feature_metadata.get_features(required_special_types=[S_STACK])
 
         if self.problem_type == QUANTILE:
-            columns_class_0 = [column for column in stack_column_names if
-                               column.endswith('_{}'.format(str(self.quantile_levels[0])))]
-            base_model_names = [column.rsplit('_', 1)[0] for column in columns_class_0]
+            columns_class_0 = [column for column in stack_column_names if column.endswith("_{}".format(str(self.quantile_levels[0])))]
+            base_model_names = [column.rsplit("_", 1)[0] for column in columns_class_0]
         elif self.num_pred_cols_per_model > 1:
-            columns_class_0 = [column for column in stack_column_names if column.endswith('_0')]
+            columns_class_0 = [column for column in stack_column_names if column.endswith("_0")]
             base_model_names = [column[:-2] for column in columns_class_0]
         else:
             base_model_names = stack_column_names
         return base_model_names
 
     def _get_model_weights(self):
         num_models = len(self.base_model_names)
         model_weight_dict = {self.base_model_names[i]: self.weights_[i] for i in range(num_models)}
         return model_weight_dict
 
     def get_info(self):
         info = super().get_info()
-        info['model_weights'] = self._get_model_weights()
+        info["model_weights"] = self._get_model_weights()
         return info
 
     @classmethod
     def _get_default_ag_args(cls) -> dict:
         default_ag_args = super()._get_default_ag_args()
-        extra_ag_args = {'valid_base': False}
+        extra_ag_args = {"valid_base": False}
         default_ag_args.update(extra_ag_args)
         return default_ag_args
 
     def _get_default_stopping_metric(self):
         return self.eval_metric
 
 
 class SimpleWeightedEnsembleModel(GreedyWeightedEnsembleModel):
     def __init__(self, model_base=SimpleWeightedEnsemble, **kwargs):
         super().__init__(model_base=model_base, **kwargs)
 
     def _fit(self, **kwargs):
         params = self._get_model_params()
-        if 'weights' not in params:
+        if "weights" not in params:
             raise ValueError('Missing required parameter "weights" to fit SimpleWeightedEnsembleModel.')
-        if len(params['weights']) != len(self.base_model_names):
+        if len(params["weights"]) != len(self.base_model_names):
             raise AssertionError(f'Length of weights does not equal length of self.base_model_names ({len(params["weights"])}, {len(self.base_model_names)})')
 
         if self.model is None:
             self.model = self.model_base(problem_type=self.problem_type, **params)
             self.base_model_names, self.model.weights_ = self.remove_zero_weight_models(self.base_model_names, self.model.weights_)
         self.features = self._set_stack_columns(base_model_names=self.base_model_names)
         self.weights_ = self.model.weights_
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/problem_type.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/problem_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Dict, List
 
-from .constants import BINARY, MULTICLASS, REGRESSION, SOFTCLASS, QUANTILE
+from .constants import BINARY, MULTICLASS, QUANTILE, REGRESSION, SOFTCLASS
 
-__all__ = ['problem_type_info']
+__all__ = ["problem_type_info"]
 
 
 # Note to developers: This is a free-form class. If you need additional parameters, add them.
 class ProblemType:
     """
     Simple class that holds information on what a problem type is capable of doing.
 
@@ -18,25 +18,24 @@
         Whether models for this problem type have the ability to predict probabilities via `model.predict_proba(...)`.
     is_classification : bool
         Whether this is considered a classification problem type.
         For example:
             `binary`, `multiclass`, and `softclass` are considered classification problem types.
             `regression` and `quantile` are not considered classification problem types.
     """
-    def __init__(self,
-                 can_predict: bool,
-                 can_predict_proba: bool,
-                 is_classification: bool):
+
+    def __init__(self, can_predict: bool, can_predict_proba: bool, is_classification: bool):
         self.can_predict = can_predict
         self.can_predict_proba = can_predict_proba
         self.is_classification = is_classification
 
 
 class ProblemTypeInfo:
     """Class that stores all problem_type information, and can vend this information via the provided methods."""
+
     def __init__(self, problem_type_dict: Dict[str, ProblemType]):
         self.problem_type_dict = problem_type_dict
 
     def list_problem_types(self):
         return [self.problem_type_dict.keys()]
 
     def can_predict(self, problem_type: str) -> bool:
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/pseudolabeling/pseudolabeling.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/pseudolabeling/pseudolabeling.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 
 import numpy as np
 import pandas as pd
+
 from autogluon.core.constants import PROBLEM_TYPES_CLASSIFICATION
 
 logger = logging.getLogger(__name__)
 
 
 def sample_bins_uniformly(y_pred_proba: pd.DataFrame, df_indexes):
     """
@@ -30,15 +31,15 @@
     min_count = class_value_counts.min()
     class_keys = list(class_value_counts.keys())
     test_pseudo_indices = pd.Series(data=False, index=y_pred_proba.index)
 
     if len(class_keys) < 1:
         return test_pseudo_indices
 
-    logging.log(15, f'Taking {min_count} rows from the following classes: {class_keys}')
+    logging.log(15, f"Taking {min_count} rows from the following classes: {class_keys}")
 
     new_test_pseudo_indices = None
     for k in class_keys:
         class_k_pseudo_idxes = pred_idxmax == k
         selected_rows = class_k_pseudo_idxes[class_k_pseudo_idxes].sample(min_count)
 
         if new_test_pseudo_indices is None:
@@ -47,17 +48,17 @@
             new_test_pseudo_indices = new_test_pseudo_indices.append(selected_rows.index)
 
     test_pseudo_indices.loc[new_test_pseudo_indices] = True
 
     return test_pseudo_indices
 
 
-def filter_pseudo(y_pred_proba_og, problem_type,
-                  min_proportion_prob: float = 0.05, max_proportion_prob: float = 0.6,
-                  threshold: float = 0.95, proportion_sample: float = 0.3):
+def filter_pseudo(
+    y_pred_proba_og, problem_type, min_proportion_prob: float = 0.05, max_proportion_prob: float = 0.6, threshold: float = 0.95, proportion_sample: float = 0.3
+):
     """
     Takes in the predicted probabilities of the model (y_pred_proba_og) and chooses the indices that meet
     a criteria to incorporate into training data. Criteria is determined by problem_type.
     If multiclass or binary will choose all rows with max prob over threshold. For regression
     chooses 30% of the labeled data randomly. This filter is used pseudo labeled data.
 
     Parameters:
@@ -91,15 +92,15 @@
         if curr_percentage > max_proportion_prob or curr_percentage < min_proportion_prob:
             if curr_percentage > max_proportion_prob:
                 num_rows_threshold = max(np.ceil(max_proportion_prob * num_rows), 1)
             else:
                 num_rows_threshold = max(np.ceil(min_proportion_prob * num_rows), 1)
             curr_threshold = y_pred_proba_max.sort_values(ascending=False).iloc[int(num_rows_threshold) - 1]
 
-        test_pseudo_indices = (y_pred_proba_max >= curr_threshold)
+        test_pseudo_indices = y_pred_proba_max >= curr_threshold
         test_pseudo_indices = sample_bins_uniformly(y_pred_proba=y_pred_proba_og, df_indexes=test_pseudo_indices)
     else:
         test_pseudo_indices = pd.Series(data=False, index=y_pred_proba_og.index)
         test_pseudo_indices_true = test_pseudo_indices.sample(frac=proportion_sample, random_state=0)
         test_pseudo_indices[test_pseudo_indices_true.index] = True
 
     test_pseudo_indices = test_pseudo_indices[test_pseudo_indices]
@@ -127,29 +128,26 @@
     pd.Series of indices that met pseudo labeling requirements
     """
     original_k = num_models
     leaderboard = predictor._trainer.leaderboard()
     num_models = len(leaderboard)
 
     if num_models < 2:
-        raise Exception('Ensemble pseudo labeling was enabled, but only one model was trained')
+        raise Exception("Ensemble pseudo labeling was enabled, but only one model was trained")
 
     if num_models != num_models:
-        logging.warning(f'Ensemble pseudo labeling expected {original_k}, but only {num_models} fit.')
+        logging.warning(f"Ensemble pseudo labeling expected {original_k}, but only {num_models} fit.")
 
     if predictor.problem_type in PROBLEM_TYPES_CLASSIFICATION:
-        return filter_ensemble_classification(predictor=predictor, unlabeled_data=unlabeled_data,
-                                              leaderboard=leaderboard, num_models=num_models)
+        return filter_ensemble_classification(predictor=predictor, unlabeled_data=unlabeled_data, leaderboard=leaderboard, num_models=num_models)
     else:
-        return filter_pseudo_std_regression(predictor=predictor, unlabeled_data=unlabeled_data,
-                                            leaderboard=leaderboard, num_models=num_models)
+        return filter_pseudo_std_regression(predictor=predictor, unlabeled_data=unlabeled_data, leaderboard=leaderboard, num_models=num_models)
 
 
-def filter_pseudo_std_regression(predictor, unlabeled_data: pd.DataFrame, num_models, leaderboard,
-                                 lower_bound: float = -0.25, upper_bound: float = 0.25):
+def filter_pseudo_std_regression(predictor, unlabeled_data: pd.DataFrame, num_models, leaderboard, lower_bound: float = -0.25, upper_bound: float = 0.25):
     """
     Predicts on unlabeled_data using the top num_models. Then gets standard deviation of each
     row's predictions across the top num_models and the standard deviation across all rows of standard
     deviations of the top num_models. Calculates z-score using top num_models predictions standard
     deviation minus the mean of the top num_models standard deviation divided by the standard deviation of
     the top num_model predictions across all rows. The indices of all top num_model predictions who's z-score
     falls within lower_bound and upper_bound will be returned.
@@ -164,15 +162,15 @@
         incorporate
     upper_bound: Upper threshold that z-score needs to be below to incorporate
 
     Returns:
     --------
     pd.Series of indices that met pseudo labeling requirements
     """
-    top_k_models_list = leaderboard.head(num_models)['model']
+    top_k_models_list = leaderboard.head(num_models)["model"]
     top_k_preds = None
 
     for model in top_k_models_list:
         y_test_pred = predictor.predict(data=unlabeled_data, model=model)
 
         if model == top_k_models_list[0]:
             top_k_preds = y_test_pred
@@ -188,37 +186,36 @@
     preds_sd = pd.Series(data=np.std(top_k_preds, axis=1), index=unlabeled_data.index)
     preds_z_score = (preds_sd - preds_sd.mean()) / preds_sd.std()
     df_filtered = preds_z_score.between(lower_bound, upper_bound)
 
     return df_filtered[df_filtered], top_k_avg_preds
 
 
-def filter_ensemble_classification(predictor, unlabeled_data: pd.DataFrame, leaderboard,
-                                   num_models, threshold: float = 0.95):
+def filter_ensemble_classification(predictor, unlabeled_data: pd.DataFrame, leaderboard, num_models, threshold: float = 0.95):
     """
     Calculates predictive probabilities of unlabeled data by predicting with top num_models
     then averages pre-row over predictions from top num_models and selects rows where confidence
     (predicted probability of the most likely class) is above threshold. Then samples minimum
     bin count from all bins, where bins are rows of averaged predictions with the same peak
     predicted probability class.
-    
+
     Parameters:
     -----------
     predictor: Fitted TabularPredictor
     unlabeled_data: Unlabeled data for top k models to predict on
     leaderboard: pd.DataFrame of leaderboard of models in AutoGluon based on validation score
     num_models: Number of top models to ensemble
     threshold: The predictive probability a row must exceed in order to be
         selected
 
     Returns:
     --------
     pd.Series of indices that met pseudo labeling requirements
     """
-    top_k_model_names = leaderboard.head(num_models)['model']
+    top_k_model_names = leaderboard.head(num_models)["model"]
 
     y_pred_proba_ensemble = None
     for model_name in top_k_model_names:
         y_pred_proba_curr_model = predictor.predict_proba(data=unlabeled_data, model=model_name)
 
         if y_pred_proba_ensemble is None:
             y_pred_proba_ensemble = y_pred_proba_curr_model
@@ -227,13 +224,13 @@
 
     # Todo: This doesn't make total sense, because weighted ensemble
     # will ensemble the top models and weigh them according to validation score
     # maybe should just force prediction using weighted ensemble instead of
     # uniform across top k?
     y_pred_proba_ensemble /= num_models
     y_max_prob = y_pred_proba_ensemble.max(axis=1)
-    pseudo_indexes = (y_max_prob >= threshold)
+    pseudo_indexes = y_max_prob >= threshold
     y_pred_ensemble = y_pred_proba_ensemble.idxmax(axis=1)
 
     test_pseudo_indices = sample_bins_uniformly(y_pred_proba=y_pred_proba_ensemble, df_indexes=pseudo_indexes)
 
     return test_pseudo_indices[test_pseudo_indices], y_pred_proba_ensemble, y_pred_ensemble
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/ray/resources_calculator.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/ray/resources_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import logging
 import math
-
 from abc import ABC, abstractmethod
+
 from autogluon.common.utils.resource_utils import ResourceManager
 
 logger = logging.getLogger(__name__)
 
 
 class ResourceCalculator(ABC):
-
     @property
     @abstractmethod
     def calc_type(self):
         """Type of the resource calculator"""
         raise NotImplementedError
 
     @abstractmethod
@@ -22,126 +21,111 @@
 
     def wrap_resources_per_job_into_placement_group(self, resources_per_job):
         """
         When doing parallel training inside parallel trials, Ray requires to provide placement group for resource scheduling
         We wrap a group where the resource requirement is 0 because the trial only spread the task and doesn't require too much resources.
         """
         from ray import tune
-        num_cpus = resources_per_job.get('cpu', 0)
-        num_gpus = resources_per_job.get('gpu', 0)
+
+        num_cpus = resources_per_job.get("cpu", 0)
+        num_gpus = resources_per_job.get("gpu", 0)
         # The head bundle doesn't actually require resources.
         # This memory constraint is a hack (1024 is a random number, unit is bytes) to trick ray to schedule bundles on the same node
         # Currently we force the trial and its underlying folds being trained on the same node to avoid synchronization
         # TODO: consider seperate the sub-bundle of folding so they can be scheduled on seperate nodes
-        return tune.PlacementGroupFactory([{"memory": 1024}, {'CPU': num_cpus, 'GPU': num_gpus}], strategy="STRICT_PACK")
+        return tune.PlacementGroupFactory([{"memory": 1024}, {"CPU": num_cpus, "GPU": num_gpus}], strategy="STRICT_PACK")
 
 
 class CpuResourceCalculator(ResourceCalculator):
-
     @property
     def calc_type(self):
-        return 'cpu'
+        return "cpu"
 
     def get_resources_per_job(
         self,
         total_num_cpus,
         num_jobs,
         minimum_cpu_per_job,
         model_estimate_memory_usage=None,
         wrap_resources_per_job_into_placement_group=False,
         user_resources_per_job=None,
         **kwargs,
     ):
         if user_resources_per_job is not None:
-            cpu_per_job = user_resources_per_job.get('num_cpus', 0)
-            assert cpu_per_job <= total_num_cpus, \
-                f"Detected model level cpu requirement = {cpu_per_job} > total cpu granted to AG predictor = {total_num_cpus}"
-            assert cpu_per_job >= minimum_cpu_per_job, \
-                f"The model requires minimum cpu {minimum_cpu_per_job}, but you only specified {cpu_per_job}"
+            cpu_per_job = user_resources_per_job.get("num_cpus", 0)
+            assert cpu_per_job <= total_num_cpus, f"Detected model level cpu requirement = {cpu_per_job} > total cpu granted to AG predictor = {total_num_cpus}"
+            assert cpu_per_job >= minimum_cpu_per_job, f"The model requires minimum cpu {minimum_cpu_per_job}, but you only specified {cpu_per_job}"
             num_parallel_jobs = total_num_cpus // cpu_per_job
             batches = math.ceil(num_jobs / num_parallel_jobs)
         else:
             cpu_per_job = max(minimum_cpu_per_job, int(total_num_cpus // num_jobs))
             max_jobs_in_parallel_memory = num_jobs
 
             if model_estimate_memory_usage is not None:
                 mem_available = ResourceManager.get_available_virtual_mem()
                 # calculate how many jobs can run in parallel given memory available
                 max_jobs_in_parallel_memory = max(1, int(mem_available // model_estimate_memory_usage))
             num_parallel_jobs = min(num_jobs, total_num_cpus // cpu_per_job, max_jobs_in_parallel_memory)
             if num_parallel_jobs == 0:
-                error_msg = ('Cannot train model with provided resources! '
-                                f'num_cpus=={total_num_cpus} | '
-                                f'min_cpus=={minimum_cpu_per_job}')
+                error_msg = "Cannot train model with provided resources! " f"num_cpus=={total_num_cpus} | " f"min_cpus=={minimum_cpu_per_job}"
                 if model_estimate_memory_usage is not None:
-                    error_msg += (
-                        f' | mem_available=={mem_available} | '
-                        f'model_estimate_memory_usage=={model_estimate_memory_usage}'
-                    )
+                    error_msg += f" | mem_available=={mem_available} | " f"model_estimate_memory_usage=={model_estimate_memory_usage}"
                 raise AssertionError(error_msg)
             cpu_per_job = int(total_num_cpus // num_parallel_jobs)  # update cpu_per_job in case memory is not enough and can use more cores for each job
             batches = math.ceil(num_jobs / num_parallel_jobs)
 
         resources_per_job = dict(cpu=cpu_per_job)
         if wrap_resources_per_job_into_placement_group:
             resources_per_job = self.wrap_resources_per_job_into_placement_group(resources_per_job)
 
-        resources_info = dict(
-            resources_per_job=resources_per_job,
-            num_parallel_jobs=num_parallel_jobs,
-            batches=batches,
-            cpu_per_job=cpu_per_job
-        )
-        logger.log(10, f'Resources info for {self.__class__.__name__}: {resources_info}')
+        resources_info = dict(resources_per_job=resources_per_job, num_parallel_jobs=num_parallel_jobs, batches=batches, cpu_per_job=cpu_per_job)
+        logger.log(10, f"Resources info for {self.__class__.__name__}: {resources_info}")
 
         return resources_info
 
 
 class GpuResourceCalculator(ResourceCalculator):
-
     @property
     def calc_type(self):
-        return 'gpu'
+        return "gpu"
 
     def get_resources_per_job(
         self,
         total_num_cpus,
         total_num_gpus,
         num_jobs,
         minimum_cpu_per_job,
         minimum_gpu_per_job,
         wrap_resources_per_job_into_placement_group=False,
         user_resources_per_job=None,
         **kwargs,
     ):
         if user_resources_per_job is not None:
-            cpu_per_job = user_resources_per_job.get('num_cpus', minimum_cpu_per_job)
-            assert cpu_per_job <= total_num_cpus, \
-                f"Detected model level cpu requirement = {cpu_per_job} > total cpu granted to AG predictor = {total_num_cpus}"
-            assert cpu_per_job >= minimum_cpu_per_job, \
-                f"The model requires minimum cpu {minimum_cpu_per_job}, but you only specified {cpu_per_job}"
-            gpu_per_job = user_resources_per_job.get('num_gpus', minimum_gpu_per_job)
-            assert gpu_per_job <= total_num_gpus, \
-                f"Detected model level gpu requirement = {gpu_per_job} > total cpu granted to AG predictor = {total_num_gpus}"
-            assert gpu_per_job >= minimum_gpu_per_job, \
-                f"The model requires minimum gpu {minimum_gpu_per_job}, but you only specified {gpu_per_job}"
+            cpu_per_job = user_resources_per_job.get("num_cpus", minimum_cpu_per_job)
+            assert cpu_per_job <= total_num_cpus, f"Detected model level cpu requirement = {cpu_per_job} > total cpu granted to AG predictor = {total_num_cpus}"
+            assert cpu_per_job >= minimum_cpu_per_job, f"The model requires minimum cpu {minimum_cpu_per_job}, but you only specified {cpu_per_job}"
+            gpu_per_job = user_resources_per_job.get("num_gpus", minimum_gpu_per_job)
+            assert gpu_per_job <= total_num_gpus, f"Detected model level gpu requirement = {gpu_per_job} > total cpu granted to AG predictor = {total_num_gpus}"
+            assert gpu_per_job >= minimum_gpu_per_job, f"The model requires minimum gpu {minimum_gpu_per_job}, but you only specified {gpu_per_job}"
             num_parallel_jobs = min(total_num_cpus // cpu_per_job, total_num_gpus / gpu_per_job)
             batches = math.ceil(num_jobs / num_parallel_jobs)
         else:
             cpu_per_job = max(minimum_cpu_per_job, int(total_num_cpus // num_jobs))
             gpu_per_job = max(minimum_gpu_per_job, total_num_gpus / num_jobs)
             num_parallel_jobs = num_jobs
             if cpu_per_job:
                 num_parallel_jobs = min(num_parallel_jobs, total_num_cpus // cpu_per_job)
             if gpu_per_job:
                 num_parallel_jobs = min(num_parallel_jobs, total_num_gpus // gpu_per_job)
             if num_parallel_jobs == 0:
-                raise AssertionError('Cannot train model with provided resources! '
-                                        f'(num_cpus, num_gpus)==({total_num_cpus}, {total_num_gpus}) | '
-                                        f'(min_cpus, min_gpus)==({minimum_cpu_per_job}, {minimum_gpu_per_job})')
+                raise AssertionError(
+                    "Cannot train model with provided resources! "
+                    f"(num_cpus, num_gpus)==({total_num_cpus}, {total_num_gpus}) | "
+                    f"(min_cpus, min_gpus)==({minimum_cpu_per_job}, {minimum_gpu_per_job})"
+                )
             cpu_per_job = int(total_num_cpus // num_parallel_jobs)
             gpu_per_job = total_num_gpus / num_parallel_jobs
             batches = math.ceil(num_jobs / num_parallel_jobs)
 
         resources_per_job = dict(cpu=cpu_per_job, gpu=gpu_per_job)
         if wrap_resources_per_job_into_placement_group:
             resources_per_job = self.wrap_resources_per_job_into_placement_group(resources_per_job)
@@ -149,50 +133,52 @@
         resources_info = dict(
             resources_per_job=resources_per_job,
             num_parallel_jobs=num_parallel_jobs,
             batches=batches,
             cpu_per_job=cpu_per_job,
             gpu_per_job=gpu_per_job,
         )
-        logger.log(10, f'Resources info for {self.__class__.__name__}: {resources_info}')
+        logger.log(10, f"Resources info for {self.__class__.__name__}: {resources_info}")
 
         return resources_info
 
 
 class NonParallelGpuResourceCalculator(ResourceCalculator):
     """
     This calculator will only assign < 1 gpu to each job because some job cannot be parallelized
     """
 
     @property
     def calc_type(self):
-        return 'non_parallel_gpu'
+        return "non_parallel_gpu"
 
     def get_resources_per_job(
         self,
         total_num_cpus,
         total_num_gpus,
         num_jobs,
         minimum_cpu_per_job,
         minimum_gpu_per_job,
         wrap_resources_per_job_into_placement_group=False,
         **kwargs,
     ):
-        assert 0 < minimum_gpu_per_job <= 1, f'{self.__class__.__name__} only supports assigning < 1 gpu to each job' 
+        assert 0 < minimum_gpu_per_job <= 1, f"{self.__class__.__name__} only supports assigning < 1 gpu to each job"
         cpu_per_job = max(minimum_cpu_per_job, int(total_num_cpus // num_jobs))
         gpu_per_job = min(minimum_gpu_per_job, 1)
         num_parallel_jobs = num_jobs
         if cpu_per_job:
             num_parallel_jobs = min(num_parallel_jobs, total_num_cpus // cpu_per_job)
         if gpu_per_job:
             num_parallel_jobs = min(num_parallel_jobs, total_num_gpus // gpu_per_job)
         if num_parallel_jobs == 0:
-            raise AssertionError('Cannot train model with provided resources! '
-                                 f'(num_cpus, num_gpus)==({total_num_cpus}, {total_num_gpus}) | '
-                                 f'(min_cpus, min_gpus)==({cpu_per_job}, {gpu_per_job})')
+            raise AssertionError(
+                "Cannot train model with provided resources! "
+                f"(num_cpus, num_gpus)==({total_num_cpus}, {total_num_gpus}) | "
+                f"(min_cpus, min_gpus)==({cpu_per_job}, {gpu_per_job})"
+            )
         cpu_per_job = int(total_num_cpus // num_parallel_jobs)
         gpu_per_job = min(1, total_num_gpus / num_parallel_jobs)
 
         resources_per_job = dict(cpu=cpu_per_job, gpu=gpu_per_job)
         if wrap_resources_per_job_into_placement_group:
             resources_per_job = self.wrap_resources_per_job_into_placement_group(resources_per_job)
         batches = math.ceil(num_jobs / num_parallel_jobs)
@@ -200,135 +186,124 @@
         resources_info = dict(
             resources_per_job=resources_per_job,
             num_parallel_jobs=num_parallel_jobs,
             batches=batches,
             cpu_per_job=cpu_per_job,
             gpu_per_job=gpu_per_job,
         )
-        logger.log(10, f'Resources info for {self.__class__.__name__}: {resources_info}')
+        logger.log(10, f"Resources info for {self.__class__.__name__}: {resources_info}")
 
         return resources_info
 
 
 class RayLightningCpuResourceCalculator(ResourceCalculator):
-
     @property
     def calc_type(self):
-        return 'ray_lightning_cpu'
+        return "ray_lightning_cpu"
 
     def get_resources_per_job(
         self,
         total_num_cpus,
         num_jobs,
         minimum_cpu_per_job,
         model_estimate_memory_usage=None,
         **kwargs,
     ):
         from ray_lightning.tune import get_tune_resources
+
         # TODO: for cpu case, is it better to have more workers or more cpus per worker?
         cpu_per_job = max(minimum_cpu_per_job, total_num_cpus // num_jobs)
         max_jobs_in_parallel_memory = num_jobs
         if model_estimate_memory_usage is not None:
             mem_available = ResourceManager.get_available_virtual_mem()
             # calculate how many jobs can run in parallel given memory available
             max_jobs_in_parallel_memory = max(1, int(mem_available // model_estimate_memory_usage))
         num_parallel_jobs = min(num_jobs, total_num_cpus // cpu_per_job, max_jobs_in_parallel_memory)
         if num_parallel_jobs == 0:
-            error_msg = ('Cannot train model with provided resources! '
-                         f'num_cpus=={total_num_cpus} | '
-                         f'min_cpus=={minimum_cpu_per_job}')
+            error_msg = "Cannot train model with provided resources! " f"num_cpus=={total_num_cpus} | " f"min_cpus=={minimum_cpu_per_job}"
             if model_estimate_memory_usage is not None:
-                error_msg += (
-                    f' | mem_available=={mem_available} | '
-                    f'model_estimate_memory_usage=={model_estimate_memory_usage}'
-                )
+                error_msg += f" | mem_available=={mem_available} | " f"model_estimate_memory_usage=={model_estimate_memory_usage}"
             raise AssertionError(error_msg)
         num_workers = max(minimum_cpu_per_job, cpu_per_job - 1)  # 1 cpu for master process
         cpu_per_worker = 1
-        resources_per_job = get_tune_resources(
-            num_workers=num_workers,
-            num_cpus_per_worker=cpu_per_worker,
-            use_gpu=False
-        )
+        resources_per_job = get_tune_resources(num_workers=num_workers, num_cpus_per_worker=cpu_per_worker, use_gpu=False)
         batches = math.ceil(num_jobs / num_parallel_jobs)
 
         resources_info = dict(
             resources_per_job=resources_per_job,
             num_parallel_jobs=num_parallel_jobs,
             batches=batches,
             cpu_per_job=cpu_per_job,
             num_workers=num_workers,
         )
-        logger.log(10, f'Resources info for {self.__class__.__name__}: {resources_info}')
+        logger.log(10, f"Resources info for {self.__class__.__name__}: {resources_info}")
 
         return resources_info
 
 
 class RayLightningGpuResourceCalculator(ResourceCalculator):
-
     @property
     def calc_type(self):
-        return 'ray_lightning_gpu'
+        return "ray_lightning_gpu"
 
     def get_resources_per_job(
         self,
         total_num_cpus,
         total_num_gpus,
         num_jobs,
         minimum_cpu_per_job,
         minimum_gpu_per_job,
         **kwargs,
     ):
         from ray_lightning.tune import get_tune_resources
-        # Ray Tune requires 1 additional CPU per trial to use for the Trainable driver. 
+
+        # Ray Tune requires 1 additional CPU per trial to use for the Trainable driver.
         # So the actual number of cpu resources each trial requires is num_workers * num_cpus_per_worker + 1
         # Each ray worker will reserve 1 gpu
         # The num_workers in ray stands for worker process to train the model
         # The num_workers in AutoMM stands for worker process to load data
         gpu_per_job = max(int(minimum_gpu_per_job), total_num_gpus // num_jobs)
         num_workers = gpu_per_job  # each worker uses 1 gpu
         num_parallel_jobs = min(num_jobs, total_num_gpus // gpu_per_job)
         if num_parallel_jobs == 0:
-            raise AssertionError('Cannot train model with provided resources! '
-                                 f'(num_cpus, num_gpus)==({total_num_cpus}, {total_num_gpus}) | '
-                                 f'(min_cpus, min_gpus)==({minimum_cpu_per_job}, {minimum_gpu_per_job})')
-        num_cpus = (total_num_cpus - num_parallel_jobs)  # reserve cpus for the master process
+            raise AssertionError(
+                "Cannot train model with provided resources! "
+                f"(num_cpus, num_gpus)==({total_num_cpus}, {total_num_gpus}) | "
+                f"(min_cpus, min_gpus)==({minimum_cpu_per_job}, {minimum_gpu_per_job})"
+            )
+        num_cpus = total_num_cpus - num_parallel_jobs  # reserve cpus for the master process
         assert num_cpus > 0
         cpu_per_job = max(minimum_cpu_per_job, num_cpus // num_parallel_jobs)
         cpu_per_worker = max(1, cpu_per_job // num_workers)
-        resources_per_job = get_tune_resources(
-            num_workers=num_workers,
-            num_cpus_per_worker=cpu_per_worker,
-            use_gpu=True
-        )
+        resources_per_job = get_tune_resources(num_workers=num_workers, num_cpus_per_worker=cpu_per_worker, use_gpu=True)
         batches = math.ceil(num_jobs / num_parallel_jobs)
 
         resources_info = dict(
             resources_per_job=resources_per_job,
             num_parallel_jobs=num_parallel_jobs,
             batches=batches,
             cpu_per_job=cpu_per_job,
             gpu_per_job=gpu_per_job,
             num_workers=num_workers,
             cpu_per_worker=cpu_per_worker,
         )
-        logger.log(10, f'Resources info for {self.__class__.__name__}: {resources_info}')
+        logger.log(10, f"Resources info for {self.__class__.__name__}: {resources_info}")
 
         return resources_info
 
 
 class ResourceCalculatorFactory:
 
     __supported_calculators = [
         CpuResourceCalculator,
         GpuResourceCalculator,
         NonParallelGpuResourceCalculator,
         RayLightningCpuResourceCalculator,
-        RayLightningGpuResourceCalculator
+        RayLightningGpuResourceCalculator,
     ]
     __type_to_calculator = {cls().calc_type: cls for cls in __supported_calculators}
 
     @staticmethod
     def get_resource_calculator(calculator_type: str) -> ResourceCalculator:
         """Return the resource calculator"""
-        assert calculator_type in ResourceCalculatorFactory.__type_to_calculator, f'{calculator_type} not supported'
+        assert calculator_type in ResourceCalculatorFactory.__type_to_calculator, f"{calculator_type} not supported"
         return ResourceCalculatorFactory.__type_to_calculator[calculator_type]()
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/scheduler/scheduler_factory.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/scheduler/scheduler_factory.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,21 @@
 from ..task.base import compile_scheduler_options_v2
 from ..task.base.base_task import schedulers
 
 logger = logging.getLogger(__name__)
 
 
 _scheduler_presets = {
-    'auto': {'scheduler': 'local', 'searcher': 'local_random'},
-    'local_random': {'scheduler': 'local', 'searcher': 'local_random'},
-    'random': {'scheduler': 'local', 'searcher': 'random'},
+    "auto": {"scheduler": "local", "searcher": "local_random"},
+    "local_random": {"scheduler": "local", "searcher": "local_random"},
+    "random": {"scheduler": "local", "searcher": "random"},
 }
 
 
-def scheduler_factory(
-        hyperparameter_tune_kwargs,
-        time_out: float = None,
-        num_trials: int = None,
-        nthreads_per_trial='all',
-        ngpus_per_trial='all',
-        **kwargs):
+def scheduler_factory(hyperparameter_tune_kwargs, time_out: float = None, num_trials: int = None, nthreads_per_trial="all", ngpus_per_trial="all", **kwargs):
     """
     Constructs a scheduler via lazy initialization based on the input hyperparameter_tune_kwargs.
     The output will contain the scheduler class and init arguments except for the `train_fn` argument, which must be specified downstream.
 
     Parameters
     ----------
     hyperparameter_tune_kwargs : str or dict
@@ -68,51 +62,52 @@
     """
     if hyperparameter_tune_kwargs is None:
         raise ValueError(f"hyperparameter_tune_kwargs cannot be None.")
     if isinstance(hyperparameter_tune_kwargs, str):
         hyperparameter_tune_kwargs = get_hyperparameter_tune_kwargs_preset(hyperparameter_tune_kwargs)
     if not isinstance(hyperparameter_tune_kwargs, dict):
         raise ValueError(f"hyperparameter_tune_kwargs must be of type str or dict, but is type: {type(hyperparameter_tune_kwargs)}")
-    if 'scheduler' not in hyperparameter_tune_kwargs:
+    if "scheduler" not in hyperparameter_tune_kwargs:
         raise ValueError(f"Required key 'scheduler' is not present in hyperparameter_tune_kwargs: {hyperparameter_tune_kwargs}")
-    if 'searcher' not in hyperparameter_tune_kwargs:
+    if "searcher" not in hyperparameter_tune_kwargs:
         raise ValueError(f"Required key 'searcher' is not present in hyperparameter_tune_kwargs: {hyperparameter_tune_kwargs}")
     if num_trials is None and time_out is not None:
         num_trials = 1000
 
     scheduler_params = compile_scheduler_options_v2(
         scheduler_options=hyperparameter_tune_kwargs,
         nthreads_per_trial=nthreads_per_trial,
         ngpus_per_trial=ngpus_per_trial,
         num_trials=num_trials,
         time_out=time_out,
         **kwargs,
     )
 
-    scheduler_cls = hyperparameter_tune_kwargs.get('scheduler', 'unknown')
+    scheduler_cls = hyperparameter_tune_kwargs.get("scheduler", "unknown")
     if isinstance(scheduler_cls, str):
         scheduler_cls = get_scheduler_from_preset(scheduler_cls)
     if not inspect.isclass(scheduler_cls):
-        raise ValueError(f'scheduler_cls must be a class, but was instead: {scheduler_cls}')
+        raise ValueError(f"scheduler_cls must be a class, but was instead: {scheduler_cls}")
 
-    if scheduler_params['time_out'] is None:
-        scheduler_params.pop('time_out', None)
+    if scheduler_params["time_out"] is None:
+        scheduler_params.pop("time_out", None)
     return scheduler_cls, scheduler_params
 
 
 def get_scheduler_from_preset(scheduler_cls):
     scheduler_cls = scheduler_cls.lower()
     if scheduler_cls not in schedulers.keys():
-        raise ValueError(f"Required key 'scheduler' in hyperparameter_tune_kwargs must be one of the "
-                         f"values {schedulers.keys()}, but was instead: {scheduler_cls}")
+        raise ValueError(
+            f"Required key 'scheduler' in hyperparameter_tune_kwargs must be one of the " f"values {schedulers.keys()}, but was instead: {scheduler_cls}"
+        )
     scheduler_cls = schedulers.get(scheduler_cls)
     return scheduler_cls
 
 
 def get_hyperparameter_tune_kwargs_preset(preset: str):
     # TODO: re-enable bayesopt after it's been implemented
-    if preset == 'bayesopt':
-        logger.warning(f'Bayesopt hyperparameter tuning is currently disabled. Will use random hyperparameter tuning instead.')
-        preset = 'random'
+    if preset == "bayesopt":
+        logger.warning(f"Bayesopt hyperparameter tuning is currently disabled. Will use random hyperparameter tuning instead.")
+        preset = "random"
     if preset not in _scheduler_presets:
         raise ValueError(f'Invalid hyperparameter_tune_kwargs preset value "{preset}". Valid presets: {list(_scheduler_presets.keys())}')
     return _scheduler_presets[preset].copy()
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/scheduler/seq_scheduler.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/scheduler/seq_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
-import time
 import os
+import time
 from collections import OrderedDict
 from copy import deepcopy
 from typing import Tuple
 
 from tqdm.auto import tqdm
 
-from .reporter import FakeReporter
 from ..searcher import searcher_factory
 from ..searcher.exceptions import ExhaustedSearchSpaceError
 from ..searcher.local_searcher import LocalSearcher
+from .reporter import FakeReporter
 
 logger = logging.getLogger(__name__)
 
 
 class LocalReporter:
     """
     Reporter implementation for LocalSequentialScheduler
@@ -28,37 +28,37 @@
         self.config_history = config_history
         self.trial_started = time.time()
         self.last_reported_time = self.trial_started
         self.last_result = None
 
     def __call__(self, *args, **kwargs):
         result = deepcopy(kwargs)
-        if 'done' not in result:
-            result['trial'] = self.trial
+        if "done" not in result:
+            result["trial"] = self.trial
 
             now = time.time()
-            result['time_this_iter'] = now - self.last_reported_time
-            result['time_since_start'] = now - self.trial_started
+            result["time_this_iter"] = now - self.last_reported_time
+            result["time_since_start"] = now - self.trial_started
             self.last_reported_time = now
 
             self.training_history[self.trial].append(result)
 
             if self.trial not in self.config_history:
                 self.config_history[self.trial] = self.searcher_config
-                if 'util_args' in self.searcher_config:
-                    self.searcher_config.pop('util_args')
+                if "util_args" in self.searcher_config:
+                    self.searcher_config.pop("util_args")
 
             self.last_result = result
 
     def terminate(self):
         pass  # compatibility
 
 
 class LocalSequentialScheduler(object):
-    """ Simple scheduler which schedules all HPO jobs in sequence without any parallelism.
+    """Simple scheduler which schedules all HPO jobs in sequence without any parallelism.
     The next trial scheduling will be decided based on the available time left within `time_out` setting
     and average time required for a trial to complete multiplied by the fill_factor (0.95) by default to
     accommodate variance in runtimes per HPO run.
 
     Parameters
     ----------
     train_fn : callable
@@ -82,117 +82,116 @@
     time_attr : str
         Name of resource (or time) attribute in data obtained from reporter.
         This attribute is optional for FIFO scheduling, but becomes mandatory
         in multi-fidelity scheduling (e.g., Hyperband).
         Note: The type of resource must be int.
     """
 
-    def __init__(self, train_fn, search_space, train_fn_kwargs=None, searcher='auto', reward_attr='reward', resource=None, **kwargs):
+    def __init__(self, train_fn, search_space, train_fn_kwargs=None, searcher="auto", reward_attr="reward", resource=None, **kwargs):
         self.train_fn = train_fn
         self.training_history = None
         self.config_history = None
         self._reward_attr = reward_attr
-        self.time_attr = kwargs.get('time_attr', None)
+        self.time_attr = kwargs.get("time_attr", None)
         self.resource = resource
-        self.max_reward = kwargs.get('max_reward', None)
+        self.max_reward = kwargs.get("max_reward", None)
         self.searcher: LocalSearcher = self.get_searcher_(searcher, train_fn, search_space=search_space, **kwargs)
         self.init_limits_(kwargs)
         self.train_fn_kwargs = train_fn_kwargs
         self.metadata = {
-            'search_space': search_space,
-            'search_strategy': self.searcher,
-            'stop_criterion': {
-                'time_limits': self.time_out,
-                'max_reward': self.max_reward},
-            'resources_per_trial': self.resource
+            "search_space": search_space,
+            "search_strategy": self.searcher,
+            "stop_criterion": {"time_limits": self.time_out, "max_reward": self.max_reward},
+            "resources_per_trial": self.resource,
         }
 
     def init_limits_(self, kwargs):
-        if kwargs.get('num_trials', None) is None:
-            assert kwargs.get('time_out', None) is not None, "Need stopping criterion: Either num_trials or time_out"
-        self.num_trials = kwargs.get('num_trials', 9999)
-        self.time_out = kwargs.get('time_out', None)
+        if kwargs.get("num_trials", None) is None:
+            assert kwargs.get("time_out", None) is not None, "Need stopping criterion: Either num_trials or time_out"
+        self.num_trials = kwargs.get("num_trials", 9999)
+        self.time_out = kwargs.get("time_out", None)
         if self.num_trials is None:
             assert self.time_out is not None, "Need stopping criterion: Either num_trials or time_out"
 
     def get_searcher_(self, searcher, train_fn, search_space, **kwargs) -> LocalSearcher:
         scheduler_opts = {}
-        if searcher == 'auto':
-            searcher = 'local_random'
-            scheduler_opts = {'scheduler': 'local'}
-        elif searcher == 'random':
+        if searcher == "auto":
+            searcher = "local_random"
+            scheduler_opts = {"scheduler": "local"}
+        elif searcher == "random":
             # FIXME: Hack to be compatible with gluoncv
-            searcher = 'local_random'
+            searcher = "local_random"
 
-        search_options = kwargs.get('search_options', None)
+        search_options = kwargs.get("search_options", None)
         if isinstance(searcher, str):
             if search_options is None:
                 search_options = dict()
             _search_options = search_options.copy()
-            _search_options['search_space'] = search_space
-            _search_options['reward_attribute'] = self._reward_attr
+            _search_options["search_space"] = search_space
+            _search_options["reward_attribute"] = self._reward_attr
             # Adjoin scheduler info to search_options, if not already done by
             # subclass
-            if 'scheduler' not in _search_options:
-                _search_options['scheduler'] = 'local'
+            if "scheduler" not in _search_options:
+                _search_options["scheduler"] = "local"
             searcher = searcher_factory(searcher, **{**scheduler_opts, **_search_options})
         else:
             assert isinstance(searcher, LocalSearcher)
         return searcher
 
     def run(self, **kwargs):
-        """Run multiple trials given specific time and trial numbers limits.
-        """
+        """Run multiple trials given specific time and trial numbers limits."""
         self.searcher.configure_scheduler(self)
 
         self.training_history = OrderedDict()
         self.config_history = OrderedDict()
 
         failure_count = 0
         trial_count = 0
         trials_total_time = 0
         min_failure_threshold = 5
         failure_rate_threshold = 0.8
         time_start = time.time()
 
         r = range(self.num_trials)
-        for i in (tqdm(r) if self.num_trials < 1000 else r):
+        for i in tqdm(r) if self.num_trials < 1000 else r:
             trial_start_time = time.time()
             try:
                 is_failed, result = self.run_trial(task_id=i)
             except ExhaustedSearchSpaceError:
                 break
             except Exception:
                 # TODO: Add special exception type when there are no more new configurations to try (exhausted search space)
-                logger.log(30, f'\tWARNING: Encountered unexpected exception during trial {i}, stopping HPO early.')
-                logger.exception('Detailed Traceback:')  # TODO: Avoid logging if verbosity=0
+                logger.log(30, f"\tWARNING: Encountered unexpected exception during trial {i}, stopping HPO early.")
+                logger.exception("Detailed Traceback:")  # TODO: Avoid logging if verbosity=0
                 break
             trial_end_time = time.time()
 
             trial_count += 1
             if is_failed:
                 failure_count += 1
             else:
                 trials_total_time += trial_end_time - trial_start_time
 
             if self.max_reward and self.get_best_reward() >= self.max_reward:
-                logger.log(20, f'\tStopping HPO: Max reward reached')
+                logger.log(20, f"\tStopping HPO: Max reward reached")
                 break
 
             if failure_count >= min_failure_threshold and (failure_count / trial_count) >= failure_rate_threshold:
-                logger.warning(f'Warning: Detected a large trial failure rate: '
-                               f'{failure_count}/{trial_count} attempted trials failed ({round((failure_count / trial_count) * 100, 1)}%)! '
-                               f'Stopping HPO early due to reaching failure threshold ({round(failure_rate_threshold*100, 1)}%).\n'
-                               f'\tFailures may be caused by invalid configurations within the provided search space.')
+                logger.warning(
+                    f"Warning: Detected a large trial failure rate: "
+                    f"{failure_count}/{trial_count} attempted trials failed ({round((failure_count / trial_count) * 100, 1)}%)! "
+                    f"Stopping HPO early due to reaching failure threshold ({round(failure_rate_threshold*100, 1)}%).\n"
+                    f"\tFailures may be caused by invalid configurations within the provided search space."
+                )
                 break
 
             if self.time_out is not None:
                 avg_trial_run_time = 0 if trial_count == failure_count else trials_total_time / (trial_count - failure_count)
                 if not self.has_enough_time_for_trial_(self.time_out, time_start, trial_start_time, trial_end_time, avg_trial_run_time):
-                    logger.log(20, f'\tStopping HPO to satisfy time limit...')
+                    logger.log(20, f"\tStopping HPO to satisfy time limit...")
                     break
 
     @classmethod
     def has_enough_time_for_trial_(cls, time_out, time_start, trial_start_time, trial_end_time, avg_trial_run_time, fill_factor=0.95):
         """
         Checks if the remaining time is enough to run another trial.
 
@@ -249,94 +248,91 @@
         trial_start_time
             Trial start time
         trial_end_time
             Trial end time
 
         """
         new_searcher_config = self.searcher.get_config()
-        searcher_config = deepcopy(self.metadata['search_space'])
+        searcher_config = deepcopy(self.metadata["search_space"])
         searcher_config.update(new_searcher_config)
         reporter = LocalReporter(task_id, searcher_config, self.training_history, self.config_history)
         return self.run_job_(task_id, searcher_config, reporter)
 
     def run_job_(self, task_id, searcher_config, reporter):
         args = dict()
         if self.train_fn_kwargs is not None:
             # TODO: Consider avoiding deepcopy and just do shallow copy,
             #  Risk is that it will allow values in self.train_fn_kwargs to be altered by HPO trials, causing early trials to alter later trials.
             train_fn_kwargs = deepcopy(self.train_fn_kwargs)
         else:
             train_fn_kwargs = dict()
         args.update(searcher_config)
 
-        args['task_id'] = task_id
+        args["task_id"] = task_id
         self.searcher.register_pending(searcher_config)
         is_failed = False
         try:
             result = self.train_fn(args, reporter=reporter, **train_fn_kwargs)
             if type(reporter) is not FakeReporter:
                 if reporter.last_result:
                     self.searcher.update(config=searcher_config, **reporter.last_result)
                 else:
                     is_failed = True
         except Exception as e:
-            logger.error(f'Exception during a trial: {e}')
+            logger.error(f"Exception during a trial: {e}")
             self.searcher.evaluation_failed(config=searcher_config)
             reporter(traceback=e)
             is_failed = True
-            result = {'traceback': str(e)}
+            result = {"traceback": str(e)}
         return is_failed, result
 
     def run_with_config(self, config):
         """Run with config for final fit.
         It launches a single training trial under any fixed values of the hyperparameters.
         For example, after HPO has identified the best hyperparameter values based on a hold-out dataset,
         one can use this function to retrain a model with the same hyperparameters on all the available labeled data
         (including the hold out set). It can also returns other objects or states.
         """
-        is_failed, result = self.run_job_('run_with_config', config, FakeReporter())
+        is_failed, result = self.run_job_("run_with_config", config, FakeReporter())
         return result
 
     def join_jobs(self, timeout=None):
         pass  # Compatibility
 
     def get_best_config(self):
-        """Get the best configuration from the finished jobs.
-        """
+        """Get the best configuration from the finished jobs."""
         # TODO: Consider passing the metadata search space to searcher to avoid having to do this
-        searcher_config = deepcopy(self.metadata['search_space'])
+        searcher_config = deepcopy(self.metadata["search_space"])
         searcher_config.update(self.searcher.get_best_config())
         return searcher_config
 
     def get_best_reward(self):
-        """Get the best reward from the finished jobs.
-        """
+        """Get the best reward from the finished jobs."""
         return self.searcher.get_best_reward()
 
     def get_training_curves(self, filename=None, plot=False, use_legend=True):
-        """Get Training Curves
-        """
+        """Get Training Curves"""
         if filename is None and not plot:
-            logger.warning('Please either provide filename or allow plot in get_training_curves')
+            logger.warning("Please either provide filename or allow plot in get_training_curves")
         import matplotlib.pyplot as plt
 
-        eval_metric = self.__get_training_history_metric('eval_metric', default='validation_performance')
-        sign_mult = int(self.__get_training_history_metric('greater_is_better', default=True)) * 2 - 1
+        eval_metric = self.__get_training_history_metric("eval_metric", default="validation_performance")
+        sign_mult = int(self.__get_training_history_metric("greater_is_better", default=True)) * 2 - 1
 
         plt.ylabel(eval_metric)
         plt.xlabel(self.time_attr)
         plt.title("Performance vs Training-Time in each HPO Trial")
         for task_id, task_res in self.training_history.items():
             rewards = [x[self._reward_attr] * sign_mult for x in task_res]
             x = [x[self.time_attr] for x in task_res]
-            plt.plot(x, rewards, label=f'task {task_id}')
+            plt.plot(x, rewards, label=f"task {task_id}")
         if use_legend:
-            plt.legend(loc='best')
+            plt.legend(loc="best")
         if filename:
-            logger.info(f'Saving Training Curve in {filename}')
+            logger.info(f"Saving Training Curve in {filename}")
             file_dir = os.path.split(os.path.abspath(filename))[0]
             if not os.path.exists(file_dir):
                 os.makedirs(file_dir)
             plt.savefig(filename)
         if plot:
             plt.show()
 
@@ -351,9 +347,8 @@
 
         If there are duplicated configurations, we return the id of the first one.
         """
         best_config = self.get_best_config()
         for task_id, config in self.config_history.items():
             if best_config == config:
                 return task_id
-        raise RuntimeError('The best config {} is not found in config history = {}. '
-                           'This should never happen!'.format(best_config, self.config_history))
+        raise RuntimeError("The best config {} is not found in config history = {}. " "This should never happen!".format(best_config, self.config_history))
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/dummy_searcher.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/dummy_searcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import logging
 
-from .local_searcher import LocalSearcher
 from .exceptions import ExhaustedSearchSpaceError
+from .local_searcher import LocalSearcher
 
-__all__ = ['DummySearcher']
+__all__ = ["DummySearcher"]
 
 logger = logging.getLogger(__name__)
 
 
 class DummySearcher(LocalSearcher):
     """Searcher which only returns the default config."""
+
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self._exhausted = False
 
     def get_config(self, **kwargs) -> dict:
         if self._exhausted:
-            raise ExhaustedSearchSpaceError('Default config already provided. Search space is exhausted!')
+            raise ExhaustedSearchSpaceError("Default config already provided. Search space is exhausted!")
         self._exhausted = True
         return self._params_default
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/local_grid_searcher.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/local_grid_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import numpy as np
 from sklearn.model_selection import ParameterGrid
 
 from autogluon.common import space as ag_space
 
 from .local_searcher import LocalSearcher
 
-
-__all__ = ['LocalGridSearcher']
+__all__ = ["LocalGridSearcher"]
 
 logger = logging.getLogger(__name__)
 
 
 class LocalGridSearcher(LocalSearcher):
     """
     Grid Searcher that exhaustively tries all possible configurations. Grid with Int/Real ignores 'default' values in search spaces.
@@ -62,17 +61,17 @@
             samples = self._grid_num_sample_settings.get(key, samples)
         return samples
 
     def __len__(self):
         return self._grid_length - self._grid_index
 
     def get_config(self):
-        """ Return new hyperparameter configuration to try next."""
+        """Return new hyperparameter configuration to try next."""
         if len(self) <= 0:
-            raise AssertionError(f'No configs left to get. All {self._grid_length} configs have been accessed already.')
+            raise AssertionError(f"No configs left to get. All {self._grid_length} configs have been accessed already.")
         config = self._params_grid[self._grid_index]
         self._grid_index += 1
         for key, val in config.items():
             # If this isn't done, warnings are spammed in XGBoost
             if isinstance(val, np.int64):
                 config[key] = int(val)
             elif isinstance(val, np.float64):
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/local_random_searcher.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/local_random_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import logging
 
 import numpy as np
 from sklearn.model_selection import ParameterSampler
 
 from autogluon.common import space
 
-from .local_searcher import LocalSearcher
 from .exceptions import ExhaustedSearchSpaceError
+from .local_searcher import LocalSearcher
 
-
-__all__ = ['LocalRandomSearcher']
+__all__ = ["LocalRandomSearcher"]
 
 logger = logging.getLogger(__name__)
 
 
 class LocalRandomSearcher(LocalSearcher):
     """Searcher which randomly samples configurations to try next."""
+
     MAX_RETRIES = 100
 
     def __init__(self, *, first_is_default=True, random_seed=0, **kwargs):
         super().__init__(**kwargs)
         self._first_is_default = first_is_default
         # We use an explicit random_state here, in order to better support checkpoint and resume
         self.random_state = np.random.RandomState(random_seed)
@@ -67,14 +67,14 @@
         else:
             new_config = self._sample_config()
         num_tries = 1
         while self._pickle_config(new_config) in self._results:
             if num_tries > self.MAX_RETRIES:
                 if self._num_configs is not None:
                     num_results = len(self._results)
-                    logger.log(30, f'Stopping HPO due to exhausted search space: {num_results} of {self._num_configs} possible configs ran.')
+                    logger.log(30, f"Stopping HPO due to exhausted search space: {num_results} of {self._num_configs} possible configs ran.")
                     raise ExhaustedSearchSpaceError
                 assert num_tries <= self.MAX_RETRIES, f"Cannot find new config in LocalRandomSearcher, even after {self.MAX_RETRIES} trials"
             new_config = self._sample_config()
             num_tries += 1
         self._add_result(new_config, self._reward_while_pending())
         return new_config
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/local_searcher.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/local_searcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import logging
 import pickle
-
-from autogluon.common import space
-
 from collections import OrderedDict
 
+from autogluon.common import space
 
-__all__ = ['LocalSearcher']
+__all__ = ["LocalSearcher"]
 
 logger = logging.getLogger(__name__)
 
 
 class LocalSearcher(object):
     """Local Searcher (virtual class to inherit from if you are creating a custom Searcher).
 
     Parameters
     ----------
     search_space: dict
         The configuration space to sample from. It contains the full
         specification of the Hyperparameters with their priors
     """
-    def __init__(self, search_space: dict, reward_attribute: str = 'reward', **kwargs):
+
+    def __init__(self, search_space: dict, reward_attribute: str = "reward", **kwargs):
         """
         :param search_space: Configuration space to sample from or search in
         :param reward_attribute: Reward attribute passed to update.
             Default: 'reward'
 
         """
         self.search_space = search_space
@@ -47,14 +46,15 @@
 
         Args:
             scheduler: TaskScheduler
                 Scheduler the searcher is used with.
 
         """
         from ..scheduler.seq_scheduler import LocalSequentialScheduler
+
         if isinstance(scheduler, LocalSequentialScheduler):
             self._reward_attribute = scheduler._reward_attr
 
     @staticmethod
     def _reward_while_pending():
         """Defines the reward value which is assigned to config, while it is pending."""
         return float("-inf")
@@ -66,15 +66,15 @@
 
         Args:
         kwargs:
             Extra information may be passed from scheduler to searcher
         returns: (config, info_dict)
             must return a valid configuration and a (possibly empty) info dict
         """
-        raise NotImplementedError(f'This function needs to be overwritten in {self.__class__.__name__}.')
+        raise NotImplementedError(f"This function needs to be overwritten in {self.__class__.__name__}.")
 
     def update(self, config: dict, **kwargs):
         """
         Update the searcher with the newest metric report.
         Will error if config contains unknown parameters, values outside the valid search space, or is missing parameters.
         """
         reward = kwargs.get(self._reward_attribute, None)
@@ -100,30 +100,28 @@
         searcher should react appropriately (e.g., remove pending evaluations
         for this config, and blacklist config).
         """
         pass
 
     def get_best_reward(self):
         """Calculates the reward (i.e. validation performance) produced by training under the best configuration identified so far.
-           Assumes higher reward values indicate better performance.
+        Assumes higher reward values indicate better performance.
         """
         if self._results:
             return max(self._results.values())
         return self._reward_while_pending()
 
     def get_reward(self, config):
-        """Calculates the reward (i.e. validation performance) produced by training with the given configuration.
-        """
+        """Calculates the reward (i.e. validation performance) produced by training with the given configuration."""
         config_pkl = self._pickle_config(config=config)
         assert config_pkl in self._results
         return self._results[config_pkl]
 
     def get_best_config(self):
-        """Returns the best configuration found so far.
-        """
+        """Returns the best configuration found so far."""
         if self._results:
             config_pkl = max(self._results, key=self._results.get)
             return self._unpickle_config(config_pkl=config_pkl)
         else:
             return dict()
 
     def get_results(self, sort=True) -> list:
@@ -185,17 +183,17 @@
     def _add_result(self, config: dict, result: float):
         assert isinstance(result, (float, int)), f"result must be a float or int! Was instead {type(result)} | Value: {result}"
         config_pkl = self._pickle_config(config=config)
         self._results[config_pkl] = result
 
     def _pickle_config(self, config: dict) -> bytes:
         assert isinstance(config, dict), f"config must be a dict! Was instead {type(config)} | Value: {config}"
-        assert len(config) == len(self._params_order), f'Config length does not match expected params count!\n' \
-                                                       f'Expected: {self._params_order}\n' \
-                                                       f'Actual:   {list(config.keys())}'
+        assert len(config) == len(self._params_order), (
+            f"Config length does not match expected params count!\n" f"Expected: {self._params_order}\n" f"Actual:   {list(config.keys())}"
+        )
 
         # Note: This code is commented out because it can be computationally and memory expensive if user sends large objects in search space, such as datasets.
         """
         for key in self._params_static:
             assert pickle.dumps(config[key]) == pickle.dumps(self._params_static[key]), \
                 f'Invalid config value for search space parameter "{key}" | Invalid Value: {config[key]} | Expected Value: {self._params_static[key]}'
         """
@@ -203,16 +201,18 @@
         for key in self._params_order:
             if key in self._params_static:
                 pass
             elif key in self._params_cat_dict:
                 try:
                     cat_idx = self._params_cat_dict[key][pickle.dumps(config[key])]
                 except KeyError:
-                    raise AssertionError(f'Invalid config value for search space parameter "{key}" | '
-                                         f'Invalid Value: {config[key]} | Valid Values: {self.search_space[key].data}')
+                    raise AssertionError(
+                        f'Invalid config value for search space parameter "{key}" | '
+                        f"Invalid Value: {config[key]} | Valid Values: {self.search_space[key].data}"
+                    )
                 config_to_pkl.append(cat_idx)
             else:
                 config_to_pkl.append(config[key])
         return pickle.dumps(config_to_pkl)
 
     def _unpickle_config(self, config_pkl: bytes) -> dict:
         assert isinstance(config_pkl, bytes), f"config_pkl must be a bytes object! Was instead {type(config_pkl)} | Value: {config_pkl}"
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/searcher/searcher_factory.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/searcher/searcher_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from .local_grid_searcher import LocalGridSearcher
 from .local_random_searcher import LocalRandomSearcher
 
-__all__ = ['searcher_factory']
+__all__ = ["searcher_factory"]
 
 SEARCHER_CONFIGS = dict(
-    local_random=dict(
-        searcher_cls=LocalRandomSearcher
-    ),
+    local_random=dict(searcher_cls=LocalRandomSearcher),
     local_grid=dict(
         searcher_cls=LocalGridSearcher,
     ),
     # Fall back to random search since Bayes searcher is not supported
-    bayes=dict(
-        searcher_cls=LocalRandomSearcher
-    ),
+    bayes=dict(searcher_cls=LocalRandomSearcher),
 )
 
 
 def searcher_factory(searcher_name, **kwargs):
     """Factory for searcher objects
 
     This function creates searcher objects from string argument name and
@@ -49,24 +45,23 @@
     See Also
     --------
     GPFIFOSearcher
     GPMultiFidelitySearcher
     """
     if searcher_name in SEARCHER_CONFIGS:
         searcher_config = SEARCHER_CONFIGS[searcher_name]
-        searcher_cls = searcher_config['searcher_cls']
-        scheduler = kwargs.get('scheduler')
+        searcher_cls = searcher_config["searcher_cls"]
+        scheduler = kwargs.get("scheduler")
 
         # Check if searcher_cls is a lambda - evaluate then
         if isinstance(searcher_cls, type(lambda: 0)):
             searcher_cls = searcher_cls(scheduler)
 
-        if 'supported_schedulers' in searcher_config:
-            supported_schedulers = searcher_config['supported_schedulers']
+        if "supported_schedulers" in searcher_config:
+            supported_schedulers = searcher_config["supported_schedulers"]
             assert scheduler is not None, "Scheduler must set search_options['scheduler']"
-            assert scheduler in supported_schedulers, \
-                f"Searcher '{searcher_name}' only works with schedulers {supported_schedulers} (not with '{scheduler}')"
+            assert scheduler in supported_schedulers, f"Searcher '{searcher_name}' only works with schedulers {supported_schedulers} (not with '{scheduler}')"
 
         searcher = searcher_cls(**kwargs)
         return searcher
     else:
-        raise AssertionError(f'searcher \'{searcher_name}\' is not supported')
+        raise AssertionError(f"searcher '{searcher_name}' is not supported")
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/space.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/space.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # TODO: Remove this file for v1.0 as space is moved to common
-import warnings
 import sys
-
+import warnings
 from typing import Any
 
-
 this_module = sys.modules[__name__]
 spaces = ["Space", "Categorical", "Real", "Int", "Bool"]
 
 
 class DeprecatedSpaceWrapper:
     def __init__(self, common_space) -> None:
         self.comomn_space = common_space
-    
+
     def __call__(self, *args, **kwargs) -> Any:
         from autogluon.common import space
 
         warnings.warn(
             "Accessing search spaces through `autogluon.core` is deprecated as of v0.8 and won't be supported "
             f"in the next release. Please use `from autogluon.common import {self.comomn_space}` instead."
         )
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/task/base/base_task.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/task/base/base_task.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,18 @@
 import time
 from abc import abstractmethod
 
 from ...scheduler.seq_scheduler import LocalSequentialScheduler
 from ...utils import in_ipynb
 from ...utils.utils import setup_compute
 
-__all__ = [
-    'BaseTask',
-    'compile_scheduler_options_v2',
-    'create_scheduler']
+__all__ = ["BaseTask", "compile_scheduler_options_v2", "create_scheduler"]
 
 schedulers = {
-    'local': LocalSequentialScheduler,
+    "local": LocalSequentialScheduler,
 }
 
 logger = logging.getLogger(__name__)
 
 
 def create_scheduler(train_fn, search_space, scheduler, scheduler_options, train_fn_kwargs=None):
     if isinstance(scheduler, str):
@@ -28,57 +25,72 @@
         scheduler_options = copy.copy(scheduler_options)
     return scheduler_cls(train_fn, search_space=search_space, train_fn_kwargs=train_fn_kwargs, **scheduler_options)
 
 
 # FIXME: REMOVE THIS, first GluonCV needs to stop depending on AG, as it imports this class
 class BaseTask(object):
     """BaseTask for AutoGluon applications"""
+
     @classmethod
-    def run_fit(cls, train_fn, search_space, search_strategy, scheduler_options, train_fn_kwargs=None,
-                plot_results=False):
+    def run_fit(cls, train_fn, search_space, search_strategy, scheduler_options, train_fn_kwargs=None, plot_results=False):
         start_time = time.time()
         # create scheduler and schedule tasks
         scheduler = create_scheduler(train_fn, search_space, search_strategy, scheduler_options, train_fn_kwargs=train_fn_kwargs)
         scheduler.run()
         scheduler.join_jobs()
         # gather the best configuration
         best_reward = scheduler.get_best_reward()
         best_config = scheduler.get_best_config()
         best_config_run = {**best_config}
-        best_config_run['final_fit'] = True
-        if hasattr(best_config_run, 'epochs') and hasattr(best_config_run, 'final_fit_epochs'):
-            best_config_run['epochs'] = best_config_run['final_fit_epochs']
+        best_config_run["final_fit"] = True
+        if hasattr(best_config_run, "epochs") and hasattr(best_config_run, "final_fit_epochs"):
+            best_config_run["epochs"] = best_config_run["final_fit_epochs"]
         scheduler_final = create_scheduler(train_fn, search_space, search_strategy, scheduler_options, train_fn_kwargs=train_fn_kwargs)
         results = scheduler_final.run_with_config(best_config_run)
         total_time = time.time() - start_time
         if plot_results or in_ipynb():
-            plot_training_curves = scheduler_options['checkpoint'].replace('exp1.ag', 'plot_training_curves.png')
+            plot_training_curves = scheduler_options["checkpoint"].replace("exp1.ag", "plot_training_curves.png")
             scheduler.get_training_curves(filename=plot_training_curves, plot=True, use_legend=False)
         if results is None:
-            logger.warning('No valid results obtained with best config, the result may not be useful...')
+            logger.warning("No valid results obtained with best config, the result may not be useful...")
             results = {}
-        results.update(best_reward=best_reward,
-                       best_config=best_config,
-                       total_time=total_time,
-                       metadata=scheduler.metadata,
-                       training_history=scheduler.training_history,
-                       config_history=scheduler.config_history,
-                       reward_attr=scheduler._reward_attr)
+        results.update(
+            best_reward=best_reward,
+            best_config=best_config,
+            total_time=total_time,
+            metadata=scheduler.metadata,
+            training_history=scheduler.training_history,
+            config_history=scheduler.config_history,
+            reward_attr=scheduler._reward_attr,
+        )
         return results
 
     @classmethod
     @abstractmethod
     def fit(cls, *args, **kwargs):
         pass
 
 
 def compile_scheduler_options_v2(
-        scheduler_options, nthreads_per_trial,
-        ngpus_per_trial, num_trials, time_out, scheduler=None, search_strategy=None, search_options=None, checkpoint=None, resume=False, visualizer=None,
-        time_attr=None, reward_attr=None, dist_ip_addrs=None, epochs=None):
+    scheduler_options,
+    nthreads_per_trial,
+    ngpus_per_trial,
+    num_trials,
+    time_out,
+    scheduler=None,
+    search_strategy=None,
+    search_options=None,
+    checkpoint=None,
+    resume=False,
+    visualizer=None,
+    time_attr=None,
+    reward_attr=None,
+    dist_ip_addrs=None,
+    epochs=None,
+):
     """
     Updates a copy of scheduler_options (scheduler-specific options, can be
     empty) with general options. The result can be passed to __init__ of the
     scheduler.
 
     Special role of epochs for HyperbandScheduler: If the search_strategy
     involves HyperbandScheduler and epochs is given, then this value is
@@ -109,68 +121,67 @@
         scheduler_options = dict()
     else:
         assert isinstance(scheduler_options, dict)
     scheduler_options = copy.copy(scheduler_options)
     if dist_ip_addrs is None:
         dist_ip_addrs = []
     if search_strategy is None:
-        search_strategy = 'random'
+        search_strategy = "random"
     if scheduler is None:
-        scheduler = 'local'
+        scheduler = "local"
     assert isinstance(search_strategy, str)
     if search_options is None:
         search_options = dict()
     if visualizer is None:
-        visualizer = 'none'
+        visualizer = "none"
     if time_attr is None:
-        time_attr = 'epoch'
+        time_attr = "epoch"
     if reward_attr is None:
-        reward_attr = 'validation_performance'
+        reward_attr = "validation_performance"
     scheduler_params = {
-        'resource': {
-            'num_cpus': nthreads_per_trial, 'num_gpus': ngpus_per_trial},
-        'scheduler': scheduler,
-        'searcher': search_strategy,
-        'search_options': search_options,
-        'checkpoint': checkpoint,
-        'resume': resume,
-        'num_trials': num_trials,
-        'time_out': time_out,
-        'reward_attr': reward_attr,
-        'time_attr': time_attr,
-        'visualizer': visualizer,
-        'dist_ip_addrs': dist_ip_addrs,
+        "resource": {"num_cpus": nthreads_per_trial, "num_gpus": ngpus_per_trial},
+        "scheduler": scheduler,
+        "searcher": search_strategy,
+        "search_options": search_options,
+        "checkpoint": checkpoint,
+        "resume": resume,
+        "num_trials": num_trials,
+        "time_out": time_out,
+        "reward_attr": reward_attr,
+        "time_attr": time_attr,
+        "visualizer": visualizer,
+        "dist_ip_addrs": dist_ip_addrs,
     }
     resource = None
-    if 'resource' in scheduler_options:
-        scheduler_params['resource'].update(scheduler_options['resource'])
-        resource = scheduler_params['resource'].copy()
+    if "resource" in scheduler_options:
+        scheduler_params["resource"].update(scheduler_options["resource"])
+        resource = scheduler_params["resource"].copy()
     scheduler_params.update(scheduler_options)
     if resource:
-        scheduler_params['resource'] = resource
+        scheduler_params["resource"] = resource
 
-    scheduler_params['resource']['num_cpus'], scheduler_params['resource']['num_gpus'] = setup_compute(
-        nthreads_per_trial=scheduler_params['resource']['num_cpus'],
-        ngpus_per_trial=scheduler_params['resource']['num_gpus'],
+    scheduler_params["resource"]["num_cpus"], scheduler_params["resource"]["num_gpus"] = setup_compute(
+        nthreads_per_trial=scheduler_params["resource"]["num_cpus"],
+        ngpus_per_trial=scheduler_params["resource"]["num_gpus"],
     )  # TODO: use 'auto' downstream
 
     required_options = [
-        'resource',
-        'scheduler',
-        'searcher',
-        'search_options',
-        'checkpoint',
-        'resume',
-        'num_trials',
-        'time_out',
-        'reward_attr',
-        'time_attr',
-        'visualizer',
-        'dist_ip_addrs',
+        "resource",
+        "scheduler",
+        "searcher",
+        "search_options",
+        "checkpoint",
+        "resume",
+        "num_trials",
+        "time_out",
+        "reward_attr",
+        "time_attr",
+        "visualizer",
+        "dist_ip_addrs",
     ]
     missing_options = []
     for option in required_options:
         if option not in scheduler_params:
             missing_options.append(option)
     if missing_options:
-        raise AssertionError(f'Missing required keys in scheduler_options: {missing_options}')
+        raise AssertionError(f"Missing required keys in scheduler_options: {missing_options}")
     return scheduler_params
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/trainer/abstract_trainer.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/trainer/abstract_trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,86 +1,138 @@
 from __future__ import annotations
 
 import copy
 import logging
 import os
+import shutil
 import time
 from collections import defaultdict
-from typing import Dict, List, Union, Tuple, Optional
+from pathlib import Path
+from typing import Dict, List, Optional, Tuple, Union
 
 import networkx as nx
 import numpy as np
 import pandas as pd
-import shutil
-from pathlib import Path
 
 from autogluon.common.features.feature_metadata import FeatureMetadata
 from autogluon.common.utils.lite import disable_if_lite_mode
 from autogluon.common.utils.log_utils import convert_time_in_s_to_log_friendly
 from autogluon.common.utils.path_converter import PathConverter
 from autogluon.common.utils.resource_utils import ResourceManager
 from autogluon.common.utils.try_import import try_import_torch
 
-from .utils import process_hyperparameters
-from ..augmentation.distill_utils import format_distillation_labels, augment_data
+from ..augmentation.distill_utils import augment_data, format_distillation_labels
 from ..calibrate import calibrate_decision_threshold
 from ..calibrate.conformity_score import compute_conformity_score
 from ..calibrate.temperature_scaling import tune_temperature_scaling
-from ..constants import AG_ARGS, BINARY, MULTICLASS, REGRESSION, QUANTILE, SOFTCLASS, REFIT_FULL_NAME, REFIT_FULL_SUFFIX
+from ..constants import (
+    AG_ARGS,
+    BINARY,
+    MULTICLASS,
+    QUANTILE,
+    REFIT_FULL_NAME,
+    REFIT_FULL_SUFFIX,
+    REGRESSION,
+    SOFTCLASS,
+)
 from ..data.label_cleaner import LabelCleanerMulticlassToBinary
-from ..metrics import get_metric, Scorer
-from ..models import AbstractModel, BaggedEnsembleModel, StackerEnsembleModel, WeightedEnsembleModel, GreedyWeightedEnsembleModel, SimpleWeightedEnsembleModel
-from ..utils import default_holdout_frac, get_pred_from_proba, generate_train_test_split, infer_eval_metric, compute_permutation_feature_importance, \
-    extract_column, compute_weighted_metric, convert_pred_probas_to_df
-from ..utils.exceptions import TimeLimitExceeded, NotEnoughMemoryError, NoValidFeatures, NoGPUError, NotEnoughCudaMemoryError
+from ..metrics import Scorer, get_metric
+from ..models import (
+    AbstractModel,
+    BaggedEnsembleModel,
+    GreedyWeightedEnsembleModel,
+    SimpleWeightedEnsembleModel,
+    StackerEnsembleModel,
+    WeightedEnsembleModel,
+)
+from ..utils import (
+    compute_permutation_feature_importance,
+    compute_weighted_metric,
+    convert_pred_probas_to_df,
+    default_holdout_frac,
+    extract_column,
+    generate_train_test_split,
+    get_pred_from_proba,
+    infer_eval_metric,
+)
+from ..utils.exceptions import (
+    NoGPUError,
+    NotEnoughCudaMemoryError,
+    NotEnoughMemoryError,
+    NoValidFeatures,
+    TimeLimitExceeded,
+)
+from ..utils.feature_selection import FeatureSelector
 from ..utils.loaders import load_pkl
 from ..utils.savers import save_json, save_pkl
-from ..utils.feature_selection import FeatureSelector
+from .utils import process_hyperparameters
 
 logger = logging.getLogger(__name__)
 
 
 # FIXME: Below is major defect!
 #  Weird interaction for metrics like AUC during bagging.
 #  If kfold = 5, scores are 0.9, 0.85, 0.8, 0.75, and 0.7, the score is not 0.8! It is much lower because probs are combined together and AUC is recalculated
 #  Do we want this to happen? Should we calculate score by 5 separate scores and then averaging instead?
 
 # TODO: Dynamic model loading for ensemble models during prediction, only load more models if prediction is uncertain. This dynamically reduces inference time.
 # TODO: Try midstack Semi-Supervised. Just take final models and re-train them, use bagged preds for SS rows. This would be very cheap and easy to try.
 # TODO: Move to autogluon.core
 class AbstractTrainer:
-    trainer_file_name = 'trainer.pkl'
-    trainer_info_name = 'info.pkl'
-    trainer_info_json_name = 'info.json'
-    distill_stackname = 'distill'  # name of stack-level for distilled student models
-
-    def __init__(self, path: str, problem_type: str, eval_metric=None,
-                 num_classes=None, quantile_levels=None, low_memory=False, feature_metadata=None, k_fold=0, n_repeats=1,
-                 sample_weight=None, weight_evaluation=False, save_data=False, random_state=0, verbosity=2):
+    trainer_file_name = "trainer.pkl"
+    trainer_info_name = "info.pkl"
+    trainer_info_json_name = "info.json"
+    distill_stackname = "distill"  # name of stack-level for distilled student models
+
+    def __init__(
+        self,
+        path: str,
+        problem_type: str,
+        eval_metric=None,
+        num_classes=None,
+        quantile_levels=None,
+        low_memory=False,
+        feature_metadata=None,
+        k_fold=0,
+        n_repeats=1,
+        sample_weight=None,
+        weight_evaluation=False,
+        save_data=False,
+        random_state=0,
+        verbosity=2,
+    ):
         self.path = path
         self.path = PathConverter.to_relative(self.path)
         self.problem_type = problem_type
         self.feature_metadata = feature_metadata
         self.save_data = save_data
-        self.random_state = random_state  # Integer value added to the stack level to get the random_state for kfold splits or the train/val split if bagging is disabled
+        self.random_state = (
+            random_state  # Integer value added to the stack level to get the random_state for kfold splits or the train/val split if bagging is disabled
+        )
         self.verbosity = verbosity
         self.sample_weight = sample_weight  # TODO: consider redesign where Trainer doesn't need sample_weight column name and weights are separate from X
         self.weight_evaluation = weight_evaluation
         if eval_metric is not None:
             self.eval_metric = eval_metric
         else:
             self.eval_metric = infer_eval_metric(problem_type=self.problem_type)
 
         logger.log(20, f"AutoGluon will gauge predictive performance using evaluation metric: '{self.eval_metric.name}'")
         if not self.eval_metric.greater_is_better_internal:
-            logger.log(20, "\tThis metric's sign has been flipped to adhere to being higher_is_better. "
-                           "The metric score can be multiplied by -1 to get the metric value.")
+            logger.log(
+                20,
+                "\tThis metric's sign has been flipped to adhere to being higher_is_better. "
+                "The metric score can be multiplied by -1 to get the metric value.",
+            )
         if not (self.eval_metric.needs_pred or self.eval_metric.needs_quantile):
-            logger.log(20, "\tThis metric expects predicted probabilities rather than predicted class labels, "
-                           "so you'll need to use predict_proba() instead of predict()")
+            logger.log(
+                20,
+                "\tThis metric expects predicted probabilities rather than predicted class labels, "
+                "so you'll need to use predict_proba() instead of predict()",
+            )
 
         logger.log(20, "\tTo change this, specify the eval_metric parameter of Predictor()")
         self.num_classes = num_classes
         self.quantile_levels = quantile_levels
         self.feature_prune = False  # will be set to True if feature-pruning is turned on.
         self.low_memory = low_memory
         self.bagged_mode = True if k_fold >= 2 else False
@@ -89,16 +141,20 @@
             self.n_repeats = n_repeats
         else:
             self.k_fold = 0
             self.n_repeats = 1
 
         self.model_best = None
 
-        self.models = {}  # Dict of model name -> model object. A key, value pair only exists if a model is persisted in memory.  # TODO: v0.1 Rename and consider making private
-        self.model_graph = nx.DiGraph()  # Directed Acyclic Graph (DAG) of model interactions. Describes how certain models depend on the predictions of certain other models. Contains numerous metadata regarding each model.
+        self.models = (
+            {}
+        )  # Dict of model name -> model object. A key, value pair only exists if a model is persisted in memory.  # TODO: v0.1 Rename and consider making private
+        self.model_graph = (
+            nx.DiGraph()
+        )  # Directed Acyclic Graph (DAG) of model interactions. Describes how certain models depend on the predictions of certain other models. Contains numerous metadata regarding each model.
         self.reset_paths = False
 
         self._time_limit = None  # Internal float of the total time limit allowed for a given fit call. Used in logging statements.
         self._time_train_start = None  # Internal timestamp of the time training started for a given fit call. Used in logging statements.
 
         self._num_rows_train = None
         self._num_cols_train = None
@@ -111,158 +167,177 @@
         self._y_val_saved = False
 
         self._groups = None  # custom split indices
 
         self._regress_preds_asprobas = False  # whether to treat regression predictions as class-probabilities (during distillation)
 
         self._extra_banned_names = set()  # Names which are banned but are not used by a trained model.
-        
+
         self._models_failed_to_train = []  # List of models which failed to train
 
         # self._exceptions_list = []  # TODO: Keep exceptions list for debugging during benchmarking.
 
     # path_root is the directory containing learner.pkl
     @property
     def path_root(self) -> str:
         return self.path.rsplit(os.path.sep, maxsplit=2)[0] + os.path.sep
 
     @property
     def path_utils(self) -> str:
-        return self.path_root + 'utils' + os.path.sep
+        return self.path_root + "utils" + os.path.sep
 
     @property
     def _path_attr(self) -> str:
         """Path to cached model graph attributes"""
-        return f'{self.path_utils}attr{os.path.sep}'
+        return f"{self.path_utils}attr{os.path.sep}"
 
     @property
     def path_data(self) -> str:
-        return self.path_utils + 'data' + os.path.sep
+        return self.path_utils + "data" + os.path.sep
 
     @property
     def has_val(self) -> bool:
         """Whether the trainer uses validation data"""
         return self._num_rows_val is not None
 
     def load_X(self):
         if self._X_saved:
-            path = self.path_data + 'X.pkl'
+            path = self.path_data + "X.pkl"
             return load_pkl.load(path=path)
         return None
 
     def load_X_val(self):
         if self._X_val_saved:
-            path = self.path_data + 'X_val.pkl'
+            path = self.path_data + "X_val.pkl"
             return load_pkl.load(path=path)
         return None
 
     def load_y(self):
         if self._y_saved:
-            path = self.path_data + 'y.pkl'
+            path = self.path_data + "y.pkl"
             return load_pkl.load(path=path)
         return None
 
     def load_y_val(self):
         if self._y_val_saved:
-            path = self.path_data + 'y_val.pkl'
+            path = self.path_data + "y_val.pkl"
             return load_pkl.load(path=path)
         return None
 
     def load_data(self):
         X = self.load_X()
         y = self.load_y()
         X_val = self.load_X_val()
         y_val = self.load_y_val()
 
         return X, y, X_val, y_val
 
     def save_X(self, X, verbose=True):
-        path = self.path_data + 'X.pkl'
+        path = self.path_data + "X.pkl"
         save_pkl.save(path=path, object=X, verbose=verbose)
         self._X_saved = True
 
     def save_X_val(self, X, verbose=True):
-        path = self.path_data + 'X_val.pkl'
+        path = self.path_data + "X_val.pkl"
         save_pkl.save(path=path, object=X, verbose=verbose)
         self._X_val_saved = True
 
     def save_y(self, y, verbose=True):
-        path = self.path_data + 'y.pkl'
+        path = self.path_data + "y.pkl"
         save_pkl.save(path=path, object=y, verbose=verbose)
         self._y_saved = True
 
     def save_y_val(self, y, verbose=True):
-        path = self.path_data + 'y_val.pkl'
+        path = self.path_data + "y_val.pkl"
         save_pkl.save(path=path, object=y, verbose=verbose)
         self._y_val_saved = True
 
-    def get_model_names(self, stack_name: Union[List[str], str] = None, level: Union[List[int], int] = None, can_infer: bool = None, models: List[str] = None) -> List[str]:
+    def get_model_names(
+        self, stack_name: Union[List[str], str] = None, level: Union[List[int], int] = None, can_infer: bool = None, models: List[str] = None
+    ) -> List[str]:
         if models is None:
             models = list(self.model_graph.nodes)
         if stack_name is not None:
             if not isinstance(stack_name, list):
                 stack_name = [stack_name]
-            node_attributes: dict = self.get_models_attribute_dict(attribute='stack_name', models=models)
+            node_attributes: dict = self.get_models_attribute_dict(attribute="stack_name", models=models)
             models = [model_name for model_name in models if node_attributes[model_name] in stack_name]
         if level is not None:
             if not isinstance(level, list):
                 level = [level]
-            node_attributes: dict = self.get_models_attribute_dict(attribute='level', models=models)
+            node_attributes: dict = self.get_models_attribute_dict(attribute="level", models=models)
             models = [model_name for model_name in models if node_attributes[model_name] in level]
         # TODO: can_infer is technically more complicated, if an ancestor can't infer then the model can't infer.
         if can_infer is not None:
-            node_attributes = self.get_models_attribute_full(attribute='can_infer', models=models, func=min)
+            node_attributes = self.get_models_attribute_full(attribute="can_infer", models=models, func=min)
             models = [model for model in models if node_attributes[model] == can_infer]
         return models
 
     def get_max_level(self, stack_name: str = None, models: List[str] = None) -> int:
         models = self.get_model_names(stack_name=stack_name, models=models)
-        models_attribute_dict = self.get_models_attribute_dict(attribute='level', models=models)
+        models_attribute_dict = self.get_models_attribute_dict(attribute="level", models=models)
         if models_attribute_dict:
             return max(list(models_attribute_dict.values()))
         else:
             return -1
 
     def construct_model_templates(self, hyperparameters: dict, **kwargs) -> Tuple[List[AbstractModel], dict]:
         """Constructs a list of unfit models based on the hyperparameters dict."""
         raise NotImplementedError
 
     def construct_model_templates_distillation(self, hyperparameters: dict, **kwargs) -> Tuple[List[AbstractModel], dict]:
         """Constructs a list of unfit models based on the hyperparameters dict for softclass distillation."""
         raise NotImplementedError
 
     def get_model_level(self, model_name: str) -> int:
-        return self.get_model_attribute(model=model_name, attribute='level')
+        return self.get_model_attribute(model=model_name, attribute="level")
 
     def set_contexts(self, path_context):
         self.path, model_paths = self.create_contexts(path_context)
         for model, path in model_paths.items():
-            self.set_model_attribute(model=model, attribute='path', val=path)
+            self.set_model_attribute(model=model, attribute="path", val=path)
 
     def create_contexts(self, path_context: str) -> (str, dict):
         self.path = PathConverter.to_current(self.path)
         path = path_context
-        model_paths = self.get_models_attribute_dict(attribute='path')
+        model_paths = self.get_models_attribute_dict(attribute="path")
         model_paths = {model: PathConverter.to_current(model_path) for model, model_path in model_paths.items()}
         for model, prev_path in model_paths.items():
             prev_path = os.path.abspath(prev_path) + os.path.sep
             abs_path = os.path.abspath(self.path) + os.path.sep
             model_local_path = prev_path.split(abs_path, 1)[1]
             new_path = path + model_local_path
             model_paths[model] = new_path
 
         return path, model_paths
 
     def fit(self, X, y, hyperparameters: dict, X_val=None, y_val=None, **kwargs):
         raise NotImplementedError
 
     # TODO: Enable easier re-mapping of trained models -> hyperparameters input (They don't share a key since name can change)
-    def train_multi_levels(self, X, y, hyperparameters: dict, X_val=None, y_val=None, X_unlabeled=None, base_model_names: List[str] = None,
-                           core_kwargs: dict = None, aux_kwargs: dict = None, level_start=1, level_end=1, time_limit=None, name_suffix: str = None,
-                           relative_stack=True, level_time_modifier=0.333, infer_limit=None, infer_limit_batch_size=None) -> List[str]:
+    def train_multi_levels(
+        self,
+        X,
+        y,
+        hyperparameters: dict,
+        X_val=None,
+        y_val=None,
+        X_unlabeled=None,
+        base_model_names: List[str] = None,
+        core_kwargs: dict = None,
+        aux_kwargs: dict = None,
+        level_start=1,
+        level_end=1,
+        time_limit=None,
+        name_suffix: str = None,
+        relative_stack=True,
+        level_time_modifier=0.333,
+        infer_limit=None,
+        infer_limit_batch_size=None,
+    ) -> List[str]:
         """
         Trains a multi-layer stack ensemble using the input data on the hyperparameters dict input.
             hyperparameters is used to determine the models used in each stack layer.
         If continuing a stack ensemble with level_start>1, ensure that base_model_names is set to the appropriate base models that will be used by the level_start level models.
         Trains both core and aux models.
             core models are standard models which are fit on the data features. Core models will also use model predictions if base_model_names was specified or if level != 1.
             aux models are ensemble models which only use the predictions of core models as features. These models never use the original features.
@@ -279,68 +354,74 @@
         self._time_train_start = time.time()
         time_train_start = self._time_train_start
 
         hyperparameters = self._process_hyperparameters(hyperparameters=hyperparameters)
 
         if relative_stack:
             if level_start != 1:
-                raise AssertionError(f'level_start must be 1 when `relative_stack=True`. (level_start = {level_start})')
+                raise AssertionError(f"level_start must be 1 when `relative_stack=True`. (level_start = {level_start})")
             level_add = 0
             if base_model_names:
                 max_base_model_level = self.get_max_level(models=base_model_names)
                 level_start = max_base_model_level + 1
                 level_add = level_start - 1
                 level_end += level_add
             if level_start != 1:
                 hyperparameters_relative = {}
                 for key in hyperparameters:
                     if isinstance(key, int):
-                        hyperparameters_relative[key+level_add] = hyperparameters[key]
+                        hyperparameters_relative[key + level_add] = hyperparameters[key]
                     else:
                         hyperparameters_relative[key] = hyperparameters[key]
                 hyperparameters = hyperparameters_relative
 
         core_kwargs = {} if core_kwargs is None else core_kwargs.copy()
         aux_kwargs = {} if aux_kwargs is None else aux_kwargs.copy()
 
         model_names_fit = []
         if level_start != level_end:
-            logger.log(20, f'AutoGluon will fit {level_end - level_start + 1} stack levels (L{level_start} to L{level_end}) ...')
+            logger.log(20, f"AutoGluon will fit {level_end - level_start + 1} stack levels (L{level_start} to L{level_end}) ...")
         for level in range(level_start, level_end + 1):
             core_kwargs_level = core_kwargs.copy()
             aux_kwargs_level = aux_kwargs.copy()
             if time_limit is not None:
                 time_train_level_start = time.time()
                 levels_left = level_end - level + 1
                 time_left = time_limit - (time_train_level_start - time_train_start)
                 time_limit_for_level = min(time_left / levels_left * (1 + level_time_modifier), time_left)
                 time_limit_core = time_limit_for_level
                 time_limit_aux = max(time_limit_for_level * 0.1, min(time_limit, 360))  # Allows aux to go over time_limit, but only by a small amount
-                core_kwargs_level['time_limit'] = core_kwargs_level.get('time_limit', time_limit_core)
-                aux_kwargs_level['time_limit'] = aux_kwargs_level.get('time_limit', time_limit_aux)
+                core_kwargs_level["time_limit"] = core_kwargs_level.get("time_limit", time_limit_core)
+                aux_kwargs_level["time_limit"] = aux_kwargs_level.get("time_limit", time_limit_aux)
             base_model_names, aux_models = self.stack_new_level(
-                X=X, y=y, X_val=X_val, y_val=y_val, X_unlabeled=X_unlabeled,
-                models=hyperparameters, level=level, base_model_names=base_model_names,
-                core_kwargs=core_kwargs_level, aux_kwargs=aux_kwargs_level, name_suffix=name_suffix,
-                infer_limit=infer_limit, infer_limit_batch_size=infer_limit_batch_size,
+                X=X,
+                y=y,
+                X_val=X_val,
+                y_val=y_val,
+                X_unlabeled=X_unlabeled,
+                models=hyperparameters,
+                level=level,
+                base_model_names=base_model_names,
+                core_kwargs=core_kwargs_level,
+                aux_kwargs=aux_kwargs_level,
+                name_suffix=name_suffix,
+                infer_limit=infer_limit,
+                infer_limit_batch_size=infer_limit_batch_size,
             )
             model_names_fit += base_model_names + aux_models
         if self.model_best is None and len(model_names_fit) != 0:
             self.model_best = self.get_model_best(can_infer=True, infer_limit=infer_limit)
         self._time_limit = None
         self.save()
         return model_names_fit
 
     # TODO: Consider better greedy approximation method such as via fitting a weighted ensemble to evaluate the value of a subset.
-    def _filter_base_models_via_infer_limit(self,
-                                            base_model_names: List[str],
-                                            infer_limit: float,
-                                            infer_limit_modifier: float = 1.0,
-                                            as_child: bool = True,
-                                            verbose: bool = True) -> List[str]:
+    def _filter_base_models_via_infer_limit(
+        self, base_model_names: List[str], infer_limit: float, infer_limit_modifier: float = 1.0, as_child: bool = True, verbose: bool = True
+    ) -> List[str]:
         """
         Returns a subset of base_model_names whose combined prediction time for 1 row of data does not exceed infer_limit seconds.
         With the goal of selecting the best valid subset that is most valuable to stack ensembles who use them as base models,
         this is a variant of the constrained knapsack problem and is NP-Hard and infeasible to exactly solve even with fewer than 10 models.
         For practical purposes, this method applies a greedy approximation approach to selecting the subset
         by simply removing models in reverse order of validation score until the remaining subset is valid.
 
@@ -368,17 +449,17 @@
             return base_model_names
 
         base_model_names = base_model_names.copy()
         num_models_og = len(base_model_names)
         infer_limit_threshold = infer_limit * infer_limit_modifier  # Add headroom
 
         if as_child:
-            attribute = 'predict_1_child_time'
+            attribute = "predict_1_child_time"
         else:
-            attribute = 'predict_1_time'
+            attribute = "predict_1_time"
 
         predict_1_time_full_set = self.get_model_attribute_full(model=base_model_names, attribute=attribute)
 
         messages_to_log = []
 
         base_model_names_copy = base_model_names.copy()
         # Prune models that by themselves have larger inference latency than the infer_limit, as they can never be valid
@@ -387,112 +468,153 @@
             if predict_1_time_full >= infer_limit_threshold:
                 predict_1_time_full_set_old = predict_1_time_full_set
                 base_model_names.remove(base_model_name)
                 predict_1_time_full_set = self.get_model_attribute_full(model=base_model_names, attribute=attribute)
                 if verbose:
                     predict_1_time_full_set_log, time_unit = convert_time_in_s_to_log_friendly(time_in_sec=predict_1_time_full_set)
                     predict_1_time_full_set_old_log, time_unit_old = convert_time_in_s_to_log_friendly(time_in_sec=predict_1_time_full_set_old)
-                    messages_to_log.append(f'\t{round(predict_1_time_full_set_old_log, 3)}{time_unit_old}\t-> {round(predict_1_time_full_set_log, 3)}{time_unit}\t({base_model_name})')
+                    messages_to_log.append(
+                        f"\t{round(predict_1_time_full_set_old_log, 3)}{time_unit_old}\t-> {round(predict_1_time_full_set_log, 3)}{time_unit}\t({base_model_name})"
+                    )
 
-        score_val_dict = self.get_models_attribute_dict(attribute='val_score', models=base_model_names)
+        score_val_dict = self.get_models_attribute_dict(attribute="val_score", models=base_model_names)
         sorted_scores = sorted(score_val_dict.items(), key=lambda x: x[1])
         i = 0
         # Prune models by ascending validation score until the remaining subset's combined inference latency satisfies infer_limit
         while base_model_names and (predict_1_time_full_set >= infer_limit_threshold):
             # TODO: Incorporate score vs inference speed tradeoff in a smarter way
             base_model_to_remove = sorted_scores[i][0]
             predict_1_time_full_set_old = predict_1_time_full_set
             base_model_names.remove(base_model_to_remove)
             i += 1
             predict_1_time_full_set = self.get_model_attribute_full(model=base_model_names, attribute=attribute)
             if verbose:
                 predict_1_time_full_set_log, time_unit = convert_time_in_s_to_log_friendly(time_in_sec=predict_1_time_full_set)
                 predict_1_time_full_set_old_log, time_unit_old = convert_time_in_s_to_log_friendly(time_in_sec=predict_1_time_full_set_old)
-                messages_to_log.append(f'\t{round(predict_1_time_full_set_old_log, 3)}{time_unit_old}\t-> {round(predict_1_time_full_set_log, 3)}{time_unit}\t({base_model_to_remove})')
+                messages_to_log.append(
+                    f"\t{round(predict_1_time_full_set_old_log, 3)}{time_unit_old}\t-> {round(predict_1_time_full_set_log, 3)}{time_unit}\t({base_model_to_remove})"
+                )
 
         if messages_to_log:
             infer_limit_threshold_log, time_unit_threshold = convert_time_in_s_to_log_friendly(time_in_sec=infer_limit_threshold)
-            logger.log(20, f'Removing {len(messages_to_log)}/{num_models_og} base models to satisfy inference constraint '
-                           f'(constraint={round(infer_limit_threshold_log, 3)}{time_unit_threshold}) ...')
+            logger.log(
+                20,
+                f"Removing {len(messages_to_log)}/{num_models_og} base models to satisfy inference constraint "
+                f"(constraint={round(infer_limit_threshold_log, 3)}{time_unit_threshold}) ...",
+            )
             for msg in messages_to_log:
                 logger.log(20, msg)
 
         return base_model_names
 
-    def stack_new_level(self, X, y, models: Union[List[AbstractModel], dict], X_val=None, y_val=None, X_unlabeled=None, level=1, base_model_names: List[str] = None,
-                        core_kwargs: dict = None, aux_kwargs: dict = None, name_suffix: str = None, infer_limit=None, infer_limit_batch_size=None) -> (List[str], List[str]):
+    def stack_new_level(
+        self,
+        X,
+        y,
+        models: Union[List[AbstractModel], dict],
+        X_val=None,
+        y_val=None,
+        X_unlabeled=None,
+        level=1,
+        base_model_names: List[str] = None,
+        core_kwargs: dict = None,
+        aux_kwargs: dict = None,
+        name_suffix: str = None,
+        infer_limit=None,
+        infer_limit_batch_size=None,
+    ) -> (List[str], List[str]):
         """
         Similar to calling self.stack_new_level_core, except auxiliary models will also be trained via a call to self.stack_new_level_aux, with the models trained from self.stack_new_level_core used as base models.
         """
         if base_model_names is None:
             base_model_names = []
         core_kwargs = {} if core_kwargs is None else core_kwargs.copy()
         aux_kwargs = {} if aux_kwargs is None else aux_kwargs.copy()
         if level < 1:
-            raise AssertionError(f'Stack level must be >= 1, but level={level}.')
+            raise AssertionError(f"Stack level must be >= 1, but level={level}.")
         if base_model_names and level == 1:
-            raise AssertionError(f'Stack level 1 models cannot have base models, but base_model_names={base_model_names}.')
+            raise AssertionError(f"Stack level 1 models cannot have base models, but base_model_names={base_model_names}.")
         if name_suffix:
-            core_kwargs['name_suffix'] = core_kwargs.get('name_suffix', '') + name_suffix
-            aux_kwargs['name_suffix'] = aux_kwargs.get('name_suffix', '') + name_suffix
-        core_models = self.stack_new_level_core(X=X, y=y, X_val=X_val, y_val=y_val, X_unlabeled=X_unlabeled, models=models,
-                                                level=level, infer_limit=infer_limit, infer_limit_batch_size=infer_limit_batch_size, base_model_names=base_model_names, **core_kwargs)
+            core_kwargs["name_suffix"] = core_kwargs.get("name_suffix", "") + name_suffix
+            aux_kwargs["name_suffix"] = aux_kwargs.get("name_suffix", "") + name_suffix
+        core_models = self.stack_new_level_core(
+            X=X,
+            y=y,
+            X_val=X_val,
+            y_val=y_val,
+            X_unlabeled=X_unlabeled,
+            models=models,
+            level=level,
+            infer_limit=infer_limit,
+            infer_limit_batch_size=infer_limit_batch_size,
+            base_model_names=base_model_names,
+            **core_kwargs,
+        )
 
         if X_val is None:
-            aux_models = self.stack_new_level_aux(X=X, y=y, base_model_names=core_models, level=level+1,
-                                                  infer_limit=infer_limit, infer_limit_batch_size=infer_limit_batch_size, **aux_kwargs)
+            aux_models = self.stack_new_level_aux(
+                X=X, y=y, base_model_names=core_models, level=level + 1, infer_limit=infer_limit, infer_limit_batch_size=infer_limit_batch_size, **aux_kwargs
+            )
         else:
-            aux_models = self.stack_new_level_aux(X=X_val, y=y_val, fit=False, base_model_names=core_models, level=level+1,
-                                                  infer_limit=infer_limit, infer_limit_batch_size=infer_limit_batch_size, **aux_kwargs)
+            aux_models = self.stack_new_level_aux(
+                X=X_val,
+                y=y_val,
+                fit=False,
+                base_model_names=core_models,
+                level=level + 1,
+                infer_limit=infer_limit,
+                infer_limit_batch_size=infer_limit_batch_size,
+                **aux_kwargs,
+            )
         return core_models, aux_models
 
     def stack_new_level_core(
         self,
         X,
         y,
         models: Union[List[AbstractModel], dict],
         X_val=None,
         y_val=None,
         X_unlabeled=None,
         level=1,
         base_model_names: List[str] = None,
-        stack_name='core',
+        stack_name="core",
         ag_args=None,
         ag_args_fit=None,
         ag_args_ensemble=None,
         included_model_types=None,
         excluded_model_types=None,
         ensemble_type=StackerEnsembleModel,
         name_suffix: str = None,
         get_models_func=None,
         refit_full=False,
         infer_limit=None,
         infer_limit_batch_size=None,
-        **kwargs
+        **kwargs,
     ) -> List[str]:
         """
         Trains all models using the data provided.
         If level > 1, then the models will use base model predictions as additional features.
             The base models used can be specified via base_model_names.
         If self.bagged_mode, then models will be trained as StackerEnsembleModels.
         The data provided in this method should not contain stack features, as they will be automatically generated if necessary.
         """
         if get_models_func is None:
             get_models_func = self.construct_model_templates
         if base_model_names is None:
             base_model_names = []
         if not self.bagged_mode and level != 1:
-            raise ValueError('Stack Ensembling is not valid for non-bagged mode.')
+            raise ValueError("Stack Ensembling is not valid for non-bagged mode.")
 
         base_model_names = self._filter_base_models_via_infer_limit(base_model_names=base_model_names, infer_limit=infer_limit, infer_limit_modifier=0.8)
         if ag_args_fit is None:
             ag_args_fit = {}
         ag_args_fit = ag_args_fit.copy()
         if infer_limit_batch_size is not None:
-            ag_args_fit['predict_1_batch_size'] = infer_limit_batch_size
+            ag_args_fit["predict_1_batch_size"] = infer_limit_batch_size
 
         if isinstance(models, dict):
             get_models_kwargs = dict(
                 level=level,
                 name_suffix=name_suffix,
                 ag_args=ag_args,
                 ag_args_fit=ag_args_fit,
@@ -502,38 +624,41 @@
 
             if self.bagged_mode:
                 if level == 1:
                     (base_model_names, base_model_paths, base_model_types) = (None, None, None)
                 elif level > 1:
                     base_model_names, base_model_paths, base_model_types = self._get_models_load_info(model_names=base_model_names)
                     if len(base_model_names) == 0:
-                        logger.log(20, f'No base models to train on, skipping stack level {level}...')
+                        logger.log(20, f"No base models to train on, skipping stack level {level}...")
                         return []
                 else:
-                    raise AssertionError(f'Stack level cannot be less than 1! level = {level}')
+                    raise AssertionError(f"Stack level cannot be less than 1! level = {level}")
 
                 ensemble_kwargs = {
-                    'base_model_names': base_model_names,
-                    'base_model_paths_dict': base_model_paths,
-                    'base_model_types_dict': base_model_types,
-                    'random_state': level + self.random_state,
+                    "base_model_names": base_model_names,
+                    "base_model_paths_dict": base_model_paths,
+                    "base_model_types_dict": base_model_types,
+                    "random_state": level + self.random_state,
                 }
-                get_models_kwargs.update(dict(
-                    ag_args_ensemble=ag_args_ensemble,
-                    ensemble_type=ensemble_type,
-                    ensemble_kwargs=ensemble_kwargs,
-                ))
+                get_models_kwargs.update(
+                    dict(
+                        ag_args_ensemble=ag_args_ensemble,
+                        ensemble_type=ensemble_type,
+                        ensemble_kwargs=ensemble_kwargs,
+                    )
+                )
             models, model_args_fit = get_models_func(hyperparameters=models, **get_models_kwargs)
             if model_args_fit:
                 hyperparameter_tune_kwargs = {
-                    model_name: model_args_fit[model_name]['hyperparameter_tune_kwargs']
-                    for model_name in model_args_fit if 'hyperparameter_tune_kwargs' in model_args_fit[model_name]
+                    model_name: model_args_fit[model_name]["hyperparameter_tune_kwargs"]
+                    for model_name in model_args_fit
+                    if "hyperparameter_tune_kwargs" in model_args_fit[model_name]
                 }
-                kwargs['hyperparameter_tune_kwargs'] = hyperparameter_tune_kwargs
-        logger.log(20, f'Fitting {len(models)} L{level} models ...')
+                kwargs["hyperparameter_tune_kwargs"] = hyperparameter_tune_kwargs
+        logger.log(20, f"Fitting {len(models)} L{level} models ...")
         X_init = self.get_inputs_to_stacker(X, base_models=base_model_names, fit=True)
         if X_val is not None:
             X_val = self.get_inputs_to_stacker(X_val, base_models=base_model_names, fit=False, use_val_cache=True)
         compute_score = not refit_full
         if refit_full and X_val is not None:
             X_init = pd.concat([X_init, X_val])
             y = pd.concat([y, y_val])
@@ -541,50 +666,85 @@
             y_val = None
         if X_unlabeled is not None:
             X_unlabeled = self.get_inputs_to_stacker(X_unlabeled, base_models=base_model_names, fit=False)
 
         fit_kwargs = dict(num_classes=self.num_classes)
 
         # FIXME: TODO: v0.1 X_unlabeled isn't cached so it won't be available during refit_full or fit_extra.
-        return self._train_multi(X=X_init, y=y, X_val=X_val, y_val=y_val, X_unlabeled=X_unlabeled,
-                                 models=models, level=level, stack_name=stack_name, compute_score=compute_score, fit_kwargs=fit_kwargs, **kwargs)
+        return self._train_multi(
+            X=X_init,
+            y=y,
+            X_val=X_val,
+            y_val=y_val,
+            X_unlabeled=X_unlabeled,
+            models=models,
+            level=level,
+            stack_name=stack_name,
+            compute_score=compute_score,
+            fit_kwargs=fit_kwargs,
+            **kwargs,
+        )
 
     # TODO: Consider making level be auto-determined based off of max(base_model_levels)+1
     # TODO: Remove name_suffix, hacked in
     # TODO: X can be optional because it isn't needed if fit=True
-    def stack_new_level_aux(self, X, y, base_model_names: List[str], level,
-                            fit=True, stack_name='aux1', time_limit=None, name_suffix: str = None, get_models_func=None, check_if_best=True,
-                            infer_limit=None, infer_limit_batch_size=None, use_val_cache=True, fit_weighted_ensemble=True) -> List[str]:
+    def stack_new_level_aux(
+        self,
+        X,
+        y,
+        base_model_names: List[str],
+        level,
+        fit=True,
+        stack_name="aux1",
+        time_limit=None,
+        name_suffix: str = None,
+        get_models_func=None,
+        check_if_best=True,
+        infer_limit=None,
+        infer_limit_batch_size=None,
+        use_val_cache=True,
+        fit_weighted_ensemble=True,
+    ) -> List[str]:
         """
         Trains auxiliary models (currently a single weighted ensemble) using the provided base models.
         Level must be greater than the level of any of the base models.
         Auxiliary models never use the original features and only train with the predictions of other models as features.
         """
         if fit_weighted_ensemble is False:
             # Skip fitting of aux models
             return []
         base_model_names = self._filter_base_models_via_infer_limit(base_model_names=base_model_names, infer_limit=infer_limit, infer_limit_modifier=0.95)
         if len(base_model_names) == 0:
-            logger.log(20, f'No base models to train on, skipping auxiliary stack level {level}...')
+            logger.log(20, f"No base models to train on, skipping auxiliary stack level {level}...")
             return []
 
         if infer_limit_batch_size is not None:
             ag_args_fit = dict()
-            ag_args_fit['predict_1_batch_size'] = infer_limit_batch_size
+            ag_args_fit["predict_1_batch_size"] = infer_limit_batch_size
         else:
             ag_args_fit = None
         X_stack_preds = self.get_inputs_to_stacker(X, base_models=base_model_names, fit=fit, use_orig_features=False, use_val_cache=use_val_cache)
         if self.weight_evaluation:
             X, w = extract_column(X, self.sample_weight)  # TODO: consider redesign with w as separate arg instead of bundled inside X
             if w is not None:
-                X_stack_preds[self.sample_weight] = w.values/w.mean()
-        return self.generate_weighted_ensemble(X=X_stack_preds, y=y,
-                                               level=level, base_model_names=base_model_names, k_fold=1, n_repeats=1, ag_args_fit=ag_args_fit,
-                                               stack_name=stack_name, time_limit=time_limit, name_suffix=name_suffix,
-                                               get_models_func=get_models_func, check_if_best=check_if_best)
+                X_stack_preds[self.sample_weight] = w.values / w.mean()
+        return self.generate_weighted_ensemble(
+            X=X_stack_preds,
+            y=y,
+            level=level,
+            base_model_names=base_model_names,
+            k_fold=1,
+            n_repeats=1,
+            ag_args_fit=ag_args_fit,
+            stack_name=stack_name,
+            time_limit=time_limit,
+            name_suffix=name_suffix,
+            get_models_func=get_models_func,
+            check_if_best=check_if_best,
+        )
 
     def predict(self, X, model=None):
         if model is None:
             model = self._get_best()
         cascade = isinstance(model, list)
         return self._predict_model(X, model, cascade=cascade)
 
@@ -635,30 +795,29 @@
         return X
 
     def score(self, X, y, model=None, weights=None) -> float:
         if self.eval_metric.needs_pred or self.eval_metric.needs_quantile:
             y_pred = self.predict(X=X, model=model)
         else:
             y_pred = self.predict_proba(X=X, model=model)
-        return compute_weighted_metric(y, y_pred, self.eval_metric, weights, weight_evaluation=self.weight_evaluation,
-                                       quantile_levels=self.quantile_levels)
+        return compute_weighted_metric(y, y_pred, self.eval_metric, weights, weight_evaluation=self.weight_evaluation, quantile_levels=self.quantile_levels)
 
     def score_with_y_pred_proba(self, y, y_pred_proba, weights=None) -> float:
         if self.eval_metric.needs_pred or self.eval_metric.needs_quantile:
             y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba, problem_type=self.problem_type)
         else:
             y_pred = y_pred_proba
-        return compute_weighted_metric(y, y_pred, self.eval_metric, weights, weight_evaluation=self.weight_evaluation,
-                                       quantile_levels=self.quantile_levels)
+        return compute_weighted_metric(y, y_pred, self.eval_metric, weights, weight_evaluation=self.weight_evaluation, quantile_levels=self.quantile_levels)
 
     def _score_with_y_pred(self, y, y_pred, weights=None, metric=None) -> float:
         if metric is None:
             metric = self.eval_metric
-        return compute_weighted_metric(y, y_pred, metric=metric, weights=weights, weight_evaluation=self.weight_evaluation,
-                                       quantile_levels=self.quantile_levels)
+        return compute_weighted_metric(
+            y, y_pred, metric=metric, weights=weights, weight_evaluation=self.weight_evaluation, quantile_levels=self.quantile_levels
+        )
 
     # TODO: Slow if large ensemble with many models, could cache output result to speed up cascades during inference
     def _construct_model_pred_order(self, models: List[str]) -> List[str]:
         """
         Constructs a list of model names in order of inference calls required to infer on all the models.
 
         Parameters
@@ -730,23 +889,25 @@
         # Get model prediction order
         return list(nx.lexicographical_topological_sort(subgraph))
 
     # TODO: Consider adding persist to disk functionality for pred_proba dictionary to lessen memory burden on large multiclass problems.
     #  For datasets with 100+ classes, this function could potentially run the system OOM due to each pred_proba numpy array taking significant amounts of space.
     #  This issue already existed in the previous level-based version but only had the minimum required predictions in memory at a time, whereas this has all model predictions in memory.
     # TODO: Add memory optimal topological ordering -> Minimize amount of pred_probas in memory at a time, delete pred probas that are no longer required
-    def get_model_pred_proba_dict(self,
-                                  X: pd.DataFrame,
-                                  models: List[str],
-                                  model_pred_proba_dict: dict = None,
-                                  model_pred_time_dict: dict = None,
-                                  record_pred_time: bool = False,
-                                  use_val_cache: bool = False,
-                                  cascade: bool = False,
-                                  cascade_threshold: float = 0.9):
+    def get_model_pred_proba_dict(
+        self,
+        X: pd.DataFrame,
+        models: List[str],
+        model_pred_proba_dict: dict = None,
+        model_pred_time_dict: dict = None,
+        record_pred_time: bool = False,
+        use_val_cache: bool = False,
+        cascade: bool = False,
+        cascade_threshold: float = 0.9,
+    ):
         """
         Optimally computes pred_probas (or predictions if regression) for each model in `models`.
         Will compute each necessary model only once and store predictions in a `model_pred_proba_dict` dictionary.
         Note: Mutates model_pred_proba_dict and model_pred_time_dict input if present to minimize memory usage.
 
         Parameters
         ----------
@@ -795,29 +956,31 @@
             model_pred_proba_dict = {}
         if model_pred_time_dict is None:
             model_pred_time_dict = {}
         if cascade and len(models) <= 1:
             cascade = False
         if cascade and model_pred_proba_dict:
             # Technically doesn't have to be an error, but logic gets extremely complicated if we allow this.
-            raise AssertionError('Cascade is not valid when model_pred_proba_dict is specified.')
+            raise AssertionError("Cascade is not valid when model_pred_proba_dict is specified.")
         if cascade and self.problem_type not in [BINARY, MULTICLASS]:
-            raise AssertionError(f'Ensemble Cascade not implemented for problem_type=={self.problem_type}')
+            raise AssertionError(f"Ensemble Cascade not implemented for problem_type=={self.problem_type}")
         if cascade and use_val_cache:
-            raise AssertionError('cascade and use_val_cache cannot both be True.')
+            raise AssertionError("cascade and use_val_cache cannot both be True.")
 
         if use_val_cache:
             _, model_pred_proba_dict = self._update_pred_proba_dict_with_val_cache(model_set=set(models), model_pred_proba_dict=model_pred_proba_dict)
         if not model_pred_proba_dict:
             # TODO: Pre-construct order if cascade, otherwise this will slow down prediction having to recompute each inference call.
             model_pred_order = self._construct_model_pred_order(models)
         else:
             model_pred_order = self._construct_model_pred_order_with_pred_dict(models, models_to_ignore=list(model_pred_proba_dict.keys()))
         if use_val_cache:
-            model_set, model_pred_proba_dict = self._update_pred_proba_dict_with_val_cache(model_set=set(model_pred_order), model_pred_proba_dict=model_pred_proba_dict)
+            model_set, model_pred_proba_dict = self._update_pred_proba_dict_with_val_cache(
+                model_set=set(model_pred_order), model_pred_proba_dict=model_pred_proba_dict
+            )
             model_pred_order = [model for model in model_pred_order if model in model_set]
 
         iloc_model_dict = dict()
         model_pred_proba_dict_cascade = dict()
 
         if cascade:
             num_rows = len(X)
@@ -860,45 +1023,45 @@
                 time_end = time.time()
                 model_pred_time_dict[model_name] = time_end - time_start
 
             if cascade:
                 if model_name in models:
                     cascade_order.append(model_name)
                 if self.problem_type == BINARY:
-                    tmp = np.zeros(num_rows, dtype='float32')
+                    tmp = np.zeros(num_rows, dtype="float32")
                 else:
-                    tmp = np.zeros((num_rows, self.num_classes), dtype='float32')
+                    tmp = np.zeros((num_rows, self.num_classes), dtype="float32")
                 tmp[iloc_model_dict[model_name]] = model_pred_proba_dict[model_name]
                 model_pred_proba_dict_cascade[model_name] = tmp
                 # If model is part of cascade, keep the predictions that are confident and don't predict on these rows with further models.
                 if model_name in models and model_name != models[-1]:
                     pred_proba = model_pred_proba_dict[model_name]
                     # Calculate confident predictions based on cascade threshold
                     # TODO: Support more sophisticated methods of calculating whether to keep a prediction
                     # TODO: Support per-model confidence specification
                     if self.problem_type == BINARY:
-                        confident = (pred_proba >= cascade_threshold) | (pred_proba <= (1-cascade_threshold))
+                        confident = (pred_proba >= cascade_threshold) | (pred_proba <= (1 - cascade_threshold))
                     elif self.problem_type == MULTICLASS:
                         confident = (pred_proba >= cascade_threshold).any(axis=1)
                     else:
-                        raise AssertionError(f'Invalid cascade problem_type: {self.problem_type}')
+                        raise AssertionError(f"Invalid cascade problem_type: {self.problem_type}")
                     unconfident_cur = ~confident
                     # Shrink X to only contain the remaining unconfident rows
                     X = X.iloc[unconfident_cur]
                     unconfident_idx = unconfident_idx[unconfident_cur]
                     # If no rows remain that are unconfident, exit cascade logic early.
                     if len(X) == 0:
                         break
 
         if cascade:
             # TODO: How should this be output?
             if self.problem_type == BINARY:
-                cascade_pred_proba = np.zeros(num_rows, dtype='float32')
+                cascade_pred_proba = np.zeros(num_rows, dtype="float32")
             else:
-                cascade_pred_proba = np.zeros((num_rows, self.num_classes), dtype='float32')
+                cascade_pred_proba = np.zeros((num_rows, self.num_classes), dtype="float32")
             # For each model in the cascade early exit logic from first to final, update cascade_pred_proba
             #  with the pred_proba from that model of the rows it predicted on.
             #  This will result in the final pred_proba of the cascade at the end of the for-loop.
             for m in cascade_order:
                 cascade_pred_proba[iloc_model_dict[m]] = model_pred_proba_dict[m]
             # FIXME: Temp overwrite, unsure how we want to vend cascade results? In future maybe under its own model name.
             model_pred_proba_dict[models[-1]] = cascade_pred_proba
@@ -910,19 +1073,15 @@
 
     def get_model_oof_dict(self, models: List[str]) -> dict:
         """
         Returns a dictionary of out-of-fold prediction probabilities, keyed by model name
         """
         return {model: self.get_model_oof(model) for model in models}
 
-    def get_model_pred_dict(self,
-                            X: pd.DataFrame,
-                            models: List[str],
-                            record_pred_time: bool = False,
-                            **kwargs):
+    def get_model_pred_dict(self, X: pd.DataFrame, models: List[str], record_pred_time: bool = False, **kwargs):
         """
         Optimally computes predictions for each model in `models`.
         Will compute each necessary model only once and store predictions in a `model_pred_dict` dictionary.
         Note: Mutates model_pred_proba_dict and model_pred_time_dict input if present to minimize memory usage.
 
         Acts as a wrapper to `self.get_model_pred_proba_dict`, converting the output to predictions.
 
@@ -939,18 +1098,15 @@
             Refer to `self.get_model_pred_proba_dict` for documentation of remaining arguments.
             This method shares identical arguments.
 
         Returns
         -------
         If `record_pred_time==True`, outputs tuple of dicts (model_pred_dict, model_pred_time_dict), else output only model_pred_dict
         """
-        model_pred_proba_dict = self.get_model_pred_proba_dict(X=X,
-                                                               models=models,
-                                                               record_pred_time=record_pred_time,
-                                                               **kwargs)
+        model_pred_proba_dict = self.get_model_pred_proba_dict(X=X, models=models, record_pred_time=record_pred_time, **kwargs)
         if record_pred_time:
             model_pred_proba_dict, model_pred_time_dict = model_pred_proba_dict
         else:
             model_pred_time_dict = None
 
         model_pred_dict = {}
         for m in model_pred_proba_dict:
@@ -960,45 +1116,47 @@
         if record_pred_time:
             return model_pred_dict, model_pred_time_dict
         else:
             return model_pred_dict
 
     def get_model_oof(self, model: str) -> np.ndarray:
         """Gets the out of fold prediction probabilities for a bagged ensemble model"""
-        model_type = self.get_model_attribute(model=model, attribute='type')
+        model_type = self.get_model_attribute(model=model, attribute="type")
         if issubclass(model_type, BaggedEnsembleModel):
-            model_path = self.get_model_attribute(model=model, attribute='path')
+            model_path = self.get_model_attribute(model=model, attribute="path")
             return model_type.load_oof(path=model_path)
         else:
-            raise AssertionError(f'Model {model} must be a BaggedEnsembleModel to return oof_pred_proba')
+            raise AssertionError(f"Model {model} must be a BaggedEnsembleModel to return oof_pred_proba")
 
     def _update_pred_proba_dict_with_val_cache(self, model_set: set, model_pred_proba_dict):
         """For each model in model_set, check if y_pred_proba_val is cached to disk. If so, load and add it to model_pred_proba_dict"""
         for model in model_set:
-            y_pred_proba = self.get_model_attribute(model, attribute='cached_y_pred_proba_val', default=None)
+            y_pred_proba = self.get_model_attribute(model, attribute="cached_y_pred_proba_val", default=None)
             if isinstance(y_pred_proba, bool):
                 if y_pred_proba:
                     try:
                         y_pred_proba = self._load_model_y_pred_proba_val(model)
                     except FileNotFoundError:
                         y_pred_proba = None
                 else:
                     y_pred_proba = None
             if y_pred_proba is not None:
                 model_pred_proba_dict[model] = y_pred_proba
         model_set = model_set.difference(set(model_pred_proba_dict.keys()))
         return model_set, model_pred_proba_dict
 
-    def get_inputs_to_stacker(self,
-                              X: pd.DataFrame,
-                              base_models: List[str],
-                              model_pred_proba_dict: Optional[dict] = None,
-                              fit: bool = False,
-                              use_orig_features: bool = True,
-                              use_val_cache: bool = False) -> pd.DataFrame:
+    def get_inputs_to_stacker(
+        self,
+        X: pd.DataFrame,
+        base_models: List[str],
+        model_pred_proba_dict: Optional[dict] = None,
+        fit: bool = False,
+        use_orig_features: bool = True,
+        use_val_cache: bool = False,
+    ) -> pd.DataFrame:
         """
         Returns the valid X input for a stacker model with base models equal to `base_models`.
 
         Parameters
         ----------
         X : pd.DataFrame
             Input data to augment.
@@ -1024,18 +1182,17 @@
         X : DataFrame, an updated DataFrame with the additional stack features from `base_models`.
         """
         if not base_models:
             return X
         if fit:
             model_pred_proba_dict = self.get_model_oof_dict(models=base_models)
         else:
-            model_pred_proba_dict = self.get_model_pred_proba_dict(X=X,
-                                                                   models=base_models,
-                                                                   model_pred_proba_dict=model_pred_proba_dict,
-                                                                   use_val_cache=use_val_cache)
+            model_pred_proba_dict = self.get_model_pred_proba_dict(
+                X=X, models=base_models, model_pred_proba_dict=model_pred_proba_dict, use_val_cache=use_val_cache
+            )
         pred_proba_list = [model_pred_proba_dict[model] for model in base_models]
         stack_column_names, _ = self._get_stack_column_names(models=base_models)
         X_stacker = convert_pred_probas_to_df(pred_proba_list=pred_proba_list, problem_type=self.problem_type, columns=stack_column_names, index=X.index)
         if use_orig_features:
             X = pd.concat([X_stacker, X], axis=1)
         else:
             X = X_stacker
@@ -1043,18 +1200,18 @@
 
     def _get_stack_column_names(self, models: List[str]) -> Tuple[List[str], int]:
         """
         Get the stack column names generated when the provided models are used as base models in a stack ensemble.
         Additionally output the number of columns per model as an int.
         """
         if self.problem_type in [MULTICLASS, SOFTCLASS]:
-            stack_column_names = [stack_column_prefix + '_' + str(cls) for stack_column_prefix in models for cls in range(self.num_classes)]
+            stack_column_names = [stack_column_prefix + "_" + str(cls) for stack_column_prefix in models for cls in range(self.num_classes)]
             num_columns_per_model = self.num_classes
         elif self.problem_type == QUANTILE:
-            stack_column_names = [stack_column_prefix + '_' + str(q) for stack_column_prefix in models for q in self.quantile_levels]
+            stack_column_names = [stack_column_prefix + "_" + str(q) for stack_column_prefix in models for q in self.quantile_levels]
             num_columns_per_model = len(self.quantile_levels)
         else:
             stack_column_names = models
             num_columns_per_model = 1
         return stack_column_names, num_columns_per_model
 
     # You must have previously called fit() with cache_data=True
@@ -1095,65 +1252,78 @@
                 reuse_first_fold = False
                 if isinstance(model, BaggedEnsembleModel):
                     # Re-use if model is already _FULL and no X_val
                     if X_val is None:
                         reuse_first_fold = not model._bagged_mode
                 if not reuse_first_fold:
                     if isinstance(model, BaggedEnsembleModel):
-                        can_refit_full = model._get_tags_child().get('can_refit_full', False)
+                        can_refit_full = model._get_tags_child().get("can_refit_full", False)
                     else:
-                        can_refit_full = model._get_tags().get('can_refit_full', False)
+                        can_refit_full = model._get_tags().get("can_refit_full", False)
                     reuse_first_fold = not can_refit_full
                 if reuse_first_fold:
                     # Perform fallback black-box refit logic that doesn't retrain.
                     model_full = model.convert_to_refit_full_via_copy()
-                    logger.log(20, f'Fitting model: {model_full.name} | Skipping fit via cloning parent ...')
+                    logger.log(20, f"Fitting model: {model_full.name} | Skipping fit via cloning parent ...")
                     self._add_model(model_full, stack_name=REFIT_FULL_NAME, level=level)
                     self.save_model(model_full)
                     models_trained = [model_full.name]
                 else:
                     model_full = model.convert_to_refit_full_template()
                     # Mitigates situation where bagged models barely had enough memory and refit requires more. Worst case results in OOM, but this lowers chance of failure.
-                    model_full._user_params_aux['max_memory_usage_ratio'] = model.params_aux['max_memory_usage_ratio'] * 1.15
+                    model_full._user_params_aux["max_memory_usage_ratio"] = model.params_aux["max_memory_usage_ratio"] * 1.15
                     # TODO: Do it for all models in the level at once to avoid repeated processing of data?
                     base_model_names = self.get_base_model_names(model_name)
                     models_trained = self.stack_new_level_core(
-                        X=X, y=y, X_val=X_val, y_val=y_val, X_unlabeled=X_unlabeled,
-                        models=[model_full], base_model_names=base_model_names, level=level, stack_name=REFIT_FULL_NAME,
-                        hyperparameter_tune_kwargs=None, feature_prune=False, k_fold=0, n_repeats=1, ensemble_type=type(model), refit_full=True
+                        X=X,
+                        y=y,
+                        X_val=X_val,
+                        y_val=y_val,
+                        X_unlabeled=X_unlabeled,
+                        models=[model_full],
+                        base_model_names=base_model_names,
+                        level=level,
+                        stack_name=REFIT_FULL_NAME,
+                        hyperparameter_tune_kwargs=None,
+                        feature_prune=False,
+                        k_fold=0,
+                        n_repeats=1,
+                        ensemble_type=type(model),
+                        refit_full=True,
                     )
                 if len(models_trained) == 1:
                     model_full_dict[model_name] = models_trained[0]
                 for model_trained in models_trained:
-                    self._update_model_attr(model_trained,
-                                            refit_full=True,
-                                            refit_full_parent=model_name,
-                                            refit_full_parent_val_score=self.get_model_attribute(model_name, 'val_score'),
-                                            )
+                    self._update_model_attr(
+                        model_trained,
+                        refit_full=True,
+                        refit_full_parent=model_name,
+                        refit_full_parent_val_score=self.get_model_attribute(model_name, "val_score"),
+                    )
                 models_trained_full += models_trained
 
         keys_to_del = []
         for model in model_full_dict.keys():
             if model_full_dict[model] not in models_trained_full:
                 keys_to_del.append(model)
         for key in keys_to_del:
             del model_full_dict[key]
         self.save()  # TODO: This could be more efficient by passing in arg to not save if called by refit_ensemble_full since it saves anyways later.
         return models_trained_full
 
     # Fits _FULL models and links them in the stack so _FULL models only use other _FULL models as input during stacking
     # If model is specified, will fit all _FULL models that are ancestors of the provided model, automatically linking them.
     # If no model is specified, all models are refit and linked appropriately.
-    def refit_ensemble_full(self, model='all') -> dict:
-        if model == 'all':
+    def refit_ensemble_full(self, model="all") -> dict:
+        if model == "all":
             ensemble_set = self.get_model_names()
         elif isinstance(model, list):
             ensemble_set = self.get_minimum_models_set(model)
         else:
-            if model == 'best':
+            if model == "best":
                 model = self.get_model_best()
             ensemble_set = self.get_minimum_model_set(model)
         existing_models = self.get_model_names()
         ensemble_set_valid = []
         model_full_dict = self.get_model_full_dict()
         for model in ensemble_set:
             if model in model_full_dict and model_full_dict[model] in existing_models:
@@ -1170,16 +1340,16 @@
             # TODO: Consider moving base model info to a separate pkl file so that it can be edited without having to load/save the model again
             #  Downside: Slower inference speed when models are not persisted in memory prior.
             model_loaded = self.load_model(model_full)
             if isinstance(model_loaded, StackerEnsembleModel):
                 for stack_column_prefix in model_loaded.stack_column_prefix_lst:
                     base_model = model_loaded.stack_column_prefix_to_model_map[stack_column_prefix]
                     new_base_model = model_full_dict[base_model]
-                    new_base_model_type = self.get_model_attribute(model=new_base_model, attribute='type')
-                    new_base_model_path = self.get_model_attribute(model=new_base_model, attribute='path')
+                    new_base_model_type = self.get_model_attribute(model=new_base_model, attribute="type")
+                    new_base_model_path = self.get_model_attribute(model=new_base_model, attribute="path")
 
                     model_loaded.base_model_paths_dict[new_base_model] = new_base_model_path
                     model_loaded.base_model_types_dict[new_base_model] = new_base_model_type
                     model_loaded.base_model_names.append(new_base_model)
                     model_loaded.stack_column_prefix_to_model_map[stack_column_prefix] = new_base_model
 
             model_loaded.save()  # TODO: Avoid this!
@@ -1193,44 +1363,48 @@
                     self.model_graph.add_edge(base_model_name, model_loaded.name)
 
         self.save()
         return self.get_model_full_dict()
 
     def get_refit_full_parent(self, model: str) -> str:
         """Get refit full model's parent. If model does not have a parent, return `model`."""
-        return self.get_model_attribute(model=model, attribute='refit_full_parent', default=model)
+        return self.get_model_attribute(model=model, attribute="refit_full_parent", default=model)
 
     # TODO: Take best performance model with lowest inference
     def get_model_best(self, can_infer=None, allow_full=True, infer_limit=None):
         models = self.get_model_names(can_infer=can_infer)
         if not models:
-            raise AssertionError('Trainer has no fit models that can infer.')
-        models_full = self.get_models_attribute_dict(models=models, attribute='refit_full_parent')
+            raise AssertionError("Trainer has no fit models that can infer.")
+        models_full = self.get_models_attribute_dict(models=models, attribute="refit_full_parent")
         if not allow_full:
             models = [model for model in models if model not in models_full]
 
         if infer_limit is not None:
-            models_predict_1_time = self.get_models_attribute_full(models=models, attribute='predict_1_time')
+            models_predict_1_time = self.get_models_attribute_full(models=models, attribute="predict_1_time")
             for model_key in models_predict_1_time:
                 if models_predict_1_time[model_key] > infer_limit:
                     models.remove(model_key)
-                    logger.log(20, f'Removing {model_key}')
+                    logger.log(20, f"Removing {model_key}")
         if not models:
-            raise AssertionError(f'Trainer has no fit models that can infer while satisfying the constraints: (infer_limit={infer_limit}, allow_full={allow_full}).')
-        model_performances = self.get_models_attribute_dict(models=models, attribute='val_score')
-        models_predict_time = self.get_models_attribute_full(models=models, attribute='predict_time')  # FIXME: Refit_full???
+            raise AssertionError(
+                f"Trainer has no fit models that can infer while satisfying the constraints: (infer_limit={infer_limit}, allow_full={allow_full})."
+            )
+        model_performances = self.get_models_attribute_dict(models=models, attribute="val_score")
+        models_predict_time = self.get_models_attribute_full(models=models, attribute="predict_time")  # FIXME: Refit_full???
 
         perfs = [(m, model_performances[m], models_predict_time[m]) for m in models if model_performances[m] is not None]
         if not perfs:
             models = [m for m in models if m in models_full]
-            perfs = [(m, self.get_model_attribute(model=m, attribute='refit_full_parent_val_score'), models_predict_time[m]) for m in models]
+            perfs = [(m, self.get_model_attribute(model=m, attribute="refit_full_parent_val_score"), models_predict_time[m]) for m in models]
             if not perfs:
-                raise AssertionError('No fit models that can infer exist with a validation score to choose the best model.')
+                raise AssertionError("No fit models that can infer exist with a validation score to choose the best model.")
             elif not allow_full:
-                raise AssertionError('No fit models that can infer exist with a validation score to choose the best model, but refit_full models exist. Set `allow_full=True` to get the best refit_full model.')
+                raise AssertionError(
+                    "No fit models that can infer exist with a validation score to choose the best model, but refit_full models exist. Set `allow_full=True` to get the best refit_full model."
+                )
         return max(perfs, key=lambda i: (i[1], -i[2]))[0]
 
     def save_model(self, model, reduce_memory=True):
         # TODO: In future perhaps give option for the reduce_memory_size arguments, perhaps trainer level variables specified by user?
         if reduce_memory:
             model.reduce_memory_size(remove_fit=True, remove_info=False, requires_save=True)
         if self.low_memory:
@@ -1242,125 +1416,135 @@
         models = self.models
         if self.low_memory:
             self.models = {}
         save_pkl.save(path=self.path + self.trainer_file_name, object=self)
         if self.low_memory:
             self.models = models
 
-    def compile_models(self, model_names='all', with_ancestors=False, compiler_configs=None) -> List[str]:
+    def compile_models(self, model_names="all", with_ancestors=False, compiler_configs=None) -> List[str]:
         """
         Compile a list of models for accelerated prediction.
 
         Parameters
         ----------
         model_names : str or list
             A list of model names for model compilation. Alternatively, this can be 'all' or 'best'.
         compiler_configs: dict, default=None
             Model specific compiler options.
-            This can be useful to specify the compiler backend for a specific model, 
+            This can be useful to specify the compiler backend for a specific model,
             e.g. {"RandomForest": {"compiler": "onnx"}}
         """
-        if model_names == 'all':
+        if model_names == "all":
             model_names = self.get_model_names(can_infer=True)
-        elif model_names == 'best':
+        elif model_names == "best":
             if self.model_best is not None:
                 model_names = [self.model_best]
             else:
                 model_names = [self.get_model_best(can_infer=True)]
         if not isinstance(model_names, list):
-            raise ValueError(f'model_names must be a list of model names. Invalid value: {model_names}')
+            raise ValueError(f"model_names must be a list of model names. Invalid value: {model_names}")
         if with_ancestors:
             model_names = self.get_minimum_models_set(model_names)
 
-        logger.log(20, f'Compiling {len(model_names)} Models ...')
+        logger.log(20, f"Compiling {len(model_names)} Models ...")
         total_compile_time = 0
 
         model_names_to_compile = []
         model_names_to_configs_dict = dict()
         for model_name in model_names:
-            model_type_inner = self.get_model_attribute(model_name, 'type_inner')
+            model_type_inner = self.get_model_attribute(model_name, "type_inner")
             # Get model specific compiler options
             # Model type can be described with either model type, or model name as string
             if model_name in compiler_configs:
                 config = compiler_configs[model_name]
             elif model_type_inner in compiler_configs:
                 config = compiler_configs[model_type_inner]
             else:
                 config = None
             if config is not None:
                 model_names_to_compile.append(model_name)
                 model_names_to_configs_dict[model_name] = config
             else:
-                logger.log(20, f'Skipping compilation for {model_name} ... (No config specified)')
+                logger.log(20, f"Skipping compilation for {model_name} ... (No config specified)")
         for model_name in model_names_to_compile:
             model = self.load_model(model_name)
             config = model_names_to_configs_dict[model_name]
 
             # Check if already compiled, or if can't compile due to missing dependencies,
             # or if model hasn't implemented compiling.
-            if 'compiler' in config and model.get_compiler_name() == config['compiler']:
+            if "compiler" in config and model.get_compiler_name() == config["compiler"]:
                 logger.log(20, f'Skipping compilation for {model_name} ... (Already compiled with "{model.get_compiler_name()}" backend)')
             elif model.can_compile(compiler_configs=config):
-                logger.log(20, f'Compiling model: {model.name} ... Config = {config}')
+                logger.log(20, f"Compiling model: {model.name} ... Config = {config}")
                 compile_start_time = time.time()
                 model.compile(compiler_configs=config)
                 compile_end_time = time.time()
                 model.compile_time = compile_end_time - compile_start_time
                 compile_type = model.get_compiler_name()
                 total_compile_time += model.compile_time
 
                 # Update model_graph in order to put compile_time into leaderboard,
                 # since models are saved right after training.
-                self.model_graph.nodes[model.name]['compile_time'] = model.compile_time
+                self.model_graph.nodes[model.name]["compile_time"] = model.compile_time
                 self.save_model(model, reduce_memory=False)
                 logger.log(20, f'\tCompiled model with "{compile_type}" backend ...')
-                logger.log(20, f'\t{round(model.compile_time, 2)}s\t = Compile    runtime')
+                logger.log(20, f"\t{round(model.compile_time, 2)}s\t = Compile    runtime")
             else:
-                logger.log(20, f'Skipping compilation for {model.name} ... (Unable to compile with the provided config: {config})')
-        logger.log(20, f'Finished compiling models, total runtime = {round(total_compile_time, 2)}s.')
+                logger.log(20, f"Skipping compilation for {model.name} ... (Unable to compile with the provided config: {config})")
+        logger.log(20, f"Finished compiling models, total runtime = {round(total_compile_time, 2)}s.")
         self.save()
         return model_names
 
-    def persist_models(self, model_names='all', with_ancestors=False, max_memory=None) -> List[str]:
-        if model_names == 'all':
+    def persist_models(self, model_names="all", with_ancestors=False, max_memory=None) -> List[str]:
+        if model_names == "all":
             model_names = self.get_model_names()
-        elif model_names == 'best':
+        elif model_names == "best":
             if self.model_best is not None:
                 model_names = [self.model_best]
             else:
                 model_names = [self.get_model_best(can_infer=True)]
         if not isinstance(model_names, list):
-            raise ValueError(f'model_names must be a list of model names. Invalid value: {model_names}')
+            raise ValueError(f"model_names must be a list of model names. Invalid value: {model_names}")
         if with_ancestors:
             model_names = self.get_minimum_models_set(model_names)
         model_names_already_persisted = [model_name for model_name in model_names if model_name in self.models]
         if model_names_already_persisted:
-            logger.log(30, f'The following {len(model_names_already_persisted)} models were already persisted and will be ignored in the model loading process: {model_names_already_persisted}')
+            logger.log(
+                30,
+                f"The following {len(model_names_already_persisted)} models were already persisted and will be ignored in the model loading process: {model_names_already_persisted}",
+            )
         model_names = [model_name for model_name in model_names if model_name not in model_names_already_persisted]
         if not model_names:
-            logger.log(30, f'No valid unpersisted models were specified to be persisted, so no change in model persistence was performed.')
+            logger.log(30, f"No valid unpersisted models were specified to be persisted, so no change in model persistence was performed.")
             return []
         if max_memory is not None:
+
             @disable_if_lite_mode(ret=True)
             def _check_memory():
                 info = self.get_models_info(model_names)
-                model_mem_size_map = {model: info[model]['memory_size'] for model in model_names}
+                model_mem_size_map = {model: info[model]["memory_size"] for model in model_names}
                 for model in model_mem_size_map:
-                    if 'children_info' in info[model]:
-                        for child in info[model]['children_info'].values():
-                            model_mem_size_map[model] += child['memory_size']
+                    if "children_info" in info[model]:
+                        for child in info[model]["children_info"].values():
+                            model_mem_size_map[model] += child["memory_size"]
                 total_mem_required = sum(model_mem_size_map.values())
                 available_mem = ResourceManager.get_available_virtual_mem()
                 memory_proportion = total_mem_required / available_mem
                 if memory_proportion > max_memory:
-                    logger.log(30, f'Models will not be persisted in memory as they are expected to require {round(memory_proportion * 100, 2)}% of memory, which is greater than the specified max_memory limit of {round(max_memory*100, 2)}%.')
-                    logger.log(30, f'\tModels will be loaded on-demand from disk to maintain safe memory usage, increasing inference latency. If inference latency is a concern, try to use smaller models or increase the value of max_memory.')
+                    logger.log(
+                        30,
+                        f"Models will not be persisted in memory as they are expected to require {round(memory_proportion * 100, 2)}% of memory, which is greater than the specified max_memory limit of {round(max_memory*100, 2)}%.",
+                    )
+                    logger.log(
+                        30,
+                        f"\tModels will be loaded on-demand from disk to maintain safe memory usage, increasing inference latency. If inference latency is a concern, try to use smaller models or increase the value of max_memory.",
+                    )
                     return False
                 else:
-                    logger.log(20, f'Persisting {len(model_names)} models in memory. Models will require {round(memory_proportion*100, 2)}% of memory.')
+                    logger.log(20, f"Persisting {len(model_names)} models in memory. Models will require {round(memory_proportion*100, 2)}% of memory.")
                 return True
 
             if not _check_memory():
                 return []
 
         models = []
         for model_name in model_names:
@@ -1380,73 +1564,88 @@
     def load_model(self, model_name: str, path: str = None, model_type=None) -> AbstractModel:
         if isinstance(model_name, AbstractModel):
             return model_name
         if model_name in self.models.keys():
             return self.models[model_name]
         else:
             if path is None:
-                path = self.get_model_attribute(model=model_name, attribute='path')
+                path = self.get_model_attribute(model=model_name, attribute="path")
             if model_type is None:
-                model_type = self.get_model_attribute(model=model_name, attribute='type')
+                model_type = self.get_model_attribute(model=model_name, attribute="type")
             return model_type.load(path=path, reset_paths=self.reset_paths)
 
-    def unpersist_models(self, model_names='all') -> list:
-        if model_names == 'all':
+    def unpersist_models(self, model_names="all") -> list:
+        if model_names == "all":
             model_names = list(self.models.keys())
         if not isinstance(model_names, list):
-            raise ValueError(f'model_names must be a list of model names. Invalid value: {model_names}')
+            raise ValueError(f"model_names must be a list of model names. Invalid value: {model_names}")
         unpersisted_models = []
         for model in model_names:
             if model in self.models:
                 self.models.pop(model)
                 unpersisted_models.append(model)
         if unpersisted_models:
-            logger.log(20, f'Unpersisted {len(unpersisted_models)} models: {unpersisted_models}')
+            logger.log(20, f"Unpersisted {len(unpersisted_models)} models: {unpersisted_models}")
         else:
-            logger.log(30, f'No valid persisted models were specified to be unpersisted, so no change in model persistence was performed.')
+            logger.log(30, f"No valid persisted models were specified to be unpersisted, so no change in model persistence was performed.")
         return unpersisted_models
 
-    def generate_weighted_ensemble(self, X, y, level, base_model_names, k_fold=1, n_repeats=1, stack_name=None, hyperparameters=None, ag_args_fit=None,
-                                   time_limit=None, name_suffix: str = None, save_bag_folds=None, check_if_best=True, child_hyperparameters=None,
-                                   get_models_func=None) -> List[str]:
+    def generate_weighted_ensemble(
+        self,
+        X,
+        y,
+        level,
+        base_model_names,
+        k_fold=1,
+        n_repeats=1,
+        stack_name=None,
+        hyperparameters=None,
+        ag_args_fit=None,
+        time_limit=None,
+        name_suffix: str = None,
+        save_bag_folds=None,
+        check_if_best=True,
+        child_hyperparameters=None,
+        get_models_func=None,
+    ) -> List[str]:
         if get_models_func is None:
             get_models_func = self.construct_model_templates
         if len(base_model_names) == 0:
-            logger.log(20, 'No base models to train on, skipping weighted ensemble...')
+            logger.log(20, "No base models to train on, skipping weighted ensemble...")
             return []
 
         if child_hyperparameters is None:
             child_hyperparameters = {}
 
         if save_bag_folds is None:
-            can_infer_dict = self.get_models_attribute_dict('can_infer', models=base_model_names)
+            can_infer_dict = self.get_models_attribute_dict("can_infer", models=base_model_names)
             if False in can_infer_dict.values():
                 save_bag_folds = False
             else:
                 save_bag_folds = True
 
         weighted_ensemble_model, _ = get_models_func(
             hyperparameters={
-                'default': {
-                    'ENS_WEIGHTED': [child_hyperparameters],
+                "default": {
+                    "ENS_WEIGHTED": [child_hyperparameters],
                 }
             },
             ensemble_type=WeightedEnsembleModel,
             ensemble_kwargs=dict(
                 base_model_names=base_model_names,
-                base_model_paths_dict=self.get_models_attribute_dict(attribute='path', models=base_model_names),
-                base_model_types_dict=self.get_models_attribute_dict(attribute='type', models=base_model_names),
-                base_model_types_inner_dict=self.get_models_attribute_dict(attribute='type_inner', models=base_model_names),
-                base_model_performances_dict=self.get_models_attribute_dict(attribute='val_score', models=base_model_names),
+                base_model_paths_dict=self.get_models_attribute_dict(attribute="path", models=base_model_names),
+                base_model_types_dict=self.get_models_attribute_dict(attribute="type", models=base_model_names),
+                base_model_types_inner_dict=self.get_models_attribute_dict(attribute="type_inner", models=base_model_names),
+                base_model_performances_dict=self.get_models_attribute_dict(attribute="val_score", models=base_model_names),
                 hyperparameters=hyperparameters,
                 random_state=level + self.random_state,
             ),
-            ag_args={'name_bag_suffix': ''},
+            ag_args={"name_bag_suffix": ""},
             ag_args_fit=ag_args_fit,
-            ag_args_ensemble={'save_bag_folds': save_bag_folds},
+            ag_args_ensemble={"save_bag_folds": save_bag_folds},
             name_suffix=name_suffix,
             level=level,
         )
         weighted_ensemble_model = weighted_ensemble_model[0]
         w = None
         if self.weight_evaluation:
             X, w = extract_column(X, self.sample_weight)
@@ -1466,91 +1665,81 @@
             fit_kwargs=dict(num_classes=self.num_classes, groups=None),  # FIXME: Is this the right way to do this?
         )
         for weighted_ensemble_model_name in models:
             if check_if_best and weighted_ensemble_model_name in self.get_model_names():
                 if self.model_best is None:
                     self.model_best = weighted_ensemble_model_name
                 else:
-                    best_score = self.get_model_attribute(self.model_best, 'val_score')
-                    cur_score = self.get_model_attribute(weighted_ensemble_model_name, 'val_score')
+                    best_score = self.get_model_attribute(self.model_best, "val_score")
+                    cur_score = self.get_model_attribute(weighted_ensemble_model_name, "val_score")
                     if best_score is not None and cur_score > best_score:
                         # new best model
                         self.model_best = weighted_ensemble_model_name
         return models
 
     def _train_single(self, X, y, model: AbstractModel, X_val=None, y_val=None, total_resources=None, **model_fit_kwargs) -> AbstractModel:
         """
         Trains model but does not add the trained model to this Trainer.
         Returns trained model object.
         """
         model = model.fit(X=X, y=y, X_val=X_val, y_val=y_val, total_resources=total_resources, **model_fit_kwargs)
         return model
 
     def _train_and_save(
-        self,
-        X,
-        y,
-        model: AbstractModel,
-        X_val=None,
-        y_val=None,
-        stack_name='core',
-        level=1,
-        compute_score=True,
-        total_resources=None,
-        **model_fit_kwargs
+        self, X, y, model: AbstractModel, X_val=None, y_val=None, stack_name="core", level=1, compute_score=True, total_resources=None, **model_fit_kwargs
     ) -> List[str]:
         """
         Trains model and saves it to disk, returning a list with a single element: The name of the model, or no elements if training failed.
         If the model name is returned:
             The model can be accessed via self.load_model(model.name).
             The model will have metadata information stored in self.model_graph.
             The model's name will be appended to self.models_level[stack_name][level]
             The model will be accessible and usable through any Trainer function that takes as input 'model' or 'model_name'.
         Note: self._train_and_save should not be used outside of self._train_single_full
         """
-        X_pseudo = model_fit_kwargs.get('X_pseudo', None)
-        y_pseudo = model_fit_kwargs.get('y_pseudo', None)
+        X_pseudo = model_fit_kwargs.get("X_pseudo", None)
+        y_pseudo = model_fit_kwargs.get("y_pseudo", None)
         fit_start_time = time.time()
-        time_limit = model_fit_kwargs.get('time_limit', None)
+        time_limit = model_fit_kwargs.get("time_limit", None)
         model_names_trained = []
         y_pred_proba_val = None
         try:
-            fit_log_message = f'Fitting model: {model.name} ...'
+            fit_log_message = f"Fitting model: {model.name} ..."
             if time_limit is not None:
                 if time_limit <= 0:
-                    logger.log(15, f'Skipping {model.name} due to lack of time remaining.')
+                    logger.log(15, f"Skipping {model.name} due to lack of time remaining.")
                     return model_names_trained
                 if self._time_limit is not None and self._time_train_start is not None:
                     time_left_total = self._time_limit - (fit_start_time - self._time_train_start)
                 else:
                     time_left_total = time_limit
-                fit_log_message += f' Training model for up to {round(time_limit, 2)}s of the {round(time_left_total, 2)}s of remaining time.'
+                fit_log_message += f" Training model for up to {round(time_limit, 2)}s of the {round(time_left_total, 2)}s of remaining time."
             logger.log(20, fit_log_message)
 
             if isinstance(model, BaggedEnsembleModel) and not compute_score:
                 # Do not perform OOF predictions when we don't compute a score.
-                model_fit_kwargs['_skip_oof'] = True
+                model_fit_kwargs["_skip_oof"] = True
 
             # If model is not bagged model and not stacked then pseudolabeled data needs to be incorporated at this level
             # Bagged model does validation on the fit level where as single models do it separately. Hence this if statement
             # is required
             if not isinstance(model, BaggedEnsembleModel) and X_pseudo is not None and y_pseudo is not None and X_pseudo.columns.equals(X.columns):
                 X_w_pseudo = pd.concat([X, X_pseudo])
                 y_w_pseudo = pd.concat([y, y_pseudo])
-                model_fit_kwargs.pop('X_pseudo')
-                model_fit_kwargs.pop('y_pseudo')
-                logger.log(15, f'{len(X_pseudo)} extra rows of pseudolabeled data added to training set for {model.name}')
+                model_fit_kwargs.pop("X_pseudo")
+                model_fit_kwargs.pop("y_pseudo")
+                logger.log(15, f"{len(X_pseudo)} extra rows of pseudolabeled data added to training set for {model.name}")
                 model = self._train_single(X_w_pseudo, y_w_pseudo, model, X_val, y_val, **model_fit_kwargs)
             else:
                 model = self._train_single(X, y, model, X_val, y_val, total_resources=total_resources, **model_fit_kwargs)
 
             fit_end_time = time.time()
             if self.weight_evaluation:
-                w = model_fit_kwargs.get('sample_weight', None)
-                w_val = model_fit_kwargs.get('sample_weight_val', None)
+                w = model_fit_kwargs.get("sample_weight", None)
+                w_val = model_fit_kwargs.get("sample_weight_val", None)
             else:
                 w = None
                 w_val = None
             if not compute_score:
                 score = None
                 model.predict_time = None
             elif isinstance(model, BaggedEnsembleModel):
@@ -1575,55 +1764,55 @@
                     model.predict_time = None
                 else:
                     model.predict_time = pred_end_time - fit_end_time
             model.val_score = score
             # TODO: Add recursive=True to avoid repeatedly loading models each time this is called for bagged ensembles (especially during repeated bagging)
             self.save_model(model=model)
         except TimeLimitExceeded:
-            logger.log(20, f'\tTime limit exceeded... Skipping {model.name}.')
+            logger.log(20, f"\tTime limit exceeded... Skipping {model.name}.")
             # logger.log(20, '\tTime wasted: ' + str(time.time() - fit_start_time))
             self._models_failed_to_train.append(model.name)
             del model
         except NotEnoughMemoryError:
-            logger.warning(f'\tNot enough memory to train {model.name}... Skipping this model.')
+            logger.warning(f"\tNot enough memory to train {model.name}... Skipping this model.")
             self._models_failed_to_train.append(model.name)
             del model
         except NoValidFeatures:
-            logger.warning(f'\tNo valid features to train {model.name}... Skipping this model.')
+            logger.warning(f"\tNo valid features to train {model.name}... Skipping this model.")
             self._models_failed_to_train.append(model.name)
             del model
         except NoGPUError:
-            logger.warning(f'\tNo GPUs available to train {model.name}... Skipping this model.')
+            logger.warning(f"\tNo GPUs available to train {model.name}... Skipping this model.")
             self._models_failed_to_train.append(model.name)
             del model
         except NotEnoughCudaMemoryError:
-            logger.warning(f'\tNot enough CUDA memory available to train {model.name}... Skipping this model.')
+            logger.warning(f"\tNot enough CUDA memory available to train {model.name}... Skipping this model.")
             self._models_failed_to_train.append(model.name)
             del model
         except ImportError as err:
-            logger.error(f'\tWarning: Exception caused {model.name} to fail during training (ImportError)... Skipping this model.')
-            logger.error(f'\t\t{err}')
+            logger.error(f"\tWarning: Exception caused {model.name} to fail during training (ImportError)... Skipping this model.")
+            logger.error(f"\t\t{err}")
             self._models_failed_to_train.append(model.name)
             if self.verbosity > 2:
-                logger.exception('Detailed Traceback:')
+                logger.exception("Detailed Traceback:")
         except Exception as err:
-            logger.error(f'\tWarning: Exception caused {model.name} to fail during training... Skipping this model.')
-            logger.error(f'\t\t{err}')
+            logger.error(f"\tWarning: Exception caused {model.name} to fail during training... Skipping this model.")
+            logger.error(f"\t\t{err}")
             self._models_failed_to_train.append(model.name)
             if self.verbosity > 0:
-                logger.exception('Detailed Traceback:')
+                logger.exception("Detailed Traceback:")
             del model
         else:
             self._add_model(model=model, stack_name=stack_name, level=level, y_pred_proba_val=y_pred_proba_val)
             model_names_trained.append(model.name)
             if self.low_memory:
                 del model
         return model_names_trained
 
-    def _add_model(self, model: AbstractModel, stack_name: str = 'core', level: int = 1, y_pred_proba_val=None) -> bool:
+    def _add_model(self, model: AbstractModel, stack_name: str = "core", level: int = 1, y_pred_proba_val=None) -> bool:
         """
         Registers the fit model in the Trainer object. Stores information such as model performance, save path, model type, and more.
         To use a model in Trainer, self._add_model must be called.
         If self.low_memory, then the model object will be deleted after this call. Use Trainer directly to leverage the model further.
 
         Parameters
         ----------
@@ -1637,31 +1826,33 @@
             The model's base_models (if it has any) must all be a lower level than the model.
 
         Returns
         -------
         boolean, True if model was registered, False if model was found to be invalid and not registered.
         """
         if model.val_score is not None and np.isnan(model.val_score):
-            logger.warning(f'WARNING: {model.name} has a val_score of {model.val_score} (NaN)! This should never happen. The model will not be saved to avoid instability.')
+            logger.warning(
+                f"WARNING: {model.name} has a val_score of {model.val_score} (NaN)! This should never happen. The model will not be saved to avoid instability."
+            )
             return False
         # TODO: Add to HPO
         if isinstance(model, BaggedEnsembleModel):
             type_inner = model._child_type
         else:
             type_inner = type(model)
-        num_children = len(model.models) if hasattr(model, 'models') else 1
+        num_children = len(model.models) if hasattr(model, "models") else 1
         predict_child_time = model.predict_time / num_children if model.predict_time is not None else None
         predict_1_child_time = model.predict_1_time / num_children if model.predict_1_time is not None else None
         fit_metadata = model.get_fit_metadata()
 
         extra_attributes = dict()
         if y_pred_proba_val is not None:
             # Cache y_pred_proba_val for later reuse to avoid redundant predict calls
             self._save_model_y_pred_proba_val(model=model.name, y_pred_proba_val=y_pred_proba_val)
-            extra_attributes['cached_y_pred_proba_val'] = True
+            extra_attributes["cached_y_pred_proba_val"] = True
 
         self.model_graph.add_node(
             model.name,
             fit_time=model.fit_time,
             compile_time=model.compile_time,
             predict_time=model.predict_time,
             predict_1_time=model.predict_1_time,
@@ -1682,38 +1873,42 @@
         )
         if isinstance(model, StackerEnsembleModel):
             prior_models = self.get_model_names()
             # TODO: raise exception if no base models and level != 1?
             for stack_column_prefix in model.stack_column_prefix_lst:
                 base_model_name = model.stack_column_prefix_to_model_map[stack_column_prefix]
                 if base_model_name not in prior_models:
-                    raise AssertionError(f"Model '{model.name}' depends on model '{base_model_name}', but '{base_model_name}' is not registered as a trained model! Valid models: {prior_models}")
-                elif level <= self.model_graph.nodes[base_model_name]['level']:
-                    raise AssertionError(f"Model '{model.name}' depends on model '{base_model_name}', but '{base_model_name}' is not in a lower stack level. ('{model.name}' level: {level}, '{base_model_name}' level: {self.model_graph.nodes[base_model_name]['level']})")
+                    raise AssertionError(
+                        f"Model '{model.name}' depends on model '{base_model_name}', but '{base_model_name}' is not registered as a trained model! Valid models: {prior_models}"
+                    )
+                elif level <= self.model_graph.nodes[base_model_name]["level"]:
+                    raise AssertionError(
+                        f"Model '{model.name}' depends on model '{base_model_name}', but '{base_model_name}' is not in a lower stack level. ('{model.name}' level: {level}, '{base_model_name}' level: {self.model_graph.nodes[base_model_name]['level']})"
+                    )
                 self.model_graph.add_edge(base_model_name, model.name)
         self._log_model_stats(model)
         if self.low_memory:
             del model
         return True
 
     def _path_attr_model(self, model: str):
         """Returns directory where attributes are cached"""
-        return f'{self._path_attr}{model}{os.path.sep}'
+        return f"{self._path_attr}{model}{os.path.sep}"
 
     def _path_to_model_attr(self, model: str, attribute: str):
         """Returns pkl file path for a cached model attribute"""
-        return f'{self._path_attr_model(model)}{attribute}.pkl'
+        return f"{self._path_attr_model(model)}{attribute}.pkl"
 
     def _save_model_y_pred_proba_val(self, model: str, y_pred_proba_val):
         """Cache y_pred_proba_val for later reuse to avoid redundant predict calls"""
-        save_pkl.save(path=self._path_to_model_attr(model=model, attribute='y_pred_proba_val'), object=y_pred_proba_val)
+        save_pkl.save(path=self._path_to_model_attr(model=model, attribute="y_pred_proba_val"), object=y_pred_proba_val)
 
     def _load_model_y_pred_proba_val(self, model: str):
         """Load cached y_pred_proba_val for a given model"""
-        return load_pkl.load(path=self._path_to_model_attr(model=model, attribute='y_pred_proba_val'))
+        return load_pkl.load(path=self._path_to_model_attr(model=model, attribute="y_pred_proba_val"))
 
     # TODO: Once Python min-version is 3.8, can refactor to use positional-only argument for model
     #  https://peps.python.org/pep-0570/#empowering-library-authors
     #  Currently this method cannot accept the attribute key 'model' without making usage ugly.
     def _update_model_attr(self, model: str, **attributes):
         """Updates model node in graph with the input attributes dictionary"""
         if model not in self.model_graph:
@@ -1721,150 +1916,154 @@
         self.model_graph.nodes[model].update(attributes)
 
     def _log_model_stats(self, model):
         """Logs model fit time, val score, predict time, and predict_1_time"""
         model = self.load_model(model)
         if model.val_score is not None:
             if model.eval_metric.name != self.eval_metric.name:
-                logger.log(20, f'\tNote: model has different eval_metric than default.')
+                logger.log(20, f"\tNote: model has different eval_metric than default.")
             if not model.eval_metric.greater_is_better_internal:
-                sign_str = '-'
+                sign_str = "-"
             else:
-                sign_str = ''
-            logger.log(20, f'\t{round(model.val_score, 4)}\t = Validation score   ({sign_str}{model.eval_metric.name})')
+                sign_str = ""
+            logger.log(20, f"\t{round(model.val_score, 4)}\t = Validation score   ({sign_str}{model.eval_metric.name})")
         if model.fit_time is not None:
-            logger.log(20, f'\t{round(model.fit_time, 2)}s\t = Training   runtime')
+            logger.log(20, f"\t{round(model.fit_time, 2)}s\t = Training   runtime")
         if model.predict_time is not None:
-            logger.log(20, f'\t{round(model.predict_time, 2)}s\t = Validation runtime')
+            logger.log(20, f"\t{round(model.predict_time, 2)}s\t = Validation runtime")
         if model.predict_1_time is not None:
             fit_metadata = model.get_fit_metadata()
-            predict_1_batch_size = fit_metadata.get('predict_1_batch_size', None)
+            predict_1_batch_size = fit_metadata.get("predict_1_batch_size", None)
             assert predict_1_batch_size is not None, "predict_1_batch_size cannot be None if predict_1_time is not None"
             predict_1_time = model.predict_1_time
             predict_1_time_log, time_unit = convert_time_in_s_to_log_friendly(time_in_sec=predict_1_time)
-            logger.log(20, f'\t{round(predict_1_time_log, 3)}{time_unit}\t = Validation runtime (1 row | {predict_1_batch_size} batch size | MARGINAL)')
+            logger.log(20, f"\t{round(predict_1_time_log, 3)}{time_unit}\t = Validation runtime (1 row | {predict_1_batch_size} batch size | MARGINAL)")
 
-            predict_1_time_full = self.get_model_attribute_full(model=model.name, attribute='predict_1_time')
+            predict_1_time_full = self.get_model_attribute_full(model=model.name, attribute="predict_1_time")
             predict_1_time_full_log, time_unit = convert_time_in_s_to_log_friendly(time_in_sec=predict_1_time_full)
-            logger.log(20, f'\t{round(predict_1_time_full_log, 3)}{time_unit}\t = Validation runtime (1 row | {predict_1_batch_size} batch size)')
+            logger.log(20, f"\t{round(predict_1_time_full_log, 3)}{time_unit}\t = Validation runtime (1 row | {predict_1_batch_size} batch size)")
 
     # TODO: Split this to avoid confusion, HPO should go elsewhere?
-    def _train_single_full(self,
-                           X,
-                           y,
-                           model: AbstractModel,
-                           X_unlabeled=None,
-                           X_val=None,
-                           y_val=None,
-                           X_pseudo=None,
-                           y_pseudo=None,
-                           feature_prune=False,
-                           hyperparameter_tune_kwargs=None,
-                           stack_name='core',
-                           k_fold=None,
-                           k_fold_start=0,
-                           k_fold_end=None,
-                           n_repeats=None,
-                           n_repeat_start=0,
-                           level=1,
-                           time_limit=None,
-                           fit_kwargs=None,
-                           compute_score=True,
-                           total_resources=None,
-                           **kwargs) -> List[str]:
+    def _train_single_full(
+        self,
+        X,
+        y,
+        model: AbstractModel,
+        X_unlabeled=None,
+        X_val=None,
+        y_val=None,
+        X_pseudo=None,
+        y_pseudo=None,
+        feature_prune=False,
+        hyperparameter_tune_kwargs=None,
+        stack_name="core",
+        k_fold=None,
+        k_fold_start=0,
+        k_fold_end=None,
+        n_repeats=None,
+        n_repeat_start=0,
+        level=1,
+        time_limit=None,
+        fit_kwargs=None,
+        compute_score=True,
+        total_resources=None,
+        **kwargs,
+    ) -> List[str]:
         """
         Trains a model, with the potential to train multiple versions of this model with hyperparameter tuning and feature pruning.
         Returns a list of successfully trained and saved model names.
         Models trained from this method will be accessible in this Trainer.
         """
-        model_fit_kwargs = self._get_model_fit_kwargs(X=X, X_val=X_val, time_limit=time_limit, k_fold=k_fold, fit_kwargs=fit_kwargs,
-                                                      ens_sample_weight=kwargs.get('ens_sample_weight', None))
+        model_fit_kwargs = self._get_model_fit_kwargs(
+            X=X, X_val=X_val, time_limit=time_limit, k_fold=k_fold, fit_kwargs=fit_kwargs, ens_sample_weight=kwargs.get("ens_sample_weight", None)
+        )
         if hyperparameter_tune_kwargs:
             if n_repeat_start != 0:
-                raise ValueError(f'n_repeat_start must be 0 to hyperparameter_tune, value = {n_repeat_start}')
+                raise ValueError(f"n_repeat_start must be 0 to hyperparameter_tune, value = {n_repeat_start}")
             elif k_fold_start != 0:
-                raise ValueError(f'k_fold_start must be 0 to hyperparameter_tune, value = {k_fold_start}')
+                raise ValueError(f"k_fold_start must be 0 to hyperparameter_tune, value = {k_fold_start}")
             # hpo_models (dict): keys = model_names, values = model_paths
-            fit_log_message = f'Hyperparameter tuning model: {model.name} ...'
+            fit_log_message = f"Hyperparameter tuning model: {model.name} ..."
             if time_limit is not None:
                 if time_limit <= 0:
-                    logger.log(15, f'Skipping {model.name} due to lack of time remaining.')
+                    logger.log(15, f"Skipping {model.name} due to lack of time remaining.")
                     return []
                 fit_start_time = time.time()
                 if self._time_limit is not None and self._time_train_start is not None:
                     time_left_total = self._time_limit - (fit_start_time - self._time_train_start)
                 else:
                     time_left_total = time_limit
-                fit_log_message += f' Tuning model for up to {round(time_limit, 2)}s of the {round(time_left_total, 2)}s of remaining time.'
+                fit_log_message += f" Tuning model for up to {round(time_limit, 2)}s of the {round(time_left_total, 2)}s of remaining time."
             logger.log(20, fit_log_message)
             try:
                 if isinstance(model, BaggedEnsembleModel):
-                    bagged_model_fit_kwargs = self._get_bagged_model_fit_kwargs(k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold_end, n_repeats=n_repeats, n_repeat_start=n_repeat_start)
+                    bagged_model_fit_kwargs = self._get_bagged_model_fit_kwargs(
+                        k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold_end, n_repeats=n_repeats, n_repeat_start=n_repeat_start
+                    )
                     model_fit_kwargs.update(bagged_model_fit_kwargs)
                     hpo_models, hpo_results = model.hyperparameter_tune(
                         X=X,
                         y=y,
                         model=model,
                         X_val=X_val,
                         y_val=y_val,
                         X_unlabeled=X_unlabeled,
                         stack_name=stack_name,
                         level=level,
                         compute_score=compute_score,
                         hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
                         total_resources=total_resources,
-                        **model_fit_kwargs
+                        **model_fit_kwargs,
                     )
                 else:
                     hpo_models, hpo_results = model.hyperparameter_tune(
                         X=X,
                         y=y,
                         X_val=X_val,
                         y_val=y_val,
                         hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
                         total_resources=total_resources,
-                        **model_fit_kwargs
+                        **model_fit_kwargs,
                     )
                 if len(hpo_models) == 0:
-                    logger.warning(f'No model was trained during hyperparameter tuning {model.name}... Skipping this model.')
+                    logger.warning(f"No model was trained during hyperparameter tuning {model.name}... Skipping this model.")
             except Exception as err:
-                logger.exception(f'Warning: Exception caused {model.name} to fail during hyperparameter tuning... Skipping this model.')
+                logger.exception(f"Warning: Exception caused {model.name} to fail during hyperparameter tuning... Skipping this model.")
                 logger.warning(err)
                 del model
                 model_names_trained = []
             else:
                 # Commented out because it takes too much space (>>5 GB if run for an hour on a small-medium sized dataset)
                 # self.hpo_results[model.name] = hpo_results
                 model_names_trained = []
                 self._extra_banned_names.add(model.name)
                 for model_hpo_name, model_info in hpo_models.items():
-                    model_hpo = self.load_model(model_hpo_name, path=model_info['path'], model_type=type(model))
-                    logger.log(20, f'Fitted model: {model_hpo.name} ...')
+                    model_hpo = self.load_model(model_hpo_name, path=model_info["path"], model_type=type(model))
+                    logger.log(20, f"Fitted model: {model_hpo.name} ...")
                     if self._add_model(model=model_hpo, stack_name=stack_name, level=level):
                         model_names_trained.append(model_hpo.name)
         else:
-            model_fit_kwargs.update(dict(
-                X_pseudo=X_pseudo,
-                y_pseudo=y_pseudo
-            ))
+            model_fit_kwargs.update(dict(X_pseudo=X_pseudo, y_pseudo=y_pseudo))
             if isinstance(model, BaggedEnsembleModel):
-                bagged_model_fit_kwargs = self._get_bagged_model_fit_kwargs(k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold_end, n_repeats=n_repeats, n_repeat_start=n_repeat_start)
+                bagged_model_fit_kwargs = self._get_bagged_model_fit_kwargs(
+                    k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold_end, n_repeats=n_repeats, n_repeat_start=n_repeat_start
+                )
                 model_fit_kwargs.update(bagged_model_fit_kwargs)
             model_names_trained = self._train_and_save(
                 X=X,
                 y=y,
                 model=model,
                 X_val=X_val,
                 y_val=y_val,
                 X_unlabeled=X_unlabeled,
                 stack_name=stack_name,
                 level=level,
                 compute_score=compute_score,
                 total_resources=total_resources,
-                **model_fit_kwargs
+                **model_fit_kwargs,
             )
         self.save()
         return model_names_trained
 
     # TODO: How to deal with models that fail during this? They have trained valid models before, but should we still use those models or remove the entire model? Currently we still use models.
     # TODO: Time allowance can be made better by only using time taken during final model training and not during HPO and feature pruning.
     # TODO: Time allowance not accurate if running from fit_continue
@@ -1888,45 +2087,51 @@
                 break  # No models to repeat
             if time_limit is not None:
                 time_start_repeat = time.time()
                 time_left = time_limit - (time_start_repeat - time_start)
                 if n == n_repeat_start:
                     time_required = time_limit_total_level * 0.575  # Require slightly over 50% to be safe
                 else:
-                    time_required = (time_start_repeat - time_start) / repeats_completed * (0.575/0.425)
+                    time_required = (time_start_repeat - time_start) / repeats_completed * (0.575 / 0.425)
                 if time_left < time_required:
-                    logger.log(15, 'Not enough time left to finish repeated k-fold bagging, stopping early ...')
+                    logger.log(15, "Not enough time left to finish repeated k-fold bagging, stopping early ...")
                     break
-            logger.log(20, f'Repeating k-fold bagging: {n+1}/{n_repeats}')
+            logger.log(20, f"Repeating k-fold bagging: {n+1}/{n_repeats}")
             for i, model in enumerate(models_valid):
-                if not self.get_model_attribute(model=model, attribute='can_fit'):
+                if not self.get_model_attribute(model=model, attribute="can_fit"):
                     if isinstance(model, str):
                         models_valid_next.append(model)
                     else:
                         models_valid_next.append(model.name)
                     continue
 
                 if isinstance(model, str):
                     model = self.load_model(model)
                 if not isinstance(model, BaggedEnsembleModel):
-                    raise AssertionError(f'{model.name} must inherit from BaggedEnsembleModel to perform repeated k-fold bagging. Model type: {type(model).__name__}')
+                    raise AssertionError(
+                        f"{model.name} must inherit from BaggedEnsembleModel to perform repeated k-fold bagging. Model type: {type(model).__name__}"
+                    )
                 if time_limit is None:
                     time_left = None
                 else:
                     time_start_model = time.time()
                     time_left = time_limit - (time_start_model - time_start)
 
-                models_valid_next += self._train_single_full(X=X, y=y, model=model, k_fold_start=0, k_fold_end=None, n_repeats=n + 1, n_repeat_start=n, time_limit=time_left, **kwargs)
+                models_valid_next += self._train_single_full(
+                    X=X, y=y, model=model, k_fold_start=0, k_fold_end=None, n_repeats=n + 1, n_repeat_start=n, time_limit=time_left, **kwargs
+                )
             models_valid = copy.deepcopy(models_valid_next)
             models_valid_next = []
             repeats_completed += 1
-        logger.log(20, f'Completed {n_repeat_start + repeats_completed}/{n_repeats} k-fold bagging repeats ...')
+        logger.log(20, f"Completed {n_repeat_start + repeats_completed}/{n_repeats} k-fold bagging repeats ...")
         return models_valid
 
-    def _train_multi_initial(self, X, y, models: List[AbstractModel], k_fold, n_repeats, hyperparameter_tune_kwargs=None, time_limit=None, feature_prune_kwargs=None, **kwargs):
+    def _train_multi_initial(
+        self, X, y, models: List[AbstractModel], k_fold, n_repeats, hyperparameter_tune_kwargs=None, time_limit=None, feature_prune_kwargs=None, **kwargs
+    ):
         """
         Fits models that have not previously been fit.
         This method should only be called in self._train_multi
         Returns a list of successfully trained and saved model names.
         """
         multi_fold_time_start = time.time()
         fit_args = dict(
@@ -1948,62 +2153,101 @@
             time_split = True
         else:
             time_split = False
         k_fold_start = 0
         bagged = k_fold > 0
         if not bagged:
             time_ratio = hpo_time_ratio if hpo_enabled else 1
-            models = self._train_multi_fold(models=models, hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
-                                            time_limit=time_limit, time_split=time_split, time_ratio=time_ratio, **fit_args)
+            models = self._train_multi_fold(
+                models=models,
+                hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
+                time_limit=time_limit,
+                time_split=time_split,
+                time_ratio=time_ratio,
+                **fit_args,
+            )
         else:
             time_ratio = hpo_time_ratio if hpo_enabled else 1
-            models = self._train_multi_fold(models=models, hyperparameter_tune_kwargs=hyperparameter_tune_kwargs, k_fold_start=0,
-                                            k_fold_end=k_fold, n_repeats=n_repeats, n_repeat_start=0, time_limit=time_limit,
-                                            time_split=time_split, time_ratio=time_ratio, **fit_args)
+            models = self._train_multi_fold(
+                models=models,
+                hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
+                k_fold_start=0,
+                k_fold_end=k_fold,
+                n_repeats=n_repeats,
+                n_repeat_start=0,
+                time_limit=time_limit,
+                time_split=time_split,
+                time_ratio=time_ratio,
+                **fit_args,
+            )
 
         multi_fold_time_elapsed = time.time() - multi_fold_time_start
         if time_limit is not None:
             time_limit = time_limit - multi_fold_time_elapsed
 
         if feature_prune_kwargs is not None and len(models) > 0:
             feature_prune_time_start = time.time()
-            model_fit_kwargs = self._get_model_fit_kwargs(X=X, X_val=kwargs.get('X_val', None), time_limit=None, k_fold=k_fold,
-                                                          fit_kwargs=kwargs.get('fit_kwargs', {}), ens_sample_weight=kwargs.get('ens_sample_weight'))
-            model_fit_kwargs.update(dict(X=X, y=y, X_val=kwargs.get('X_val', None), y_val=kwargs.get('y_val', None)))
+            model_fit_kwargs = self._get_model_fit_kwargs(
+                X=X,
+                X_val=kwargs.get("X_val", None),
+                time_limit=None,
+                k_fold=k_fold,
+                fit_kwargs=kwargs.get("fit_kwargs", {}),
+                ens_sample_weight=kwargs.get("ens_sample_weight"),
+            )
+            model_fit_kwargs.update(dict(X=X, y=y, X_val=kwargs.get("X_val", None), y_val=kwargs.get("y_val", None)))
             if bagged:
-                bagged_model_fit_kwargs = self._get_bagged_model_fit_kwargs(k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold, n_repeats=n_repeats, n_repeat_start=0)
+                bagged_model_fit_kwargs = self._get_bagged_model_fit_kwargs(
+                    k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold, n_repeats=n_repeats, n_repeat_start=0
+                )
                 model_fit_kwargs.update(bagged_model_fit_kwargs)
 
-            candidate_features = self._proxy_model_feature_prune(time_limit=time_limit, layer_fit_time=multi_fold_time_elapsed, level=kwargs['level'],
-                                                                 features=X.columns.tolist(), model_fit_kwargs=model_fit_kwargs, **feature_prune_kwargs)
+            candidate_features = self._proxy_model_feature_prune(
+                time_limit=time_limit,
+                layer_fit_time=multi_fold_time_elapsed,
+                level=kwargs["level"],
+                features=X.columns.tolist(),
+                model_fit_kwargs=model_fit_kwargs,
+                **feature_prune_kwargs,
+            )
             if time_limit is not None:
                 time_limit = time_limit - (time.time() - feature_prune_time_start)
 
-            fit_args['X'] = X[candidate_features]
-            fit_args['X_val'] = kwargs['X_val'][candidate_features] if isinstance(kwargs.get('X_val', None), pd.DataFrame) else kwargs.get('X_val', None)
+            fit_args["X"] = X[candidate_features]
+            fit_args["X_val"] = kwargs["X_val"][candidate_features] if isinstance(kwargs.get("X_val", None), pd.DataFrame) else kwargs.get("X_val", None)
 
             if len(candidate_features) < len(X.columns):
                 unfit_models = []
                 original_prune_map = {}
                 for model in models:
                     unfit_model = self.load_model(model).convert_to_template()
                     unfit_model.rename(f"{unfit_model.name}_Prune")
                     unfit_models.append(unfit_model)
                     original_prune_map[unfit_model.name] = model
-                pruned_models = self._train_multi_fold(models=unfit_models, hyperparameter_tune_kwargs=None, k_fold_start=k_fold_start,
-                                                       k_fold_end=k_fold, n_repeats=n_repeats, n_repeat_start=0, time_limit=time_limit, **fit_args)
-                force_prune = feature_prune_kwargs.get('force_prune', False)
+                pruned_models = self._train_multi_fold(
+                    models=unfit_models,
+                    hyperparameter_tune_kwargs=None,
+                    k_fold_start=k_fold_start,
+                    k_fold_end=k_fold,
+                    n_repeats=n_repeats,
+                    n_repeat_start=0,
+                    time_limit=time_limit,
+                    **fit_args,
+                )
+                force_prune = feature_prune_kwargs.get("force_prune", False)
                 models = self._retain_better_pruned_models(pruned_models=pruned_models, original_prune_map=original_prune_map, force_prune=force_prune)
         return models
 
     # TODO: Ban KNN from being a Stacker model outside of aux. Will need to ensemble select on all stack layers ensemble selector to make it work
     # TODO: Robert dataset, LightGBM is super good but RF and KNN take all the time away from it on 1h despite being much worse
     # TODO: Add time_limit_per_model
     # TODO: Rename for v0.1
-    def _train_multi_fold(self, X, y, models: List[AbstractModel], time_limit=None, time_split=False, time_ratio=1, hyperparameter_tune_kwargs=None, **kwargs) -> List[str]:
+    def _train_multi_fold(
+        self, X, y, models: List[AbstractModel], time_limit=None, time_split=False, time_ratio=1, hyperparameter_tune_kwargs=None, **kwargs
+    ) -> List[str]:
         """
         Trains and saves a list of models sequentially.
         This method should only be called in self._train_multi_initial
         Returns a list of trained model names.
         """
         models_valid = []
         time_start = time.time()
@@ -2027,87 +2271,133 @@
                 time_left = time_limit_model_split
             else:
                 if time_limit is None:
                     time_left = None
                 else:
                     time_start_model = time.time()
                     time_left = time_limit - (time_start_model - time_start)
-            model_name_trained_lst = self._train_single_full(X, y, model, time_limit=time_left, hyperparameter_tune_kwargs=hyperparameter_tune_kwargs_model, **kwargs)
+            model_name_trained_lst = self._train_single_full(
+                X, y, model, time_limit=time_left, hyperparameter_tune_kwargs=hyperparameter_tune_kwargs_model, **kwargs
+            )
 
             if self.low_memory:
                 del model
             models_valid += model_name_trained_lst
 
         return models_valid
 
-    def _train_multi(self, X, y, models: List[AbstractModel], hyperparameter_tune_kwargs=None, feature_prune_kwargs=None, k_fold=None, n_repeats=None, n_repeat_start=0, time_limit=None, **kwargs) -> List[str]:
+    def _train_multi(
+        self,
+        X,
+        y,
+        models: List[AbstractModel],
+        hyperparameter_tune_kwargs=None,
+        feature_prune_kwargs=None,
+        k_fold=None,
+        n_repeats=None,
+        n_repeat_start=0,
+        time_limit=None,
+        **kwargs,
+    ) -> List[str]:
         """
         Train a list of models using the same data.
         Assumes that input data has already been processed in the form the models will receive as input (including stack feature generation).
         Trained models are available in the trainer object.
         Note: Consider using public APIs instead of this.
         Returns a list of trained model names.
         """
         time_limit_total_level = time_limit
         if k_fold is None:
             k_fold = self.k_fold
         if n_repeats is None:
             n_repeats = self.n_repeats
         if (k_fold == 0) and (n_repeats != 1):
-            raise ValueError(f'n_repeats must be 1 when k_fold is 0, values: ({n_repeats}, {k_fold})')
+            raise ValueError(f"n_repeats must be 1 when k_fold is 0, values: ({n_repeats}, {k_fold})")
         if time_limit is None and feature_prune_kwargs is None:
             n_repeats_initial = n_repeats
         else:
             n_repeats_initial = 1
         if n_repeat_start == 0:
             time_start = time.time()
-            model_names_trained = self._train_multi_initial(X=X, y=y, models=models, k_fold=k_fold, n_repeats=n_repeats_initial, hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
-                                                            feature_prune_kwargs=feature_prune_kwargs, time_limit=time_limit, **kwargs)
+            model_names_trained = self._train_multi_initial(
+                X=X,
+                y=y,
+                models=models,
+                k_fold=k_fold,
+                n_repeats=n_repeats_initial,
+                hyperparameter_tune_kwargs=hyperparameter_tune_kwargs,
+                feature_prune_kwargs=feature_prune_kwargs,
+                time_limit=time_limit,
+                **kwargs,
+            )
             n_repeat_start = n_repeats_initial
             if time_limit is not None:
                 time_limit = time_limit - (time.time() - time_start)
         else:
             model_names_trained = models
         if (n_repeats > 1) and (n_repeat_start < n_repeats):
-            model_names_trained = self._train_multi_repeats(X=X, y=y, models=model_names_trained,
-                                                            k_fold=k_fold, n_repeats=n_repeats, n_repeat_start=n_repeat_start, time_limit=time_limit, time_limit_total_level=time_limit_total_level, **kwargs)
+            model_names_trained = self._train_multi_repeats(
+                X=X,
+                y=y,
+                models=model_names_trained,
+                k_fold=k_fold,
+                n_repeats=n_repeats,
+                n_repeat_start=n_repeat_start,
+                time_limit=time_limit,
+                time_limit_total_level=time_limit_total_level,
+                **kwargs,
+            )
         return model_names_trained
 
-    def _train_multi_and_ensemble(self, X, y, X_val, y_val, hyperparameters: dict = None, X_unlabeled=None, num_stack_levels=0, time_limit=None, groups=None, **kwargs) -> List[str]:
+    def _train_multi_and_ensemble(
+        self, X, y, X_val, y_val, hyperparameters: dict = None, X_unlabeled=None, num_stack_levels=0, time_limit=None, groups=None, **kwargs
+    ) -> List[str]:
         """Identical to self.train_multi_levels, but also saves the data to disk. This should only ever be called once."""
         if time_limit is not None and time_limit <= 0:
-            raise AssertionError(f'Not enough time left to train models. Consider specifying a larger time_limit. Time remaining: {round(time_limit, 2)}s')
+            raise AssertionError(f"Not enough time left to train models. Consider specifying a larger time_limit. Time remaining: {round(time_limit, 2)}s")
         if self.save_data and not self.is_data_saved:
             self.save_X(X)
             self.save_y(y)
             if X_val is not None:
                 self.save_X_val(X_val)
                 if y_val is not None:
                     self.save_y_val(y_val)
             self.is_data_saved = True
         if self._groups is None:
             self._groups = groups
         self._num_rows_train = len(X)
         if X_val is not None:
             self._num_rows_val = len(X_val)
         self._num_cols_train = len(list(X.columns))
-        model_names_fit = self.train_multi_levels(X, y, hyperparameters=hyperparameters, X_val=X_val, y_val=y_val,
-                                                  X_unlabeled=X_unlabeled, level_start=1, level_end=num_stack_levels+1, time_limit=time_limit, **kwargs)
+        model_names_fit = self.train_multi_levels(
+            X,
+            y,
+            hyperparameters=hyperparameters,
+            X_val=X_val,
+            y_val=y_val,
+            X_unlabeled=X_unlabeled,
+            level_start=1,
+            level_end=num_stack_levels + 1,
+            time_limit=time_limit,
+            **kwargs,
+        )
         if len(self.get_model_names()) == 0:
-            raise ValueError('AutoGluon did not successfully train any models')
+            raise ValueError("AutoGluon did not successfully train any models")
         return model_names_fit
 
     def _predict_model(self, X, model, model_pred_proba_dict=None, cascade=False):
         y_pred_proba = self._predict_proba_model(X=X, model=model, model_pred_proba_dict=model_pred_proba_dict, cascade=cascade)
         return get_pred_from_proba(y_pred_proba=y_pred_proba, problem_type=self.problem_type)
 
     def _predict_proba_model(self, X, model, model_pred_proba_dict=None, cascade=False):
         return self.get_pred_proba_from_model(model=model, X=X, model_pred_proba_dict=model_pred_proba_dict, cascade=cascade)
 
-    def _proxy_model_feature_prune(self, model_fit_kwargs: dict, time_limit: float, layer_fit_time: float, level: int, features: List[str], **feature_prune_kwargs: dict) -> List[str]:
+    def _proxy_model_feature_prune(
+        self, model_fit_kwargs: dict, time_limit: float, layer_fit_time: float, level: int, features: List[str], **feature_prune_kwargs: dict
+    ) -> List[str]:
         """
         Uses the best LightGBM-based base learner of this layer to perform time-aware permutation feature importance based feature pruning.
         If all LightGBM models fail, use the model that achieved the highest validation accuracy. Feature pruning gets the smaller of the
         remaining layer time limit and k times (default=2) it took to fit the base learners of this layer as its resource. Note that feature pruning can
         exit earlier based on arguments in feature_prune_kwargs. The method returns the list of feature names that survived the pruning procedure.
 
         Parameters
@@ -2128,36 +2418,39 @@
             The list of feature names in the inputted dataset.
 
         Returns
         -------
         candidate_features : List[str]
             Feature names that survived the pruning procedure.
         """
-        k = feature_prune_kwargs.pop('k', 2)
-        proxy_model_class = feature_prune_kwargs.pop('proxy_model_class', self._get_default_proxy_model_class())
-        feature_prune_time_limit = feature_prune_kwargs.pop('feature_prune_time_limit', None)
-        raise_exception_on_fail = feature_prune_kwargs.pop('raise_exception', False)
+        k = feature_prune_kwargs.pop("k", 2)
+        proxy_model_class = feature_prune_kwargs.pop("proxy_model_class", self._get_default_proxy_model_class())
+        feature_prune_time_limit = feature_prune_kwargs.pop("feature_prune_time_limit", None)
+        raise_exception_on_fail = feature_prune_kwargs.pop("raise_exception", False)
 
         proxy_model = self._get_feature_prune_proxy_model(proxy_model_class=proxy_model_class, level=level)
         if proxy_model is None:
             return features
 
         if feature_prune_time_limit is not None:
             feature_prune_time_limit = min(max(time_limit - layer_fit_time, 0), feature_prune_time_limit)
         elif time_limit is not None:
             feature_prune_time_limit = min(max(time_limit - layer_fit_time, 0), max(k * layer_fit_time, 0.05 * time_limit))
         else:
             feature_prune_time_limit = max(k * layer_fit_time, 300)
 
         if feature_prune_time_limit < 2 * proxy_model.fit_time:
-            logger.warning(f"Insufficient time to train even a single feature pruning model (remaining: {feature_prune_time_limit}, "
-                           f"needed: {proxy_model.fit_time}). Skipping feature pruning.")
+            logger.warning(
+                f"Insufficient time to train even a single feature pruning model (remaining: {feature_prune_time_limit}, "
+                f"needed: {proxy_model.fit_time}). Skipping feature pruning."
+            )
             return features
-        selector = FeatureSelector(model=proxy_model, time_limit=feature_prune_time_limit,
-                                   raise_exception=raise_exception_on_fail, problem_type=self.problem_type)
+        selector = FeatureSelector(
+            model=proxy_model, time_limit=feature_prune_time_limit, raise_exception=raise_exception_on_fail, problem_type=self.problem_type
+        )
         candidate_features = selector.select_features(**feature_prune_kwargs, **model_fit_kwargs)
         return candidate_features
 
     def _get_default_proxy_model_class(self):
         return None
 
     def _retain_better_pruned_models(self, pruned_models: List[str], original_prune_map: dict, force_prune: bool = False) -> List[str]:
@@ -2179,16 +2472,16 @@
         models : List[str]
             A list of model names.
         """
         models = []
         for pruned_model in pruned_models:
             original_model = original_prune_map[pruned_model]
             leaderboard = self.leaderboard()
-            original_score = leaderboard[leaderboard['model'] == original_model]['score_val'].item()
-            pruned_score = leaderboard[leaderboard['model'] == pruned_model]['score_val'].item()
+            original_score = leaderboard[leaderboard["model"] == original_model]["score_val"].item()
+            pruned_score = leaderboard[leaderboard["model"] == pruned_model]["score_val"].item()
             score_str = f"({round(pruned_score, 4)} vs {round(original_score, 4)})"
             if force_prune:
                 logger.log(30, f"Pruned score vs original score is {score_str}. Replacing original model since force_prune=True...")
                 self.delete_models(models_to_delete=original_model, dry_run=False)
                 models.append(pruned_model)
             elif pruned_score > original_score:
                 logger.log(30, f"Model trained with feature pruning score is better than original model's score {score_str}. Replacing original model...")
@@ -2204,32 +2497,38 @@
     #  This is non-trivial to implement for multi-layer stacking ensembles on the OOF data.
     # TODO: Consider limiting X to 10k rows here instead of inside the model call
     def get_feature_importance(self, model=None, X=None, y=None, raw=True, **kwargs) -> pd.DataFrame:
         if model is None:
             model = self.model_best
         model: AbstractModel = self.load_model(model)
         if X is None and model.val_score is None:
-            raise AssertionError(f'Model {model.name} is not valid for generating feature importances on original training data because no validation data was used during training, please specify new test data to compute feature importances.')
+            raise AssertionError(
+                f"Model {model.name} is not valid for generating feature importances on original training data because no validation data was used during training, please specify new test data to compute feature importances."
+            )
 
         if X is None:
             if isinstance(model, WeightedEnsembleModel):
                 if self.bagged_mode:
                     if raw:
-                        raise AssertionError('`feature_stage=\'transformed\'` feature importance on the original training data is not yet supported when bagging is enabled, please specify new test data to compute feature importances.')
+                        raise AssertionError(
+                            "`feature_stage='transformed'` feature importance on the original training data is not yet supported when bagging is enabled, please specify new test data to compute feature importances."
+                        )
                     X = None
                     is_oof = True
                 else:
                     if raw:
                         X = self.load_X_val()
                     else:
                         X = None
                     is_oof = False
             elif isinstance(model, BaggedEnsembleModel):
                 if raw:
-                    raise AssertionError('`feature_stage=\'transformed\'` feature importance on the original training data is not yet supported when bagging is enabled, please specify new test data to compute feature importances.')
+                    raise AssertionError(
+                        "`feature_stage='transformed'` feature importance on the original training data is not yet supported when bagging is enabled, please specify new test data to compute feature importances."
+                    )
                 X = self.load_X()
                 X = self.get_inputs_to_model(model=model, X=X, fit=True)
                 is_oof = True
             else:
                 X = self.load_X_val()
                 if not raw:
                     X = self.get_inputs_to_model(model=model, X=X, fit=False)
@@ -2245,15 +2544,15 @@
             else:
                 y = self.load_y_val()
 
         if raw:
             return self._get_feature_importance_raw(X=X, y=y, model=model, **kwargs)
         else:
             if is_oof:
-                kwargs['is_oof'] = is_oof
+                kwargs["is_oof"] = is_oof
             return model.compute_feature_importance(X=X, y=y, **kwargs)
 
     # TODO: Can get feature importances of all children of model at no extra cost, requires scoring the values after predict_proba on each model
     #  Could solve by adding a self.score_all() function which takes model as input and also returns scores of all children models.
     #  This would be best solved after adding graph representation, it lives most naturally in AbstractModel
     # TODO: Can skip features which were pruned on all models that model depends on (Complex to implement, requires graph representation)
     # TODO: Note that raw importance will not equal non-raw importance for bagged models, even if raw features are identical to the model features.
@@ -2269,21 +2568,27 @@
         if eval_metric.needs_pred:
             predict_func = self.predict
         else:
             predict_func = self.predict_proba
         model: AbstractModel = self.load_model(model)
         predict_func_kwargs = dict(model=model)
         return compute_permutation_feature_importance(
-            X=X, y=y, predict_func=predict_func, predict_func_kwargs=predict_func_kwargs, eval_metric=eval_metric, quantile_levels=self.quantile_levels, **kwargs
+            X=X,
+            y=y,
+            predict_func=predict_func,
+            predict_func_kwargs=predict_func_kwargs,
+            eval_metric=eval_metric,
+            quantile_levels=self.quantile_levels,
+            **kwargs,
         )
 
     def _get_models_load_info(self, model_names):
         model_names = copy.deepcopy(model_names)
-        model_paths = self.get_models_attribute_dict(attribute='path', models=model_names)
-        model_types = self.get_models_attribute_dict(attribute='type', models=model_names)
+        model_paths = self.get_models_attribute_dict(attribute="path", models=model_names)
+        model_types = self.get_models_attribute_dict(attribute="type", models=model_names)
         return model_names, model_paths, model_types
 
     # Sums the attribute value across all models that the provided model depends on, including itself.
     # For instance, this function can return the expected total predict_time of a model.
     # attribute is the name of the desired attribute to be summed, or a dictionary of model name -> attribute value if the attribute is not present in the graph.
     def get_model_attribute_full(self, model: Union[str, List[str]], attribute: str, func=sum):
         if isinstance(model, list):
@@ -2342,20 +2647,20 @@
         Return model attribute value.
         If `default` is specified, return default value if attribute does not exist.
         If `default` is not specified, raise ValueError if attribute does not exist.
         """
         if not isinstance(model, str):
             model = model.name
         if model not in self.model_graph.nodes:
-            raise ValueError(f'Model does not exist: (model={model})')
+            raise ValueError(f"Model does not exist: (model={model})")
         if attribute not in self.model_graph.nodes[model]:
-            if 'default' in kwargs:
-                return kwargs['default']
+            if "default" in kwargs:
+                return kwargs["default"]
             else:
-                raise ValueError(f'Model does not contain attribute: (model={model}, attribute={attribute})')
+                raise ValueError(f"Model does not contain attribute: (model={model}, attribute={attribute})")
         return self.model_graph.nodes[model][attribute]
 
     def set_model_attribute(self, model, attribute: str, val):
         if not isinstance(model, str):
             model = model.name
         self.model_graph.nodes[model][attribute] = val
 
@@ -2387,15 +2692,15 @@
 
     def get_model_full_dict(self, inverse=False) -> Dict[str, str]:
         """
         Returns dict of parent model -> refit model
 
         If inverse=True, return dict of refit model -> parent model
         """
-        model_full_dict = self.get_models_attribute_dict(attribute='refit_full_parent')
+        model_full_dict = self.get_models_attribute_dict(attribute="refit_full_parent")
         if not inverse:
             model_full_dict = {parent: refit for refit, parent in model_full_dict.items()}
         return model_full_dict
 
     def model_exists(self, model: str) -> bool:
         return model in self.get_model_names()
 
@@ -2408,21 +2713,21 @@
         score_val = []
         fit_time_marginal = []
         pred_time_val_marginal = []
         stack_level = []
         fit_time = []
         pred_time_val = []
         can_infer = []
-        fit_order = list(range(1, len(model_names)+1))
-        score_val_dict = self.get_models_attribute_dict('val_score')
-        fit_time_marginal_dict = self.get_models_attribute_dict('fit_time')
-        predict_time_marginal_dict = self.get_models_attribute_dict('predict_time')
-        fit_time_dict = self.get_models_attribute_full(attribute='fit_time', models=model_names, func=sum)
-        pred_time_val_dict = self.get_models_attribute_full(attribute='predict_time', models=model_names, func=sum)
-        can_infer_dict = self.get_models_attribute_full(attribute='can_infer', models=model_names, func=min)
+        fit_order = list(range(1, len(model_names) + 1))
+        score_val_dict = self.get_models_attribute_dict("val_score")
+        fit_time_marginal_dict = self.get_models_attribute_dict("fit_time")
+        predict_time_marginal_dict = self.get_models_attribute_dict("predict_time")
+        fit_time_dict = self.get_models_attribute_full(attribute="fit_time", models=model_names, func=sum)
+        pred_time_val_dict = self.get_models_attribute_full(attribute="predict_time", models=model_names, func=sum)
+        can_infer_dict = self.get_models_attribute_full(attribute="can_infer", models=model_names, func=min)
         for model_name in model_names:
             score_val.append(score_val_dict[model_name])
             fit_time_marginal.append(fit_time_marginal_dict[model_name])
             fit_time.append(fit_time_dict[model_name])
             pred_time_val_marginal.append(predict_time_marginal_dict[model_name])
             pred_time_val.append(pred_time_val_dict[model_name])
             stack_level.append(self.get_model_level(model_name))
@@ -2434,90 +2739,107 @@
             # TODO: disk size
             # TODO: load time
             # TODO: Add persist_if_mem_safe() function to persist in memory all models if reasonable memory size (or a specific model+ancestors)
             # TODO: Add is_persisted() function to check which models are persisted in memory
             # TODO: package_dependencies, package_dependencies_full
 
             info = self.get_info(include_model_info=True)
-            model_info = info['model_info']
+            model_info = info["model_info"]
             custom_model_info = {}
             for model_name in model_info:
                 custom_info = {}
-                bagged_info = model_info[model_name].get('bagged_info', {})
-                custom_info['num_models'] = bagged_info.get('num_child_models', 1)
-                custom_info['memory_size'] = bagged_info.get('max_memory_size', model_info[model_name]['memory_size'])
-                custom_info['memory_size_min'] = bagged_info.get('min_memory_size', model_info[model_name]['memory_size'])
-                custom_info['compile_time'] = bagged_info.get('compile_time', model_info[model_name]['compile_time'])
-                custom_info['child_model_type'] = bagged_info.get('child_model_type', None)
-                custom_info['child_hyperparameters'] = bagged_info.get('child_hyperparameters', None)
-                custom_info['child_hyperparameters_fit'] = bagged_info.get('child_hyperparameters_fit', None)
-                custom_info['child_ag_args_fit'] = bagged_info.get('child_ag_args_fit', None)
+                bagged_info = model_info[model_name].get("bagged_info", {})
+                custom_info["num_models"] = bagged_info.get("num_child_models", 1)
+                custom_info["memory_size"] = bagged_info.get("max_memory_size", model_info[model_name]["memory_size"])
+                custom_info["memory_size_min"] = bagged_info.get("min_memory_size", model_info[model_name]["memory_size"])
+                custom_info["compile_time"] = bagged_info.get("compile_time", model_info[model_name]["compile_time"])
+                custom_info["child_model_type"] = bagged_info.get("child_model_type", None)
+                custom_info["child_hyperparameters"] = bagged_info.get("child_hyperparameters", None)
+                custom_info["child_hyperparameters_fit"] = bagged_info.get("child_hyperparameters_fit", None)
+                custom_info["child_ag_args_fit"] = bagged_info.get("child_ag_args_fit", None)
                 custom_model_info[model_name] = custom_info
 
-            model_info_keys = ['num_features', 'model_type', 'hyperparameters', 'hyperparameters_fit', 'ag_args_fit', 'features']
+            model_info_keys = ["num_features", "model_type", "hyperparameters", "hyperparameters_fit", "ag_args_fit", "features"]
             model_info_sum_keys = []
             for key in model_info_keys:
                 model_info_dict[key] = [model_info[model_name][key] for model_name in model_names]
                 if key in model_info_sum_keys:
                     key_dict = {model_name: model_info[model_name][key] for model_name in model_names}
-                    model_info_dict[key + '_full'] = [self.get_model_attribute_full(model=model_name, attribute=key_dict) for model_name in model_names]
+                    model_info_dict[key + "_full"] = [self.get_model_attribute_full(model=model_name, attribute=key_dict) for model_name in model_names]
 
-            model_info_keys = ['num_models', 'memory_size', 'memory_size_min', 'compile_time', 'child_model_type', 'child_hyperparameters', 'child_hyperparameters_fit', 'child_ag_args_fit']
-            model_info_full_keys = {'memory_size': [('memory_size_w_ancestors', sum)], 'memory_size_min': [('memory_size_min_w_ancestors', max)], 'num_models': [('num_models_w_ancestors', sum)]}
+            model_info_keys = [
+                "num_models",
+                "memory_size",
+                "memory_size_min",
+                "compile_time",
+                "child_model_type",
+                "child_hyperparameters",
+                "child_hyperparameters_fit",
+                "child_ag_args_fit",
+            ]
+            model_info_full_keys = {
+                "memory_size": [("memory_size_w_ancestors", sum)],
+                "memory_size_min": [("memory_size_min_w_ancestors", max)],
+                "num_models": [("num_models_w_ancestors", sum)],
+            }
             for key in model_info_keys:
                 model_info_dict[key] = [custom_model_info[model_name][key] for model_name in model_names]
                 if key in model_info_full_keys:
                     key_dict = {model_name: custom_model_info[model_name][key] for model_name in model_names}
                     for column_name, func in model_info_full_keys[key]:
-                        model_info_dict[column_name] = [self.get_model_attribute_full(model=model_name, attribute=key_dict, func=func) for model_name in model_names]
+                        model_info_dict[column_name] = [
+                            self.get_model_attribute_full(model=model_name, attribute=key_dict, func=func) for model_name in model_names
+                        ]
 
             ancestors = [list(nx.dag.ancestors(self.model_graph, model_name)) for model_name in model_names]
             descendants = [list(nx.dag.descendants(self.model_graph, model_name)) for model_name in model_names]
 
-            model_info_dict['num_ancestors'] = [len(ancestor_lst) for ancestor_lst in ancestors]
-            model_info_dict['num_descendants'] = [len(descendant_lst) for descendant_lst in descendants]
-            model_info_dict['ancestors'] = ancestors
-            model_info_dict['descendants'] = descendants
-
-        df = pd.DataFrame(data={
-            'model': model_names,
-            'score_val': score_val,
-            'pred_time_val': pred_time_val,
-            'fit_time': fit_time,
-            'pred_time_val_marginal': pred_time_val_marginal,
-            'fit_time_marginal': fit_time_marginal,
-            'stack_level': stack_level,
-            'can_infer': can_infer,
-            'fit_order': fit_order,
-            **model_info_dict,
-        })
-        df_sorted = df.sort_values(by=['score_val', 'pred_time_val', 'model'], ascending=[False, True, False]).reset_index(drop=True)
+            model_info_dict["num_ancestors"] = [len(ancestor_lst) for ancestor_lst in ancestors]
+            model_info_dict["num_descendants"] = [len(descendant_lst) for descendant_lst in descendants]
+            model_info_dict["ancestors"] = ancestors
+            model_info_dict["descendants"] = descendants
+
+        df = pd.DataFrame(
+            data={
+                "model": model_names,
+                "score_val": score_val,
+                "pred_time_val": pred_time_val,
+                "fit_time": fit_time,
+                "pred_time_val_marginal": pred_time_val_marginal,
+                "fit_time_marginal": fit_time_marginal,
+                "stack_level": stack_level,
+                "can_infer": can_infer,
+                "fit_order": fit_order,
+                **model_info_dict,
+            }
+        )
+        df_sorted = df.sort_values(by=["score_val", "pred_time_val", "model"], ascending=[False, True, False]).reset_index(drop=True)
 
         df_columns_lst = df_sorted.columns.tolist()
         explicit_order = [
-            'model',
-            'score_val',
-            'pred_time_val',
-            'fit_time',
-            'pred_time_val_marginal',
-            'fit_time_marginal',
-            'stack_level',
-            'can_infer',
-            'fit_order',
-            'num_features',
-            'num_models',
-            'num_models_w_ancestors',
-            'memory_size',
-            'memory_size_w_ancestors',
-            'memory_size_min',
-            'memory_size_min_w_ancestors',
-            'num_ancestors',
-            'num_descendants',
-            'model_type',
-            'child_model_type'
+            "model",
+            "score_val",
+            "pred_time_val",
+            "fit_time",
+            "pred_time_val_marginal",
+            "fit_time_marginal",
+            "stack_level",
+            "can_infer",
+            "fit_order",
+            "num_features",
+            "num_models",
+            "num_models_w_ancestors",
+            "memory_size",
+            "memory_size_w_ancestors",
+            "memory_size_min",
+            "memory_size_min_w_ancestors",
+            "num_ancestors",
+            "num_descendants",
+            "model_type",
+            "child_model_type",
         ]
         explicit_order = [column for column in explicit_order if column in df_columns_lst]
         df_columns_other = [column for column in df_columns_lst if column not in explicit_order]
         df_columns_new = explicit_order + df_columns_other
         df_sorted = df_sorted[df_columns_new]
 
         return df_sorted
@@ -2528,22 +2850,22 @@
             best_model = self.model_best
         else:
             try:
                 best_model = self.get_model_best()
             except AssertionError:
                 best_model = None
         if best_model is not None:
-            best_model_score_val = self.get_model_attribute(model=best_model, attribute='val_score')
+            best_model_score_val = self.get_model_attribute(model=best_model, attribute="val_score")
             best_model_stack_level = self.get_model_level(best_model)
         else:
             best_model_score_val = None
             best_model_stack_level = None
         # fit_time = None
         num_bag_folds = self.k_fold
-        max_core_stack_level = self.get_max_level('core')
+        max_core_stack_level = self.get_max_level("core")
         max_stack_level = self.get_max_level()
 
         problem_type = self.problem_type
         eval_metric = self.eval_metric.name
         time_train_start = self._time_train_start
         num_rows_train = self._num_rows_train
         num_cols_train = self._num_cols_train
@@ -2558,58 +2880,60 @@
         #  Exception count / models failed count
         #  True model count (models * kfold)
         #  AutoGluon version fit on
         #  Max memory usage
         #  CPU count used / GPU count used
 
         info = {
-            'time_train_start': time_train_start,
-            'num_rows_train': num_rows_train,
-            'num_cols_train': num_cols_train,
-            'num_rows_val': num_rows_val,
-            'num_classes': num_classes,
-            'problem_type': problem_type,
-            'eval_metric': eval_metric,
-            'best_model': best_model,
-            'best_model_score_val': best_model_score_val,
-            'best_model_stack_level': best_model_stack_level,
-            'num_models_trained': num_models_trained,
-            'num_bag_folds': num_bag_folds,
-            'max_stack_level': max_stack_level,
-            'max_core_stack_level': max_core_stack_level,
+            "time_train_start": time_train_start,
+            "num_rows_train": num_rows_train,
+            "num_cols_train": num_cols_train,
+            "num_rows_val": num_rows_val,
+            "num_classes": num_classes,
+            "problem_type": problem_type,
+            "eval_metric": eval_metric,
+            "best_model": best_model,
+            "best_model_score_val": best_model_score_val,
+            "best_model_stack_level": best_model_stack_level,
+            "num_models_trained": num_models_trained,
+            "num_bag_folds": num_bag_folds,
+            "max_stack_level": max_stack_level,
+            "max_core_stack_level": max_core_stack_level,
         }
 
         if include_model_info:
-            info['model_info'] = self.get_models_info()
+            info["model_info"] = self.get_models_info()
 
         return info
 
     def get_models_info(self, models: List[str] = None) -> dict:
         if models is None:
             models = self.get_model_names()
         model_info_dict = dict()
         for model in models:
             if isinstance(model, str):
                 if model in self.models.keys():
                     model = self.models[model]
             if isinstance(model, str):
-                model_type = self.get_model_attribute(model=model, attribute='type')
-                model_path = self.get_model_attribute(model=model, attribute='path')
+                model_type = self.get_model_attribute(model=model, attribute="type")
+                model_path = self.get_model_attribute(model=model, attribute="path")
                 model_info_dict[model] = model_type.load_info(path=model_path)
             else:
                 model_info_dict[model.name] = model.get_info()
         return model_info_dict
 
-    def reduce_memory_size(self, remove_data=True, remove_fit_stack=False, remove_fit=True, remove_info=False, requires_save=True, reduce_children=False, **kwargs):
+    def reduce_memory_size(
+        self, remove_data=True, remove_fit_stack=False, remove_fit=True, remove_info=False, requires_save=True, reduce_children=False, **kwargs
+    ):
         if remove_data and self.is_data_saved:
             data_files = [
-                self.path_data + 'X.pkl',
-                self.path_data + 'X_val.pkl',
-                self.path_data + 'y.pkl',
-                self.path_data + 'y_val.pkl',
+                self.path_data + "X.pkl",
+                self.path_data + "X_val.pkl",
+                self.path_data + "y.pkl",
+                self.path_data + "y_val.pkl",
             ]
             for data_file in data_files:
                 try:
                     os.remove(data_file)
                 except FileNotFoundError:
                     pass
             if requires_save:
@@ -2622,26 +2946,33 @@
             try:
                 os.rmdir(self.path_utils)
             except OSError:
                 pass
         models = self.get_model_names()
         for model in models:
             model = self.load_model(model)
-            model.reduce_memory_size(remove_fit_stack=remove_fit_stack, remove_fit=remove_fit, remove_info=remove_info, requires_save=requires_save, reduce_children=reduce_children, **kwargs)
+            model.reduce_memory_size(
+                remove_fit_stack=remove_fit_stack,
+                remove_fit=remove_fit,
+                remove_info=remove_info,
+                requires_save=requires_save,
+                reduce_children=reduce_children,
+                **kwargs,
+            )
             if requires_save:
                 self.save_model(model, reduce_memory=False)
         if requires_save:
             self.save()
 
     # TODO: Also enable deletion of models which didn't succeed in training (files may still be persisted)
     #  This includes the original HPO fold for stacking
     # Deletes specified models from trainer and from disk (if delete_from_disk=True).
     def delete_models(self, models_to_keep=None, models_to_delete=None, allow_delete_cascade=False, delete_from_disk=True, dry_run=True):
         if models_to_keep is not None and models_to_delete is not None:
-            raise ValueError('Exactly one of [models_to_keep, models_to_delete] must be set.')
+            raise ValueError("Exactly one of [models_to_keep, models_to_delete] must be set.")
         if models_to_keep is not None:
             if not isinstance(models_to_keep, list):
                 models_to_keep = [models_to_keep]
             minimum_model_set = set()
             for model in models_to_keep:
                 minimum_model_set.update(self.get_minimum_model_set(model))
             minimum_model_set = list(minimum_model_set)
@@ -2651,27 +2982,29 @@
                 models_to_delete = [models_to_delete]
             minimum_model_set = set(models_to_delete)
             minimum_model_set_orig = copy.deepcopy(minimum_model_set)
             for model in models_to_delete:
                 minimum_model_set.update(nx.algorithms.dag.descendants(self.model_graph, model))
             if not allow_delete_cascade:
                 if minimum_model_set != minimum_model_set_orig:
-                    raise AssertionError('models_to_delete contains models which cause a delete cascade due to other models being dependent on them. Set allow_delete_cascade=True to enable the deletion.')
+                    raise AssertionError(
+                        "models_to_delete contains models which cause a delete cascade due to other models being dependent on them. Set allow_delete_cascade=True to enable the deletion."
+                    )
             minimum_model_set = list(minimum_model_set)
             models_to_remove = [model for model in self.get_model_names() if model in minimum_model_set]
         else:
-            raise ValueError('Exactly one of [models_to_keep, models_to_delete] must be set.')
+            raise ValueError("Exactly one of [models_to_keep, models_to_delete] must be set.")
 
         if dry_run:
-            logger.log(30, f'Dry run enabled, AutoGluon would have deleted the following models: {models_to_remove}')
+            logger.log(30, f"Dry run enabled, AutoGluon would have deleted the following models: {models_to_remove}")
             if delete_from_disk:
                 for model in models_to_remove:
                     model = self.load_model(model)
-                    logger.log(30, f'\tDirectory {model.path} would have been deleted.')
-            logger.log(30, f'To perform the deletion, set dry_run=False')
+                    logger.log(30, f"\tDirectory {model.path} would have been deleted.")
+            logger.log(30, f"To perform the deletion, set dry_run=False")
             return
 
         if delete_from_disk:
             for model in models_to_remove:
                 model = self.load_model(model)
                 model.delete_from_disk()
 
@@ -2725,57 +3058,73 @@
         save_pkl.save(path=self.path + self.trainer_info_name, object=info)
         save_json.save(path=self.path + self.trainer_info_json_name, obj=info)
         return info
 
     def _process_hyperparameters(self, hyperparameters: dict) -> dict:
         return process_hyperparameters(hyperparameters=hyperparameters)
 
-    def distill(self, X=None, y=None, X_val=None, y_val=None, X_unlabeled=None,
-                time_limit=None, hyperparameters=None, holdout_frac=None, verbosity=None,
-                models_name_suffix=None, teacher=None, teacher_preds='soft',
-                augmentation_data=None, augment_method='spunge', augment_args={'size_factor':5,'max_size':int(1e5)},
-                augmented_sample_weight=1.0):
-        """ Various distillation algorithms.
-            Args:
-                X, y: pd.DataFrame and pd.Series of training data.
-                    If None, original training data used during predictor.fit() will be loaded.
-                    This data is split into train/validation if X_val, y_val are None.
-                X_val, y_val: pd.DataFrame and pd.Series of validation data.
-                time_limit, hyperparameters, holdout_frac: defined as in predictor.fit()
-                teacher (None or str):
-                    If None, uses the model with the highest validation score as the teacher model, otherwise use the specified model name as the teacher.
-                teacher_preds (None or str): If None, we only train with original labels (no data augmentation, overrides augment_method)
-                    If 'hard', labels are hard teacher predictions given by: teacher.predict()
-                    If 'soft', labels are soft teacher predictions given by: teacher.predict_proba()
-                    Note: 'hard' and 'soft' are equivalent for regression problems.
-                    If augment_method specified, teacher predictions are only used to label augmented data (training data keeps original labels).
-                    To apply label-smoothing: teacher_preds='onehot' will use original training data labels converted to one-hots for multiclass (no data augmentation).  # TODO: expose smoothing-hyperparameter.
-                models_name_suffix (str): Suffix to append to each student model's name, new names will look like: 'MODELNAME_dstl_SUFFIX'
-                augmentation_data: pd.DataFrame of additional data to use as "augmented data" (does not contain labels).
-                    When specified, augment_method, augment_args are ignored, and this is the only augmented data that is used (teacher_preds cannot be None).
-                augment_method (None or str): specifies which augmentation strategy to utilize. Options: [None, 'spunge','munge']
-                    If None, no augmentation gets applied.
-                }
-                augment_args (dict): args passed into the augmentation function corresponding to augment_method.
-                augmented_sample_weight (float): Nonnegative value indicating how much to weight augmented samples. This is only considered if sample_weight was initially specified in Predictor.
+    def distill(
+        self,
+        X=None,
+        y=None,
+        X_val=None,
+        y_val=None,
+        X_unlabeled=None,
+        time_limit=None,
+        hyperparameters=None,
+        holdout_frac=None,
+        verbosity=None,
+        models_name_suffix=None,
+        teacher=None,
+        teacher_preds="soft",
+        augmentation_data=None,
+        augment_method="spunge",
+        augment_args={"size_factor": 5, "max_size": int(1e5)},
+        augmented_sample_weight=1.0,
+    ):
+        """Various distillation algorithms.
+        Args:
+            X, y: pd.DataFrame and pd.Series of training data.
+                If None, original training data used during predictor.fit() will be loaded.
+                This data is split into train/validation if X_val, y_val are None.
+            X_val, y_val: pd.DataFrame and pd.Series of validation data.
+            time_limit, hyperparameters, holdout_frac: defined as in predictor.fit()
+            teacher (None or str):
+                If None, uses the model with the highest validation score as the teacher model, otherwise use the specified model name as the teacher.
+            teacher_preds (None or str): If None, we only train with original labels (no data augmentation, overrides augment_method)
+                If 'hard', labels are hard teacher predictions given by: teacher.predict()
+                If 'soft', labels are soft teacher predictions given by: teacher.predict_proba()
+                Note: 'hard' and 'soft' are equivalent for regression problems.
+                If augment_method specified, teacher predictions are only used to label augmented data (training data keeps original labels).
+                To apply label-smoothing: teacher_preds='onehot' will use original training data labels converted to one-hots for multiclass (no data augmentation).  # TODO: expose smoothing-hyperparameter.
+            models_name_suffix (str): Suffix to append to each student model's name, new names will look like: 'MODELNAME_dstl_SUFFIX'
+            augmentation_data: pd.DataFrame of additional data to use as "augmented data" (does not contain labels).
+                When specified, augment_method, augment_args are ignored, and this is the only augmented data that is used (teacher_preds cannot be None).
+            augment_method (None or str): specifies which augmentation strategy to utilize. Options: [None, 'spunge','munge']
+                If None, no augmentation gets applied.
+            }
+            augment_args (dict): args passed into the augmentation function corresponding to augment_method.
+            augmented_sample_weight (float): Nonnegative value indicating how much to weight augmented samples. This is only considered if sample_weight was initially specified in Predictor.
         """
         if verbosity is None:
             verbosity = self.verbosity
 
         if teacher is None:
             teacher = self._get_best()
 
         hyperparameter_tune = False  # TODO: add as argument with scheduler options.
         if augmentation_data is not None and teacher_preds is None:
             raise ValueError("augmentation_data must be None if teacher_preds is None")
 
         logger.log(20, f"Distilling with teacher='{teacher}', teacher_preds={str(teacher_preds)}, augment_method={str(augment_method)} ...")
         if teacher not in self.get_model_names(can_infer=True):
-            raise AssertionError(f"Teacher model '{teacher}' is not a valid teacher model! Either it does not exist or it cannot infer on new data.\n"
-                                 f"Valid teacher models: {self.get_model_names(can_infer=True)}")
+            raise AssertionError(
+                f"Teacher model '{teacher}' is not a valid teacher model! Either it does not exist or it cannot infer on new data.\n"
+                f"Valid teacher models: {self.get_model_names(can_infer=True)}"
+            )
         if X is None:
             if y is not None:
                 raise ValueError("X cannot be None when y specified.")
             X = self.load_X()
             X_val = self.load_X_val()
 
         if y is None:
@@ -2794,24 +3143,26 @@
         og_verbosity = self.verbosity
         self.bagged_mode = False  # turn off bagging
         self.verbosity = verbosity  # change verbosity for distillation
 
         if self.sample_weight is not None:
             X, w = extract_column(X, self.sample_weight)
 
-        if teacher_preds is None or teacher_preds == 'onehot':
+        if teacher_preds is None or teacher_preds == "onehot":
             augment_method = None
-            logger.log(20, "Training students without a teacher model. Set teacher_preds = 'soft' or 'hard' to distill using the best AutoGluon predictor as teacher.")
+            logger.log(
+                20, "Training students without a teacher model. Set teacher_preds = 'soft' or 'hard' to distill using the best AutoGluon predictor as teacher."
+            )
 
-        if teacher_preds in ['onehot','soft']:
+        if teacher_preds in ["onehot", "soft"]:
             y = format_distillation_labels(y, self.problem_type, self.num_classes)
             y_val = format_distillation_labels(y_val, self.problem_type, self.num_classes)
 
         if augment_method is None and augmentation_data is None:
-            if teacher_preds == 'hard':
+            if teacher_preds == "hard":
                 y_pred = pd.Series(self.predict(X, model=teacher))
                 if (self.problem_type != REGRESSION) and (len(y_pred.unique()) < len(y.unique())):  # add missing labels
                     logger.log(15, "Adding missing labels to distillation dataset by including some real training examples")
                     indices_to_add = []
                     for clss in y.unique():
                         if clss not in y_pred.unique():
                             logger.log(15, f"Fetching a row with label={clss} from training data")
@@ -2820,63 +3171,66 @@
                     X_extra = X.loc[indices_to_add].copy()
                     y_extra = y.loc[indices_to_add].copy()  # these are actually real training examples
                     X = pd.concat([X, X_extra])
                     y_pred = pd.concat([y_pred, y_extra])
                     if self.sample_weight is not None:
                         w = pd.concat([w, w[indices_to_add]])
                 y = y_pred
-            elif teacher_preds == 'soft':
+            elif teacher_preds == "soft":
                 y = self.predict_proba(X, model=teacher)
                 if self.problem_type == MULTICLASS:
                     y = pd.DataFrame(y)
                 else:
                     y = pd.Series(y)
         else:
-            X_aug = augment_data(X=X, feature_metadata=self.feature_metadata,
-                                 augmentation_data=augmentation_data, augment_method=augment_method, augment_args=augment_args)
+            X_aug = augment_data(
+                X=X, feature_metadata=self.feature_metadata, augmentation_data=augmentation_data, augment_method=augment_method, augment_args=augment_args
+            )
             if len(X_aug) > 0:
-                if teacher_preds == 'hard':
+                if teacher_preds == "hard":
                     y_aug = pd.Series(self.predict(X_aug, model=teacher))
-                elif teacher_preds == 'soft':
+                elif teacher_preds == "soft":
                     y_aug = self.predict_proba(X_aug, model=teacher)
                     if self.problem_type == MULTICLASS:
                         y_aug = pd.DataFrame(y_aug)
                     else:
                         y_aug = pd.Series(y_aug)
                 else:
                     raise ValueError(f"Unknown teacher_preds specified: {teacher_preds}")
 
                 X = pd.concat([X, X_aug])
                 y = pd.concat([y, y_aug])
                 if self.sample_weight is not None:
-                     w = pd.concat([w, pd.Series([augmented_sample_weight]*len(X_aug))])
+                    w = pd.concat([w, pd.Series([augmented_sample_weight] * len(X_aug))])
 
         X.reset_index(drop=True, inplace=True)
         y.reset_index(drop=True, inplace=True)
         if self.sample_weight is not None:
             w.reset_index(drop=True, inplace=True)
             X[self.sample_weight] = w
 
-        name_suffix = '_DSTL'  # all student model names contain this substring
+        name_suffix = "_DSTL"  # all student model names contain this substring
         if models_name_suffix is not None:
             name_suffix = name_suffix + "_" + models_name_suffix
 
         if hyperparameters is None:
-            hyperparameters = {'GBM': {}, 'CAT': {}, 'NN_TORCH': {}, 'RF': {}}
-        hyperparameters = self._process_hyperparameters(hyperparameters=hyperparameters)  # TODO: consider exposing ag_args_fit, excluded_model_types as distill() arguments.
-        if teacher_preds is not None and teacher_preds != 'hard' and self.problem_type != REGRESSION:
+            hyperparameters = {"GBM": {}, "CAT": {}, "NN_TORCH": {}, "RF": {}}
+        hyperparameters = self._process_hyperparameters(
+            hyperparameters=hyperparameters
+        )  # TODO: consider exposing ag_args_fit, excluded_model_types as distill() arguments.
+        if teacher_preds is not None and teacher_preds != "hard" and self.problem_type != REGRESSION:
             self._regress_preds_asprobas = True
 
         core_kwargs = {
-            'stack_name': self.distill_stackname,
-            'get_models_func': self.construct_model_templates_distillation,
+            "stack_name": self.distill_stackname,
+            "get_models_func": self.construct_model_templates_distillation,
         }
         aux_kwargs = {
-            'get_models_func': self.construct_model_templates_distillation,
-            'check_if_best': False,
+            "get_models_func": self.construct_model_templates_distillation,
+            "check_if_best": False,
         }
 
         # self.bagged_mode = True  # TODO: Add options for bagging
         models = self.train_multi_levels(
             X=X,
             y=y,
             X_val=X_val,
@@ -2893,106 +3247,110 @@
         if self.weight_evaluation:
             X_val, w_val = extract_column(X_val, self.sample_weight)
         for model_name in models:  # finally measure original metric on validation data and overwrite stored val_scores
             model_score = self.score(X_val, y_val_og, model=model_name, weights=w_val)
             model_obj = self.load_model(model_name)
             model_obj.val_score = model_score
             model_obj.save()  # TODO: consider omitting for sake of efficiency
-            self.model_graph.nodes[model_name]['val_score'] = model_score
+            self.model_graph.nodes[model_name]["val_score"] = model_score
             distilled_model_names.append(model_name)
         leaderboard = self.leaderboard()
-        logger.log(20, 'Distilled model leaderboard:')
-        leaderboard_distilled = leaderboard[leaderboard['model'].isin(models)].reset_index(drop=True)
-        with pd.option_context('display.max_rows', None, 'display.max_columns', None, 'display.width', 1000):
+        logger.log(20, "Distilled model leaderboard:")
+        leaderboard_distilled = leaderboard[leaderboard["model"].isin(models)].reset_index(drop=True)
+        with pd.option_context("display.max_rows", None, "display.max_columns", None, "display.width", 1000):
             logger.log(20, leaderboard_distilled)
 
         # reset trainer to old state before distill() was called:
         self.bagged_mode = og_bagged_mode  # TODO: Confirm if safe to train future models after training models in both bagged and non-bagged modes
         self.verbosity = og_verbosity
         return distilled_model_names
 
-    def _get_model_fit_kwargs(self, X: pd.DataFrame, X_val: pd.DataFrame, time_limit: float, k_fold: int, fit_kwargs: dict, ens_sample_weight: List = None) -> dict:
+    def _get_model_fit_kwargs(
+        self, X: pd.DataFrame, X_val: pd.DataFrame, time_limit: float, k_fold: int, fit_kwargs: dict, ens_sample_weight: List = None
+    ) -> dict:
         # Returns kwargs to be passed to AbstractModel's fit function
         if fit_kwargs is None:
             fit_kwargs = dict()
 
         model_fit_kwargs = dict(time_limit=time_limit, verbosity=self.verbosity, **fit_kwargs)
         if self.sample_weight is not None:
             X, w_train = extract_column(X, self.sample_weight)
             if w_train is not None:  # may be None for ensemble
                 # TODO: consider moving weight normalization into AbstractModel.fit()
-                model_fit_kwargs['sample_weight'] = w_train.values/w_train.mean()  # normalization can affect gradient algorithms like boosting
+                model_fit_kwargs["sample_weight"] = w_train.values / w_train.mean()  # normalization can affect gradient algorithms like boosting
             if X_val is not None:
                 X_val, w_val = extract_column(X_val, self.sample_weight)
                 if self.weight_evaluation and w_val is not None:  # ignore validation sample weights unless weight_evaluation specified
-                    model_fit_kwargs['sample_weight_val'] = w_val.values/w_val.mean()
+                    model_fit_kwargs["sample_weight_val"] = w_val.values / w_val.mean()
             if ens_sample_weight is not None:
-                model_fit_kwargs['sample_weight'] = ens_sample_weight  # sample weights to use for weighted ensemble only
-        if self._groups is not None and 'groups' not in model_fit_kwargs:
+                model_fit_kwargs["sample_weight"] = ens_sample_weight  # sample weights to use for weighted ensemble only
+        if self._groups is not None and "groups" not in model_fit_kwargs:
             if k_fold == self.k_fold:  # don't do this on refit full
-                model_fit_kwargs['groups'] = self._groups
+                model_fit_kwargs["groups"] = self._groups
 
         #######################
         # FIXME: This section is a hack, compute genuine feature_metadata for each stack level instead
         #  Don't do this here, do this upstream so it isn't recomputed for each model
         #  Add feature_metadata to model_fit_kwargs
         # FIXME: Sample weight `extract_column` is a hack, have to compute feature_metadata here because sample weight column could be in X upstream, extract sample weight column upstream instead.
         # FIXME: This doesn't assign proper special types to stack features, relying on a hack in StackerEnsembleModel to assign S_STACK to feature metadata, don't do this.
         #  Remove hack in StackerEnsembleModel
         feature_metadata = self.feature_metadata
         features_base = self.feature_metadata.get_features()
         features_new = [feature for feature in X.columns if feature not in features_base]
         if features_new:
             feature_metadata_new = FeatureMetadata.from_df(X[features_new])
             feature_metadata = feature_metadata.join_metadata(feature_metadata_new).keep_features(list(X.columns))
-        model_fit_kwargs['feature_metadata'] = feature_metadata
+        model_fit_kwargs["feature_metadata"] = feature_metadata
         #######################
         return model_fit_kwargs
 
     def _get_bagged_model_fit_kwargs(self, k_fold: int, k_fold_start: int, k_fold_end: int, n_repeats: int, n_repeat_start: int) -> dict:
         # Returns additional kwargs (aside from _get_model_fit_kwargs) to be passed to BaggedEnsembleModel's fit function
         if k_fold is None:
             k_fold = self.k_fold
         if n_repeats is None:
             n_repeats = self.n_repeats
-        return dict(k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold_end, n_repeats=n_repeats, n_repeat_start=n_repeat_start, compute_base_preds=False)
+        return dict(
+            k_fold=k_fold, k_fold_start=k_fold_start, k_fold_end=k_fold_end, n_repeats=n_repeats, n_repeat_start=n_repeat_start, compute_base_preds=False
+        )
 
     def _get_feature_prune_proxy_model(self, proxy_model_class: Union[AbstractModel, None], level: int) -> AbstractModel:
         """
         Returns proxy model to be used for feature pruning - the base learner that has the highest validation score in a particular stack layer.
         Ties are broken by inference speed. If proxy_model_class is not None, take the best base learner belonging to proxy_model_class.
         proxy_model_class is an AbstractModel class (ex. LGBModel).
         """
         proxy_model = None
         if isinstance(proxy_model_class, str):
-            raise AssertionError(f'proxy_model_class must be a subclass of AbstractModel. Was instead a string: {proxy_model_class}')
+            raise AssertionError(f"proxy_model_class must be a subclass of AbstractModel. Was instead a string: {proxy_model_class}")
         banned_models = [GreedyWeightedEnsembleModel, SimpleWeightedEnsembleModel]
         assert proxy_model_class not in banned_models, "WeightedEnsemble models cannot be feature pruning proxy models."
 
         leaderboard = self.leaderboard()
         banned_names = []
-        candidate_model_rows = leaderboard[(~leaderboard['score_val'].isna()) & (leaderboard['stack_level'] == level)]
-        candidate_models_type_inner = self.get_models_attribute_dict(attribute='type_inner', models=candidate_model_rows['model'])
+        candidate_model_rows = leaderboard[(~leaderboard["score_val"].isna()) & (leaderboard["stack_level"] == level)]
+        candidate_models_type_inner = self.get_models_attribute_dict(attribute="type_inner", models=candidate_model_rows["model"])
         for model_name, type_inner in candidate_models_type_inner.copy().items():
             if type_inner in banned_models:
                 banned_names.append(model_name)
                 candidate_models_type_inner.pop(model_name, None)
         banned_names = set(banned_names)
-        candidate_model_rows = candidate_model_rows[~candidate_model_rows['model'].isin(banned_names)]
+        candidate_model_rows = candidate_model_rows[~candidate_model_rows["model"].isin(banned_names)]
         if proxy_model_class is not None:
             candidate_model_names = [model_name for model_name, model_class in candidate_models_type_inner.items() if model_class == proxy_model_class]
-            candidate_model_rows = candidate_model_rows[candidate_model_rows['model'].isin(candidate_model_names)]
+            candidate_model_rows = candidate_model_rows[candidate_model_rows["model"].isin(candidate_model_names)]
         if len(candidate_model_rows) == 0:
             if proxy_model_class is None:
                 logger.warning(f"No models from level {level} have been successfully fit. Skipping feature pruning.")
             else:
                 logger.warning(f"No models of type {proxy_model_class} have finished training in level {level}. Skipping feature pruning.")
             return proxy_model
-        best_candidate_model_rows = candidate_model_rows.loc[candidate_model_rows['score_val'] == candidate_model_rows['score_val'].max()]
-        return self.load_model(best_candidate_model_rows.loc[best_candidate_model_rows['fit_time'].idxmin()]['model'])
+        best_candidate_model_rows = candidate_model_rows.loc[candidate_model_rows["score_val"] == candidate_model_rows["score_val"].max()]
+        return self.load_model(best_candidate_model_rows.loc[best_candidate_model_rows["fit_time"].idxmin()]["model"])
 
     def calibrate_model(self, model_name: str = None, lr: float = 0.01, max_iter: int = 1000, init_val: float = 1.0):
         """
         Applies temperature scaling to a model.
         Applies inverse softmax to predicted probs then trains temperature scalar
         on validation data to maximize negative log likelihood.
         Inversed softmaxes are divided by temperature scalar
@@ -3012,15 +3370,15 @@
             The initial value for temperature scalar term
         """
         # TODO: Note that temperature scaling is known to worsen calibration in the face of shifted test data.
         try:
             # FIXME: Avoid depending on torch for temp scaling
             try_import_torch()
         except ImportError:
-            logger.log(30, 'Warning: Torch is not installed, skipping calibration step...')
+            logger.log(30, "Warning: Torch is not installed, skipping calibration step...")
             return
 
         if model_name is None:
             if self.model_best is not None:
                 models = self.get_model_names(can_infer=True)
                 if self.model_best in models:
                     model_name = self.model_best
@@ -3043,59 +3401,64 @@
 
         if self.problem_type == BINARY:
             # Convert one-dimensional array to be in the form of a 2-class multiclass predict_proba output
             y_val_probs = LabelCleanerMulticlassToBinary.convert_binary_proba_to_multiclass_proba(y_val_probs)
 
         model = self.load_model(model_name=model_name)
         if self.problem_type == QUANTILE:
-            logger.log(15, f'Conformity scores being computed to calibrate model: {model_name}')
-            conformalize = compute_conformity_score(y_val_pred=y_val_probs, y_val=y_val,
-                                                    quantile_levels=self.quantile_levels)
+            logger.log(15, f"Conformity scores being computed to calibrate model: {model_name}")
+            conformalize = compute_conformity_score(y_val_pred=y_val_probs, y_val=y_val, quantile_levels=self.quantile_levels)
             model.conformalize = conformalize
             model.save()
         else:
-            logger.log(15, f'Temperature scaling term being tuned for model: {model_name}')
-            temp_scalar = tune_temperature_scaling(y_val_probs=y_val_probs, y_val=y_val,
-                                                   init_val=init_val, max_iter=max_iter, lr=lr)
+            logger.log(15, f"Temperature scaling term being tuned for model: {model_name}")
+            temp_scalar = tune_temperature_scaling(y_val_probs=y_val_probs, y_val=y_val, init_val=init_val, max_iter=max_iter, lr=lr)
             if temp_scalar is None:
-                logger.log(15, f'Warning: Infinity found during calibration, skipping calibration on {model.name}! '
-                               f'This can occur when the model is absolutely certain of a validation prediction (1.0 pred_proba).')
+                logger.log(
+                    15,
+                    f"Warning: Infinity found during calibration, skipping calibration on {model.name}! "
+                    f"This can occur when the model is absolutely certain of a validation prediction (1.0 pred_proba).",
+                )
             else:
-                logger.log(15, f'Temperature term found is: {temp_scalar}')
+                logger.log(15, f"Temperature term found is: {temp_scalar}")
                 model.params_aux["temperature_scalar"] = temp_scalar
                 model.save()
 
-    def calibrate_decision_threshold(self,
-                                     X: pd.DataFrame | None = None,
-                                     y: np.array | None = None,
-                                     metric: str | Scorer | None = None,
-                                     model: str = 'best',
-                                     weights=None,
-                                     decision_thresholds: int | List[float] = 50,
-                                     verbose: bool = True) -> float:
+    def calibrate_decision_threshold(
+        self,
+        X: pd.DataFrame | None = None,
+        y: np.array | None = None,
+        metric: str | Scorer | None = None,
+        model: str = "best",
+        weights=None,
+        decision_thresholds: int | List[float] = 50,
+        verbose: bool = True,
+    ) -> float:
         # TODO: Docstring
         assert self.problem_type == BINARY, f'calibrate_decision_threshold is only available for `problem_type="{BINARY}"`'
 
         if metric is None:
             metric = self.eval_metric
         elif isinstance(metric, str):
-            metric = get_metric(metric, self.problem_type, 'eval_metric')
+            metric = get_metric(metric, self.problem_type, "eval_metric")
 
-        if model == 'best':
+        if model == "best":
             model = self.get_model_best()
 
         if y is None:
             # If model is refit_full, use its parent to avoid over-fitting
             model_parent = self.get_refit_full_parent(model=model)
             if not self.model_exists(model_parent):
-                raise AssertionError(f'Unable to calibrate the decision threshold on the internal data because the '
-                                     f'model "{model}" is a refit_full model trained on all of the internal data, '
-                                     f'whose parent model "{model_parent}" does not exist or was deleted.\n'
-                                     f'It may have been deleted due to `predictor.fit(..., keep_only_best=True)`. '
-                                     f'Ensure `keep_only_best=False` to be able to calibrate refit_full models.')
+                raise AssertionError(
+                    f"Unable to calibrate the decision threshold on the internal data because the "
+                    f'model "{model}" is a refit_full model trained on all of the internal data, '
+                    f'whose parent model "{model_parent}" does not exist or was deleted.\n'
+                    f"It may have been deleted due to `predictor.fit(..., keep_only_best=True)`. "
+                    f"Ensure `keep_only_best=False` to be able to calibrate refit_full models."
+                )
             model = model_parent
 
             # TODO: Add helpful logging when data is not available, for example post optimize for deployment
             if self.has_val:
                 # Use validation data
                 X = self.load_X_val()
                 if self.weight_evaluation:
@@ -3109,18 +3472,22 @@
                     X, weights = extract_column(X=X, col_name=self.sample_weight)
                 y: np.array = self.load_y()
                 y_pred_proba = self.get_model_oof(model=model)
         else:
             y_pred_proba = self.predict_proba(X=X, model=model)
 
         if not metric.needs_pred:
-            logger.warning(f'WARNING: The provided metric "{metric.name}" does not use class predictions for scoring, '
-                           f'and thus is invalid for decision threshold calibration. '
-                           f'Falling back to `decision_threshold=0.5`.')
+            logger.warning(
+                f'WARNING: The provided metric "{metric.name}" does not use class predictions for scoring, '
+                f"and thus is invalid for decision threshold calibration. "
+                f"Falling back to `decision_threshold=0.5`."
+            )
             return 0.5
 
-        return calibrate_decision_threshold(y=y,
-                                            y_pred_proba=y_pred_proba,
-                                            metric=lambda y, y_pred : self._score_with_y_pred(y=y, y_pred=y_pred, weights=weights, metric=metric),
-                                            decision_thresholds=decision_thresholds,
-                                            metric_name=metric.name,
-                                            verbose=verbose)
+        return calibrate_decision_threshold(
+            y=y,
+            y_pred_proba=y_pred_proba,
+            metric=lambda y, y_pred: self._score_with_y_pred(y=y, y_pred=y_pred, weights=weights, metric=metric),
+            decision_thresholds=decision_thresholds,
+            metric_name=metric.name,
+            verbose=verbose,
+        )
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/trainer/utils.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/trainer/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 def process_hyperparameters(hyperparameters: dict) -> dict:
     hyperparameters = copy.deepcopy(hyperparameters)
 
     has_levels = False
     top_level_keys = hyperparameters.keys()
     for key in top_level_keys:
-        if isinstance(key, int) or key == 'default':
+        if isinstance(key, int) or key == "default":
             has_levels = True
     if not has_levels:
-        hyperparameters = {'default': hyperparameters}
+        hyperparameters = {"default": hyperparameters}
     top_level_keys = hyperparameters.keys()
     for key in top_level_keys:
         for subkey in hyperparameters[key].keys():
             if not isinstance(hyperparameters[key][subkey], list):
                 hyperparameters[key][subkey] = [hyperparameters[key][subkey]]
-    if 'default' not in hyperparameters.keys():
+    if "default" not in hyperparameters.keys():
         level_keys = [key for key in hyperparameters.keys() if isinstance(key, int)]
         max_level_key = max(level_keys)
-        hyperparameters['default'] = copy.deepcopy(hyperparameters[max_level_key])
+        hyperparameters["default"] = copy.deepcopy(hyperparameters[max_level_key])
     return hyperparameters
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/decorators.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,23 @@
     >>> @unpack(g)
     >>> def f(**kwargs):
     >>>     print(kwargs)
     >>>
     >>> f(a=2)  # kwargs is now the output of g(a=2), which is {'b': 3}
     >>> f(c=4)  # kwargs is now the output of g(c=4), which is {'b': 1, 'c': 4}
     """
+
     def _unpack_inner(f):
         @functools.wraps(f)
         def _call(*args, **kwargs):
             gargs, gkwargs = g(*other_args, *args, **kwargs)
             return f(*gargs, **gkwargs)
+
         return _call
+
     return _unpack_inner
 
 
 def _apply_presets(preset_dict: Dict[str, dict], presets_alias: Dict[str, str] = None, *args, **kwargs):
     """
     Pair with `unpack` to alter input arguments with preset values.
 
@@ -53,35 +56,35 @@
         args and kwargs take priority over presets, and if specified in the input will not be overwritten.
         Presets will add new key-values to kwargs if the key did not previously exist.
 
     Returns
     -------
     (*args, **kwargs) with kwargs updated based on specified presets.
     """
-    presets = kwargs.get('presets', None)
+    presets = kwargs.get("presets", None)
     if presets is not None:
         if not isinstance(presets, list):
             presets = [presets]
         preset_kwargs = {}
         for preset in presets:
             if isinstance(preset, str):
                 preset_og = preset
                 preset = preset_dict.get(preset_og, None)
                 if preset is None and presets_alias is not None:
                     preset = presets_alias.get(preset_og, None)
                     if preset is not None:
                         logger.log(20, f"Preset alias specified: '{preset_og}' maps to '{preset}'.")
                         preset = preset_dict.get(preset, None)
                 if preset is None:
-                    raise ValueError(f'Preset \'{preset_og}\' was not found. Valid presets: {list(preset_dict.keys())}')
+                    raise ValueError(f"Preset '{preset_og}' was not found. Valid presets: {list(preset_dict.keys())}")
             if isinstance(preset, dict):
                 for key in preset:
                     preset_kwargs[key] = preset[key]
             else:
-                raise TypeError(f'Preset of type {type(preset)} was given, but only presets of type [dict, str] are valid.')
+                raise TypeError(f"Preset of type {type(preset)} was given, but only presets of type [dict, str] are valid.")
         for key in preset_kwargs:
             if key not in kwargs:
                 kwargs[key] = preset_kwargs[key]
     return args, kwargs
 
 
 def apply_presets(preset_dict: Dict[str, dict], presets_alias: Dict[str, str] = None):
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/early_stopping.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/early_stopping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-
 class AbstractES:
     """
     Abstract early stopping class
     """
+
     def update(self, cur_round, is_best=False) -> bool:
         raise NotImplementedError
 
     def early_stop(self, cur_round, is_best=False) -> bool:
         raise NotImplementedError
 
 
@@ -15,14 +15,15 @@
     Implements early stopping with fixed patience
 
     Parameters
     ----------
     patience : int, default 10
         If no improvement occurs in `patience` rounds or greater, self.early_stop will return True.
     """
+
     def __init__(self, patience=10):
         self.patience = patience
         self.best_round = 0
 
     def update(self, cur_round, is_best=False):
         if is_best:
             self.best_round = cur_round
@@ -67,14 +68,15 @@
         Dictates patience and is used to determine if self.early_stop() returns True.
     patience : int
         If no improvement occurs in `patience` rounds or greater, self.early_stop will return True.
         patience is dictated by the following formula:
         patience = min(self.max_patience, (max(self.min_patience, round(self.best_round * self.adaptive_rate + self.adaptive_offset))))
         Effectively, patience = self.best_round * self.adaptive_rate + self.adaptive_offset, bound by min_patience and max_patience
     """
+
     def __init__(self, adaptive_rate=0.3, adaptive_offset=10, min_patience=10, max_patience=10000):
         self.adaptive_rate = adaptive_rate
         self.adaptive_offset = adaptive_offset
         self.min_patience = min_patience
         self.max_patience = max_patience
         self.best_round = 0
         self.patience = self._update_patience(self.best_round)
@@ -103,15 +105,15 @@
         return min(
             self.max_patience,
             (
                 max(
                     self.min_patience,
                     round(best_round * self.adaptive_rate + self.adaptive_offset),
                 )
-            )
+            ),
         )
 
 
 ES_CLASS_MAP = {
-    'simple': SimpleES,
-    'adaptive': AdaptiveES,
+    "simple": SimpleES,
+    "adaptive": AdaptiveES,
 }
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/feature_selection.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/feature_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from copy import deepcopy
 import logging
 import time
 import traceback
-from typing import List, Set, Tuple, Union
 import uuid
+from copy import deepcopy
+from typing import List, Set, Tuple, Union
 
 import numpy as np
 import pandas as pd
 
 from autogluon.common.features.types import R_FLOAT
 
 from ..models.abstract.abstract_model import AbstractModel
@@ -20,15 +20,15 @@
 
 def add_noise_column(X: pd.DataFrame, rng: np.random.Generator, noise_columns: List[str] = None, count: int = 1) -> Tuple[pd.DataFrame, List[str]]:
     """
     Create a copy of dataset X with extra synthetic columns generated from standard normal distribution.
     """
     X = X.copy()
     if noise_columns is None:
-        noise_columns = [str(uuid.uuid4()) for _ in range(1, count+1)]
+        noise_columns = [str(uuid.uuid4()) for _ in range(1, count + 1)]
     for col_name in noise_columns:
         noise = rng.standard_normal(len(X))
         X[col_name] = noise
     return X, noise_columns
 
 
 def merge_importance_dfs(df_old: pd.DataFrame, df_new: pd.DataFrame, using_prev_fit_fi: Set[str]) -> pd.DataFrame:
@@ -38,19 +38,19 @@
     has not been calculated, the resulting dataframe will contain the other dataframe's feature importance stats.
     df_old is assumed to have been from previous feature importance computation round or even pruning round and
     can have more features (rows) than df_new. Also, update using_prev_fit_fi to indicate the updated feature list that
     uses feature importance values from previous fit.
     """
     if df_old is None:
         # Remove features whose importance has just been computed from using_prev_fit_fi if they exist
-        using_prev_fit_fi.difference_update(df_new[df_new['n'] > 0].index.tolist())
+        using_prev_fit_fi.difference_update(df_new[df_new["n"] > 0].index.tolist())
         return df_new
     assert len(df_old) >= len(df_new), "df_old cannot have less rows than df_new."
-    evaluated_old_rows, evaluated_new_rows = df_old[df_old['n'] > 0], df_new[df_new['n'] > 0]
-    unevaluated_old_rows, unevaluated_new_rows = df_old[df_old['n'] == 0], df_new[df_new['n'] == 0]
+    evaluated_old_rows, evaluated_new_rows = df_old[df_old["n"] > 0], df_new[df_new["n"] > 0]
+    unevaluated_old_rows, unevaluated_new_rows = df_old[df_old["n"] == 0], df_new[df_new["n"] == 0]
     evaluated_both = evaluated_new_rows.index.intersection(evaluated_old_rows.index).difference(using_prev_fit_fi).tolist()
     evaluated_neither = unevaluated_new_rows.index.intersection(unevaluated_old_rows.index).tolist()
     evaluated_old_only = evaluated_old_rows[evaluated_old_rows.index.isin(unevaluated_new_rows.index)].index.tolist()
     evaluated_new_only = evaluated_new_rows[evaluated_new_rows.index.isin(unevaluated_old_rows.index)].index.tolist()
     evaluated_new_first_time = evaluated_new_rows.index.intersection(using_prev_fit_fi).tolist()
 
     # for features with no info on both df_old and df_new, return no info rows
@@ -59,26 +59,28 @@
     evaluated_old_only_rows = evaluated_old_rows.loc[evaluated_old_only]
     # for features with info on only df_new or whose df_old feature importance came from the previous model, return corresponding df_new rows
     evaluated_new_only_rows = evaluated_new_rows.loc[set(evaluated_new_only + evaluated_new_first_time)]
     # for features with info on both df_new and whose df_old feature importance came from the current model, return combined statistics
     evaluated_both_rows = pd.DataFrame()
     evaluated_both_rows_new = evaluated_new_rows.loc[evaluated_both].sort_index()
     evaluated_both_rows_old = evaluated_old_rows.loc[evaluated_both].sort_index()
-    mean_old, mean_new = evaluated_both_rows_old['importance'], evaluated_both_rows_new['importance']
-    stddev_old, stddev_new = evaluated_both_rows_old['stddev'], evaluated_both_rows_new['stddev']
-    n_old, n_new = evaluated_both_rows_old['n'], evaluated_both_rows_new['n']
-    evaluated_both_rows['importance'] = (n_old * mean_old + n_new * mean_new) / (n_old + n_new)
+    mean_old, mean_new = evaluated_both_rows_old["importance"], evaluated_both_rows_new["importance"]
+    stddev_old, stddev_new = evaluated_both_rows_old["stddev"], evaluated_both_rows_new["stddev"]
+    n_old, n_new = evaluated_both_rows_old["n"], evaluated_both_rows_new["n"]
+    evaluated_both_rows["importance"] = (n_old * mean_old + n_new * mean_new) / (n_old + n_new)
     # Refer to https://math.stackexchange.com/questions/2971315/how-do-i-combine-standard-deviations-of-two-groups
-    evaluated_both_rows['stddev'] = (((n_old - 1) * stddev_old ** 2 + (n_new - 1) * stddev_new ** 2) / (n_old + n_new - 1) +
-                                     (n_old * n_new * (mean_old - mean_new) ** 2) / ((n_old + n_new) * (n_old + n_new - 1))) ** 0.5
-    evaluated_both_rows['p_value'] = None
-    evaluated_both_rows['n'] = n_old + n_new
+    evaluated_both_rows["stddev"] = (
+        ((n_old - 1) * stddev_old**2 + (n_new - 1) * stddev_new**2) / (n_old + n_new - 1)
+        + (n_old * n_new * (mean_old - mean_new) ** 2) / ((n_old + n_new) * (n_old + n_new - 1))
+    ) ** 0.5
+    evaluated_both_rows["p_value"] = None
+    evaluated_both_rows["n"] = n_old + n_new
     # remove features evaluated in df_new from using_prev_fit_fi if they exist
     using_prev_fit_fi.difference_update(evaluated_new_rows.index.tolist())
-    result = pd.concat([evaluated_both_rows, evaluated_new_only_rows, evaluated_old_only_rows, evaluated_neither_rows]).sort_values('importance')
+    result = pd.concat([evaluated_both_rows, evaluated_new_only_rows, evaluated_old_only_rows, evaluated_neither_rows]).sort_values("importance")
     assert len(result) == len(df_new), "Length of the updated DataFrame must be equal to the inputted DataFrame."
     return result
 
 
 def sort_features_by_priority(features: List[str], prev_importance_df: pd.DataFrame, using_prev_fit_fi: Set[str]) -> List[str]:
     """
     Return a list of features sorted by feature importance calculation priority in ascending order.
@@ -89,19 +91,21 @@
     noise prune_threshold, noise columns are prioritized first since their scores are needed to determine
     the pruning threshold.
     """
     is_first_run = prev_importance_df is None
     if not is_first_run:
         prev_deleted_features = [feature for feature in prev_importance_df.index if feature not in features]
         prev_importance_df = prev_importance_df.drop(prev_deleted_features)
-        unevaluated_rows = prev_importance_df[prev_importance_df['importance'].isna()]
-        prev_fit_evaluated_rows = prev_importance_df[~(prev_importance_df['importance'].isna()) &
-                                                      (prev_importance_df.index.isin(using_prev_fit_fi))].sort_values(by='importance')
-        curr_fit_evaluated_rows = prev_importance_df[~(prev_importance_df['importance'].isna()) &
-                                                     ~(prev_importance_df.index.isin(using_prev_fit_fi))].sort_values(by='importance')
+        unevaluated_rows = prev_importance_df[prev_importance_df["importance"].isna()]
+        prev_fit_evaluated_rows = prev_importance_df[
+            ~(prev_importance_df["importance"].isna()) & (prev_importance_df.index.isin(using_prev_fit_fi))
+        ].sort_values(by="importance")
+        curr_fit_evaluated_rows = prev_importance_df[
+            ~(prev_importance_df["importance"].isna()) & ~(prev_importance_df.index.isin(using_prev_fit_fi))
+        ].sort_values(by="importance")
         features = unevaluated_rows.index.tolist() + prev_fit_evaluated_rows.index.tolist() + curr_fit_evaluated_rows.index.tolist()
     return features
 
 
 class FeatureSelector:
     def __init__(self, model: AbstractModel, time_limit: float, problem_type: str, seed: int = 0, raise_exception=False) -> None:
         """
@@ -120,37 +124,49 @@
         """
         # TODO: Make this work with unlabelled data
         assert time_limit is not None, "Time limit cannot be unspecified."
         self.is_bagged = isinstance(model, BaggedEnsembleModel)
 
         self.model_class = model.__class__
         self.model_params = model.get_params()
-        self.model_name = "FeatureSelector_" + self.model_params['name']
-        self.model_params['name'] = self.model_name
+        self.model_name = "FeatureSelector_" + self.model_params["name"]
+        self.model_params["name"] = self.model_name
         if self.is_bagged:
             # required for feature importance computation
-            self.model_params['hyperparameters']['use_child_oof'] = False
-            self.model_params['hyperparameters']['save_bag_folds'] = True
+            self.model_params["hyperparameters"]["use_child_oof"] = False
+            self.model_params["hyperparameters"]["save_bag_folds"] = True
         del model
 
         self.time_limit = time_limit
         self.time_start = time.time()
         self.problem_type = problem_type
         self.rng = np.random.default_rng(seed)
         self.fit_score_time = None
         self.model_predict_time = None
         self.attempted_removals = set()
         self.replace_bag = False
         self.max_n_shuffle = 20
         self.min_prune_ratio = 0.01
         self.raise_exception = raise_exception
 
-    def select_features(self, X: pd.DataFrame, y: pd.Series, X_val: pd.DataFrame = None, y_val: pd.Series = None, n_train_subsample: int = 50000,
-                        n_fi_subsample: int = 10000, prune_threshold: float = 'noise', prune_ratio: float = 0.05, stopping_round: int = 10,
-                        min_improvement: float = 1e-6, max_fits: int = None, **kwargs) -> List[str]:
+    def select_features(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        X_val: pd.DataFrame = None,
+        y_val: pd.Series = None,
+        n_train_subsample: int = 50000,
+        n_fi_subsample: int = 10000,
+        prune_threshold: float = "noise",
+        prune_ratio: float = 0.05,
+        stopping_round: int = 10,
+        min_improvement: float = 1e-6,
+        max_fits: int = None,
+        **kwargs,
+    ) -> List[str]:
         """
         Performs time-aware recursive feature elimination based on permutation feature importance. While time remains, compute feature importance
         score for as many features as possible over at least min_fi_samples validation datapoints, discard features whose score is less than or
         equal to prune_threshold, fit the model on those features and keep the feature subset if its validation score is better, and repeat.
 
         Parameters
         ----------
@@ -190,217 +206,262 @@
 
         Returns
         -------
         candidate_features : List[str]
             Optimal feature subset selected by this method. Set to original features if no features are below pruning threshold or we run
             out of time before finding a better feature subset.
         """
-        logger.log(20, f"Performing feature pruning with model: {self.model_name}, total time limit: {round(self.time_limit, 2)}s, "
-                       f"stop threshold: {stopping_round}, prune ratio: {prune_ratio}, prune threshold: {prune_threshold}.")
+        logger.log(
+            20,
+            f"Performing feature pruning with model: {self.model_name}, total time limit: {round(self.time_limit, 2)}s, "
+            f"stop threshold: {stopping_round}, prune ratio: {prune_ratio}, prune threshold: {prune_threshold}.",
+        )
         original_features = X.columns.tolist()
         if len(original_features) <= 1:
             logger.log(20, f"\tSkipping feature pruning since there is less than 2 features in the dataset.")
             return original_features
-        X, y, X_val, y_val, X_fi, y_fi, prune_threshold, noise_columns, feature_metadata = self.setup(X=X, y=y, X_val=X_val, y_val=y_val,
-                                                                                                      n_train_subsample=n_train_subsample,
-                                                                                                      prune_threshold=prune_threshold, **kwargs)
-        kwargs['feature_metadata'] = feature_metadata
+        X, y, X_val, y_val, X_fi, y_fi, prune_threshold, noise_columns, feature_metadata = self.setup(
+            X=X, y=y, X_val=X_val, y_val=y_val, n_train_subsample=n_train_subsample, prune_threshold=prune_threshold, **kwargs
+        )
+        kwargs["feature_metadata"] = feature_metadata
         try:
             index = 1
             candidate_features = X.columns.tolist()
-            best_info = {'features': candidate_features, 'index': 1, 'model': None, 'score': None}
+            best_info = {"features": candidate_features, "index": 1, "model": None, "score": None}
             curr_model, score, fit_score_time = self.fit_score_model(X, y, X_val, y_val, candidate_features, f"{self.model_name}_1", **kwargs)
-            best_info['model'], best_info['score'] = curr_model, score
+            best_info["model"], best_info["score"] = curr_model, score
 
             time_budget_fi = self.compute_time_budget_fi(X_fi=X_fi, n_subsample=n_fi_subsample, **kwargs)
             logger.log(20, f"\tExpected model fit time: {round(fit_score_time, 2)}s, and expected candidate generation time: {round(time_budget_fi, 2)}s.")
-            logger.log(20, f"\tRound 1 of feature pruning model fit ({round(fit_score_time, 2)}s):\n"
-                           f"\t\tValidation score of the model fit on original features is ({round(best_info['score'], 4)}).")
+            logger.log(
+                20,
+                f"\tRound 1 of feature pruning model fit ({round(fit_score_time, 2)}s):\n"
+                f"\t\tValidation score of the model fit on original features is ({round(best_info['score'], 4)}).",
+            )
             time_remaining = self.time_limit - (time.time() - self.time_start)
             if time_remaining < self.fit_score_time + time_budget_fi:
                 logger.warning(f"\tNo time to perform the next pruning round (remaining: {time_remaining}, needed: {self.fit_score_time + time_budget_fi}).")
                 raise TimeLimitExceeded
 
             importance_df = None
             while True:
                 index = index + 1
                 model_name = f"{self.model_name}_{index}"
                 prioritize_fi = set(noise_columns)
-                fn_args = {'X': X_fi, 'y': y_fi, 'model': best_info['model'], 'time_budget': time_budget_fi, 'features': best_info['features'],
-                           'n_subsample': n_fi_subsample, 'prune_threshold': prune_threshold, 'prune_ratio': prune_ratio, 'prioritized': prioritize_fi}
+                fn_args = {
+                    "X": X_fi,
+                    "y": y_fi,
+                    "model": best_info["model"],
+                    "time_budget": time_budget_fi,
+                    "features": best_info["features"],
+                    "n_subsample": n_fi_subsample,
+                    "prune_threshold": prune_threshold,
+                    "prune_ratio": prune_ratio,
+                    "prioritized": prioritize_fi,
+                }
                 fn_args.update(self.get_extra_fn_args(**kwargs))
-                candidate_features, importance_df, success, prune_time = self.compute_next_candidate(fn_args=fn_args, round_time_budget=time_budget_fi,
-                                                                                                     prev_best_features=best_info['features'],
-                                                                                                     prev_importance_df=importance_df)
+                candidate_features, importance_df, success, prune_time = self.compute_next_candidate(
+                    fn_args=fn_args, round_time_budget=time_budget_fi, prev_best_features=best_info["features"], prev_importance_df=importance_df
+                )
                 if not success:
                     logger.log(20, f"\tTime is up while computing feature importance or there are no more features to prune. Ending...")
                     break
                 curr_model, score, fit_score_time = self.fit_score_model(X, y, X_val, y_val, candidate_features, model_name, **kwargs)
 
                 new_feature_count = len(candidate_features) - (1 if len(noise_columns) > 0 else 0)
-                prev_feature_count = len(best_info['features']) - (1 if len(noise_columns) > 0 else 0)
-                if score >= best_info['score'] * (1 + min_improvement):
-                    logger.log(20, f"\tRound {index} of feature pruning model fit ({round(fit_score_time, 2)}s):\n"
-                                   f"\t\tValidation score of the current model fit on {new_feature_count} features ({round(score, 4)}) is better than "
-                                   f"validation score of the best model fit on {prev_feature_count} features ({round(best_info['score'], 4)}). Updating model.")
-                    best_info['model'].delete_from_disk(silent=True)
-                    best_info = {'model': curr_model, 'features': candidate_features, 'score': score, 'index': index}
+                prev_feature_count = len(best_info["features"]) - (1 if len(noise_columns) > 0 else 0)
+                if score >= best_info["score"] * (1 + min_improvement):
+                    logger.log(
+                        20,
+                        f"\tRound {index} of feature pruning model fit ({round(fit_score_time, 2)}s):\n"
+                        f"\t\tValidation score of the current model fit on {new_feature_count} features ({round(score, 4)}) is better than "
+                        f"validation score of the best model fit on {prev_feature_count} features ({round(best_info['score'], 4)}). Updating model.",
+                    )
+                    best_info["model"].delete_from_disk(silent=True)
+                    best_info = {"model": curr_model, "features": candidate_features, "score": score, "index": index}
                 else:
-                    logger.log(20, f"\tRound {index} of feature pruning model fit ({round(fit_score_time, 2)}s):\n"
-                                   f"\t\tValidation score of the current model fit on {new_feature_count} features ({round(score, 4)}) is not better than "
-                                   f"validation score of the best model fit on {prev_feature_count} features ({round(best_info['score'], 4)}). Retrying.")
+                    logger.log(
+                        20,
+                        f"\tRound {index} of feature pruning model fit ({round(fit_score_time, 2)}s):\n"
+                        f"\t\tValidation score of the current model fit on {new_feature_count} features ({round(score, 4)}) is not better than "
+                        f"validation score of the best model fit on {prev_feature_count} features ({round(best_info['score'], 4)}). Retrying.",
+                    )
                     curr_model.delete_from_disk(silent=True)
 
                 time_remaining = self.time_limit - (time.time() - self.time_start)
                 if max_fits is not None and index >= max_fits:
                     logger.log(20, f"\tReached maximum number of allowed fits, {max_fits}, during feature selection. Ending...")
                     break
-                if stopping_round is not None and index - best_info['index'] >= stopping_round:
+                if stopping_round is not None and index - best_info["index"] >= stopping_round:
                     logger.log(20, f"\tScore has not improved for {stopping_round} feature pruning rounds. Ending...")
                     break
                 if time_remaining <= self.fit_score_time + prune_time:
                     logger.log(20, f"\tInsufficient time to finish next pruning round. Ending...")
                     break
         except TimeLimitExceeded:
             logger.log(20, f"\tTime limit exceeded while pruning features. Ending...")
         except Exception as e:
             logger.error(traceback.format_exc())
             logger.error(f"\tERROR: Exception raised during feature pruning. Reason: {e}. Ending...")
             if self.raise_exception:
                 raise e
 
         if len(noise_columns) > 0:
-            best_info['features'] = [feature for feature in best_info['features'] if feature not in noise_columns]
-        if isinstance(best_info['model'], AbstractModel):
-            best_info['model'].delete_from_disk(silent=True)
+            best_info["features"] = [feature for feature in best_info["features"] if feature not in noise_columns]
+        if isinstance(best_info["model"], AbstractModel):
+            best_info["model"].delete_from_disk(silent=True)
         logger.log(20, f"\tSuccessfully ended prune loop after {index} feature pruning rounds ({round(time.time() - self.time_start, 2)}s).")
         logger.log(20, f"\tFeature count before/after feature pruning: {len(original_features)} -> {len(best_info['features'])}.")
-        return best_info['features']
+        return best_info["features"]
 
-    def compute_next_candidate(self, fn_args: dict, round_time_budget: float, prev_best_features: List[str], prev_importance_df: pd.DataFrame
-                               ) -> Tuple[List[str], pd.DataFrame, bool, float]:
+    def compute_next_candidate(
+        self, fn_args: dict, round_time_budget: float, prev_best_features: List[str], prev_importance_df: pd.DataFrame
+    ) -> Tuple[List[str], pd.DataFrame, bool, float]:
         """
         While time allows, repeatedly compute feature importance and generate candidate feature subsets using a fixed time budget.
         If at least self.min_prune_ratio of the features can be pruned or all feature importances are calculated, return. If less than
         self.min_prune_ratio of the features can be pruned but not all importance scores have been calculated, repeat the procedure.
         Note: If we have feature importance information from previously fitted model, make use of them since we might not have time this
         iteration to evaluate importance scores for all features. Any feature importance calculated within this call of compute_next_candidate
         will override previous feature importance info.
         """
         candidate_features = prev_best_features
         importance_df = unevaluated_fi_df_template(candidate_features)
         candidate_found = False
-        total_prune_time = 0.
+        total_prune_time = 0.0
         # mark previous fit's computed feature importances here.
         if prev_importance_df is not None:
-            fn_args['prev_importance_df'] = prev_importance_df
-            fn_args['using_prev_fit_fi'] = set(prev_importance_df[prev_importance_df['n'] > 0].index.tolist())
+            fn_args["prev_importance_df"] = prev_importance_df
+            fn_args["using_prev_fit_fi"] = set(prev_importance_df[prev_importance_df["n"] > 0].index.tolist())
         while self.time_limit - (time.time() - self.time_start) > round_time_budget + self.fit_score_time:
             candidate_features, importance_df, prune_time = self.compute_next_candidate_round(**fn_args)
             # HACK: Line below is needed to get this working with n-repeated bagged models. Related to feature ordering.
-            candidate_features = [feature for feature in fn_args['X'].columns.tolist() if feature in candidate_features]
-            candidate_found = len(candidate_features) > 0 and len(candidate_features) <= (1. - self.min_prune_ratio) * len(prev_best_features)
-            all_features_evaluated = len(importance_df[importance_df['importance'].isna()]) == 0
-            fn_args['prev_importance_df'] = importance_df
+            candidate_features = [feature for feature in fn_args["X"].columns.tolist() if feature in candidate_features]
+            candidate_found = len(candidate_features) > 0 and len(candidate_features) <= (1.0 - self.min_prune_ratio) * len(prev_best_features)
+            all_features_evaluated = len(importance_df[importance_df["importance"].isna()]) == 0
+            fn_args["prev_importance_df"] = importance_df
             total_prune_time = total_prune_time + prune_time
             if candidate_found or all_features_evaluated:
                 break
         logger.log(15, f"\tCandidate generation time: ({round(total_prune_time, 2)}s), Cardinality: {len(candidate_features)}")
         return candidate_features, importance_df, candidate_found, total_prune_time
 
-    def compute_next_candidate_round(self, X: pd.DataFrame, y: pd.Series, model: AbstractModel, time_budget: float, features: List[str],
-                                     n_subsample: int, min_fi_samples: int, max_fi_samples: int, prune_ratio: float, prune_threshold: float,
-                                     prev_importance_df: pd.DataFrame = None, prioritized: Set[str] = set(), using_prev_fit_fi: Set[str] = set(),
-                                     weighted: bool = True) -> Tuple[List[str], pd.DataFrame, float]:
+    def compute_next_candidate_round(
+        self,
+        X: pd.DataFrame,
+        y: pd.Series,
+        model: AbstractModel,
+        time_budget: float,
+        features: List[str],
+        n_subsample: int,
+        min_fi_samples: int,
+        max_fi_samples: int,
+        prune_ratio: float,
+        prune_threshold: float,
+        prev_importance_df: pd.DataFrame = None,
+        prioritized: Set[str] = set(),
+        using_prev_fit_fi: Set[str] = set(),
+        weighted: bool = True,
+    ) -> Tuple[List[str], pd.DataFrame, float]:
         """
         Compute permutation feature importance for as many features as possible under time_budget. Ensure each returned feature importance
         scores are computed from at least n_sample datapoints.
         """
         # determine how many subsamples and shuffles to use for feature importance calculation
         time_start = time.time()
         n_features = len(features)
         n_subsample = min(n_subsample, len(X))
         n_total_sample = max(min_fi_samples, min(max_fi_samples, len(X)))
         n_shuffle = min(np.ceil(n_total_sample / n_subsample).astype(int), self.max_n_shuffle)
-        single_feature_fi_time = self.compute_expected_fi_time_single(X_fi=X, model_predict_time=self.model_predict_time,
-                                                                      n_subsample=n_subsample, n_total_sample=n_total_sample)
+        single_feature_fi_time = self.compute_expected_fi_time_single(
+            X_fi=X, model_predict_time=self.model_predict_time, n_subsample=n_subsample, n_total_sample=n_total_sample
+        )
         noise_threshold = len(prioritized) > 0
         features = sort_features_by_priority(features=features, prev_importance_df=prev_importance_df, using_prev_fit_fi=using_prev_fit_fi)
         if noise_threshold:
             features = list(prioritized) + [feature for feature in features if feature not in prioritized]
 
         # if we do not have enough time to evaluate feature importance for all features, do so only for some (first n_evaluated_features elements of features)
-        n_evaluated_features = max([i for i in range(0, n_features+1) if i * single_feature_fi_time + self.model_predict_time <= time_budget])
+        n_evaluated_features = max([i for i in range(0, n_features + 1) if i * single_feature_fi_time + self.model_predict_time <= time_budget])
         if n_evaluated_features == 0:
             prune_time = time.time() - time_start
             return features, unevaluated_fi_df_template(features), prune_time
         evaluated_features = features[:n_evaluated_features]
         unevaluated_features = features[n_evaluated_features:]
         time_budget_fi = time_budget - (time.time() - time_start)
         logger.log(15, f"\tComputing feature importance for {n_evaluated_features}/{n_features} features with {n_shuffle} shuffles.")
-        fi_kwargs = {'X': X, 'y': y, 'num_shuffle_sets': n_shuffle, 'subsample_size': n_subsample, 'features': evaluated_features,
-                     'time_limit': time_budget_fi, 'silent': True, 'random_state': self.rng.integers(low=0, high=1e5)}
-        fi_kwargs.update({'is_oof': True} if self.is_bagged else {})
+        fi_kwargs = {
+            "X": X,
+            "y": y,
+            "num_shuffle_sets": n_shuffle,
+            "subsample_size": n_subsample,
+            "features": evaluated_features,
+            "time_limit": time_budget_fi,
+            "silent": True,
+            "random_state": self.rng.integers(low=0, high=1e5),
+        }
+        fi_kwargs.update({"is_oof": True} if self.is_bagged else {})
         # FIXME: Right now the upper bound on the number of features we evaluate feature importance at once is determined by our expected feature
         # importance computation time. While this estimate is relatively accurate on most datasets, on some high dimensional datasets it underestimates
         # the time needed to evaluate n_shuffles of permutations and ends up only evaluating a few shuffles. Consider making a feature importance
         # method that parallelizes across individual shuffles instead.
         evaluated_df = model.compute_feature_importance(**fi_kwargs)
         if self.is_bagged:
             # If the bagged model includes 5 models and we evaluate a single permutation feature importance shuffle, the above method returns n=5 instead of 1.
-            evaluated_df['n'] = (evaluated_df['n'] // len(model.models)).clip(lower=1)
+            evaluated_df["n"] = (evaluated_df["n"] // len(model.models)).clip(lower=1)
 
         # if we could not compute feature importance for all features and previous feature importance estimates exist, use them
         importance_df = pd.concat([evaluated_df, unevaluated_fi_df_template(unevaluated_features)])
         importance_df = merge_importance_dfs(prev_importance_df, importance_df, using_prev_fit_fi)
 
         # if using noise threshold, threshold is the mean of noise column importance score
         if noise_threshold:
             noise_rows = importance_df[importance_df.index.isin(prioritized)]
             importance_df = importance_df.drop(prioritized)
-            prune_threshold = noise_rows['importance'].mean()
+            prune_threshold = noise_rows["importance"].mean()
 
         # use importance_df to generate next candidate features
-        candidate_features = self.compute_next_candidate_given_fi(importance_df=importance_df, prune_threshold=prune_threshold,
-                                                                  prune_ratio=prune_ratio, weighted=weighted)
+        candidate_features = self.compute_next_candidate_given_fi(
+            importance_df=importance_df, prune_threshold=prune_threshold, prune_ratio=prune_ratio, weighted=weighted
+        )
 
         # if noise columns exist, they should never be removed
         if noise_threshold:
             candidate_features = candidate_features + list(prioritized)
             importance_df = pd.concat([importance_df, noise_rows])
 
         feature_selection_time = time.time() - time_start
-        return candidate_features, importance_df.sort_values(by='importance', axis=0), feature_selection_time
+        return candidate_features, importance_df.sort_values(by="importance", axis=0), feature_selection_time
 
     def compute_next_candidate_given_fi(self, importance_df: pd.DataFrame, prune_threshold: float, prune_ratio: float, weighted: bool) -> List[str]:
         """
         Keep features whose importance scores are above threshold or have not yet had a chance to be calculated,
         as well as some features whose importance scores are below threshold if more than prune_ratio * num features
         features are below threshold. In the latter case, randomly sample without replacement from features whose
         importance scores are below threshold until removal candidate configuration that has not yet been tried
         is encountered. Give higher probability to features whose scores are lower than others when sampling.
         """
         n_remove = max(1, int(prune_ratio * len(importance_df)))
-        above_threshold_rows = importance_df[(importance_df['importance'] > prune_threshold) | (importance_df['importance'].isna())]
-        below_threshold_rows = importance_df[importance_df['importance'] <= prune_threshold].sort_values(by='importance', axis=0, ascending=True)
+        above_threshold_rows = importance_df[(importance_df["importance"] > prune_threshold) | (importance_df["importance"].isna())]
+        below_threshold_rows = importance_df[importance_df["importance"] <= prune_threshold].sort_values(by="importance", axis=0, ascending=True)
         logger.log(15, f"\tNumber of identified features below prune threshold {round(prune_threshold, 4)}: {len(below_threshold_rows)}/{len(importance_df)}")
         if len(below_threshold_rows) <= n_remove:
             acceptance_candidates = above_threshold_rows.index.tolist()
             self.attempted_removals.add(tuple(below_threshold_rows.index))
             return acceptance_candidates
 
         # Try removing features with lowest importance first
         removal_candidate_rows = below_threshold_rows[:n_remove]
         removal_candidates = tuple(removal_candidate_rows.index)
         if removal_candidates not in self.attempted_removals:
             acceptance_candidates = importance_df[~importance_df.index.isin(removal_candidates)].index.tolist()
             self.attempted_removals.add(removal_candidates)
             return acceptance_candidates
 
-        sample_weights = [1/i for i in range(1, len(below_threshold_rows)+1)] if weighted else None
+        sample_weights = [1 / i for i in range(1, len(below_threshold_rows) + 1)] if weighted else None
         for _ in range(50):
             random_state = self.rng.integers(low=0, high=1e5)
             removal_candidate_rows = below_threshold_rows.sample(n=n_remove, random_state=random_state, replace=False, weights=sample_weights)
             removal_candidates = tuple(removal_candidate_rows.index)
             if removal_candidates not in self.attempted_removals:
                 acceptance_candidates = importance_df[~importance_df.index.isin(removal_candidates)].index.tolist()
                 self.attempted_removals.add(removal_candidates)
@@ -418,94 +479,97 @@
         return model_predict_time * ((n_subsample / len(X_fi)) * n_shuffle)
 
     def compute_time_budget_fi(self, X_fi: pd.DataFrame, n_subsample: int, **kwargs):
         """
         Return the time that a single feature importance computation round can take up to. Currently the time it
         takes to fully evaluated minimum of 50 features or the number of features in the dataset.
         """
-        min_fi_samples = kwargs.get('min_fi_samples', 10000)
-        max_fi_samples = kwargs.get('max_fi_samples', 50000)
+        min_fi_samples = kwargs.get("min_fi_samples", 10000)
+        max_fi_samples = kwargs.get("max_fi_samples", 50000)
         n_total_samples = max(min_fi_samples, min(max_fi_samples, len(X_fi)))
         baseline_time = self.model_predict_time
-        fi_time_single = self.compute_expected_fi_time_single(X_fi=X_fi, model_predict_time=self.model_predict_time,
-                                                              n_subsample=n_subsample, n_total_sample=n_total_samples)
+        fi_time_single = self.compute_expected_fi_time_single(
+            X_fi=X_fi, model_predict_time=self.model_predict_time, n_subsample=n_subsample, n_total_sample=n_total_samples
+        )
         return fi_time_single * min(len(X_fi.columns), 50) + baseline_time
 
-    def fit_score_model(self, X: pd.DataFrame, y: pd.Series, X_val: pd.DataFrame, y_val: pd.Series,
-                        features: List[str], model_name: str, **kwargs) -> Tuple[AbstractModel, float, float]:
+    def fit_score_model(
+        self, X: pd.DataFrame, y: pd.Series, X_val: pd.DataFrame, y_val: pd.Series, features: List[str], model_name: str, **kwargs
+    ) -> Tuple[AbstractModel, float, float]:
         """
         Fits and scores a model over the given feature subset (ex. features remaining in a particular feature pruning round).
         Returns the fitted model, its score, and time elapsed. If this is the first time we are fitting a model in the pruning
         procedure, save time and score statistics.
         """
         time_start = time.time()
         model = self.model_class(**self.model_params)
         if self.replace_bag:
             model = model.convert_to_template_child()
         model.rename(model_name)
         X = X[features]
         X_val = None if self.is_bagged else X_val[features]
-        if 'time_limit' in kwargs:
+        if "time_limit" in kwargs:
             time_remaining = self.time_limit - (time.time() - self.time_start)
-            kwargs['time_limit'] = time_remaining
+            kwargs["time_limit"] = time_remaining
         model.fit(X=X, y=y, X_val=X_val, y_val=y_val, **kwargs)
         time_fit = time.time() - time_start
         score = model.score_with_oof(y) if self.is_bagged else model.score(X=X_val, y=y_val)
         time_fit_score = time.time() - time_start
         if self.fit_score_time is None:
             self.fit_score_time = time_fit_score
         if self.model_predict_time is None:
             self.model_predict_time = model.predict_time if self.is_bagged else time_fit_score - time_fit
         return model, score, time_fit_score
 
     def get_extra_fn_args(self, **kwargs) -> dict:
         return {
-            'weighted': kwargs.get('weighted', True),
-            'min_fi_samples': kwargs.get('min_fi_samples', 10000),
-            'max_fi_samples': kwargs.get('max_fi_samples', 50000),
+            "weighted": kwargs.get("weighted", True),
+            "min_fi_samples": kwargs.get("min_fi_samples", 10000),
+            "max_fi_samples": kwargs.get("max_fi_samples", 50000),
         }
 
-    def setup(self, X: pd.DataFrame, y: pd.DataFrame, X_val: pd.DataFrame, y_val: pd.DataFrame, n_train_subsample: int, prune_threshold: float,
-              **kwargs: dict) -> Tuple[pd.DataFrame, pd.Series, pd.DataFrame, pd.Series, pd.DataFrame, pd.Series, Union[float, str], List[str]]:
+    def setup(
+        self, X: pd.DataFrame, y: pd.DataFrame, X_val: pd.DataFrame, y_val: pd.DataFrame, n_train_subsample: int, prune_threshold: float, **kwargs: dict
+    ) -> Tuple[pd.DataFrame, pd.Series, pd.DataFrame, pd.Series, pd.DataFrame, pd.Series, Union[float, str], List[str]]:
         """
         Modify training data, validation data, and model fit kwargs appropriately by subsampling, adding noise columns, replacing bagged
         models, and more.
         """
         # subsample training data
-        min_fi_samples = kwargs.get('min_fi_samples', 10000)
+        min_fi_samples = kwargs.get("min_fi_samples", 10000)
         random_state = self.rng.integers(low=0, high=1e5)
         if n_train_subsample is not None and len(X) > n_train_subsample:
             logger.log(20, f"\tNumber of training samples {len(X)} is greater than {n_train_subsample}. Using {n_train_subsample} samples as training data.")
-            drop_ratio = 1. - n_train_subsample / len(X)
+            drop_ratio = 1.0 - n_train_subsample / len(X)
             X_train, _, y_train, _ = generate_train_test_split(X=X, y=y, problem_type=self.problem_type, random_state=random_state, test_size=drop_ratio)
         else:
             X_train, y_train = X, y
 
         # replace bagged model with its child model for the proxy model if replace_bag=True (overrides subsampling if triggered)
         if n_train_subsample is None:
-            trigger_replace_bag = kwargs.get('replace_bag', False) and self.is_bagged
+            trigger_replace_bag = kwargs.get("replace_bag", False) and self.is_bagged
         else:
-            trigger_replace_bag = kwargs.get('replace_bag', True) and self.is_bagged and len(X) > n_train_subsample + min_fi_samples
+            trigger_replace_bag = kwargs.get("replace_bag", True) and self.is_bagged and len(X) > n_train_subsample + min_fi_samples
         if trigger_replace_bag:
             logger.log(20, f"\tFeature selection model is bagged and replace_bag=True. Using a non-bagged version of the model for feature selection.")
-            val_ratio = 1. - n_train_subsample / len(X) if n_train_subsample is not None else 0.25
+            val_ratio = 1.0 - n_train_subsample / len(X) if n_train_subsample is not None else 0.25
             X_train, X_val, y_train, y_val = generate_train_test_split(X=X, y=y, problem_type=self.problem_type, random_state=random_state, test_size=val_ratio)
             self.is_bagged = False
             self.replace_bag = True
 
         # Be more lenient with feature importance computation shuffles for very high dimensional datasets for time's sake
         if len(X_train.columns) > 1000:
             self.max_n_shuffle = self.max_n_shuffle // 2
 
         # set prune_threshold and optionally modify feature_metadata
         noise_columns = []
-        feature_metadata = deepcopy(kwargs.get('feature_metadata', None))
-        if prune_threshold == 'none':
-            prune_threshold = float('inf')
-        elif prune_threshold == 'noise':
+        feature_metadata = deepcopy(kwargs.get("feature_metadata", None))
+        if prune_threshold == "none":
+            prune_threshold = float("inf")
+        elif prune_threshold == "noise":
             X_train, noise_columns = add_noise_column(X=X_train, rng=self.rng)
             if feature_metadata is not None:
                 for noise_column in noise_columns:
                     feature_metadata.type_map_raw[noise_column] = R_FLOAT
             if isinstance(X_val, pd.DataFrame):
                 X_val, _ = add_noise_column(X=X_val, rng=self.rng, noise_columns=noise_columns)
         else:
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/files.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/files.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import contextlib
+import hashlib
+import logging
 import os
-from pathlib import Path
 import shutil
-import hashlib
+import tempfile
 import zipfile
-import logging
+from pathlib import Path
+
 from tqdm import tqdm
-import tempfile
 
 logger = logging.getLogger(__name__)
 
-__all__ = ['unzip', 'download']
+__all__ = ["unzip", "download"]
 
 
-def unzip(zip_file_path, root=os.path.expanduser('./')):
-    """Unzips files located at `zip_file_path` into parent directory specified by `root`.
-    """
+def unzip(zip_file_path, root=os.path.expanduser("./")):
+    """Unzips files located at `zip_file_path` into parent directory specified by `root`."""
     folders = []
     with zipfile.ZipFile(zip_file_path) as zf:
         zf.extractall(root)
         for name in zf.namelist():
             folder = Path(name).parts[0]
             if folder not in folders:
                 folders.append(folder)
@@ -45,50 +45,51 @@
 
     Returns
     -------
     str
         The file path of the downloaded file.
     """
     if path is None:
-        fname = url.split('/')[-1]
+        fname = url.split("/")[-1]
     else:
         path = os.path.expanduser(path)
         if os.path.isdir(path):
-            fname = os.path.join(path, url.split('/')[-1])
+            fname = os.path.join(path, url.split("/")[-1])
         else:
             fname = path
 
     if overwrite or not os.path.exists(fname) or (sha1_hash and not check_sha1(fname, sha1_hash)):
         import requests
+
         dirname = os.path.dirname(os.path.abspath(os.path.expanduser(fname)))
         if not os.path.exists(dirname):
             os.makedirs(dirname)
 
-        logger.info('Downloading %s from %s...'%(fname, url))
+        logger.info("Downloading %s from %s..." % (fname, url))
         r = requests.get(url, stream=True)
         if r.status_code != 200:
-            raise RuntimeError("Failed downloading url %s"%url)
-        total_length = r.headers.get('content-length')
-        with open(fname, 'wb') as f:
-            if total_length is None: # no content length header
+            raise RuntimeError("Failed downloading url %s" % url)
+        total_length = r.headers.get("content-length")
+        with open(fname, "wb") as f:
+            if total_length is None:  # no content length header
                 for chunk in r.iter_content(chunk_size=1024):
-                    if chunk: # filter out keep-alive new chunks
+                    if chunk:  # filter out keep-alive new chunks
                         f.write(chunk)
             else:
                 total_length = int(total_length)
-                for chunk in tqdm(r.iter_content(chunk_size=1024),
-                                  total=int(total_length / 1024. + 0.5),
-                                  unit='KB', unit_scale=False, dynamic_ncols=True):
+                for chunk in tqdm(r.iter_content(chunk_size=1024), total=int(total_length / 1024.0 + 0.5), unit="KB", unit_scale=False, dynamic_ncols=True):
                     f.write(chunk)
 
         if sha1_hash and not check_sha1(fname, sha1_hash):
-            raise UserWarning('File {} is downloaded but the content hash does not match. ' \
-                              'The repo may be outdated or download may be incomplete. ' \
-                              'If the "repo_url" is overridden, consider switching to ' \
-                              'the default repo.'.format(fname))
+            raise UserWarning(
+                "File {} is downloaded but the content hash does not match. "
+                "The repo may be outdated or download may be incomplete. "
+                'If the "repo_url" is overridden, consider switching to '
+                "the default repo.".format(fname)
+            )
 
     return fname
 
 
 def check_sha1(filename, sha1_hash):
     """Check whether the sha1 hash of the file content matches the expected hash.
 
@@ -101,15 +102,15 @@
 
     Returns
     -------
     bool
         Whether the file content matches the expected hash.
     """
     sha1 = hashlib.sha1()
-    with open(filename, 'rb') as f:
+    with open(filename, "rb") as f:
         while True:
             data = f.read(1048576)
             if not data:
                 break
             sha1.update(data)
 
     return sha1.hexdigest() == sha1_hash
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/infer_utils.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/infer_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,11 @@
 import pandas as pd
 
 
-def get_model_true_infer_speed_per_row_batch(
-        data,
-        *,
-        predictor,
-        batch_size: int = 100000,
-        repeats=1,
-        persist_models=True,
-        silent=False):
+def get_model_true_infer_speed_per_row_batch(data, *, predictor, batch_size: int = 100000, repeats=1, persist_models=True, silent=False):
     """
     Get per-model true inference speed per row for a given batch size of data.
 
     Parameters
     ----------
     data : :class:`TabularDataset` or :class:`pd.DataFrame`
         Table of the data, which is similar to a pandas DataFrame.
@@ -36,16 +29,18 @@
             'pred_time_test_with_transform' is the end-to-end prediction time per row in seconds if calling `predictor.predict(data, model=model)`
             'pred_time_test' is the end-to-end prediction time per row in seconds minus the global feature preprocessing time.
             'pred_time_test_marginal' is the prediction time needed to predict for this particular model minus dependent model inference times and global preprocessing time.
         time_per_row_transform is the time in seconds per row to do the feature preprocessing.
     """
     import copy
     import time
+
     import numpy as np
     import pandas as pd
+
     data_batch = copy.deepcopy(data)
     len_data = len(data_batch)
     if len_data == batch_size:
         pass
     elif len_data < batch_size:
         # add more rows
         duplicate_count = int(np.ceil(batch_size / len_data))
@@ -53,70 +48,65 @@
         len_data = len(data_batch)
     if len_data > batch_size:
         # sample rows
         data_batch = data_batch.sample(n=batch_size, random_state=0)
         len_data = len(data_batch)
 
     if len_data != batch_size:
-        raise AssertionError(f'len(data_batch) must equal batch_size! ({len_data} != {batch_size})')
+        raise AssertionError(f"len(data_batch) must equal batch_size! ({len_data} != {batch_size})")
 
     if persist_models:
-        predictor.persist_models(models='all')
+        predictor.persist_models(models="all")
 
     ts = time.time()
     for i in range(repeats):
         predictor.transform_features(data_batch)
     time_transform = (time.time() - ts) / repeats
 
     leaderboards = []
     for i in range(repeats):
         leaderboard = predictor.leaderboard(data_batch, skip_score=True, silent=True)
-        leaderboard = leaderboard[leaderboard['can_infer']][['model', 'pred_time_test', 'pred_time_test_marginal']]
-        leaderboard = leaderboard.set_index('model')
+        leaderboard = leaderboard[leaderboard["can_infer"]][["model", "pred_time_test", "pred_time_test_marginal"]]
+        leaderboard = leaderboard.set_index("model")
         leaderboards.append(leaderboard)
     leaderboard = pd.concat(leaderboards)
     time_per_batch_df = leaderboard.groupby(level=0).mean()
-    time_per_batch_df['pred_time_test_with_transform'] = time_per_batch_df['pred_time_test'] + time_transform
+    time_per_batch_df["pred_time_test_with_transform"] = time_per_batch_df["pred_time_test"] + time_transform
     time_per_row_df = time_per_batch_df / batch_size
     time_per_row_transform = time_transform / batch_size
 
     if not silent:
-        print(f'Throughput for batch_size={batch_size}:')
+        print(f"Throughput for batch_size={batch_size}:")
         for index, row in time_per_row_df.iterrows():
-            time_per_row = row['pred_time_test_with_transform']
+            time_per_row = row["pred_time_test_with_transform"]
             time_per_row_print = time_per_row
-            unit = 's'
+            unit = "s"
             if time_per_row_print < 1e-2:
                 time_per_row_print *= 1000
-                unit = 'ms'
+                unit = "ms"
                 if time_per_row_print < 1e-2:
                     time_per_row_print *= 1000
-                    unit = 'μs'
+                    unit = "μs"
             print(f"\t{round(time_per_row_print, 3)}{unit} per row | {index}")
         time_per_row_transform_print = time_per_row_transform
-        unit = 's'
+        unit = "s"
         if time_per_row_transform_print < 1e-2:
             time_per_row_transform_print *= 1000
-            unit = 'ms'
+            unit = "ms"
             if time_per_row_transform_print < 1e-2:
                 time_per_row_transform_print *= 1000
-                unit = 'μs'
+                unit = "μs"
         print(f"\t{round(time_per_row_transform_print, 3)}{unit} per row | transform_features")
 
     return time_per_row_df, time_per_row_transform
 
 
-def get_model_true_infer_speed_per_row_batch_bulk(data: pd.DataFrame,
-                                                  *,
-                                                  predictor,
-                                                  batch_sizes: list = None,
-                                                  repeats=1,
-                                                  persist_models=True,
-                                                  include_transform_features=False,
-                                                  silent=False) -> (pd.DataFrame, pd.DataFrame):
+def get_model_true_infer_speed_per_row_batch_bulk(
+    data: pd.DataFrame, *, predictor, batch_sizes: list = None, repeats=1, persist_models=True, include_transform_features=False, silent=False
+) -> (pd.DataFrame, pd.DataFrame):
     """
     Get per-model true inference speed per row for a list of batch sizes of data.
 
     Parameters
     ----------
     data : :class:`TabularDataset` or :class:`pd.DataFrame`
         Table of the data, which is similar to a pandas DataFrame.
@@ -156,38 +146,35 @@
             1000,
             10000,
         ]
     infer_dfs = dict()
     infer_transform_dfs = dict()
 
     if persist_models:
-        predictor.persist_models(models='all')
+        predictor.persist_models(models="all")
 
     for batch_size in batch_sizes:
-        infer_df, time_per_row_transform = get_model_true_infer_speed_per_row_batch(data=data,
-                                                                                    predictor=predictor,
-                                                                                    batch_size=batch_size,
-                                                                                    repeats=repeats,
-                                                                                    persist_models=False,
-                                                                                    silent=silent)
+        infer_df, time_per_row_transform = get_model_true_infer_speed_per_row_batch(
+            data=data, predictor=predictor, batch_size=batch_size, repeats=repeats, persist_models=False, silent=silent
+        )
         infer_dfs[batch_size] = infer_df
         infer_transform_dfs[batch_size] = time_per_row_transform
     for key in infer_dfs.keys():
         infer_dfs[key] = infer_dfs[key].reset_index()
-        infer_dfs[key]['batch_size'] = key
+        infer_dfs[key]["batch_size"] = key
 
-    infer_df_full_transform = pd.Series(infer_transform_dfs, name='pred_time_test').to_frame().rename_axis('batch_size')
-    infer_df_full_transform['pred_time_test_marginal'] = infer_df_full_transform['pred_time_test']
-    infer_df_full_transform['pred_time_test_with_transform'] = infer_df_full_transform['pred_time_test']
+    infer_df_full_transform = pd.Series(infer_transform_dfs, name="pred_time_test").to_frame().rename_axis("batch_size")
+    infer_df_full_transform["pred_time_test_marginal"] = infer_df_full_transform["pred_time_test"]
+    infer_df_full_transform["pred_time_test_with_transform"] = infer_df_full_transform["pred_time_test"]
     infer_df_full_transform = infer_df_full_transform.reset_index()
 
     infer_df_full = pd.concat([infer_dfs[key] for key in infer_dfs.keys()])
 
     if include_transform_features:
         infer_df_full_transform_include = infer_df_full_transform.copy()
-        infer_df_full_transform_include['model'] = 'transform_features'
+        infer_df_full_transform_include["model"] = "transform_features"
         infer_df_full = pd.concat([infer_df_full, infer_df_full_transform_include])
 
-    infer_df_full = infer_df_full.sort_values(by=['batch_size'])
+    infer_df_full = infer_df_full.sort_values(by=["batch_size"])
     infer_df_full = infer_df_full.reset_index(drop=True)
 
     return infer_df_full, infer_df_full_transform
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/miscs.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/miscs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import warnings
 
-__all__ = ['in_ipynb', 'warning_filter']
+__all__ = ["in_ipynb", "warning_filter"]
 
 
 def in_ipynb():
-    if 'AG_DOCS' in os.environ and os.environ['AG_DOCS']:
+    if "AG_DOCS" in os.environ and os.environ["AG_DOCS"]:
         return False
     try:
-        cfg = get_ipython().config 
-        if 'IPKernelApp' in cfg:
+        cfg = get_ipython().config
+        if "IPKernelApp" in cfg:
             return True
         else:
             return False
     except NameError:
         return False
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/plots.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/plots.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,218 +1,266 @@
 """ Methods to create various plots used throughout AutoGluon.
     If matplotlib or bokeh are not installed, simply will print warning message that plots cannot be shown.
 """
 
-import warnings, os
-import numpy as np
+import os
+import warnings
 from collections import OrderedDict
 
+import numpy as np
+
 from .miscs import warning_filter
 
-__all__ = ['plot_performance_vs_trials', 'plot_summary_of_models', 'plot_tabular_models', 'mousover_plot']
+__all__ = ["plot_performance_vs_trials", "plot_summary_of_models", "plot_tabular_models", "mousover_plot"]
 
 
 def plot_performance_vs_trials(results, output_directory, save_file="PerformanceVsTrials.png", plot_title="", show_plot=True):
     try:
         import matplotlib.pyplot as plt
+
         matplotlib_imported = True
     except ImportError:
         matplotlib_imported = False
-    
+
     if not matplotlib_imported:
         warnings.warn('AutoGluon summary plots cannot be created because matplotlib is not installed. Please do: "pip install matplotlib"')
         return None
-    
-    ordered_trials = sorted(list(results['trial_info'].keys()))
-    ordered_val_perfs = [results['trial_info'][trial_id][results['reward_attr']] for trial_id in ordered_trials]
-    x = range(1, len(ordered_trials)+1)
+
+    ordered_trials = sorted(list(results["trial_info"].keys()))
+    ordered_val_perfs = [results["trial_info"][trial_id][results["reward_attr"]] for trial_id in ordered_trials]
+    x = range(1, len(ordered_trials) + 1)
     y = []
     for i in x:
-        y.append(max([ordered_val_perfs[j] for j in range(i)])) # best validation performance in trials up until ith one (assuming higher = better)
+        y.append(max([ordered_val_perfs[j] for j in range(i)]))  # best validation performance in trials up until ith one (assuming higher = better)
     fig, ax = plt.subplots()
     ax.plot(x, y)
-    ax.set(xlabel='Completed Trials', ylabel='Best Performance', title = plot_title)
+    ax.set(xlabel="Completed Trials", ylabel="Best Performance", title=plot_title)
     if output_directory is not None:
         outputfile = os.path.join(output_directory, save_file)
         fig.savefig(outputfile)
         print("Plot of HPO performance saved to file: %s" % outputfile)
     if show_plot:
         plt.show()
 
 
-def plot_summary_of_models(results, output_directory, save_file='SummaryOfModels.html', plot_title="Models produced during fit()", show_plot=True):
-    """ Plot dynamic scatterplot summary of each model encountered during fit(), based on the returned Results object. 
-    """
-    num_trials = len(results['trial_info'])
+def plot_summary_of_models(results, output_directory, save_file="SummaryOfModels.html", plot_title="Models produced during fit()", show_plot=True):
+    """Plot dynamic scatterplot summary of each model encountered during fit(), based on the returned Results object."""
+    num_trials = len(results["trial_info"])
     attr_color = None
     attr_size = None
-    datadict = {'trial_id': sorted(results['trial_info'].keys())}
-    datadict['performance'] = [results['trial_info'][trial_id][results['reward_attr']] for trial_id in datadict['trial_id']]
-    datadict['hyperparameters'] = [_formatDict(results['trial_info'][trial_id]['config']) for trial_id in datadict['trial_id']]
+    datadict = {"trial_id": sorted(results["trial_info"].keys())}
+    datadict["performance"] = [results["trial_info"][trial_id][results["reward_attr"]] for trial_id in datadict["trial_id"]]
+    datadict["hyperparameters"] = [_formatDict(results["trial_info"][trial_id]["config"]) for trial_id in datadict["trial_id"]]
     hidden_keys = []
     # Determine x-axis attribute:
-    if 'latency' in results['metadata']:
-        datadict['latency'] = [results['trial_info'][trial_id]['metadata']['latency'] for trial_id in datadict['trial_id']]
-        attr_x = 'latency'
+    if "latency" in results["metadata"]:
+        datadict["latency"] = [results["trial_info"][trial_id]["metadata"]["latency"] for trial_id in datadict["trial_id"]]
+        attr_x = "latency"
     else:
-        attr_x = list(results['best_config'].keys())[0]
-        datadict[attr_x] = [results['trial_info'][trial_id]['config'][attr_x] for trial_id in datadict['trial_id']]
+        attr_x = list(results["best_config"].keys())[0]
+        datadict[attr_x] = [results["trial_info"][trial_id]["config"][attr_x] for trial_id in datadict["trial_id"]]
         hidden_keys.append(attr_x)
     # Determine size attribute:
-    if 'memory' in results['metadata']:
-        datadict['memory'] = [results['trial_info'][trial_id]['metadata']['memory'] for trial_id in datadict['trial_id']]
-        attr_size = 'memory'
-    
+    if "memory" in results["metadata"]:
+        datadict["memory"] = [results["trial_info"][trial_id]["metadata"]["memory"] for trial_id in datadict["trial_id"]]
+        attr_size = "memory"
+
     # Determine color attribute:
-    if 'training_loss' in results:
-        datadict['training_loss'] = [results['trial_info'][trial_id]['training_loss'] for trial_id in datadict['trial_id']]
-        attr_color = 'training_loss'
+    if "training_loss" in results:
+        datadict["training_loss"] = [results["trial_info"][trial_id]["training_loss"] for trial_id in datadict["trial_id"]]
+        attr_color = "training_loss"
 
     save_path = os.path.join(output_directory, save_file) if output_directory else None
-    mousover_plot(datadict, attr_x=attr_x, attr_y='performance', attr_color=attr_color, 
-                  attr_size=attr_size, save_file=save_path, plot_title=plot_title, hidden_keys=hidden_keys, show_plot=show_plot)
+    mousover_plot(
+        datadict,
+        attr_x=attr_x,
+        attr_y="performance",
+        attr_color=attr_color,
+        attr_size=attr_size,
+        save_file=save_path,
+        plot_title=plot_title,
+        hidden_keys=hidden_keys,
+        show_plot=show_plot,
+    )
     if save_path is not None:
         print("Plot summary of models saved to file: %s" % save_file)
 
 
 def plot_tabular_models(results, output_directory=None, save_file="SummaryOfModels.html", plot_title="Models produced during fit()", show_plot=True):
-    """ Plot dynamic scatterplot of every single model trained during tabular_prediction.fit()
-        Args:
-            results: 
-                Dict created during TabularPredictor.fit_summary().
-                Must at least contain key: 'model_performance'.
+    """Plot dynamic scatterplot of every single model trained during tabular_prediction.fit()
+    Args:
+        results:
+            Dict created during TabularPredictor.fit_summary().
+            Must at least contain key: 'model_performance'.
     """
     save_path = output_directory + save_file if output_directory else None
     hidden_keys = []
-    model_performancedict = results['model_performance']
+    model_performancedict = results["model_performance"]
     model_names = list(model_performancedict.keys())
     val_perfs = [model_performancedict[key] for key in model_names]
-    model_types = [results['model_types'][key] for key in model_names]
+    model_types = [results["model_types"][key] for key in model_names]
     hidden_keys.append(model_types)
-    model_hyperparams = [_formatDict(results['model_hyperparams'][key]) for key in model_names]
-    datadict = {'performance': val_perfs, 'model': model_names, 'model_type': model_types, 'hyperparameters': model_hyperparams}
-    leaderboard = results['leaderboard'].copy()
-    leaderboard['fit_time'] = leaderboard['fit_time'].fillna(0)
-    leaderboard['pred_time_val'] = leaderboard['pred_time_val'].fillna(0)
-
-    datadict['inference_latency'] = [leaderboard['pred_time_val'][leaderboard['model'] == m].values[0] for m in model_names]
-    datadict['training_time'] = [leaderboard['fit_time'][leaderboard['model'] == m].values[0] for m in model_names]
-    mousover_plot(datadict, attr_x='inference_latency', attr_y='performance', attr_color='model_type',
-                  save_file=save_path, plot_title=plot_title, hidden_keys=hidden_keys, show_plot=show_plot)
+    model_hyperparams = [_formatDict(results["model_hyperparams"][key]) for key in model_names]
+    datadict = {"performance": val_perfs, "model": model_names, "model_type": model_types, "hyperparameters": model_hyperparams}
+    leaderboard = results["leaderboard"].copy()
+    leaderboard["fit_time"] = leaderboard["fit_time"].fillna(0)
+    leaderboard["pred_time_val"] = leaderboard["pred_time_val"].fillna(0)
+
+    datadict["inference_latency"] = [leaderboard["pred_time_val"][leaderboard["model"] == m].values[0] for m in model_names]
+    datadict["training_time"] = [leaderboard["fit_time"][leaderboard["model"] == m].values[0] for m in model_names]
+    mousover_plot(
+        datadict,
+        attr_x="inference_latency",
+        attr_y="performance",
+        attr_color="model_type",
+        save_file=save_path,
+        plot_title=plot_title,
+        hidden_keys=hidden_keys,
+        show_plot=show_plot,
+    )
 
 
 def _formatDict(d):
-    """ Returns dict as string with HTML new-line tags <br> between key-value pairs. """
-    s = ''
+    """Returns dict as string with HTML new-line tags <br> between key-value pairs."""
+    s = ""
     for key in d:
         new_s = str(key) + ": " + str(d[key]) + "<br>"
         s += new_s
     return s[:-4]
 
 
-def mousover_plot(datadict, attr_x, attr_y, attr_color=None, attr_size=None, save_file=None, plot_title="",
-                  point_transparency = 0.5, point_size=20, default_color="#2222aa", hidden_keys = [], show_plot=False):
-    """ Produces dynamic scatter plot that can be interacted with by mousing over each point to see its label
-        Args:
-            datadict (dict): keys contain attributes, values of lists of data from each attribute to plot (each list index corresponds to datapoint).
-                             The values of all extra keys in this dict are considered (string) labels to assign to datapoints when they are moused over.
-                             Apply _formatDict() to any entries in datadict which are themselves dicts.
-            attr_x (str): name of column in dataframe whose values are shown on x-axis (eg. 'latency'). Can be categorical or numeric values
-            attr_y (str): name of column in dataframe whose values are shown on y-axis (eg. 'validation performance'). Must be numeric values.
-            attr_size (str): name of column in dataframe whose values determine size of dots (eg. 'memory consumption'). Must be numeric values.
-            attr_color (str): name of column in dataframe whose values determine color of dots  (eg. one of the hyperparameters). Can be categorical or numeric values
-            point_labels (list): list of strings describing the label for each dot (must be in same order as rows of dataframe)
-            save_file (str): where to save plot to (html) file (if None, plot is not saved)
-            plot_title (str): Title of plot and html file
-            point_transparency (float): alpha value of points, lower = more transparent
-            point_size (int): size of points, higher = larger
-            hidden keys (list[str]): which keys of datadict NOT to show labels for.
-            show_plot (bool): whether to show plot
+def mousover_plot(
+    datadict,
+    attr_x,
+    attr_y,
+    attr_color=None,
+    attr_size=None,
+    save_file=None,
+    plot_title="",
+    point_transparency=0.5,
+    point_size=20,
+    default_color="#2222aa",
+    hidden_keys=[],
+    show_plot=False,
+):
+    """Produces dynamic scatter plot that can be interacted with by mousing over each point to see its label
+    Args:
+        datadict (dict): keys contain attributes, values of lists of data from each attribute to plot (each list index corresponds to datapoint).
+                         The values of all extra keys in this dict are considered (string) labels to assign to datapoints when they are moused over.
+                         Apply _formatDict() to any entries in datadict which are themselves dicts.
+        attr_x (str): name of column in dataframe whose values are shown on x-axis (eg. 'latency'). Can be categorical or numeric values
+        attr_y (str): name of column in dataframe whose values are shown on y-axis (eg. 'validation performance'). Must be numeric values.
+        attr_size (str): name of column in dataframe whose values determine size of dots (eg. 'memory consumption'). Must be numeric values.
+        attr_color (str): name of column in dataframe whose values determine color of dots  (eg. one of the hyperparameters). Can be categorical or numeric values
+        point_labels (list): list of strings describing the label for each dot (must be in same order as rows of dataframe)
+        save_file (str): where to save plot to (html) file (if None, plot is not saved)
+        plot_title (str): Title of plot and html file
+        point_transparency (float): alpha value of points, lower = more transparent
+        point_size (int): size of points, higher = larger
+        hidden keys (list[str]): which keys of datadict NOT to show labels for.
+        show_plot (bool): whether to show plot
     """
     try:
         with warning_filter():
             import bokeh
-            from bokeh.plotting import output_file, ColumnDataSource, show, figure, save
-            from bokeh.models import HoverTool, CategoricalColorMapper, LinearColorMapper, Legend, LegendItem, ColorBar
+            from bokeh.models import CategoricalColorMapper, ColorBar, HoverTool, Legend, LegendItem, LinearColorMapper
             from bokeh.palettes import Category20
+            from bokeh.plotting import ColumnDataSource, figure, output_file, save, show
     except ImportError:
         warnings.warn('AutoGluon summary plots cannot be created because bokeh is not installed. To see plots, please do: "pip install bokeh==2.0.1"')
         return None
 
     n = len(datadict[attr_x])
     for key in datadict.keys():  # Check lengths are all the same
         if len(datadict[key]) != n:
             raise ValueError("Key %s in datadict has different length than %s" % (key, attr_x))
 
-    attr_x_is_string = any([type(val)==str for val in datadict[attr_x]])
+    attr_x_is_string = any([type(val) == str for val in datadict[attr_x]])
     if attr_x_is_string:
         attr_x_levels = list(set(datadict[attr_x]))  # use this to translate between int-indices and x-values
         og_x_vals = datadict[attr_x][:]
         attr_x2 = attr_x + "___"  # this key must not already be in datadict.
         hidden_keys.append(attr_x2)
-        datadict[attr_x2] = [attr_x_levels.index(category) for category in og_x_vals] # convert to ints
+        datadict[attr_x2] = [attr_x_levels.index(category) for category in og_x_vals]  # convert to ints
 
     legend = None
     if attr_color is not None:
         attr_color_is_string = any([type(val) == str for val in datadict[attr_color]])
         color_datavals = datadict[attr_color]
         if attr_color_is_string:
             attr_color_levels = list(set(color_datavals))
             colorpalette = Category20[20]
-            color_mapper = CategoricalColorMapper(factors=attr_color_levels, palette=[colorpalette[2*i % len(colorpalette)] for i in range(len(attr_color_levels))])
+            color_mapper = CategoricalColorMapper(
+                factors=attr_color_levels, palette=[colorpalette[2 * i % len(colorpalette)] for i in range(len(attr_color_levels))]
+            )
             legend = attr_color
         else:
-            color_mapper = LinearColorMapper(palette='Magma256', low=min(datadict[attr_color]), high=max(datadict[attr_color])*1.25)
-        default_color = {'field': attr_color, 'transform': color_mapper}
+            color_mapper = LinearColorMapper(palette="Magma256", low=min(datadict[attr_color]), high=max(datadict[attr_color]) * 1.25)
+        default_color = {"field": attr_color, "transform": color_mapper}
 
     if attr_size is not None:  # different size for each point, ensure mean-size == point_size
         attr_size2 = attr_size + "____"
         hidden_keys.append(attr_size2)
         og_sizevals = np.array(datadict[attr_size])
-        sizevals = point_size + (og_sizevals - np.mean(og_sizevals))/np.std(og_sizevals) * (point_size/2)
+        sizevals = point_size + (og_sizevals - np.mean(og_sizevals)) / np.std(og_sizevals) * (point_size / 2)
         if np.min(sizevals) < 0:
             sizevals = -np.min(sizevals) + sizevals + 1.0
         datadict[attr_size2] = list(sizevals)
         point_size = attr_size2
 
     if save_file is not None:
         output_file(save_file, title=plot_title)
         print("Plot summary of models saved to file: %s" % save_file)
 
     source = ColumnDataSource(datadict)
-    TOOLS="crosshair,pan,wheel_zoom,box_zoom,reset,hover,save"
+    TOOLS = "crosshair,pan,wheel_zoom,box_zoom,reset,hover,save"
     p = figure(title=plot_title, tools=TOOLS)
     if attr_x_is_string:
-        circ = p.circle(attr_x2, attr_y, line_color=default_color, line_alpha = point_transparency,
-                        fill_color=default_color, fill_alpha=point_transparency, size=point_size, source=source)
+        circ = p.circle(
+            attr_x2,
+            attr_y,
+            line_color=default_color,
+            line_alpha=point_transparency,
+            fill_color=default_color,
+            fill_alpha=point_transparency,
+            size=point_size,
+            source=source,
+        )
     else:
-        circ = p.circle(attr_x, attr_y, line_color=default_color, line_alpha = point_transparency,
-                        fill_color=default_color, fill_alpha=point_transparency, size=point_size, source=source)
+        circ = p.circle(
+            attr_x,
+            attr_y,
+            line_color=default_color,
+            line_alpha=point_transparency,
+            fill_color=default_color,
+            fill_alpha=point_transparency,
+            size=point_size,
+            source=source,
+        )
     hover = p.select(dict(type=HoverTool))
-    hover.tooltips = OrderedDict([(key,'@'+key+'{safe}') for key in datadict.keys() if key not in hidden_keys])
+    hover.tooltips = OrderedDict([(key, "@" + key + "{safe}") for key in datadict.keys() if key not in hidden_keys])
     # Format axes:
     p.xaxis.axis_label = attr_x
     p.yaxis.axis_label = attr_y
-    if attr_x_is_string: # add x-ticks:
+    if attr_x_is_string:  # add x-ticks:
         p.xaxis.ticker = list(range(len(attr_x_levels)))
         p.xaxis.major_label_overrides = {i: attr_x_levels[i] for i in range(len(attr_x_levels))}
 
     # Legend additions:
     if attr_color is not None and attr_color_is_string:
         legend_it = []
         for i in range(len(attr_color_levels)):
             legend_it.append(LegendItem(label=attr_color_levels[i], renderers=[circ], index=datadict[attr_color].index(attr_color_levels[i])))
         legend = Legend(items=legend_it, location=(0, 0))
-        p.add_layout(legend, 'right')
+        p.add_layout(legend, "right")
 
     if attr_color is not None and not attr_color_is_string:
-        color_bar = ColorBar(color_mapper=color_mapper, title = attr_color,
-                             label_standoff=12, border_line_color=None, location=(0,0))
-        p.add_layout(color_bar, 'right')
+        color_bar = ColorBar(color_mapper=color_mapper, title=attr_color, label_standoff=12, border_line_color=None, location=(0, 0))
+        p.add_layout(color_bar, "right")
 
     if attr_size is not None:
-        p.add_layout(Legend(items=[LegendItem(label='Size of points based on "'+attr_size + '"')]), 'below')
+        p.add_layout(Legend(items=[LegendItem(label='Size of points based on "' + attr_size + '"')]), "below")
 
     if show_plot:
         show(p)
     elif save_file is not None:
         save(p)
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/time.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     f(*args, **kwargs)
     time_end = time.time()
     avg_time = time_end - time_start
     if max_repeats == 1:
         return avg_time
     if time_limit is None or avg_time < (time_limit / max_repeats):
         time_start_loop = time.time()
-        for i in range(max_repeats-1):
+        for i in range(max_repeats - 1):
             f(*args, **kwargs)
         time_end_loop = time.time()
         total_time_loop = time_end_loop - time_start_loop
         avg_time = (avg_time + total_time_loop) / max_repeats
     return avg_time
 
 
@@ -74,20 +74,20 @@
     -------
     df_out : DataFrame
         Sampled DataFrame. User can get the effective sample_size via len(df_out).
     """
     len_df = len(df)
     if max_sample_size is None:
         max_sample_size = sample_size
-    assert isinstance(sample_size, int), 'sample_size must be of type int'
-    assert isinstance(max_sample_size, int), 'max_sample_size must be of type int'
+    assert isinstance(sample_size, int), "sample_size must be of type int"
+    assert isinstance(max_sample_size, int), "max_sample_size must be of type int"
     if sample_size < 1:
-        raise AssertionError(f'sample_size must be >=1, but was {sample_size}')
+        raise AssertionError(f"sample_size must be >=1, but was {sample_size}")
     if max_sample_size < 1:
-        raise AssertionError(f'max_sample_size must be >=1, but was {max_sample_size}')
+        raise AssertionError(f"max_sample_size must be >=1, but was {max_sample_size}")
 
     if len_df > sample_size:
         df_out = df.head(sample_size)
     elif len_df < sample_size and len_df < max_sample_size:
         sample_size = min(sample_size, max_sample_size)  # No need to sample more than 10,000 generally
         df_out = df.sample(sample_size, replace=True, random_state=0, ignore_index=True)
     else:
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/utils.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,57 @@
 import logging
 import math
 import pickle
-import time
 import random
 import sys
+import time
 from typing import Callable, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import scipy.stats
 from numpy.typing import ArrayLike
 from pandas import DataFrame, Series
-from sklearn.model_selection import RepeatedKFold, RepeatedStratifiedKFold, LeaveOneGroupOut
-from sklearn.model_selection import train_test_split
+from sklearn.model_selection import LeaveOneGroupOut, RepeatedKFold, RepeatedStratifiedKFold, train_test_split
 
 from autogluon.common.utils.resource_utils import ResourceManager
-from .miscs import warning_filter
+
 from ..constants import (
-    BINARY, LARGE_DATA_THRESHOLD, MULTICLASS, MULTICLASS_UPPER_LIMIT, QUANTILE,
-    REGRESS_THRESHOLD_LARGE_DATA, REGRESS_THRESHOLD_SMALL_DATA, REGRESSION, SOFTCLASS
+    BINARY,
+    LARGE_DATA_THRESHOLD,
+    MULTICLASS,
+    MULTICLASS_UPPER_LIMIT,
+    QUANTILE,
+    REGRESS_THRESHOLD_LARGE_DATA,
+    REGRESS_THRESHOLD_SMALL_DATA,
+    REGRESSION,
+    SOFTCLASS,
 )
-from ..metrics import accuracy, root_mean_squared_error, pinball_loss, Scorer
+from ..metrics import Scorer, accuracy, pinball_loss, root_mean_squared_error
+from .miscs import warning_filter
 
 logger = logging.getLogger(__name__)
 
 
 class CVSplitter:
-    def __init__(self,
-                 splitter_cls=None,
-                 n_splits=5,
-                 n_repeats=1,
-                 random_state=0,
-                 stratified=False,
-                 groups=None):
+    def __init__(self, splitter_cls=None, n_splits=5, n_repeats=1, random_state=0, stratified=False, groups=None):
         self.n_splits = n_splits
         self.n_repeats = n_repeats
         self.random_state = random_state
         self.stratified = stratified
         self.groups = groups
         if splitter_cls is None:
             splitter_cls = self._get_splitter_cls()
         self._splitter = self._get_splitter(splitter_cls)
 
     def _get_splitter_cls(self):
         if self.groups is not None:
             num_groups = len(self.groups.unique())
             if self.n_repeats != 1:
-                raise AssertionError(f'n_repeats must be 1 when split groups are specified. (n_repeats={self.n_repeats})')
+                raise AssertionError(f"n_repeats must be 1 when split groups are specified. (n_repeats={self.n_repeats})")
             self.n_splits = num_groups
             splitter_cls = LeaveOneGroupOut
             # pass
         elif self.stratified:
             splitter_cls = RepeatedStratifiedKFold
         else:
             splitter_cls = RepeatedKFold
@@ -58,15 +59,15 @@
 
     def _get_splitter(self, splitter_cls):
         if splitter_cls == LeaveOneGroupOut:
             return splitter_cls()
         elif splitter_cls in [RepeatedKFold, RepeatedStratifiedKFold]:
             return splitter_cls(n_splits=self.n_splits, n_repeats=self.n_repeats, random_state=self.random_state)
         else:
-            raise AssertionError(f'{splitter_cls} is not supported as a valid `splitter_cls` input to CVSplitter.')
+            raise AssertionError(f"{splitter_cls} is not supported as a valid `splitter_cls` input to CVSplitter.")
 
     def split(self, X, y):
         if isinstance(self._splitter, RepeatedStratifiedKFold):
             # FIXME: There is a bug in sklearn that causes an incorrect ValueError if performing stratification and all classes have fewer than n_splits samples.
             #  This is hacked by adding a dummy class with n_splits samples, performing the kfold split, then removing the dummy samples from all resulting indices.
             #  This is very inefficient and complicated and ideally should be fixed in sklearn.
             with warning_filter():
@@ -84,29 +85,31 @@
                         out[i][1] = [index for index in test_index if index not in invalid_index]
             return out
         else:
             return [[train_index, test_index] for train_index, test_index in self._splitter.split(X, y, groups=self.groups)]
 
 
 def setup_compute(nthreads_per_trial, ngpus_per_trial):
-    if nthreads_per_trial is None or nthreads_per_trial == 'all':
-        nthreads_per_trial = ResourceManager.get_cpu_count()  # Use all of processing power / trial by default. To use just half: # int(np.floor(multiprocessing.cpu_count()/2))
+    if nthreads_per_trial is None or nthreads_per_trial == "all":
+        nthreads_per_trial = (
+            ResourceManager.get_cpu_count()
+        )  # Use all of processing power / trial by default. To use just half: # int(np.floor(multiprocessing.cpu_count()/2))
     if ngpus_per_trial is None:
         ngpus_per_trial = 0  # do not use GPU by default
-    elif ngpus_per_trial == 'all':
+    elif ngpus_per_trial == "all":
         ngpus_per_trial = ResourceManager.get_gpu_count_all()
-    if not isinstance(nthreads_per_trial, int) and nthreads_per_trial != 'auto':
+    if not isinstance(nthreads_per_trial, int) and nthreads_per_trial != "auto":
         raise ValueError(f'nthreads_per_trial must be an integer or "auto": nthreads_per_trial = {nthreads_per_trial}')
-    if not isinstance(ngpus_per_trial, int) and ngpus_per_trial != 'auto':
+    if not isinstance(ngpus_per_trial, int) and ngpus_per_trial != "auto":
         raise ValueError(f'ngpus_per_trial must be an integer or "auto": ngpus_per_trial = {ngpus_per_trial}')
     return nthreads_per_trial, ngpus_per_trial
 
 
 def setup_trial_limits(time_limit, num_trials, hyperparameters):
-    """ Adjust default time limits / num_trials """
+    """Adjust default time limits / num_trials"""
     if num_trials is None:
         if time_limit is None:
             time_limit = 10 * 60  # run for 10min by default
         time_limit /= float(len(hyperparameters))  # each model type gets half the available time
         num_trials = 1000  # run up to 1000 trials (or as you can within the given time_limit)
     elif time_limit is None:
         time_limit = int(1e6)  # user only specified num_trials, so run all of them regardless of time_limit
@@ -115,15 +118,15 @@
 
     if time_limit <= 10:  # threshold = 10sec, ie. too little time to run >1 trial.
         num_trials = 1
     time_limit *= 0.9  # reduce slightly to account for extra time overhead
     return time_limit, num_trials
 
 
-def get_leaderboard_pareto_frontier(leaderboard: DataFrame, score_col='score_val', inference_time_col='pred_time_val_full') -> DataFrame:
+def get_leaderboard_pareto_frontier(leaderboard: DataFrame, score_col="score_val", inference_time_col="pred_time_val_full") -> DataFrame:
     """
     Given a set of models, returns in ranked order from best score to worst score models which satisfy the criteria:
     1. No other model in the set has both a lower inference time and a better or equal score.
 
     :param leaderboard: Leaderboard DataFrame of model info containing score_col and inference_time_col
     :param score_col: Column name in leaderboard of model score values
     :param inference_time_col: Column name in leaderboard of model inference times
@@ -152,71 +155,73 @@
     X_shuffled = X.iloc[rand_shuffle]
     if reset_index:
         X_shuffled.reset_index(inplace=True, drop=True)
     return X_shuffled
 
 
 def normalize_binary_probas(y_predprob, eps):
-    """ Remaps the predicted probabilities to open interval (0,1) while maintaining rank order """
-    (pmin,pmax) = (eps, 1-eps)  # predicted probs outside this range will be remapped into (0,1)
+    """Remaps the predicted probabilities to open interval (0,1) while maintaining rank order"""
+    (pmin, pmax) = (eps, 1 - eps)  # predicted probs outside this range will be remapped into (0,1)
     which_toobig = y_predprob > pmax
     if np.sum(which_toobig) > 0:  # remap overly large probs
-        y_predprob = np.logical_not(which_toobig)*y_predprob + which_toobig*(1-(eps*np.exp(-(y_predprob-pmax))))
+        y_predprob = np.logical_not(which_toobig) * y_predprob + which_toobig * (1 - (eps * np.exp(-(y_predprob - pmax))))
     which_toosmall = y_predprob < pmin
     if np.sum(which_toosmall) > 0:  # remap overly small probs
-        y_predprob = np.logical_not(which_toosmall)*y_predprob + which_toosmall*eps*np.exp(-(pmin-y_predprob))
+        y_predprob = np.logical_not(which_toosmall) * y_predprob + which_toosmall * eps * np.exp(-(pmin - y_predprob))
     return y_predprob
 
 
 def normalize_multi_probas(y_predprob, eps):
-    """ Remaps the predicted probabilities to lie in (0,1) where eps controls how far from 0 smallest class-probability lies """
+    """Remaps the predicted probabilities to lie in (0,1) where eps controls how far from 0 smallest class-probability lies"""
     min_predprob = np.min(y_predprob)
     if min_predprob < 0:  # ensure nonnegative rows
         most_negative_rowvals = np.clip(np.min(y_predprob, axis=1), a_min=None, a_max=0)
-        y_predprob = y_predprob - most_negative_rowvals[:,None]
+        y_predprob = y_predprob - most_negative_rowvals[:, None]
     if min_predprob < eps:
         y_predprob = np.clip(y_predprob, a_min=eps, a_max=None)  # ensure no entries < eps
         y_predprob = y_predprob / y_predprob.sum(axis=1, keepdims=1)  # renormalize
     return y_predprob
 
 
 def default_holdout_frac(num_train_rows, hyperparameter_tune=False):
-    """ Returns default holdout_frac used in fit().
-        Between row count 5,000 and 25,000 keep 0.1 holdout_frac, as we want to grow validation set to a stable 2500 examples.
+    """Returns default holdout_frac used in fit().
+    Between row count 5,000 and 25,000 keep 0.1 holdout_frac, as we want to grow validation set to a stable 2500 examples.
     """
     if num_train_rows < 5000:
         holdout_frac = max(0.1, min(0.2, 500.0 / num_train_rows))
     else:
         holdout_frac = max(0.01, min(0.1, 2500.0 / num_train_rows))
 
     if hyperparameter_tune:
         holdout_frac = min(0.2, holdout_frac * 2)  # We want to allocate more validation data for HPO to avoid overfitting
 
     return holdout_frac
 
 
 def augment_rare_classes(X, label, threshold):
-    """ Use this method when using certain eval_metrics like log_loss, for which no classes may be filtered out.
-        This method will augment dataset with additional examples of rare classes.
+    """Use this method when using certain eval_metrics like log_loss, for which no classes may be filtered out.
+    This method will augment dataset with additional examples of rare classes.
     """
     class_counts = X[label].value_counts()
     class_counts_invalid = class_counts[class_counts < threshold]
     if len(class_counts_invalid) == 0:
         logger.debug("augment_rare_classes did not need to duplicate any data from rare classes")
         return X
 
     missing_classes = []
     for clss, n_clss in class_counts_invalid.items():
         if n_clss == 0:
             missing_classes.append(clss)
     if missing_classes:
-        logger.warning(f'WARNING: {len(missing_classes)} classes were found that have 0 training examples, '
-                       f'and may lead to downstream issues. '
-                       f'Consider either providing data for these classes or removing them from the class categories. '
-                       f'These classes will be ignored: {missing_classes}')
+        logger.warning(
+            f"WARNING: {len(missing_classes)} classes were found that have 0 training examples, "
+            f"and may lead to downstream issues. "
+            f"Consider either providing data for these classes or removing them from the class categories. "
+            f"These classes will be ignored: {missing_classes}"
+        )
         class_counts_invalid = class_counts_invalid[~class_counts_invalid.index.isin(set(missing_classes))]
 
     if len(class_counts_invalid) == 0:
         # This avoids crash when the only invalid classes were those that appeared 0 times
         return X
 
     aug_df = None
@@ -238,41 +243,40 @@
     # Ensure new samples generated via augmentation have unique indices
     aug_df = aug_df.reset_index(drop=True)
     aug_df_len = len(aug_df)
     X_index_aug_start = X.index.max() + 1
     aug_index = [X_index_aug_start + i for i in range(aug_df_len)]
     aug_df.index = aug_index
 
-    logger.log(20, f"Duplicated {len(aug_df)} samples from {len(class_counts_invalid)} rare classes in training set because eval_metric requires all classes have at least {threshold} samples.")
+    logger.log(
+        20,
+        f"Duplicated {len(aug_df)} samples from {len(class_counts_invalid)} rare classes in training set because eval_metric requires all classes have at least {threshold} samples.",
+    )
 
     X = pd.concat([X, aug_df], axis=0)
     class_counts = X[label].value_counts()
     class_counts_invalid = class_counts[class_counts < threshold]
     class_counts_invalid = class_counts_invalid[~class_counts_invalid.index.isin(set(missing_classes))]
     if len(class_counts_invalid) > 0:
         raise RuntimeError("augment_rare_classes failed to produce enough data from rare classes")
     return X
 
 
-def get_pred_from_proba_df(y_pred_proba: pd.DataFrame,
-                           problem_type: str = BINARY,
-                           decision_threshold: float = None) -> pd.Series:
+def get_pred_from_proba_df(y_pred_proba: pd.DataFrame, problem_type: str = BINARY, decision_threshold: float = None) -> pd.Series:
     """
     From input DataFrame of pred_proba, return Series of pred.
     The input DataFrame's columns must be the names of the target classes.
     """
     if problem_type == REGRESSION:
         y_pred = y_pred_proba
     elif problem_type == QUANTILE:
         y_pred = y_pred_proba
     elif problem_type == BINARY and decision_threshold is not None:
         negative_class, positive_class = y_pred_proba.columns
-        y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba.values,
-                                     problem_type=problem_type,
-                                     decision_threshold=decision_threshold)
+        y_pred = get_pred_from_proba(y_pred_proba=y_pred_proba.values, problem_type=problem_type, decision_threshold=decision_threshold)
         y_pred = [positive_class if pred == 1 else negative_class for pred in y_pred]
         y_pred = pd.Series(data=y_pred, index=y_pred_proba.index)
     else:
         y_pred = y_pred_proba.idxmax(axis=1)
     return y_pred
 
 
@@ -296,18 +300,15 @@
     else:
         y_pred = []
         if not len(y_pred_proba) == 0:
             y_pred = np.argmax(y_pred_proba, axis=1)
     return y_pred
 
 
-def convert_pred_probas_to_df(pred_proba_list: List[ArrayLike],
-                              columns: List[str],
-                              problem_type: str,
-                              index: pd.Index = None) -> DataFrame:
+def convert_pred_probas_to_df(pred_proba_list: List[ArrayLike], columns: List[str], problem_type: str, index: pd.Index = None) -> DataFrame:
     """
     Converts a list of pred_proba model outputs to a DataFrame
 
     Parameters
     ----------
     pred_proba_list : List[ArrayLike]
         A list of prediction probabilities.
@@ -353,20 +354,17 @@
     if label not in list(data.columns):
         raise ValueError(f"Provided DataFrame does not contain label column: {label}")
     y = data[label].copy()
     X = data.drop(label, axis=1)
     return X, y
 
 
-def generate_train_test_split_combined(data: DataFrame,
-                                       label: str,
-                                       problem_type: str,
-                                       test_size: float = 0.1,
-                                       random_state: int = 0,
-                                       min_cls_count_train: int = 1) -> (DataFrame, DataFrame):
+def generate_train_test_split_combined(
+    data: DataFrame, label: str, problem_type: str, test_size: float = 0.1, random_state: int = 0, min_cls_count_train: int = 1
+) -> (DataFrame, DataFrame):
     """
     Generate a train test split from a DataFrame that contains the label column.
 
     Parameters
     ----------
     data : DataFrame
         DataFrame containing the features plus the label column to split into train and test sets.
@@ -390,31 +388,24 @@
     Returns
     -------
     train_data, test_data : (DataFrame, DataFrame)
         The train_data and test_data after performing the split. Includes the label column.
     """
     X, y = extract_label(data=data, label=label)
     train_data, test_data, y_train, y_test = generate_train_test_split(
-        X=X,
-        y=y,
-        problem_type=problem_type,
-        test_size=test_size,
-        random_state=random_state,
-        min_cls_count_train=min_cls_count_train)
+        X=X, y=y, problem_type=problem_type, test_size=test_size, random_state=random_state, min_cls_count_train=min_cls_count_train
+    )
     train_data[label] = y_train
     test_data[label] = y_test
     return train_data, test_data
 
 
-def generate_train_test_split(X: DataFrame,
-                              y: Series,
-                              problem_type: str,
-                              test_size: Union[float, int] = 0.1,
-                              random_state=0,
-                              min_cls_count_train=1) -> Tuple[DataFrame, DataFrame, Series, Series]:
+def generate_train_test_split(
+    X: DataFrame, y: Series, problem_type: str, test_size: Union[float, int] = 0.1, random_state=0, min_cls_count_train=1
+) -> Tuple[DataFrame, DataFrame, Series, Series]:
     """
     Generate a train test split from input X, y.
     If you have a combined X, y DataFrame, refer to `generate_train_test_split_combined` instead.
 
     Parameters
     ----------
     X : DataFrame
@@ -464,28 +455,30 @@
     # This code will ensure that the sample will be part of the train split, meaning the test split will have 0 samples of the rare class.
     rare_indices = None
     if stratify is not None:
         cls_counts = y.value_counts()
         cls_counts_invalid = cls_counts[cls_counts < min_cls_count_train]
 
         if len(cls_counts_invalid) > 0:
-            logger.error(f'ERROR: Classes have too few samples to split the data! At least {min_cls_count_train} are required.')
+            logger.error(f"ERROR: Classes have too few samples to split the data! At least {min_cls_count_train} are required.")
             logger.error(cls_counts_invalid)
-            raise AssertionError('Not enough data to split data into train and val without dropping classes!')
+            raise AssertionError("Not enough data to split data into train and val without dropping classes!")
         elif min_cls_count_train < 2:
             cls_counts_rare = cls_counts[cls_counts < 2]
             if len(cls_counts_rare) > 0:
                 cls_counts_rare_val = set(cls_counts_rare.index)
                 y_rare = y[y.isin(cls_counts_rare_val)]
                 rare_indices = list(y_rare.index)
                 X_split = X.drop(index=rare_indices)
                 y_split = y.drop(index=rare_indices)
                 stratify = y_split
 
-    X_train, X_test, y_train, y_test = train_test_split(X_split, y_split.values, test_size=test_size, shuffle=True, random_state=random_state, stratify=stratify)
+    X_train, X_test, y_train, y_test = train_test_split(
+        X_split, y_split.values, test_size=test_size, shuffle=True, random_state=random_state, stratify=stratify
+    )
     if problem_type != SOFTCLASS:
         y_train = pd.Series(y_train, index=X_train.index)
         y_test = pd.Series(y_test, index=X_test.index)
     else:
         y_train = pd.DataFrame(y_train, index=X_train.index)
         y_test = pd.DataFrame(y_test, index=X_test.index)
 
@@ -503,15 +496,15 @@
         random.seed(random_state)
         for cls in class_counts_dict_orig.keys():
             count = class_counts_dict.get(cls, 0)
             if count >= min_cls_count_train:
                 continue
             count_test = class_counts_dict_test.get(cls, 0)
             if count + count_test < min_cls_count_train:
-                raise AssertionError('Not enough data to split data into train and val without dropping classes!')
+                raise AssertionError("Not enough data to split data into train and val without dropping classes!")
             count_to_move = min_cls_count_train - count
             indices_of_cls_test = list(y_test[y_test == cls].index)
             indices_to_move_cls = random.sample(indices_of_cls_test, count_to_move)
             indices_to_move += indices_to_move_cls
         random.setstate(random_state_init)
         if indices_to_move:
             y_test_moved = y_test.loc[indices_to_move].copy()
@@ -522,20 +515,20 @@
             X_test = X_test.drop(index=indices_to_move)
         y_train.name = y_split.name
         y_test.name = y_split.name
     return X_train, X_test, y_train, y_test
 
 
 def normalize_pred_probas(y_predprob, problem_type, eps=1e-7):
-    """ Remaps the predicted probabilities to ensure there are no zeros (needed for certain metrics like log-loss)
-        and that no predicted probability exceeds [0,1] (eg. in distillation when classification is treated as regression).
-        Args:
-            y_predprob: 1D (for binary classification) or 2D (for multiclass) numpy array of predicted probabilities
-            problem_type: We only consider normalization if the problem_type is one of: [BINARY, MULTICLASS, SOFTCLASS]
-            eps: controls around how far from 0 remapped predicted probabilities should be (larger `eps` means predicted probabilities will lie further from 0).
+    """Remaps the predicted probabilities to ensure there are no zeros (needed for certain metrics like log-loss)
+    and that no predicted probability exceeds [0,1] (eg. in distillation when classification is treated as regression).
+    Args:
+        y_predprob: 1D (for binary classification) or 2D (for multiclass) numpy array of predicted probabilities
+        problem_type: We only consider normalization if the problem_type is one of: [BINARY, MULTICLASS, SOFTCLASS]
+        eps: controls around how far from 0 remapped predicted probabilities should be (larger `eps` means predicted probabilities will lie further from 0).
     """
     if (problem_type == REGRESSION) and (len(y_predprob.shape) > 1) and (y_predprob.shape[1] > 1):
         problem_type = SOFTCLASS  # this was MULTICLASS problem converted to REGRESSION (as done in distillation)
 
     if problem_type in [BINARY, REGRESSION]:
         if len(y_predprob.shape) > 1 and min(y_predprob.shape) > 1:
             raise ValueError(f"cannot call normalize_pred_probas with problem_type={problem_type} and y_predprob.shape=={y_predprob.shape}")
@@ -546,36 +539,38 @@
         else:
             return normalize_multi_probas(y_predprob, eps)
     else:
         raise ValueError(f"Invalid problem_type")
 
 
 def infer_problem_type(y: Series, silent=False) -> str:
-    """ Identifies which type of prediction problem we are interested in (if user has not specified).
-        Ie. binary classification, multi-class classification, or regression.
+    """Identifies which type of prediction problem we are interested in (if user has not specified).
+    Ie. binary classification, multi-class classification, or regression.
     """
-    with pd.option_context('mode.use_inf_as_na', True): # treat None, NaN, INF, NINF as NA
+    with pd.option_context("mode.use_inf_as_na", True):  # treat None, NaN, INF, NINF as NA
         y = y.dropna()
     num_rows = len(y)
 
     if num_rows == 0:
         raise ValueError("Label column cannot have 0 valid values")
 
     unique_values = y.unique()
 
     if num_rows > LARGE_DATA_THRESHOLD:
-        regression_threshold = REGRESS_THRESHOLD_LARGE_DATA  # if the unique-ratio is less than this, we assume multiclass classification, even when labels are integers
+        regression_threshold = (
+            REGRESS_THRESHOLD_LARGE_DATA  # if the unique-ratio is less than this, we assume multiclass classification, even when labels are integers
+        )
     else:
         regression_threshold = REGRESS_THRESHOLD_SMALL_DATA
 
     unique_count = len(unique_values)
     if unique_count == 2:
         problem_type = BINARY
         reason = "only two unique label-values observed"
-    elif y.dtype.name in ['object', 'category', 'string']:
+    elif y.dtype.name in ["object", "category", "string"]:
         problem_type = MULTICLASS
         reason = f"dtype of label-column == {y.dtype.name}"
     elif np.issubdtype(y.dtype, np.floating):
         unique_ratio = unique_count / float(num_rows)
         if (unique_ratio <= regression_threshold) and (unique_count <= MULTICLASS_UPPER_LIMIT):
             try:
                 can_convert_to_int = np.array_equal(y, y.astype(int))
@@ -596,33 +591,36 @@
         if (unique_ratio <= regression_threshold) and (unique_count <= MULTICLASS_UPPER_LIMIT):
             problem_type = MULTICLASS  # TODO: Check if integers are from 0 to n-1 for n unique values, if they have a wide spread, it could still be regression
             reason = "dtype of label-column == int, but few unique label-values observed"
         else:
             problem_type = REGRESSION
             reason = "dtype of label-column == int and many unique label-values observed"
     else:
-        raise NotImplementedError(f'label dtype {y.dtype} not supported!')
+        raise NotImplementedError(f"label dtype {y.dtype} not supported!")
     if not silent:
         logger.log(25, f"AutoGluon infers your prediction problem is: '{problem_type}' (because {reason}).")
 
         # TODO: Move this outside of this function so it is visible even if problem type was not inferred.
         if problem_type in [BINARY, MULTICLASS]:
             if unique_count > 10:
-                logger.log(20, f'\tFirst 10 (of {unique_count}) unique label values:  {list(unique_values[:10])}')
+                logger.log(20, f"\tFirst 10 (of {unique_count}) unique label values:  {list(unique_values[:10])}")
             else:
-                logger.log(20, f'\t{unique_count} unique label values:  {list(unique_values)}')
+                logger.log(20, f"\t{unique_count} unique label values:  {list(unique_values)}")
         elif problem_type == REGRESSION:
             y_max = y.max()
             y_min = y.min()
             y_mean = y.mean()
             y_stddev = y.std()
-            logger.log(20, f'\tLabel info (max, min, mean, stddev): ({y_max}, {y_min}, {round(y_mean, 5)}, {round(y_stddev, 5)})')
+            logger.log(20, f"\tLabel info (max, min, mean, stddev): ({y_max}, {y_min}, {round(y_mean, 5)}, {round(y_stddev, 5)})")
 
-        logger.log(25, f"\tIf '{problem_type}' is not the correct problem_type, please manually specify the problem_type parameter during predictor init "
-                       f"(You may specify problem_type as one of: {[BINARY, MULTICLASS, REGRESSION]})")
+        logger.log(
+            25,
+            f"\tIf '{problem_type}' is not the correct problem_type, please manually specify the problem_type parameter during predictor init "
+            f"(You may specify problem_type as one of: {[BINARY, MULTICLASS, REGRESSION]})",
+        )
     return problem_type
 
 
 def infer_eval_metric(problem_type: str) -> Scorer:
     """Infers appropriate default eval metric based on problem_type. Useful when no eval_metric was provided."""
     if problem_type == BINARY:
         return accuracy
@@ -631,64 +629,66 @@
     elif problem_type == QUANTILE:
         return pinball_loss
     else:
         return root_mean_squared_error
 
 
 def extract_column(X, col_name):
-    """Extract specified column from dataframe. """
+    """Extract specified column from dataframe."""
     if col_name is None or col_name not in list(X.columns):
         return X, None
     w = X[col_name].copy()
     X = X.drop(col_name, axis=1)
     return X, w
 
 
 def compute_weighted_metric(y, y_pred, metric, weights, weight_evaluation=None, **kwargs):
-    """ Report weighted metric if: weights is not None, weight_evaluation=True, and the given metric supports sample weights.
-        If weight_evaluation=None, it will be set to False if weights=None, True otherwise.
+    """Report weighted metric if: weights is not None, weight_evaluation=True, and the given metric supports sample weights.
+    If weight_evaluation=None, it will be set to False if weights=None, True otherwise.
     """
     if not metric.needs_quantile:
-        kwargs.pop('quantile_levels', None)
+        kwargs.pop("quantile_levels", None)
     if weight_evaluation is None:
         weight_evaluation = not (weights is None)
     if weight_evaluation and weights is None:
         raise ValueError("Sample weights cannot be None when weight_evaluation=True.")
     if not weight_evaluation:
         return metric(y, y_pred, **kwargs)
     try:
         weighted_metric = metric(y, y_pred, sample_weight=weights, **kwargs)
     except (ValueError, TypeError, KeyError):
-        if hasattr(metric, 'name'):
+        if hasattr(metric, "name"):
             metric_name = metric.name
         else:
             metric_name = metric
         logger.log(30, f"WARNING: eval_metric='{metric_name}' does not support sample weights so they will be ignored in reported metric.")
         weighted_metric = metric(y, y_pred, **kwargs)
     return weighted_metric
 
 
 # Note: Do not send training data as input or the importances will be overfit.
 # TODO: Improve time estimate (Currently pessimistic)
-def compute_permutation_feature_importance(X: pd.DataFrame,
-                                           y: pd.Series,
-                                           predict_func: Callable[..., np.ndarray],
-                                           eval_metric: Scorer,
-                                           features: list = None,
-                                           subsample_size=None,
-                                           num_shuffle_sets: int = None,
-                                           predict_func_kwargs: dict = None,
-                                           transform_func: Callable[..., pd.DataFrame] = None,
-                                           transform_func_kwargs: dict = None,
-                                           time_limit: float = None,
-                                           silent=False,
-                                           log_prefix='',
-                                           importance_as_list=False,
-                                           random_state=0,
-                                           **kwargs) -> pd.DataFrame:
+def compute_permutation_feature_importance(
+    X: pd.DataFrame,
+    y: pd.Series,
+    predict_func: Callable[..., np.ndarray],
+    eval_metric: Scorer,
+    features: list = None,
+    subsample_size=None,
+    num_shuffle_sets: int = None,
+    predict_func_kwargs: dict = None,
+    transform_func: Callable[..., pd.DataFrame] = None,
+    transform_func_kwargs: dict = None,
+    time_limit: float = None,
+    silent=False,
+    log_prefix="",
+    importance_as_list=False,
+    random_state=0,
+    **kwargs,
+) -> pd.DataFrame:
     """
     Computes a trained model's feature importance via permutation shuffling (https://explained.ai/rf-importance/).
     A feature's importance score represents the performance drop that results when the model makes predictions on a perturbed copy of the dataset where this feature's values have been randomly shuffled across rows.
     A feature score of 0.01 would indicate that the predictive performance dropped by 0.01 when the feature was randomly shuffled.
     The higher the score a feature has, the more important it is to the model's performance.
     If a feature has a negative score, this means that the feature is likely harmful to the final model, and a model trained with the feature removed would be expected to achieve a better predictive performance.
     Note that calculating feature importance can be a very computationally expensive process, particularly if the model uses hundreds or thousands of features. In many cases, this can take longer than the original model training.
@@ -766,15 +766,15 @@
         'p_value': P-value for a statistical t-test of the null hypothesis: importance = 0, vs the (one-sided) alternative: importance > 0.
             Features with low p-value appear confidently useful to the predictor, while the other features may be useless to the predictor (or even harmful to include in its training data).
             A p-value of 0.01 indicates that there is a 1% chance that the feature is useless or harmful, and a 99% chance that the feature is useful.
             A p-value of 0.99 indicates that there is a 99% chance that the feature is useless or harmful, and a 1% chance that the feature is useful.
         'n': The number of shuffles performed to estimate importance score (corresponds to sample-size used to determine confidence interval for true score).
     """
     if not eval_metric.needs_quantile:
-        kwargs.pop('quantile_levels', None)
+        kwargs.pop("quantile_levels", None)
 
     if num_shuffle_sets is None:
         num_shuffle_sets = 1 if time_limit is None else 10
 
     time_start = time.time()
     if predict_func_kwargs is None:
         predict_func_kwargs = dict()
@@ -790,23 +790,23 @@
     if subsample_size is not None:
         num_rows = min(len(X), subsample_size)
     else:
         num_rows = len(X)
     subsample = num_rows < len(X)
 
     if not silent:
-        logging_message = f'{log_prefix}Computing feature importance via permutation shuffling for {num_features} features using {num_rows} rows with {num_shuffle_sets} shuffle sets...'
+        logging_message = f"{log_prefix}Computing feature importance via permutation shuffling for {num_features} features using {num_rows} rows with {num_shuffle_sets} shuffle sets..."
         if time_limit is not None:
-            logging_message = f'{logging_message} Time limit: {time_limit}s...'
+            logging_message = f"{logging_message} Time limit: {time_limit}s..."
         logger.log(20, logging_message)
 
     time_permutation_start = time.time()
     fi_dict_list = []
     shuffle_repeats_completed = 0
-    log_final_suffix = ''
+    log_final_suffix = ""
 
     X_orig = X
     y_orig = y
     feature_batch_count = None
     X_raw = None
     score_baseline = None
     initial_random_state = random_state
@@ -826,45 +826,45 @@
             y_pred = predict_func(X_transformed, **predict_func_kwargs)
             score_baseline = eval_metric(y, y_pred, **kwargs)
             if shuffle_repeat == 0:
                 if not silent:
                     time_score = time.time() - time_start_score
                     time_estimated = ((num_features + 1) * time_score) * num_shuffle_sets + time_start_score - time_start
                     time_estimated_per_set = time_estimated / num_shuffle_sets
-                    logger.log(20, f'{log_prefix}\t{round(time_estimated, 2)}s\t= Expected runtime ({round(time_estimated_per_set, 2)}s per shuffle set)')
+                    logger.log(20, f"{log_prefix}\t{round(time_estimated, 2)}s\t= Expected runtime ({round(time_estimated_per_set, 2)}s per shuffle set)")
 
                 if transform_func is None:
                     feature_batch_count = _get_safe_fi_batch_count(X=X, num_features=num_features)
                 else:
                     feature_batch_count = _get_safe_fi_batch_count(X=X, num_features=num_features, X_transformed=X_transformed)
 
             # creating copy of original data N=feature_batch_count times for parallel processing
             X_raw = pd.concat([X.copy() for _ in range(feature_batch_count)], ignore_index=True, sort=False).reset_index(drop=True)
 
         row_count = len(X)
 
         X_shuffled = shuffle_df_rows(X=X, seed=random_state)
 
         for i in range(0, num_features, feature_batch_count):
-            parallel_computed_features = features[i:i + feature_batch_count]
+            parallel_computed_features = features[i : i + feature_batch_count]
 
             # if final iteration, leaving only necessary part of X_raw
             num_features_processing = len(parallel_computed_features)
             final_iteration = i + num_features_processing == num_features
 
             row_index = 0
             for feature in parallel_computed_features:
                 if isinstance(feature, tuple):
                     feature = feature[1]
                 row_index_end = row_index + row_count
-                X_raw.loc[row_index:row_index_end - 1, feature] = X_shuffled[feature].values
+                X_raw.loc[row_index : row_index_end - 1, feature] = X_shuffled[feature].values
                 row_index = row_index_end
 
             if (num_features_processing < feature_batch_count) and final_iteration:
-                X_raw_transformed = X_raw.loc[:row_count * num_features_processing - 1]
+                X_raw_transformed = X_raw.loc[: row_count * num_features_processing - 1]
                 X_raw_transformed = X_raw_transformed if transform_func is None else transform_func(X_raw_transformed, **transform_func_kwargs)
             else:
                 X_raw_transformed = X_raw if transform_func is None else transform_func(X_raw, **transform_func_kwargs)
             y_pred = predict_func(X_raw_transformed, **predict_func_kwargs)
 
             row_index = 0
             for feature in parallel_computed_features:
@@ -877,37 +877,40 @@
                 # calculating importance score for given feature
                 row_index_end = row_index + row_count
                 y_pred_cur = y_pred[row_index:row_index_end]
                 score = eval_metric(y, y_pred_cur, **kwargs)
                 fi[feature_name] = score_baseline - score
 
                 # resetting to original values for processed feature
-                X_raw.loc[row_index:row_index_end - 1, feature_list] = X[feature_list].values
+                X_raw.loc[row_index : row_index_end - 1, feature_list] = X[feature_list].values
 
                 row_index = row_index_end
         fi_dict_list.append(fi)
         shuffle_repeats_completed = shuffle_repeat + 1
         if time_limit is not None and shuffle_repeat != (num_shuffle_sets - 1):
             time_now = time.time()
             time_left = time_limit - (time_now - time_start)
             time_permutation_average = (time_now - time_permutation_start) / (shuffle_repeat + 1)
             if time_left < (time_permutation_average * 1.1):
-                log_final_suffix = ' (Early stopping due to lack of time...)'
+                log_final_suffix = " (Early stopping due to lack of time...)"
                 break
 
     fi_list_dict = dict()
     for val in fi_dict_list:
         for key in val:
             if key not in fi_list_dict:
                 fi_list_dict[key] = []
             fi_list_dict[key].append(val[key])
     fi_df = _compute_fi_with_stddev(fi_list_dict, importance_as_list=importance_as_list)
 
     if not silent:
-        logger.log(20, f'{log_prefix}\t{round(time.time() - time_start, 2)}s\t= Actual runtime (Completed {shuffle_repeats_completed} of {num_shuffle_sets} shuffle sets){log_final_suffix}')
+        logger.log(
+            20,
+            f"{log_prefix}\t{round(time.time() - time_start, 2)}s\t= Actual runtime (Completed {shuffle_repeats_completed} of {num_shuffle_sets} shuffle sets){log_final_suffix}",
+        )
 
     return fi_df
 
 
 def _validate_features(features: list, valid_features: list):
     """Raises exception if features list contains invalid features or duplicate features"""
     valid_features = set(valid_features)
@@ -915,31 +918,30 @@
     # validate features
     for feature in features:
         if isinstance(feature, tuple):
             feature_name = feature[0]
             feature_list = feature[1]
             feature_list_set = set(feature_list)
             if len(feature_list_set) != len(feature_list):
-                raise ValueError(f'Feature list contains duplicate features:\n'
-                                 f'{feature_list}')
+                raise ValueError(f"Feature list contains duplicate features:\n" f"{feature_list}")
             for feature_in_list in feature_list:
                 if feature_in_list not in valid_features:
-                    raise ValueError(f'Feature does not exist in data: {feature_in_list}\n'
-                                     f'This feature came from the following feature set:\n'
-                                     f'{feature}\n'
-                                     f'Valid Features:\n'
-                                     f'{valid_features}')
+                    raise ValueError(
+                        f"Feature does not exist in data: {feature_in_list}\n"
+                        f"This feature came from the following feature set:\n"
+                        f"{feature}\n"
+                        f"Valid Features:\n"
+                        f"{valid_features}"
+                    )
         else:
             feature_name = feature
             if feature_name not in valid_features:
-                raise ValueError(f'Feature does not exist in data: {feature_name}\n'
-                                 f'Valid Features:\n'
-                                 f'{valid_features}')
+                raise ValueError(f"Feature does not exist in data: {feature_name}\n" f"Valid Features:\n" f"{valid_features}")
         if feature_name in used_features:
-            raise ValueError(f'Feature is present multiple times in feature list: {feature_name}')
+            raise ValueError(f"Feature is present multiple times in feature list: {feature_name}")
         used_features.add(feature_name)
 
 
 def _compute_fi_with_stddev(fi_list_dict: dict, importance_as_list=False) -> DataFrame:
     features = list(fi_list_dict.keys())
     fi = dict()
     fi_stddev = dict()
@@ -949,31 +951,31 @@
         fi[feature], fi_stddev[feature], fi_p_value[feature], fi_n[feature] = _compute_mean_stddev_and_p_value(fi_list_dict[feature])
         if importance_as_list:
             fi[feature] = fi_list_dict[feature]
 
     fi = pd.Series(fi).sort_values(ascending=False)
     fi_stddev = pd.Series(fi_stddev)
     fi_p_value = pd.Series(fi_p_value)
-    fi_n = pd.Series(fi_n, dtype='int64')
+    fi_n = pd.Series(fi_n, dtype="int64")
 
-    fi_df = fi.to_frame(name='importance')
-    fi_df['stddev'] = fi_stddev
-    fi_df['p_value'] = fi_p_value
-    fi_df['n'] = fi_n
+    fi_df = fi.to_frame(name="importance")
+    fi_df["stddev"] = fi_stddev
+    fi_df["p_value"] = fi_p_value
+    fi_df["n"] = fi_n
     return fi_df
 
 
 def _compute_mean_stddev_and_p_value(values: list):
     mean = np.mean(values)
     n = len(values)
     p_value = np.nan
     stddev = np.std(values, ddof=1) if n > 1 else np.nan
     if stddev != np.nan and stddev != 0:
         t_stat = mean / (stddev / math.sqrt(n))
-        p_value = scipy.stats.t.sf(t_stat, n-1)
+        p_value = scipy.stats.t.sf(t_stat, n - 1)
     elif stddev == 0:
         p_value = 0.5
 
     return mean, stddev, p_value, n
 
 
 def _get_safe_fi_batch_count(X, num_features, X_transformed=None, max_memory_ratio=0.2, max_feature_batch_count=200):
@@ -987,14 +989,9 @@
     feature_batch_count_safe = math.floor(max_memory_ratio / X_memory_ratio)
     feature_batch_count = max(1, min(max_feature_batch_count, feature_batch_count_safe))
     feature_batch_count = min(feature_batch_count, num_features)
     return feature_batch_count
 
 
 def unevaluated_fi_df_template(features: List[str]) -> pd.DataFrame:
-    importance_df = pd.DataFrame({
-        'importance': None,
-        'stddev': None,
-        'p_value': None,
-        'n': 0
-    }, index=features)
+    importance_df = pd.DataFrame({"importance": None, "stddev": None, "p_value": None, "n": 0}, index=features)
     return importance_df
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon/core/utils/version_utils.py` & `autogluon.core-0.8.1b20230622/src/autogluon/core/utils/version_utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import pkgutil
 import platform
 import re
 import sys
 from datetime import datetime
-from importlib.metadata import version, distribution
+from importlib.metadata import distribution, version
 
 import autogluon
 from autogluon.common.utils.nvutil import cudaInit, cudaSystemGetNVMLVersion
 from autogluon.common.utils.resource_utils import ResourceManager
 
 
 def _get_autogluon_versions():
     """Retrieve version of all autogluon subpackages and its dependencies"""
     versions = dict()
-    for pkg in list(pkgutil.iter_modules(autogluon.__path__, autogluon.__name__ + '.')):
+    for pkg in list(pkgutil.iter_modules(autogluon.__path__, autogluon.__name__ + ".")):
         # The following packages will be recognized as a submodule by pkgutil -exclude them.
-        if pkg.name in ['autogluon.version', 'autogluon.setup', 'autogluon._internal_']:
+        if pkg.name in ["autogluon.version", "autogluon.setup", "autogluon._internal_"]:
             continue
         try:
             versions[pkg.name] = version(pkg.name)
             versions.update(_get_dependency_versions(pkg.name))
         except ImportError:
             versions[pkg.name] = None
     return versions
@@ -30,17 +30,17 @@
 
     Args:
         package (str): name of the package
     """
     # Get all requires for the package
     dependencies = distribution(package).requires
     # Filter-out test dependencies
-    dependencies = [req for req in dependencies if not bool(re.search('extra.*test', req))]
+    dependencies = [req for req in dependencies if not bool(re.search("extra.*test", req))]
     # keep only package name
-    dependencies = [re.findall('[a-zA-Z0-9_\\-]+', req)[0].strip() for req in dependencies]
+    dependencies = [re.findall("[a-zA-Z0-9_\\-]+", req)[0].strip() for req in dependencies]
     versions = dict()
     for dependency in dependencies:
         try:
             versions[dependency] = version(dependency)
         except ImportError:
             versions[dependency] = None
     return versions
@@ -53,28 +53,28 @@
     if cudaInit():
         try:
             cuda_version = cudaSystemGetNVMLVersion()
         except:
             cuda_version = None
 
     return {
-        'date': datetime.date(datetime.now()),
-        'time': datetime.time(datetime.now()),
-        'python': '.'.join(str(i) for i in sys.version_info),
-        'OS': uname.system,
-        'OS-release': uname.release,
-        'Version': uname.version,
-        'machine': uname.machine,
-        'processor': uname.processor,
-        'num_cores': ResourceManager.get_cpu_count(),
-        'cpu_ram_mb': ResourceManager.get_memory_size(),
-        'cuda version': cuda_version,
-        'num_gpus': ResourceManager.get_gpu_count_all(),
-        'gpu_ram_mb': ResourceManager.get_gpu_free_memory(),
-        'avail_disk_size_mb': ResourceManager.get_available_disk_size(),
+        "date": datetime.date(datetime.now()),
+        "time": datetime.time(datetime.now()),
+        "python": ".".join(str(i) for i in sys.version_info),
+        "OS": uname.system,
+        "OS-release": uname.release,
+        "Version": uname.version,
+        "machine": uname.machine,
+        "processor": uname.processor,
+        "num_cores": ResourceManager.get_cpu_count(),
+        "cpu_ram_mb": ResourceManager.get_memory_size(),
+        "cuda version": cuda_version,
+        "num_gpus": ResourceManager.get_gpu_count_all(),
+        "gpu_ram_mb": ResourceManager.get_gpu_free_memory(),
+        "avail_disk_size_mb": ResourceManager.get_available_disk_size(),
     }
 
 
 def show_versions():
     """
     Provide useful information, important for bug reports.
     It comprises info about hosting operation system, autogluon subpackage versions,
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/PKG-INFO` & `autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.core
-Version: 0.8.1b20230621
+Version: 0.8.1b20230622
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.core-0.8.1b20230621/src/autogluon.core.egg-info/SOURCES.txt` & `autogluon.core-0.8.1b20230622/src/autogluon.core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

