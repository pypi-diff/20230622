# Comparing `tmp/causallib-0.9.4.tar.gz` & `tmp/causallib-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causallib-0.9.4.tar", last modified: Tue May  2 14:18:35 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
+gzip compressed data, was "causallib-0.9.5.tar", last modified: Thu Jun 22 12:39:53 2023, max speed, from FAT filesystem (MS-DOS, OS/2, NT)
```

## Comparing `causallib-0.9.4.tar` & `causallib-0.9.5.tar`

### file list

```diff
@@ -1,153 +1,157 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/
--rw-rw-rw-   0        0        0        1 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     7906 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      260 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/requires.txt
--rw-rw-rw-   0        0        0     4800 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       10 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/analysis/
--rw-rw-rw-   0        0        0        0 2019-07-12 06:29:37.000000 causallib-0.9.4/causallib/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/adversarial_balancing/
--rw-rw-rw-   0        0        0    15196 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/contrib/adversarial_balancing/adversarial_balancing.py
--rw-rw-rw-   0        0        0     5550 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/contrib/adversarial_balancing/classifier_selection.py
--rw-rw-rw-   0        0        0       57 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/contrib/adversarial_balancing/__init__.py
--rw-rw-rw-   0        0        0     5032 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/contrib/faissknn.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/hemm/
--rw-rw-rw-   0        0        0     7068 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/gen_synthetic_data.py
--rw-rw-rw-   0        0        0    17729 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm.py
--rw-rw-rw-   0        0        0    10222 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm_api.py
--rw-rw-rw-   0        0        0     4453 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm_metrics.py
--rw-rw-rw-   0        0        0     2467 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm_outcome_models.py
--rw-rw-rw-   0        0        0     3692 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/hemm_utilities.py
--rw-rw-rw-   0        0        0     4072 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/load_ihdp_data.py
--rw-rw-rw-   0        0        0     1820 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/README.md
--rw-rw-rw-   0        0        0       50 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/hemm/__init__.py
--rw-rw-rw-   0        0        0     2786 2022-02-08 08:45:42.000000 causallib-0.9.4/causallib/contrib/README.md
--rw-rw-rw-   0        0        0      109 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/contrib/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/shared_sparsity_selection/
--rw-rw-rw-   0        0        0     8498 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py
--rw-rw-rw-   0        0        0       74 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/contrib/shared_sparsity_selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/contrib/tests/
--rw-rw-rw-   0        0        0     7333 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/contrib/tests/test_adversarial_balancing.py
--rw-rw-rw-   0        0        0     3722 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/tests/test_hemm.py
--rw-rw-rw-   0        0        0     7325 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/contrib/tests/test_shared_sparsity_selection.py
--rw-rw-rw-   0        0        0        0 2020-07-07 16:46:29.000000 causallib-0.9.4/causallib/contrib/tests/__init__.py
--rw-rw-rw-   0        0        0        0 2020-02-13 16:38:56.000000 causallib-0.9.4/causallib/contrib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/datasets/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/datasets/data/
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/
--rw-rw-rw-   0        0        0   702589 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/x.csv
--rw-rw-rw-   0        0        0   344363 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_1.csv
--rw-rw-rw-   0        0        0   357958 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_10.csv
--rw-rw-rw-   0        0        0   338894 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_2.csv
--rw-rw-rw-   0        0        0   347947 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_3.csv
--rw-rw-rw-   0        0        0   346711 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_4.csv
--rw-rw-rw-   0        0        0   353616 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_5.csv
--rw-rw-rw-   0        0        0   349008 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_6.csv
--rw-rw-rw-   0        0        0   351869 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_7.csv
--rw-rw-rw-   0        0        0   340923 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_8.csv
--rw-rw-rw-   0        0        0   346092 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_9.csv
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/datasets/data/nhefs/
--rw-rw-rw-   0        0        0   366165 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/nhefs/NHEFS.csv
--rw-rw-rw-   0        0        0     4125 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/data/nhefs/NHEFS_codebook.csv
--rw-rw-rw-   0        0        0     9138 2023-05-02 12:28:47.000000 causallib-0.9.4/causallib/datasets/data_loader.py
--rw-rw-rw-   0        0        0     5277 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/datasets/README.md
--rw-rw-rw-   0        0        0      176 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/estimation/
--rw-rw-rw-   0        0        0    11759 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/estimation/base_estimator.py
--rw-rw-rw-   0        0        0     7794 2022-08-11 10:08:59.000000 causallib-0.9.4/causallib/estimation/base_weight.py
--rw-rw-rw-   0        0        0    26241 2023-05-02 13:20:05.000000 causallib-0.9.4/causallib/estimation/doubly_robust.py
--rw-rw-rw-   0        0        0    14022 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/estimation/ipw.py
--rw-rw-rw-   0        0        0     3752 2021-08-26 08:37:33.000000 causallib-0.9.4/causallib/estimation/marginal_outcome.py
--rw-rw-rw-   0        0        0    38742 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/estimation/matching.py
--rw-rw-rw-   0        0        0     7118 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/estimation/overlap_weights.py
--rw-rw-rw-   0        0        0     1919 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/estimation/README.md
--rw-rw-rw-   0        0        0    15805 2022-08-11 10:08:59.000000 causallib-0.9.4/causallib/estimation/rlearner.py
--rw-rw-rw-   0        0        0    16009 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/estimation/standardization.py
--rw-rw-rw-   0        0        0    16772 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/estimation/tmle.py
--rw-rw-rw-   0        0        0    15011 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/estimation/xlearner.py
--rw-rw-rw-   0        0        0      430 2022-07-18 08:01:06.000000 causallib-0.9.4/causallib/estimation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/evaluation/
--rw-rw-rw-   0        0        0     9384 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/evaluator.py
--rw-rw-rw-   0        0        0     4646 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/evaluation/plots/
--rw-rw-rw-   0        0        0    11572 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/plots/curve_data_makers.py
--rw-rw-rw-   0        0        0     8108 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/plots/data_extractors.py
--rw-rw-rw-   0        0        0    14523 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/plots/mixins.py
--rw-rw-rw-   0        0        0    39399 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/plots/plots.py
--rw-rw-rw-   0        0        0       51 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/plots/__init__.py
--rw-rw-rw-   0        0        0     9034 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/predictions.py
--rw-rw-rw-   0        0        0     8848 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/predictor.py
--rw-rw-rw-   0        0        0     5251 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/README.md
--rw-rw-rw-   0        0        0     7143 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/results.py
--rw-rw-rw-   0        0        0     6566 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/evaluation/scoring.py
--rw-rw-rw-   0        0        0      167 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/evaluation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/metrics/
--rw-rw-rw-   0        0        0     3334 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/outcome_metrics.py
--rw-rw-rw-   0        0        0     6426 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/propensity_metrics.py
--rw-rw-rw-   0        0        0     5043 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/scorers.py
--rw-rw-rw-   0        0        0     5076 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/weight_metrics.py
--rw-rw-rw-   0        0        0      370 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/model_selection/
--rw-rw-rw-   0        0        0     7665 2022-11-24 12:00:23.000000 causallib-0.9.4/causallib/model_selection/search.py
--rw-rw-rw-   0        0        0     2828 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/model_selection/split.py
--rw-rw-rw-   0        0        0      403 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/model_selection/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/preprocessing/
--rw-rw-rw-   0        0        0    14045 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/preprocessing/confounder_selection.py
--rw-rw-rw-   0        0        0     8420 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/preprocessing/filters.py
--rw-rw-rw-   0        0        0     1549 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/preprocessing/README.md
--rw-rw-rw-   0        0        0    22245 2021-10-21 13:13:46.000000 causallib-0.9.4/causallib/preprocessing/transformers.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.4/causallib/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2919 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/simulation/
--rw-rw-rw-   0        0        0   103090 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/simulation/CausalSimulator3.py
--rw-rw-rw-   0        0        0        0 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/simulation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/survival/
--rw-rw-rw-   0        0        0     2705 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/base_survival.py
--rw-rw-rw-   0        0        0      925 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/marginal_survival.py
--rw-rw-rw-   0        0        0     5921 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/regression_curve_fitter.py
--rw-rw-rw-   0        0        0     8700 2023-04-23 19:51:30.000000 causallib-0.9.4/causallib/survival/standardized_survival.py
--rw-rw-rw-   0        0        0    10306 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/survival_utils.py
--rw-rw-rw-   0        0        0     5538 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/univariate_curve_fitter.py
--rw-rw-rw-   0        0        0     5013 2023-05-02 13:20:05.000000 causallib-0.9.4/causallib/survival/weighted_standardized_survival.py
--rw-rw-rw-   0        0        0     5891 2022-11-24 12:00:23.000000 causallib-0.9.4/causallib/survival/weighted_survival.py
--rw-rw-rw-   0        0        0      584 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/survival/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/tests/
--rw-rw-rw-   0        0        0     1839 2023-02-15 16:03:50.000000 causallib-0.9.4/causallib/tests/survival_matching.py
--rw-rw-rw-   0        0        0     2154 2020-02-13 16:38:56.000000 causallib-0.9.4/causallib/tests/test_base_weight.py
--rw-rw-rw-   0        0        0    33941 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/tests/test_causal_simulator3.py
--rw-rw-rw-   0        0        0    18540 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/tests/test_confounder_selection.py
--rw-rw-rw-   0        0        0     7395 2023-05-02 12:28:47.000000 causallib-0.9.4/causallib/tests/test_datasets.py
--rw-rw-rw-   0        0        0    26809 2023-05-02 13:13:41.000000 causallib-0.9.4/causallib/tests/test_doublyrobust.py
--rw-rw-rw-   0        0        0     5694 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/tests/test_evaluation.py
--rw-rw-rw-   0        0        0     9634 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/tests/test_ipw.py
--rw-rw-rw-   0        0        0     1416 2020-02-13 16:38:56.000000 causallib-0.9.4/causallib/tests/test_marginal_outcome.py
--rw-rw-rw-   0        0        0    28672 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/tests/test_matching.py
--rw-rw-rw-   0        0        0    13540 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/tests/test_metrics.py
--rw-rw-rw-   0        0        0     4020 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/tests/test_overlap_weights.py
--rw-rw-rw-   0        0        0    10277 2023-03-29 12:20:56.000000 causallib-0.9.4/causallib/tests/test_plots.py
--rw-rw-rw-   0        0        0    17012 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/tests/test_rlearner.py
--rw-rw-rw-   0        0        0     7796 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/tests/test_scorers.py
--rw-rw-rw-   0        0        0    15776 2022-11-24 12:00:23.000000 causallib-0.9.4/causallib/tests/test_search.py
--rw-rw-rw-   0        0        0     6114 2022-09-29 12:38:27.000000 causallib-0.9.4/causallib/tests/test_split.py
--rw-rw-rw-   0        0        0    13848 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/tests/test_standardization.py
--rw-rw-rw-   0        0        0    32521 2023-05-02 13:49:18.000000 causallib-0.9.4/causallib/tests/test_survival.py
--rw-rw-rw-   0        0        0    17311 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/tests/test_tmle.py
--rw-rw-rw-   0        0        0     5124 2020-07-07 16:22:37.000000 causallib-0.9.4/causallib/tests/test_transformers.py
--rw-rw-rw-   0        0        0     4865 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/tests/test_utils.py
--rw-rw-rw-   0        0        0    18831 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/tests/test_xlearner.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.4/causallib/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:51:57.000000 causallib-0.9.4/causallib/utils/
--rw-rw-rw-   0        0        0     2343 2022-04-04 07:22:17.000000 causallib-0.9.4/causallib/utils/crossfit.py
--rw-rw-rw-   0        0        0     4530 2023-02-14 10:07:22.000000 causallib-0.9.4/causallib/utils/general_tools.py
--rw-rw-rw-   0        0        0     9194 2021-10-13 08:56:37.000000 causallib-0.9.4/causallib/utils/stat_utils.py
--rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.4/causallib/utils/__init__.py
--rw-rw-rw-   0        0        0       23 2023-05-02 13:50:06.000000 causallib-0.9.4/causallib/__init__.py
--rw-rw-rw-   0        0        0    11540 2020-07-07 16:22:37.000000 causallib-0.9.4/LICENSE
--rw-rw-rw-   0        0        0     7906 2023-05-02 13:51:57.000000 causallib-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0     6787 2023-03-29 12:38:12.000000 causallib-0.9.4/README.md
--rwxrwxrwx   0        0        0      176 2023-05-02 13:57:24.000000 causallib-0.9.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 13:51:57.000000 causallib-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     2792 2023-03-29 12:38:12.000000 causallib-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-22 12:38:58.000000 causallib-0.9.5/causallib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     7906 2023-06-22 12:38:58.000000 causallib-0.9.5/causallib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2023-06-22 12:38:58.000000 causallib-0.9.5/causallib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     4975 2023-06-22 12:38:58.000000 causallib-0.9.5/causallib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       10 2023-06-22 12:38:58.000000 causallib-0.9.5/causallib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/analysis/
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:29:37.000000 causallib-0.9.5/causallib/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/contrib/
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/contrib/adversarial_balancing/
+-rw-rw-rw-   0        0        0    15196 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/contrib/adversarial_balancing/adversarial_balancing.py
+-rw-rw-rw-   0        0        0     5550 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/contrib/adversarial_balancing/classifier_selection.py
+-rw-rw-rw-   0        0        0       57 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/contrib/adversarial_balancing/__init__.py
+-rw-rw-rw-   0        0        0     5032 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/contrib/faissknn.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/contrib/hemm/
+-rw-rw-rw-   0        0        0     7068 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/gen_synthetic_data.py
+-rw-rw-rw-   0        0        0    17729 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/hemm.py
+-rw-rw-rw-   0        0        0    10222 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/hemm_api.py
+-rw-rw-rw-   0        0        0     4453 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/hemm_metrics.py
+-rw-rw-rw-   0        0        0     2467 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/hemm_outcome_models.py
+-rw-rw-rw-   0        0        0     3692 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/hemm_utilities.py
+-rw-rw-rw-   0        0        0     4072 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/load_ihdp_data.py
+-rw-rw-rw-   0        0        0     1820 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/README.md
+-rw-rw-rw-   0        0        0       50 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/hemm/__init__.py
+-rw-rw-rw-   0        0        0     2786 2022-02-08 08:45:42.000000 causallib-0.9.5/causallib/contrib/README.md
+-rw-rw-rw-   0        0        0      109 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/contrib/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/contrib/shared_sparsity_selection/
+-rw-rw-rw-   0        0        0     8498 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py
+-rw-rw-rw-   0        0        0       74 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/contrib/shared_sparsity_selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/contrib/sklearn_scorer_wrapper/
+-rw-rw-rw-   0        0        0     1094 2023-06-22 10:32:05.000000 causallib-0.9.5/causallib/contrib/sklearn_scorer_wrapper/sklearn_scorer_wrapper.py
+-rw-rw-rw-   0        0        0       58 2023-06-22 10:32:05.000000 causallib-0.9.5/causallib/contrib/sklearn_scorer_wrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/contrib/tests/
+-rw-rw-rw-   0        0        0     7333 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/contrib/tests/test_adversarial_balancing.py
+-rw-rw-rw-   0        0        0     3722 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/tests/test_hemm.py
+-rw-rw-rw-   0        0        0     7325 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/contrib/tests/test_shared_sparsity_selection.py
+-rw-rw-rw-   0        0        0     2335 2023-06-22 10:48:08.000000 causallib-0.9.5/causallib/contrib/tests/test_sklearn_scorer_wrapper.py
+-rw-rw-rw-   0        0        0        0 2020-07-07 16:46:29.000000 causallib-0.9.5/causallib/contrib/tests/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-02-13 16:38:56.000000 causallib-0.9.5/causallib/contrib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/datasets/
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/datasets/data/
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/
+-rw-rw-rw-   0        0        0   702589 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/x.csv
+-rw-rw-rw-   0        0        0   344363 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_1.csv
+-rw-rw-rw-   0        0        0   357958 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_10.csv
+-rw-rw-rw-   0        0        0   338894 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_2.csv
+-rw-rw-rw-   0        0        0   347947 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_3.csv
+-rw-rw-rw-   0        0        0   346711 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_4.csv
+-rw-rw-rw-   0        0        0   353616 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_5.csv
+-rw-rw-rw-   0        0        0   349008 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_6.csv
+-rw-rw-rw-   0        0        0   351869 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_7.csv
+-rw-rw-rw-   0        0        0   340923 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_8.csv
+-rw-rw-rw-   0        0        0   346092 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_9.csv
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/datasets/data/nhefs/
+-rw-rw-rw-   0        0        0   366165 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/nhefs/NHEFS.csv
+-rw-rw-rw-   0        0        0     4125 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/data/nhefs/NHEFS_codebook.csv
+-rw-rw-rw-   0        0        0     9169 2023-06-22 11:18:40.000000 causallib-0.9.5/causallib/datasets/data_loader.py
+-rw-rw-rw-   0        0        0     5277 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/datasets/README.md
+-rw-rw-rw-   0        0        0      176 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/estimation/
+-rw-rw-rw-   0        0        0    11759 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/estimation/base_estimator.py
+-rw-rw-rw-   0        0        0     7794 2022-08-11 10:08:59.000000 causallib-0.9.5/causallib/estimation/base_weight.py
+-rw-rw-rw-   0        0        0    26241 2023-05-02 13:57:24.000000 causallib-0.9.5/causallib/estimation/doubly_robust.py
+-rw-rw-rw-   0        0        0    14022 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/estimation/ipw.py
+-rw-rw-rw-   0        0        0     3752 2021-08-26 08:37:33.000000 causallib-0.9.5/causallib/estimation/marginal_outcome.py
+-rw-rw-rw-   0        0        0    38742 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/estimation/matching.py
+-rw-rw-rw-   0        0        0     7118 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/estimation/overlap_weights.py
+-rw-rw-rw-   0        0        0     1919 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/estimation/README.md
+-rw-rw-rw-   0        0        0    15805 2022-08-11 10:08:59.000000 causallib-0.9.5/causallib/estimation/rlearner.py
+-rw-rw-rw-   0        0        0    16009 2023-02-14 10:07:22.000000 causallib-0.9.5/causallib/estimation/standardization.py
+-rw-rw-rw-   0        0        0    16772 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/estimation/tmle.py
+-rw-rw-rw-   0        0        0    15011 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/estimation/xlearner.py
+-rw-rw-rw-   0        0        0      430 2022-07-18 08:01:06.000000 causallib-0.9.5/causallib/estimation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/evaluation/
+-rw-rw-rw-   0        0        0     9384 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/evaluation/evaluator.py
+-rw-rw-rw-   0        0        0     4646 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/evaluation/metrics.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/evaluation/plots/
+-rw-rw-rw-   0        0        0    11572 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/evaluation/plots/curve_data_makers.py
+-rw-rw-rw-   0        0        0     8108 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/evaluation/plots/data_extractors.py
+-rw-rw-rw-   0        0        0    14523 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/evaluation/plots/mixins.py
+-rw-rw-rw-   0        0        0    39399 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/evaluation/plots/plots.py
+-rw-rw-rw-   0        0        0       51 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/evaluation/plots/__init__.py
+-rw-rw-rw-   0        0        0     9034 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/evaluation/predictions.py
+-rw-rw-rw-   0        0        0     8848 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/evaluation/predictor.py
+-rw-rw-rw-   0        0        0     5251 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/evaluation/README.md
+-rw-rw-rw-   0        0        0     7143 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/evaluation/results.py
+-rw-rw-rw-   0        0        0     6566 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/evaluation/scoring.py
+-rw-rw-rw-   0        0        0      167 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/evaluation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/metrics/
+-rw-rw-rw-   0        0        0     3349 2023-06-22 09:07:10.000000 causallib-0.9.5/causallib/metrics/outcome_metrics.py
+-rw-rw-rw-   0        0        0     6446 2023-06-22 10:00:31.000000 causallib-0.9.5/causallib/metrics/propensity_metrics.py
+-rw-rw-rw-   0        0        0     5242 2023-06-22 10:40:03.000000 causallib-0.9.5/causallib/metrics/scorers.py
+-rw-rw-rw-   0        0        0     5468 2023-06-22 09:17:13.000000 causallib-0.9.5/causallib/metrics/weight_metrics.py
+-rw-rw-rw-   0        0        0      431 2023-06-22 09:17:13.000000 causallib-0.9.5/causallib/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/model_selection/
+-rw-rw-rw-   0        0        0     7665 2022-11-24 12:00:23.000000 causallib-0.9.5/causallib/model_selection/search.py
+-rw-rw-rw-   0        0        0     2828 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/model_selection/split.py
+-rw-rw-rw-   0        0        0      403 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/model_selection/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/preprocessing/
+-rw-rw-rw-   0        0        0    14045 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/preprocessing/confounder_selection.py
+-rw-rw-rw-   0        0        0     8420 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/preprocessing/filters.py
+-rw-rw-rw-   0        0        0     1549 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/preprocessing/README.md
+-rw-rw-rw-   0        0        0    22245 2021-10-21 13:13:46.000000 causallib-0.9.5/causallib/preprocessing/transformers.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.5/causallib/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2919 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/simulation/
+-rw-rw-rw-   0        0        0   103090 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/simulation/CausalSimulator3.py
+-rw-rw-rw-   0        0        0        0 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/simulation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/survival/
+-rw-rw-rw-   0        0        0     2705 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/survival/base_survival.py
+-rw-rw-rw-   0        0        0      925 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/survival/marginal_survival.py
+-rw-rw-rw-   0        0        0     5921 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/survival/regression_curve_fitter.py
+-rw-rw-rw-   0        0        0     8700 2023-04-23 19:51:30.000000 causallib-0.9.5/causallib/survival/standardized_survival.py
+-rw-rw-rw-   0        0        0    10306 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/survival/survival_utils.py
+-rw-rw-rw-   0        0        0     5538 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/survival/univariate_curve_fitter.py
+-rw-rw-rw-   0        0        0     5013 2023-05-02 13:57:24.000000 causallib-0.9.5/causallib/survival/weighted_standardized_survival.py
+-rw-rw-rw-   0        0        0     5891 2022-11-24 12:00:23.000000 causallib-0.9.5/causallib/survival/weighted_survival.py
+-rw-rw-rw-   0        0        0      584 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/survival/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/tests/
+-rw-rw-rw-   0        0        0     1839 2023-02-15 16:03:50.000000 causallib-0.9.5/causallib/tests/survival_matching.py
+-rw-rw-rw-   0        0        0     2154 2020-02-13 16:38:56.000000 causallib-0.9.5/causallib/tests/test_base_weight.py
+-rw-rw-rw-   0        0        0    33941 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/tests/test_causal_simulator3.py
+-rw-rw-rw-   0        0        0    18540 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/tests/test_confounder_selection.py
+-rw-rw-rw-   0        0        0     7395 2023-05-02 12:28:47.000000 causallib-0.9.5/causallib/tests/test_datasets.py
+-rw-rw-rw-   0        0        0    26809 2023-05-02 13:57:24.000000 causallib-0.9.5/causallib/tests/test_doublyrobust.py
+-rw-rw-rw-   0        0        0     5694 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/tests/test_evaluation.py
+-rw-rw-rw-   0        0        0     9634 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/tests/test_ipw.py
+-rw-rw-rw-   0        0        0     1416 2020-02-13 16:38:56.000000 causallib-0.9.5/causallib/tests/test_marginal_outcome.py
+-rw-rw-rw-   0        0        0    28672 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/tests/test_matching.py
+-rw-rw-rw-   0        0        0    14500 2023-06-22 09:38:33.000000 causallib-0.9.5/causallib/tests/test_metrics.py
+-rw-rw-rw-   0        0        0     4020 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/tests/test_overlap_weights.py
+-rw-rw-rw-   0        0        0    10277 2023-03-29 12:20:56.000000 causallib-0.9.5/causallib/tests/test_plots.py
+-rw-rw-rw-   0        0        0    17012 2023-02-14 10:07:22.000000 causallib-0.9.5/causallib/tests/test_rlearner.py
+-rw-rw-rw-   0        0        0     8919 2023-06-22 11:18:40.000000 causallib-0.9.5/causallib/tests/test_scorers.py
+-rw-rw-rw-   0        0        0    15776 2022-11-24 12:00:23.000000 causallib-0.9.5/causallib/tests/test_search.py
+-rw-rw-rw-   0        0        0     6114 2022-09-29 12:38:27.000000 causallib-0.9.5/causallib/tests/test_split.py
+-rw-rw-rw-   0        0        0    13848 2023-02-14 10:07:22.000000 causallib-0.9.5/causallib/tests/test_standardization.py
+-rw-rw-rw-   0        0        0    32521 2023-05-02 13:57:24.000000 causallib-0.9.5/causallib/tests/test_survival.py
+-rw-rw-rw-   0        0        0    17311 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/tests/test_tmle.py
+-rw-rw-rw-   0        0        0     5124 2020-07-07 16:22:37.000000 causallib-0.9.5/causallib/tests/test_transformers.py
+-rw-rw-rw-   0        0        0     4865 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/tests/test_utils.py
+-rw-rw-rw-   0        0        0    18831 2023-02-14 10:07:22.000000 causallib-0.9.5/causallib/tests/test_xlearner.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.5/causallib/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 12:38:59.000000 causallib-0.9.5/causallib/utils/
+-rw-rw-rw-   0        0        0     2343 2022-04-04 07:22:17.000000 causallib-0.9.5/causallib/utils/crossfit.py
+-rw-rw-rw-   0        0        0     4530 2023-02-14 10:07:22.000000 causallib-0.9.5/causallib/utils/general_tools.py
+-rw-rw-rw-   0        0        0     9194 2021-10-13 08:56:37.000000 causallib-0.9.5/causallib/utils/stat_utils.py
+-rw-rw-rw-   0        0        0        0 2019-07-12 06:26:48.000000 causallib-0.9.5/causallib/utils/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-22 11:18:40.000000 causallib-0.9.5/causallib/__init__.py
+-rw-rw-rw-   0        0        0    11540 2020-07-07 16:22:37.000000 causallib-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0     7906 2023-06-22 12:38:59.000000 causallib-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6787 2023-03-29 12:38:12.000000 causallib-0.9.5/README.md
+-rwxrwxrwx   0        0        0      176 2023-05-02 13:57:24.000000 causallib-0.9.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 12:38:59.000000 causallib-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     2792 2023-03-29 12:38:12.000000 causallib-0.9.5/setup.py
```

### Comparing `causallib-0.9.4/causallib.egg-info/PKG-INFO` & `causallib-0.9.5/causallib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causallib
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Python package for flexible and modular causal inference modeling
 Home-page: https://github.com/BiomedSciAI/causallib
 Author: Causal Machine Learning for Healthcare and Life Sciences, IBM Research Israel
 License: Apache License 2.0
 Project-URL: Documentation, https://causallib.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BiomedSciAI/causallib
 Project-URL: Bug Tracker, https://github.com/BiomedSciAI/causallib/issues
```

### Comparing `causallib-0.9.4/causallib.egg-info/SOURCES.txt` & `causallib-0.9.5/causallib.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,18 +23,21 @@
 causallib/contrib/hemm/hemm_api.py
 causallib/contrib/hemm/hemm_metrics.py
 causallib/contrib/hemm/hemm_outcome_models.py
 causallib/contrib/hemm/hemm_utilities.py
 causallib/contrib/hemm/load_ihdp_data.py
 causallib/contrib/shared_sparsity_selection/__init__.py
 causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py
+causallib/contrib/sklearn_scorer_wrapper/__init__.py
+causallib/contrib/sklearn_scorer_wrapper/sklearn_scorer_wrapper.py
 causallib/contrib/tests/__init__.py
 causallib/contrib/tests/test_adversarial_balancing.py
 causallib/contrib/tests/test_hemm.py
 causallib/contrib/tests/test_shared_sparsity_selection.py
+causallib/contrib/tests/test_sklearn_scorer_wrapper.py
 causallib/datasets/README.md
 causallib/datasets/__init__.py
 causallib/datasets/data_loader.py
 causallib/datasets/data/acic_challenge_2016/x.csv
 causallib/datasets/data/acic_challenge_2016/zymu_1.csv
 causallib/datasets/data/acic_challenge_2016/zymu_10.csv
 causallib/datasets/data/acic_challenge_2016/zymu_2.csv
```

### Comparing `causallib-0.9.4/causallib/contrib/adversarial_balancing/adversarial_balancing.py` & `causallib-0.9.5/causallib/contrib/adversarial_balancing/adversarial_balancing.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/adversarial_balancing/classifier_selection.py` & `causallib-0.9.5/causallib/contrib/adversarial_balancing/classifier_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/faissknn.py` & `causallib-0.9.5/causallib/contrib/faissknn.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/hemm/gen_synthetic_data.py` & `causallib-0.9.5/causallib/contrib/hemm/gen_synthetic_data.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/hemm/hemm.py` & `causallib-0.9.5/causallib/contrib/hemm/hemm.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/hemm/hemm_api.py` & `causallib-0.9.5/causallib/contrib/hemm/hemm_api.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/hemm/hemm_metrics.py` & `causallib-0.9.5/causallib/contrib/hemm/hemm_metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/hemm/hemm_outcome_models.py` & `causallib-0.9.5/causallib/contrib/hemm/hemm_outcome_models.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/hemm/hemm_utilities.py` & `causallib-0.9.5/causallib/contrib/hemm/hemm_utilities.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/hemm/load_ihdp_data.py` & `causallib-0.9.5/causallib/contrib/hemm/load_ihdp_data.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/hemm/README.md` & `causallib-0.9.5/causallib/contrib/hemm/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/README.md` & `causallib-0.9.5/causallib/contrib/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py` & `causallib-0.9.5/causallib/contrib/shared_sparsity_selection/shared_sparsity_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/tests/test_adversarial_balancing.py` & `causallib-0.9.5/causallib/contrib/tests/test_adversarial_balancing.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/tests/test_hemm.py` & `causallib-0.9.5/causallib/contrib/tests/test_hemm.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/contrib/tests/test_shared_sparsity_selection.py` & `causallib-0.9.5/causallib/contrib/tests/test_shared_sparsity_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/x.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/x.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_1.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_1.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_10.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_10.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_2.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_2.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_3.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_3.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_4.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_4.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_5.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_5.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_6.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_6.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_7.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_7.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_8.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_8.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/acic_challenge_2016/zymu_9.csv` & `causallib-0.9.5/causallib/datasets/data/acic_challenge_2016/zymu_9.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/nhefs/NHEFS.csv` & `causallib-0.9.5/causallib/datasets/data/nhefs/NHEFS.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data/nhefs/NHEFS_codebook.csv` & `causallib-0.9.5/causallib/datasets/data/nhefs/NHEFS_codebook.csv`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/datasets/data_loader.py` & `causallib-0.9.5/causallib/datasets/data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,15 @@
         a (pd.Series): Treatment assignment of size (num_subjects,). Quit smoking vs. non-quit.
         t (pd.Series): Followup duration, size (num_subjects,).
         y (pd.Series): Observed outcome (1) or right censoring event (0), size (num_subjects,).
     """
     nhefs_all = load_nhefs(raw=True)[0]
     t = (nhefs_all["yrdth"] - 83) * 12 + nhefs_all["modth"]
     t = t.fillna(120)
+    t = t.rename("longevity")
     y = nhefs_all["death"]
 
     nhefs = load_nhefs(augment=augment, onehot=onehot, restrict=False)
     a = nhefs.a
     X = nhefs.X
 
     data = Bunch(X=X, a=a, t=t, y=y, descriptors=nhefs.descriptors)
```

### Comparing `causallib-0.9.4/causallib/datasets/README.md` & `causallib-0.9.5/causallib/datasets/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/base_estimator.py` & `causallib-0.9.5/causallib/estimation/base_estimator.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/base_weight.py` & `causallib-0.9.5/causallib/estimation/base_weight.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/doubly_robust.py` & `causallib-0.9.5/causallib/estimation/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/ipw.py` & `causallib-0.9.5/causallib/estimation/ipw.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/marginal_outcome.py` & `causallib-0.9.5/causallib/estimation/marginal_outcome.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/matching.py` & `causallib-0.9.5/causallib/estimation/matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/overlap_weights.py` & `causallib-0.9.5/causallib/estimation/overlap_weights.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/README.md` & `causallib-0.9.5/causallib/estimation/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/rlearner.py` & `causallib-0.9.5/causallib/estimation/rlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/standardization.py` & `causallib-0.9.5/causallib/estimation/standardization.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/tmle.py` & `causallib-0.9.5/causallib/estimation/tmle.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/estimation/xlearner.py` & `causallib-0.9.5/causallib/estimation/xlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/evaluator.py` & `causallib-0.9.5/causallib/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/metrics.py` & `causallib-0.9.5/causallib/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/plots/curve_data_makers.py` & `causallib-0.9.5/causallib/evaluation/plots/curve_data_makers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/plots/data_extractors.py` & `causallib-0.9.5/causallib/evaluation/plots/data_extractors.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/plots/mixins.py` & `causallib-0.9.5/causallib/evaluation/plots/mixins.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/plots/plots.py` & `causallib-0.9.5/causallib/evaluation/plots/plots.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/predictions.py` & `causallib-0.9.5/causallib/evaluation/predictions.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/predictor.py` & `causallib-0.9.5/causallib/evaluation/predictor.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/README.md` & `causallib-0.9.5/causallib/evaluation/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/results.py` & `causallib-0.9.5/causallib/evaluation/results.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/evaluation/scoring.py` & `causallib-0.9.5/causallib/evaluation/scoring.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/metrics/outcome_metrics.py` & `causallib-0.9.5/causallib/metrics/outcome_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     return potential_outcomes
 
 
 def balanced_residuals_error(
     y_true, y_pred, a_true,
     distance_metric=abs_standardized_mean_difference,
     distance_metric_kwargs=None,
+    **kwargs,
 ):
     """Computes how different is the residuals distribution of the control group
     from that of the treatment group.
     Residuals are based on the observed (factual) outcome prediction.
 
     Can plug in any uni-variate two-sample test function.
```

### Comparing `causallib-0.9.4/causallib/metrics/propensity_metrics.py` & `causallib-0.9.5/causallib/metrics/propensity_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import numpy as np
 from numpy import interp
 from sklearn.metrics import roc_auc_score, roc_curve
 import statsmodels.api as sm
 
 
-def weighted_roc_auc_error(y_true, y_pred, sample_weight):
+def weighted_roc_auc_error(y_true, y_pred, sample_weight, **kwargs):
     """
     Compute the squared error between the balanced (e.g. IP-weighted) ROC AUC
     to the diagonal, i.e. AUC=0.5.
 
     Shimoni, Y., et al. (2019)
     An evaluation toolkit to guide model selection and cohort definition in causal inference.
 
@@ -60,15 +60,15 @@
     expected_auc = roc_auc_score(target, p, sample_weight=w)
 
     auc = roc_auc_score(y_true, y_pred)
     score = (expected_auc - auc) ** 2
     return score
 
 
-def weighted_roc_curve_error(y_true, y_pred, sample_weight, agg=np.max):
+def weighted_roc_curve_error(y_true, y_pred, sample_weight, agg=np.max, **kwargs):
     """Compute the absolute differences between the balanced (e.g. IP-weighted) ROC curve
     and the diagonal x=y curve.
     Since difference in curves results in a multiple values (each point along the curve),
     an aggregation function is also required.
 
     Shimoni, Y., et al. (2019)
     An evaluation toolkit to guide model selection and cohort definition in causal inference.
```

### Comparing `causallib-0.9.4/causallib/metrics/scorers.py` & `causallib-0.9.5/causallib/metrics/scorers.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,16 +88,21 @@
         return score
 
 
 covariate_balancing_error_scorer = WeightScorerBase(
     weight_metrics.covariate_balancing_error, -1,
 )
 
+covariate_imbalance_count_error_scorer = WeightScorerBase(
+    weight_metrics.covariate_imbalance_count_error, -1,
+)
+
 _WEIGHT_SCORERS = dict(
     covariate_balancing_error=covariate_balancing_error_scorer,
+    covariate_imbalance_count_error=covariate_imbalance_count_error_scorer,
 )
 
 
 class OutcomeScorerBase(_BaseCausalScorer):
     def _score(self, estimator, X, a, y, sample_weight=None, **kwargs):
         potential_outcomes_pred = estimator.estimate_individual_outcome(X, a)
         score = self._score_func(
```

### Comparing `causallib-0.9.4/causallib/metrics/weight_metrics.py` & `causallib-0.9.5/causallib/metrics/weight_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,16 +97,15 @@
     w_treated = w.loc[cur_treated_mask]
     x_untreated = x.loc[~cur_treated_mask]
     w_untreated = w.loc[~cur_treated_mask]
     distribution_distance = metric(x_treated, x_untreated, w_treated, w_untreated)
     return distribution_distance
 
 
-
-def covariate_balancing_error(X, a, sample_weight, agg=max):
+def covariate_balancing_error(X, a, sample_weight, agg=max, **kwargs):
     """Computes the weighted (i.e. balanced) absolute standardized mean difference
     of every covariate in X.
 
     Args:
         X (pd.DataFrame): Covariate matrix.
         a (pd.Series): Treatment assignment vector.
         sample_weight (pd.Series): Weights balancing between the treatment groups.
@@ -116,7 +115,19 @@
     Returns:
         score (float):
     """
     asmds = calculate_covariate_balance(X, a, sample_weight, metric="abs_smd")
     weighted_asmds = asmds["weighted"]
     score = agg(weighted_asmds)
     return score
+
+
+def covariate_imbalance_count_error(
+    X, a, sample_weight, threshold=0.1, fraction=True
+) -> float:
+    asmds = calculate_covariate_balance(X, a, sample_weight, metric="abs_smd")
+    weighted_asmds = asmds["weighted"]
+    is_violating = weighted_asmds > threshold
+    score = sum(is_violating)
+    if fraction:
+        score /= is_violating.shape[0]
+    return score
```

### Comparing `causallib-0.9.4/causallib/model_selection/search.py` & `causallib-0.9.5/causallib/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/model_selection/split.py` & `causallib-0.9.5/causallib/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/preprocessing/confounder_selection.py` & `causallib-0.9.5/causallib/preprocessing/confounder_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/preprocessing/filters.py` & `causallib-0.9.5/causallib/preprocessing/filters.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/preprocessing/README.md` & `causallib-0.9.5/causallib/preprocessing/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/preprocessing/transformers.py` & `causallib-0.9.5/causallib/preprocessing/transformers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/README.md` & `causallib-0.9.5/causallib/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/simulation/CausalSimulator3.py` & `causallib-0.9.5/causallib/simulation/CausalSimulator3.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/base_survival.py` & `causallib-0.9.5/causallib/survival/base_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/marginal_survival.py` & `causallib-0.9.5/causallib/survival/marginal_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/regression_curve_fitter.py` & `causallib-0.9.5/causallib/survival/regression_curve_fitter.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/standardized_survival.py` & `causallib-0.9.5/causallib/survival/standardized_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/survival_utils.py` & `causallib-0.9.5/causallib/survival/survival_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/univariate_curve_fitter.py` & `causallib-0.9.5/causallib/survival/univariate_curve_fitter.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/weighted_standardized_survival.py` & `causallib-0.9.5/causallib/survival/weighted_standardized_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/weighted_survival.py` & `causallib-0.9.5/causallib/survival/weighted_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/survival/__init__.py` & `causallib-0.9.5/causallib/survival/__init__.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/survival_matching.py` & `causallib-0.9.5/causallib/tests/survival_matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_base_weight.py` & `causallib-0.9.5/causallib/tests/test_base_weight.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_causal_simulator3.py` & `causallib-0.9.5/causallib/tests/test_causal_simulator3.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_confounder_selection.py` & `causallib-0.9.5/causallib/tests/test_confounder_selection.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_datasets.py` & `causallib-0.9.5/causallib/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_doublyrobust.py` & `causallib-0.9.5/causallib/tests/test_doublyrobust.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_evaluation.py` & `causallib-0.9.5/causallib/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_ipw.py` & `causallib-0.9.5/causallib/tests/test_ipw.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_marginal_outcome.py` & `causallib-0.9.5/causallib/tests/test_marginal_outcome.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_matching.py` & `causallib-0.9.5/causallib/tests/test_matching.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_metrics.py` & `causallib-0.9.5/causallib/tests/test_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from sklearn.datasets import make_classification
 from sklearn.linear_model import LogisticRegression, LinearRegression
 
 from causallib.metrics import weighted_roc_auc_error, expected_roc_auc_error
 from causallib.metrics import weighted_roc_curve_error, expected_roc_curve_error
 from causallib.metrics import ici_error
 from causallib.metrics import covariate_balancing_error
+from causallib.metrics import covariate_imbalance_count_error
 from causallib.metrics import balanced_residuals_error
 
 
 class TestPropensityMetrics(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         # Data:
@@ -271,14 +272,36 @@
             score = covariate_balancing_error(
                 self.data["X"], self.data["a"], self.data["w"],
                 agg=np.mean,
             )
             expected /= 2  # Two features, the second has 0 ASMD
             self.assertAlmostEqual(score, expected, places=4)
 
+    def test_covariate_imbalance_count(self):
+        with self.subTest("High violation threshold"):
+            score = covariate_imbalance_count_error(
+                self.data["X"], self.data["a"], self.data["w"],
+                threshold=10,
+            )
+            self.assertEqual(score, 0)
+
+        with self.subTest("Low violation threshold"):
+            score = covariate_imbalance_count_error(
+                self.data["X"], self.data["a"], self.data["w"],
+                threshold=-0.1, fraction=False,
+            )
+            self.assertEqual(score, self.data["X"].shape[1])
+
+        with self.subTest("Fraction violation threshold"):
+            score = covariate_imbalance_count_error(
+                self.data["X"], self.data["a"], self.data["w"],
+                threshold=0.1, fraction=True,
+            )
+            self.assertEqual(score, 1/2)
+
 
 class TestOutcomeMetrics(unittest.TestCase):
     def test_balanced_residuals(self):
         a = pd.Series([0]*5 + [1]*6)  # Unequal group sizes
         y = pd.Series([8, 9, 10, 11, 12,
                        18, 19, 20, 20, 21, 22])
         y_pred = pd.DataFrame({  # Will only use the observed predictions
```

### Comparing `causallib-0.9.4/causallib/tests/test_overlap_weights.py` & `causallib-0.9.5/causallib/tests/test_overlap_weights.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_plots.py` & `causallib-0.9.5/causallib/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_rlearner.py` & `causallib-0.9.5/causallib/tests/test_rlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_scorers.py` & `causallib-0.9.5/causallib/tests/test_scorers.py`

 * *Files 19% similar despite different names*

```diff
@@ -137,14 +137,41 @@
         score_agg_min = scorer(
             self.estimator,
             self.data['X'], self.data['a'], self.data['y'],
             agg=np.min,
         )
         self.assertLess(-score_agg_min, -score_default)  # Default is max. Scores are negative metrics values
 
+    def test_covariate_imbalance_count_error(self):
+        X = pd.DataFrame(
+            {
+                "imbalanced": [5, 5, 5, 5, 4, 6, 0, 0, 0, 0, -1, 1],
+                "balanced": [5, 5, 5, 5, 4, 6, 5, 5, 5, 5, 4, 6],
+            }
+        )
+        a = pd.Series([1] * 6 + [0] * 6)
+        ipw = IPW(LogisticRegression())
+        ipw.fit(X, a)
+
+        with self.subTest("Count score"):
+            scorer = get_scorer("covariate_imbalance_count_error")
+            score = scorer(ipw, X, a, y_true=None, fraction=False)
+            self.assertEqual(score, -1)
+
+        with self.subTest("Fractional score"):
+            scorer = get_scorer("covariate_imbalance_count_error")
+            score = scorer(ipw, X, a, y_true=None, fraction=True)
+            self.assertEqual(score, -0.5)
+
+        with self.subTest("Non-default threshold"):
+            threshold = 10  # Should result in not violating features
+            scorer = get_scorer("covariate_imbalance_count_error")
+            score = scorer(ipw, X, a, y_true=None, threshold=threshold)
+            self.assertEqual(score, 0)
+
 
 class TestOutcomeScorer(BaseTestScorer):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.estimator = StratifiedStandardization(LinearRegression())
```

### Comparing `causallib-0.9.4/causallib/tests/test_search.py` & `causallib-0.9.5/causallib/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_split.py` & `causallib-0.9.5/causallib/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_standardization.py` & `causallib-0.9.5/causallib/tests/test_standardization.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_survival.py` & `causallib-0.9.5/causallib/tests/test_survival.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_tmle.py` & `causallib-0.9.5/causallib/tests/test_tmle.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_transformers.py` & `causallib-0.9.5/causallib/tests/test_transformers.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_utils.py` & `causallib-0.9.5/causallib/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/tests/test_xlearner.py` & `causallib-0.9.5/causallib/tests/test_xlearner.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/utils/crossfit.py` & `causallib-0.9.5/causallib/utils/crossfit.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/utils/general_tools.py` & `causallib-0.9.5/causallib/utils/general_tools.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/causallib/utils/stat_utils.py` & `causallib-0.9.5/causallib/utils/stat_utils.py`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/LICENSE` & `causallib-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/PKG-INFO` & `causallib-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causallib
-Version: 0.9.4
+Version: 0.9.5
 Summary: A Python package for flexible and modular causal inference modeling
 Home-page: https://github.com/BiomedSciAI/causallib
 Author: Causal Machine Learning for Healthcare and Life Sciences, IBM Research Israel
 License: Apache License 2.0
 Project-URL: Documentation, https://causallib.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/BiomedSciAI/causallib
 Project-URL: Bug Tracker, https://github.com/BiomedSciAI/causallib/issues
```

### Comparing `causallib-0.9.4/README.md` & `causallib-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `causallib-0.9.4/setup.py` & `causallib-0.9.5/setup.py`

 * *Files identical despite different names*

