# Comparing `tmp/rsmtool-9.0.1.tar.gz` & `tmp/rsmtool-9.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsmtool-9.0.1.tar", last modified: Tue Dec  6 22:16:57 2022, max compression
+gzip compressed data, was "rsmtool-9.1.1.tar", last modified: Fri Jan 20 19:02:06 2023, max compression
```

## Comparing `rsmtool-9.0.1.tar` & `rsmtool-9.1.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.961780 rsmtool-9.0.1/
--rw-r--r--   0 nmadnani   (501) staff       (20)    11358 2021-10-27 17:25:11.000000 rsmtool-9.0.1/LICENSE
--rw-r--r--   0 nmadnani   (501) staff       (20)      186 2022-12-06 22:06:29.000000 rsmtool-9.0.1/MANIFEST.in
--rw-r--r--   0 nmadnani   (501) staff       (20)     5872 2022-12-06 22:16:57.961881 rsmtool-9.0.1/PKG-INFO
--rw-r--r--   0 nmadnani   (501) staff       (20)     5046 2022-12-06 20:30:13.000000 rsmtool-9.0.1/README.rst
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.953277 rsmtool-9.0.1/rsmtool/
--rw-r--r--   0 nmadnani   (501) staff       (20)     1417 2022-09-21 17:34:41.000000 rsmtool-9.0.1/rsmtool/__init__.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    87373 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/analyzer.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    31358 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/comparer.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    40740 2022-12-06 20:25:40.000000 rsmtool-9.0.1/rsmtool/configuration_parser.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    11212 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/container.py
--rw-r--r--   0 nmadnani   (501) staff       (20)     2985 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/convert_feature_json.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    11287 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/fairness_utils.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    57766 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/modeler.py
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.956921 rsmtool-9.0.1/rsmtool/notebooks/
--rw-r--r--   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:14:57.000000 rsmtool-9.0.1/rsmtool/notebooks/__init__.py
--rw-r--r--   0 nmadnani   (501) staff       (20)     8847 2022-07-19 21:54:27.000000 rsmtool-9.0.1/rsmtool/notebooks/builtin_model.ipynb
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.958676 rsmtool-9.0.1/rsmtool/notebooks/comparison/
--rw-r--r--   0 nmadnani   (501) staff       (20)     7017 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/consistency.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     3477 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/evaluation.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     4551 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/feature_descriptives.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     2718 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/features_by_group.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1865 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/footer.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)    17443 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/header.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     2824 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/model.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     2053 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/notes.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1849 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/pca.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     4077 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/preprocessed_features.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1568 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/preprocessed_features_by_group.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     2837 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/score_distributions.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1910 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/sysinfo.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     2782 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/comparison/true_score_evaluation.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     8061 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/consistency.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     6749 2022-07-19 21:54:27.000000 rsmtool-9.0.1/rsmtool/notebooks/data_description.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1879 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/data_description_by_group.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     5646 2022-02-25 18:44:13.000000 rsmtool-9.0.1/rsmtool/notebooks/dff_by_group.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     8532 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/evaluation.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     6598 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/evaluation_by_group.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)    12749 2022-12-01 21:36:53.000000 rsmtool-9.0.1/rsmtool/notebooks/fairness_analyses.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     5450 2022-11-01 18:04:08.000000 rsmtool-9.0.1/rsmtool/notebooks/feature_descriptives.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     6388 2022-05-28 18:00:52.000000 rsmtool-9.0.1/rsmtool/notebooks/features_by_group.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1833 2022-07-19 21:54:27.000000 rsmtool-9.0.1/rsmtool/notebooks/footer.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)    16983 2022-07-21 16:53:05.000000 rsmtool-9.0.1/rsmtool/notebooks/header.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1090 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/intermediate_file_paths.ipynb
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.958833 rsmtool-9.0.1/rsmtool/notebooks/javascript/
--rw-r--r--   0 nmadnani   (501) staff       (20)     7587 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/javascript/sort.js
--rw-r--r--   0 nmadnani   (501) staff       (20)     2674 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/pca.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)    14602 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/preprocessed_features.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     3817 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/skll_model.ipynb
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.959870 rsmtool-9.0.1/rsmtool/notebooks/summary/
--rw-r--r--   0 nmadnani   (501) staff       (20)     8141 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/summary/evaluation.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1833 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/summary/footer.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     7881 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/notebooks/summary/header.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1285 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/summary/intermediate_file_paths.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     6166 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/summary/model.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     3844 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/summary/preprocessed_features.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1907 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/summary/sysinfo.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     4469 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/summary/true_score_evaluation.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)     1907 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/sysinfo.ipynb
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.960000 rsmtool-9.0.1/rsmtool/notebooks/templates/
--rw-r--r--   0 nmadnani   (501) staff       (20)      123 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/templates/report.tpl
--rw-r--r--   0 nmadnani   (501) staff       (20)     7601 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/notebooks/true_score_evaluation.ipynb
--rw-r--r--   0 nmadnani   (501) staff       (20)   121085 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/preprocessor.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    13678 2022-02-22 14:09:48.000000 rsmtool-9.0.1/rsmtool/reader.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    37085 2022-12-02 19:20:56.000000 rsmtool-9.0.1/rsmtool/reporter.py
--rw-r--r--   0 nmadnani   (501) staff       (20)     9457 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/rsmcompare.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    11494 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/rsmeval.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    12985 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/rsmpredict.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    12099 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/rsmsummarize.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    16607 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/rsmtool.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    13480 2022-12-05 15:05:15.000000 rsmtool-9.0.1/rsmtool/rsmxval.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    66934 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/test_utils.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    15732 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/transformer.py
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.961587 rsmtool-9.0.1/rsmtool/utils/
--rw-r--r--   0 nmadnani   (501) staff       (20)        0 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/utils/__init__.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    40279 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/utils/commandline.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    17565 2022-09-21 17:34:41.000000 rsmtool-9.0.1/rsmtool/utils/constants.py
--rw-r--r--   0 nmadnani   (501) staff       (20)      887 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/utils/conversion.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    10277 2022-12-06 15:21:28.000000 rsmtool-9.0.1/rsmtool/utils/cross_validation.py
--rw-r--r--   0 nmadnani   (501) staff       (20)     4090 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/utils/files.py
--rw-r--r--   0 nmadnani   (501) staff       (20)     3770 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/utils/logging.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    18149 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/utils/metrics.py
--rw-r--r--   0 nmadnani   (501) staff       (20)     1988 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/utils/models.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    12455 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/utils/notebook.py
--rw-r--r--   0 nmadnani   (501) staff       (20)    11984 2021-10-27 17:25:11.000000 rsmtool-9.0.1/rsmtool/utils/prmse.py
--rw-r--r--   0 nmadnani   (501) staff       (20)      237 2022-12-06 20:25:40.000000 rsmtool-9.0.1/rsmtool/version.py
--rw-r--r--   0 nmadnani   (501) staff       (20)     8657 2022-03-10 02:09:19.000000 rsmtool-9.0.1/rsmtool/writer.py
-drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2022-12-06 22:16:57.954357 rsmtool-9.0.1/rsmtool.egg-info/
--rw-r--r--   0 nmadnani   (501) staff       (20)     5872 2022-12-06 22:16:57.000000 rsmtool-9.0.1/rsmtool.egg-info/PKG-INFO
--rw-r--r--   0 nmadnani   (501) staff       (20)     2877 2022-12-06 22:16:57.000000 rsmtool-9.0.1/rsmtool.egg-info/SOURCES.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)        1 2022-12-06 22:16:57.000000 rsmtool-9.0.1/rsmtool.egg-info/dependency_links.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)      323 2022-12-06 22:16:57.000000 rsmtool-9.0.1/rsmtool.egg-info/entry_points.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)        1 2022-12-06 22:08:33.000000 rsmtool-9.0.1/rsmtool.egg-info/not-zip-safe
--rw-r--r--   0 nmadnani   (501) staff       (20)      165 2022-12-06 22:16:57.000000 rsmtool-9.0.1/rsmtool.egg-info/requires.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)        8 2022-12-06 22:16:57.000000 rsmtool-9.0.1/rsmtool.egg-info/top_level.txt
--rw-r--r--   0 nmadnani   (501) staff       (20)      116 2022-12-06 22:16:57.963225 rsmtool-9.0.1/setup.cfg
--rw-r--r--   0 nmadnani   (501) staff       (20)     2202 2022-12-06 22:16:39.000000 rsmtool-9.0.1/setup.py
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.445324 rsmtool-9.1.1/
+-rw-r--r--   0 nmadnani   (501) staff       (20)    11358 2021-10-27 17:25:11.000000 rsmtool-9.1.1/LICENSE
+-rw-r--r--   0 nmadnani   (501) staff       (20)      211 2023-01-20 18:38:43.000000 rsmtool-9.1.1/MANIFEST.in
+-rw-r--r--   0 nmadnani   (501) staff       (20)     5872 2023-01-20 19:02:06.445410 rsmtool-9.1.1/PKG-INFO
+-rw-r--r--   0 nmadnani   (501) staff       (20)     5046 2023-01-19 21:34:37.000000 rsmtool-9.1.1/README.rst
+-rw-r--r--   0 nmadnani   (501) staff       (20)      178 2023-01-19 21:32:32.000000 rsmtool-9.1.1/requirements.txt
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.436036 rsmtool-9.1.1/rsmtool/
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1395 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/__init__.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    80979 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/analyzer.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    26498 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/comparer.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    39294 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/configuration_parser.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    10984 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/container.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)     2712 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/convert_feature_json.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    10314 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/fairness_utils.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    55813 2023-01-19 21:32:32.000000 rsmtool-9.1.1/rsmtool/modeler.py
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.441367 rsmtool-9.1.1/rsmtool/notebooks/
+-rw-r--r--   0 nmadnani   (501) staff       (20)     8847 2022-07-19 21:54:27.000000 rsmtool-9.1.1/rsmtool/notebooks/builtin_model.ipynb
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.443444 rsmtool-9.1.1/rsmtool/notebooks/comparison/
+-rw-r--r--   0 nmadnani   (501) staff       (20)     7017 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/consistency.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     3477 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/evaluation.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     4551 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/feature_descriptives.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     2718 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/features_by_group.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1865 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/footer.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)    17443 2022-03-10 02:09:19.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/header.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     2824 2022-03-10 02:09:19.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/model.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     2053 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/notes.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1849 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/pca.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     4077 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/preprocessed_features.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1568 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/preprocessed_features_by_group.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     2837 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/score_distributions.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1910 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/sysinfo.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     2782 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/comparison/true_score_evaluation.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     8061 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/consistency.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     6749 2022-07-19 21:54:27.000000 rsmtool-9.1.1/rsmtool/notebooks/data_description.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1879 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/data_description_by_group.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     5646 2022-02-25 18:44:13.000000 rsmtool-9.1.1/rsmtool/notebooks/dff_by_group.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     8532 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/evaluation.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     6598 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/evaluation_by_group.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)    12749 2022-12-01 21:36:53.000000 rsmtool-9.1.1/rsmtool/notebooks/fairness_analyses.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     5450 2022-11-01 18:04:08.000000 rsmtool-9.1.1/rsmtool/notebooks/feature_descriptives.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     6388 2022-05-28 18:00:52.000000 rsmtool-9.1.1/rsmtool/notebooks/features_by_group.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1833 2022-07-19 21:54:27.000000 rsmtool-9.1.1/rsmtool/notebooks/footer.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)    16983 2022-07-21 16:53:05.000000 rsmtool-9.1.1/rsmtool/notebooks/header.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1090 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/intermediate_file_paths.ipynb
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.443599 rsmtool-9.1.1/rsmtool/notebooks/javascript/
+-rw-r--r--   0 nmadnani   (501) staff       (20)     7587 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/javascript/sort.js
+-rw-r--r--   0 nmadnani   (501) staff       (20)     2674 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/pca.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)    14602 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/preprocessed_features.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     3817 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/skll_model.ipynb
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.444801 rsmtool-9.1.1/rsmtool/notebooks/summary/
+-rw-r--r--   0 nmadnani   (501) staff       (20)     8141 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/summary/evaluation.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1833 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/summary/footer.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     7881 2022-03-10 02:09:19.000000 rsmtool-9.1.1/rsmtool/notebooks/summary/header.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1285 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/summary/intermediate_file_paths.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     6166 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/summary/model.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     3844 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/summary/preprocessed_features.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1907 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/summary/sysinfo.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     4469 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/summary/true_score_evaluation.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1907 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/sysinfo.ipynb
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.444944 rsmtool-9.1.1/rsmtool/notebooks/templates/
+-rw-r--r--   0 nmadnani   (501) staff       (20)      123 2023-01-17 15:15:45.000000 rsmtool-9.1.1/rsmtool/notebooks/templates/report.tpl
+-rw-r--r--   0 nmadnani   (501) staff       (20)     7601 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/notebooks/true_score_evaluation.ipynb
+-rw-r--r--   0 nmadnani   (501) staff       (20)   111208 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/preprocessor.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    12894 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/reader.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    32686 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/reporter.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)     8443 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/rsmcompare.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    10401 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/rsmeval.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    18438 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/rsmpredict.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    11100 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/rsmsummarize.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    14395 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/rsmtool.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    12572 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/rsmxval.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    60939 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/test_utils.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    14143 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/transformer.py
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.437572 rsmtool-9.1.1/rsmtool/utils/
+-rw-r--r--   0 nmadnani   (501) staff       (20)        0 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/utils/__init__.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    38090 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/commandline.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    11053 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/constants.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)      887 2021-10-27 17:25:11.000000 rsmtool-9.1.1/rsmtool/utils/conversion.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)     9871 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/cross_validation.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)     3946 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/files.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)     3771 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/logging.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    17515 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/metrics.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)     2034 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/models.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    11960 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/notebook.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)    11773 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/utils/prmse.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)      262 2023-01-20 19:02:03.000000 rsmtool-9.1.1/rsmtool/version.py
+-rw-r--r--   0 nmadnani   (501) staff       (20)     8039 2023-01-13 21:53:48.000000 rsmtool-9.1.1/rsmtool/writer.py
+drwxr-xr-x   0 nmadnani   (501) staff       (20)        0 2023-01-20 19:02:06.438990 rsmtool-9.1.1/rsmtool.egg-info/
+-rw-r--r--   0 nmadnani   (501) staff       (20)     5872 2023-01-20 19:02:06.000000 rsmtool-9.1.1/rsmtool.egg-info/PKG-INFO
+-rw-r--r--   0 nmadnani   (501) staff       (20)     3677 2023-01-20 19:02:06.000000 rsmtool-9.1.1/rsmtool.egg-info/SOURCES.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)        1 2023-01-20 19:02:06.000000 rsmtool-9.1.1/rsmtool.egg-info/dependency_links.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)      323 2023-01-20 19:02:06.000000 rsmtool-9.1.1/rsmtool.egg-info/entry_points.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)        1 2022-12-06 22:08:33.000000 rsmtool-9.1.1/rsmtool.egg-info/not-zip-safe
+-rw-r--r--   0 nmadnani   (501) staff       (20)      178 2023-01-20 19:02:06.000000 rsmtool-9.1.1/rsmtool.egg-info/requires.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)        8 2023-01-20 19:02:06.000000 rsmtool-9.1.1/rsmtool.egg-info/top_level.txt
+-rw-r--r--   0 nmadnani   (501) staff       (20)      118 2023-01-20 19:02:06.445704 rsmtool-9.1.1/setup.cfg
+-rw-r--r--   0 nmadnani   (501) staff       (20)     1995 2023-01-20 18:55:30.000000 rsmtool-9.1.1/setup.py
```

### Comparing `rsmtool-9.0.1/LICENSE` & `rsmtool-9.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/PKG-INFO` & `rsmtool-9.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsmtool
-Version: 9.0.1
+Version: 9.1.1
 Summary: Rater scoring modeling tool
 Home-page: http://github.com/EducationalTestingService/rsmtool
 Maintainer: Nitin Madnani
 Maintainer-email: nmadnani@ets.org
 License: Apache 2
 Keywords: scoring modeling
 Classifier: Intended Audience :: Science/Research
@@ -36,15 +36,15 @@
    :target: https://codecov.io/gh/EducationalTestingService/rsmtool
    :alt: Coverage status
 
 .. image:: https://img.shields.io/conda/v/ets/rsmtool.svg
    :target: https://anaconda.org/ets/rsmtool
    :alt: Conda package for SKLL
 
-.. image:: https://img.shields.io/readthedocs/rsmtool/v9.0.1.svg
+.. image:: https://img.shields.io/readthedocs/rsmtool/v9.1.0.svg
    :target: https://rsmtool.readthedocs.io
    :alt: Docs
 
 .. image:: https://img.shields.io/badge/DOI-10.21105%2Fjoss.00033-blue.svg
    :target: http://joss.theoj.org/papers/10.21105/joss.00033
    :alt: DOI for citing RSMTool
```

### Comparing `rsmtool-9.0.1/README.rst` & `rsmtool-9.1.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
    :target: https://codecov.io/gh/EducationalTestingService/rsmtool
    :alt: Coverage status
 
 .. image:: https://img.shields.io/conda/v/ets/rsmtool.svg
    :target: https://anaconda.org/ets/rsmtool
    :alt: Conda package for SKLL
 
-.. image:: https://img.shields.io/readthedocs/rsmtool/v9.0.1.svg
+.. image:: https://img.shields.io/readthedocs/rsmtool/v9.1.0.svg
    :target: https://rsmtool.readthedocs.io
    :alt: Docs
 
 .. image:: https://img.shields.io/badge/DOI-10.21105%2Fjoss.00033-blue.svg
    :target: http://joss.theoj.org/papers/10.21105/joss.00033
    :alt: DOI for citing RSMTool
```

### Comparing `rsmtool-9.0.1/rsmtool/__init__.py` & `rsmtool-9.1.1/rsmtool/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """
+Set up RSMTool version and global imports.
+
 :author: Jeremy Biggs {jbiggs@ets.org)}
 :author: Anastassia Loukina (aloukina@ets.org)
 :author: Nitin Madnani (nmadnani@ets.org)
 
 :organization: ETS
 
 isort:skip_file
@@ -11,41 +13,47 @@
 # do we have rsmextra installed? we try to import rsmextra here
 # to avoid doing this in each module.
 
 import re
 import warnings
 
 try:
-    import rsmextra # noqa
+    import rsmextra  # noqa
 except ImportError:
     HAS_RSMEXTRA = False
 else:
     HAS_RSMEXTRA = True
 
 from .version import __version__
 
 if HAS_RSMEXTRA:
-    from rsmextra.version import __version__ as rsmextra_version # noqa
-    VERSION_STRING = '%(prog)s {}; rsmextra {}'.format(__version__,
-                                                       rsmextra_version)
+    from rsmextra.version import __version__ as rsmextra_version  # noqa
+
+    VERSION_STRING = f"%(prog)s {__version__}; rsmextra {rsmextra_version}"
 else:
-    VERSION_STRING = '%(prog)s {}'.format(__version__)
+    VERSION_STRING = f"%(prog)s {__version__}"
 
 from .rsmcompare import run_comparison  # noqa
 
 from .rsmeval import run_evaluation  # noqa
 
 from .rsmtool import run_experiment  # noqa
 
-from .rsmpredict import compute_and_save_predictions  # noqa
+from .rsmpredict import compute_and_save_predictions, fast_predict  # noqa
 
 from .rsmsummarize import run_summary  # noqa
 
-__all__ = ['run_experiment', 'run_evaluation', 'run_comparison',
-           'compute_and_save_predictions', 'run_summary']
+__all__ = [
+    "run_experiment",
+    "run_evaluation",
+    "run_comparison",
+    "compute_and_save_predictions",
+    "fast_predict",
+    "run_summary",
+]
 
 # Make sure that DeprecationWarnings are always shown
 # within this package unless we are in test mode in
 # which case do not enable them by default.
-warnings.filterwarnings('always',
-                        category=DeprecationWarning,
-                        module=r'^{0}\.'.format(re.escape(__name__)))
+warnings.filterwarnings(
+    "always", category=DeprecationWarning, module=r"^{0}\.".format(re.escape(__name__))
+)
```

### Comparing `rsmtool-9.0.1/rsmtool/analyzer.py` & `rsmtool-9.1.1/rsmtool/analyzer.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,38 +4,41 @@
 :author: Jeremy Biggs (jbiggs@ets.org)
 :author: Anastassia Loukina (aloukina@ets.org)
 :author: Nitin Madnani (nmadnani@ets.org)
 
 :organization: ETS
 """
 
+import logging
 import warnings
 from functools import partial
-import logging
 
 import numpy as np
 import pandas as pd
 from scipy.stats import kurtosis, pearsonr
 from sklearn.decomposition import PCA
 from sklearn.metrics import confusion_matrix, mean_squared_error, r2_score
 from skll.metrics import kappa
 
 from .container import DataContainer
-from .utils.metrics import (agreement,
-                            difference_of_standardized_means,
-                            partial_correlations,
-                            quadratic_weighted_kappa,
-                            standardized_mean_difference)
+from .utils.metrics import (
+    agreement,
+    difference_of_standardized_means,
+    partial_correlations,
+    quadratic_weighted_kappa,
+    standardized_mean_difference,
+)
 from .utils.prmse import get_true_score_evaluations
 
 
 class Analyzer:
     """Class to perform analysis on all metrics, predictions, etc."""
 
     def __init__(self, logger=None):
+        """Initialize the Analyzer object."""
         self.logger = logger if logger else logging.getLogger(__name__)
 
     @staticmethod
     def check_frame_names(data_container, dataframe_names):
         """
         Check that all specified dataframes are available.
 
@@ -53,16 +56,18 @@
         Raises
         ------
         KeyError
             If a given dataframe_name is not in the DataContainer object.
         """
         for dataframe_name in dataframe_names:
             if dataframe_name not in data_container:
-                raise KeyError('The DataFrame `{}` does not exist in the '
-                               'DataContainer object.'.format(dataframe_name))
+                raise KeyError(
+                    f"The DataFrame `{dataframe_name}` does not exist "
+                    f"in the DataContainer object."
+                )
 
     @staticmethod
     def check_param_names(configuration_obj, parameter_names):
         """
         Check that all specified parameters are available.
 
         This method checks to make sure all specified parameters
@@ -79,23 +84,23 @@
         Raises
         ------
         KeyError
             If a given parameter_name is not in the Configuration object.
         """
         for parameter_name in parameter_names:
             if parameter_name not in configuration_obj:
-                raise KeyError('The parameter `{}` does not exist in the '
-                               'Configuration object.'.format(parameter_name))
+                raise KeyError(
+                    f"The parameter `{parameter_name}` does not exist "
+                    f"in the Configuration object."
+                )
 
     @staticmethod
-    def analyze_excluded_responses(df,
-                                   features,
-                                   header,
-                                   exclude_zero_scores=True,
-                                   exclude_listwise=False):
+    def analyze_excluded_responses(
+        df, features, header, exclude_zero_scores=True, exclude_listwise=False
+    ):
         """
         Compute statistics for responses excluded from analyses.
 
         This method computes various statistics for the responses that
         were excluded from analyses, either in the training set or in
         the test set.
 
@@ -121,58 +126,60 @@
         Returns
         -------
         df_full_crosstab : pandas DataFrame
             Two-dimensional data frame containing the
             exclusion statistics.
         """
         # create an empty output data frame
-        df_full_crosstab = pd.DataFrame({'all features numeric': [0, 0, 0],
-                                         'non-numeric feature values': [0, 0, 0]},
-                                        index=['numeric non-zero human score',
-                                               'zero human score',
-                                               'non-numeric human score'])
+        df_full_crosstab = pd.DataFrame(
+            {
+                "all features numeric": [0, 0, 0],
+                "non-numeric feature values": [0, 0, 0],
+            },
+            index=[
+                "numeric non-zero human score",
+                "zero human score",
+                "non-numeric human score",
+            ],
+        )
 
         if not df.empty:
             # re-code human scores into numeric, missing or zero
-            df['score_category'] = 'numeric non-zero human score'
-            df.loc[df['sc1'].isnull(), 'score_category'] = 'non-numeric human score'
-            df.loc[df['sc1'].astype(float) == 0, 'score_category'] = 'zero human score'
+            df["score_category"] = "numeric non-zero human score"
+            df.loc[df["sc1"].isnull(), "score_category"] = "non-numeric human score"
+            df.loc[df["sc1"].astype(float) == 0, "score_category"] = "zero human score"
 
             # recode feature values: a response with at least one
             # missing feature is assigned 'non-numeric feature values'
-            df_features_only = df[features + ['spkitemid']]
+            df_features_only = df[features + ["spkitemid"]]
             null_feature_rows = df_features_only.isnull().any(axis=1)
             df_null_features = df_features_only[null_feature_rows]
-            df['feat_category'] = 'all features numeric'
-            df.loc[df['spkitemid'].isin(df_null_features['spkitemid']),
-                   'feat_category'] = 'non-numeric feature values'
+            df["feat_category"] = "all features numeric"
+            df.loc[
+                df["spkitemid"].isin(df_null_features["spkitemid"]), "feat_category"
+            ] = "non-numeric feature values"
 
             # crosstabulate
-            df_crosstab = pd.crosstab(df['score_category'],
-                                      df['feat_category'])
+            df_crosstab = pd.crosstab(df["score_category"], df["feat_category"])
             df_full_crosstab.update(df_crosstab)
             # convert back to integers as these are all counts
             df_full_crosstab = df_full_crosstab.astype(int)
             df_full_crosstab.insert(0, header, df_full_crosstab.index)
 
         if not exclude_listwise:
             # if we are not excluding listwise, rename the first cell so
             # that it is not set to zero
-            assert(df_full_crosstab.loc['numeric non-zero human score',
-                                        'all features numeric'] == 0)
-            df_full_crosstab.loc['numeric non-zero human score',
-                                 'all features numeric'] = '-'
+            assert df_full_crosstab.loc["numeric non-zero human score", "all features numeric"] == 0
+            df_full_crosstab.loc["numeric non-zero human score", "all features numeric"] = "-"
 
             # if we are not excluding the zeros, rename the corresponding cells
             # so that they are not set to zero. We do not do this for listwise exclusion
             if not exclude_zero_scores:
-                assert(df_full_crosstab.loc['zero human score',
-                                            'all features numeric'] == 0)
-                df_full_crosstab.loc['zero human score',
-                                     'all features numeric'] = '-'
+                assert df_full_crosstab.loc["zero human score", "all features numeric"] == 0
+                df_full_crosstab.loc["zero human score", "all features numeric"] = "-"
 
         return df_full_crosstab
 
     @staticmethod
     def analyze_used_responses(df_train, df_test, subgroups, candidate_column):
         """
         Compute statistics for responses used in analyses.
@@ -199,41 +206,52 @@
         Returns
         -------
         df_analysis : pandas DataFrame
             Data frame containing information about the used
             responses.
         """
         # create a basic data frame for responses only
-        train_responses = set(df_train['spkitemid'])
-        test_responses = set(df_test['spkitemid'])
+        train_responses = set(df_train["spkitemid"])
+        test_responses = set(df_test["spkitemid"])
 
-        rows = [{'partition': 'Training', 'responses': len(train_responses)},
-                {'partition': 'Evaluation', 'responses': len(test_responses)},
-                {'partition': 'Overlapping', 'responses': len(train_responses & test_responses)},
-                {'partition': 'Total', 'responses': len(train_responses | test_responses)}]
+        rows = [
+            {"partition": "Training", "responses": len(train_responses)},
+            {"partition": "Evaluation", "responses": len(test_responses)},
+            {
+                "partition": "Overlapping",
+                "responses": len(train_responses & test_responses),
+            },
+            {"partition": "Total", "responses": len(train_responses | test_responses)},
+        ]
 
         df_analysis = pd.DataFrame.from_dict(rows)
 
-        columns = ['partition', 'responses'] + subgroups
+        columns = ["partition", "responses"] + subgroups
 
         if candidate_column:
-            train_candidates = set(df_train['candidate'])
-            test_candidates = set(df_test['candidate'])
-            df_analysis['candidates'] = [len(train_candidates), len(test_candidates),
-                                         len(train_candidates & test_candidates),
-                                         len(train_candidates | test_candidates)]
+            train_candidates = set(df_train["candidate"])
+            test_candidates = set(df_test["candidate"])
+            df_analysis["candidates"] = [
+                len(train_candidates),
+                len(test_candidates),
+                len(train_candidates & test_candidates),
+                len(train_candidates | test_candidates),
+            ]
 
-            columns = ['partition', 'responses', 'candidates'] + subgroups
+            columns = ["partition", "responses", "candidates"] + subgroups
 
         for group in subgroups:
             train_group = set(df_train[group])
             test_group = set(df_test[group])
-            df_analysis[group] = [len(train_group), len(test_group),
-                                  len(train_group & test_group),
-                                  len(train_group | test_group)]
+            df_analysis[group] = [
+                len(train_group),
+                len(test_group),
+                len(train_group & test_group),
+                len(train_group | test_group),
+            ]
 
         df_analysis = df_analysis[columns]
         return df_analysis
 
     @staticmethod
     def analyze_used_predictions(df_test, subgroups, candidate_column):
         """
@@ -252,22 +270,22 @@
 
         Returns
         -------
         df_analysis : pandas DataFrame
             Data frame containing information about the used
             predictions.
         """
-        rows = [{'partition': 'Evaluation', 'responses': df_test['spkitemid'].size}]
+        rows = [{"partition": "Evaluation", "responses": df_test["spkitemid"].size}]
 
         df_analysis = pd.DataFrame.from_dict(rows)
-        df_columns = ['partition', 'responses'] + subgroups
+        df_columns = ["partition", "responses"] + subgroups
 
         if candidate_column:
-            df_analysis['candidates'] = [df_test['candidate'].unique().size]
-            df_columns = ['partition', 'responses', 'candidates'] + subgroups
+            df_analysis["candidates"] = [df_test["candidate"].unique().size]
+            df_columns = ["partition", "responses", "candidates"] + subgroups
 
         for group in subgroups:
             df_analysis[group] = [df_test[group].unique().size]
 
         df_analysis = df_analysis[df_columns]
         return df_analysis
 
@@ -290,42 +308,55 @@
             DataFrame containing the descriptives for
             each of the features.
         """
         # select only feature columns
         df_desc = df[selected_features]
 
         # get the H1 scores
-        scores = df['sc1']
+        scores = df["sc1"]
 
         # compute correlations and p-values separately for efficiency
         cor_series = df_desc.apply(lambda s: pearsonr(s, scores))
         cors = cor_series.apply(lambda t: t[0])
         pvalues = cor_series.apply(lambda t: t[1])
 
         # create a data frame with all the descriptives
-        df_output = pd.DataFrame({'mean': df_desc.mean(),
-                                  'min': df_desc.min(),
-                                  'max': df_desc.max(),
-                                  'std. dev.': df_desc.std(),
-                                  'skewness': df_desc.skew(),
-                                  'kurtosis': df_desc.apply(lambda s: kurtosis(s, fisher=False)),
-                                  'Correlation': cors,
-                                  'p': pvalues,
-                                  'N': len(df_desc)})
+        df_output = pd.DataFrame(
+            {
+                "mean": df_desc.mean(),
+                "min": df_desc.min(),
+                "max": df_desc.max(),
+                "std. dev.": df_desc.std(),
+                "skewness": df_desc.skew(),
+                "kurtosis": df_desc.apply(lambda s: kurtosis(s, fisher=False)),
+                "Correlation": cors,
+                "p": pvalues,
+                "N": len(df_desc),
+            }
+        )
 
         # reorder the columns to make it look better
-        df_output = df_output[['mean', 'std. dev.', 'min', 'max', 'skewness',
-                               'kurtosis', 'Correlation', 'p', 'N']]
+        df_output = df_output[
+            [
+                "mean",
+                "std. dev.",
+                "min",
+                "max",
+                "skewness",
+                "kurtosis",
+                "Correlation",
+                "p",
+                "N",
+            ]
+        ]
 
         return df_output
 
     @staticmethod
-    def compute_percentiles(df,
-                            selected_features,
-                            percentiles=None):
+    def compute_percentiles(df, selected_features, percentiles=None):
         """
         Compute percentiles and outliers for columns in the given data frame.
 
         Parameters
         ----------
         df : pandas DataFrame
             Input data frame containing the feature values.
@@ -346,46 +377,46 @@
         # select only feature columns
         df_desc = df[selected_features]
 
         # compute the various percentile levels
         if percentiles is None:
             percentiles = [1, 5, 25, 50, 75, 95, 99]
 
-        df_output = df_desc.apply(lambda series: pd.Series(np.percentile(series,
-                                                                         percentiles,
-                                                                         method='lower')))
+        df_output = df_desc.apply(
+            lambda series: pd.Series(np.percentile(series, percentiles, method="lower"))
+        )
         df_output = df_output.transpose()
 
         # change the column names to be more readable
-        df_output.columns = ['{}%'.format(p) for p in percentiles]
+        df_output.columns = [f"{p}%" for p in percentiles]
 
         # add the inter-quartile range column
-        df_output['IQR'] = df_output['75%'] - df_output['25%']
+        df_output["IQR"] = df_output["75%"] - df_output["25%"]
 
         # compute the various outlier statistics
-        mild_upper = df_output['75%'] + 1.5 * df_output['IQR']
-        mild_bottom = df_output['25%'] - 1.5 * df_output['IQR']
+        mild_upper = df_output["75%"] + 1.5 * df_output["IQR"]
+        mild_bottom = df_output["25%"] - 1.5 * df_output["IQR"]
 
-        extreme_upper = df_output['75%'] + 3 * df_output['IQR']
-        extreme_bottom = df_output['25%'] - 3 * df_output['IQR']
+        extreme_upper = df_output["75%"] + 3 * df_output["IQR"]
+        extreme_bottom = df_output["25%"] - 3 * df_output["IQR"]
 
         # compute the mild and extreme outliers
         num_mild_outliers = {}
         num_extreme_outliers = {}
         for c in df_desc.columns:
             is_extreme = (df_desc[c] <= extreme_bottom[c]) | (df_desc[c] >= extreme_upper[c])
 
-            is_mild = ((df_desc[c] > extreme_bottom[c]) & (df_desc[c] <= mild_bottom[c]))
+            is_mild = (df_desc[c] > extreme_bottom[c]) & (df_desc[c] <= mild_bottom[c])
             is_mild = is_mild | ((df_desc[c] >= mild_upper[c]) & (df_desc[c] < extreme_upper[c]))
             num_mild_outliers[c] = len(df_desc[is_mild])
             num_extreme_outliers[c] = len(df_desc[is_extreme])
 
         # add those to the output data frame
-        df_output['Mild outliers'] = pd.Series(num_mild_outliers)
-        df_output['Extreme outliers'] = pd.Series(num_extreme_outliers)
+        df_output["Mild outliers"] = pd.Series(num_mild_outliers)
+        df_output["Extreme outliers"] = pd.Series(num_extreme_outliers)
 
         return df_output
 
     @staticmethod
     def compute_outliers(df, selected_features):
         """
         Compute number and percentage of outliers for given columns.
@@ -422,20 +453,24 @@
             lower_outliers[c] = len(df_desc[df_desc[c] < means[c] - 4 * stds[c]])
             upper_outliers[c] = len(df_desc[df_desc[c] > means[c] + 4 * stds[c]])
 
         # generate the output data frame
         lower_s = pd.Series(lower_outliers)
         upper_s = pd.Series(upper_outliers)
         both_s = lower_s + upper_s
-        df_output = pd.DataFrame({'lower': lower_s,
-                                  'upper': upper_s,
-                                  'both': both_s,
-                                  'lowerperc': round(lower_s / len(df_desc) * 100, 2),
-                                  'upperperc': round(upper_s / len(df_desc) * 100, 2),
-                                  'bothperc': round(both_s / len(df_desc) * 100, 2)})
+        df_output = pd.DataFrame(
+            {
+                "lower": lower_s,
+                "upper": upper_s,
+                "both": both_s,
+                "lowerperc": round(lower_s / len(df_desc) * 100, 2),
+                "upperperc": round(upper_s / len(df_desc) * 100, 2),
+                "bothperc": round(both_s / len(df_desc) * 100, 2),
+            }
+        )
 
         return df_output
 
     @staticmethod
     def compute_pca(df, selected_features):
         """
         Compute PCA decomposition of the given features.
@@ -466,41 +501,43 @@
         n_components = min(len(selected_features), len(df_pca))
         pca = PCA(n_components=n_components)
         pca.fit(df_pca)
 
         df_components = pd.DataFrame(pca.components_)
         n_components = len(df_components)
         df_components.columns = selected_features
-        df_components.index = ['PC{}'.format(i) for i in range(1, n_components + 1)]
+        df_components.index = [f"PC{i}" for i in range(1, n_components + 1)]
         df_components = df_components.transpose()
 
         # compute the variance data frame
-        df_variance = {'Eigenvalues': pca.explained_variance_,
-                       'Percentage of variance': pca.explained_variance_ratio_,
-                       'Cumulative percentage of '
-                       'variance': np.cumsum(pca.explained_variance_ratio_)
-                       }
+        df_variance = {
+            "Eigenvalues": pca.explained_variance_,
+            "Percentage of variance": pca.explained_variance_ratio_,
+            "Cumulative percentage of " "variance": np.cumsum(pca.explained_variance_ratio_),
+        }
 
         df_variance = pd.DataFrame(df_variance)
 
         # reorder the columns
-        df_variance = df_variance[['Eigenvalues', 'Percentage of variance',
-                                   'Cumulative percentage of variance']]
+        df_variance = df_variance[
+            [
+                "Eigenvalues",
+                "Percentage of variance",
+                "Cumulative percentage of variance",
+            ]
+        ]
 
         # set the row names and take the transpose
-        df_variance.index = ['PC{}'.format(i) for i in range(1, n_components + 1)]
+        df_variance.index = [f"PC{i}" for i in range(1, n_components + 1)]
         df_variance = df_variance.transpose()
 
         return df_components, df_variance
 
     @staticmethod
-    def correlation_helper(df,
-                           target_variable,
-                           grouping_variable,
-                           include_length=False):
+    def correlation_helper(df, target_variable, grouping_variable, include_length=False):
         """
         Compute marginal and partial correlations for all columns.
 
         This helper method computes marginal and partial correlations of
         all the columns in the given data frame against the target variable
         separately for each level in the the grouping variable.
         If ``include_length`` is ``True``, it additionally computes partial
@@ -546,64 +583,64 @@
         df_target_pcorr_no_length = pd.DataFrame()
 
         for group, df_group in grouped:
             df_group = df_group.drop(grouping_variable, axis=1)
 
             # first check if we have at least 2 cases and return np.nan otherwise
             if len(df_group) == 1:
-                df_target_cors[group] = pd.Series(data=np.nan,
-                                                  index=df_group.columns)
-                df_target_pcorr[group] = pd.Series(data=np.nan,
-                                                   index=df_group.columns)
-                df_target_pcorr_no_length[group] = pd.Series(data=np.nan,
-                                                             index=df_group.columns)
+                df_target_cors[group] = pd.Series(data=np.nan, index=df_group.columns)
+                df_target_pcorr[group] = pd.Series(data=np.nan, index=df_group.columns)
+                df_target_pcorr_no_length[group] = pd.Series(data=np.nan, index=df_group.columns)
             else:
                 # if we are asked to include length, that means 'length' is
                 # in the data frame which means that we want to exclude that
                 # before computing the regular marginal and partial correlations
                 if not include_length:
-                    df_target_cors[group] = df_group.apply(lambda s:
-                                                           pearsonr(s,
-                                                                    df_group[target_variable])[0])
+                    df_target_cors[group] = df_group.apply(
+                        lambda s: pearsonr(s, df_group[target_variable])[0]
+                    )
                     df_target_pcorr[group] = partial_correlations(df_group)[target_variable]
                 else:
-                    df_group_no_length = df_group.drop('length', axis=1)
+                    df_group_no_length = df_group.drop("length", axis=1)
 
                     partial_pearsonr = partial(pearsonr, y=df_group_no_length[target_variable])
-                    df_target_cors[group] = df_group_no_length.apply(lambda s:
-                                                                     partial_pearsonr(s)[0])
-
-                    df_target_pcorr[group] = partial_correlations(df_group_no_length)[target_variable]
+                    df_target_cors[group] = df_group_no_length.apply(
+                        lambda s: partial_pearsonr(s)[0]
+                    )
+
+                    df_target_pcorr[group] = partial_correlations(df_group_no_length)[
+                        target_variable
+                    ]
                     pcor_dict = {}
-                    columns = [c for c in df_group.columns if c not in ['sc1', 'length']]
+                    columns = [c for c in df_group.columns if c not in ["sc1", "length"]]
                     for c in columns:
-                        pcor_dict[c] = partial_correlations(df_group[[c,
-                                                                      'sc1',
-                                                                      'length']])['sc1'][c]
+                        pcor_dict[c] = partial_correlations(df_group[[c, "sc1", "length"]])["sc1"][
+                            c
+                        ]
                     df_target_pcorr_no_length[group] = pd.Series(pcor_dict)
 
         # remove the row containing the correlation of the target variable
         # with itself and take the transpose
         df_target_cors = df_target_cors.drop(target_variable).transpose()
         df_target_pcorr = df_target_pcorr.drop(target_variable).transpose()
         df_target_pcorr_no_length = df_target_pcorr_no_length.transpose()
 
-        return (df_target_cors,
-                df_target_pcorr,
-                df_target_pcorr_no_length)
+        return (df_target_cors, df_target_pcorr, df_target_pcorr_no_length)
 
     @staticmethod
-    def metrics_helper(human_scores,
-                       system_scores,
-                       population_human_score_sd=None,
-                       population_system_score_sd=None,
-                       population_human_score_mn=None,
-                       population_system_score_mn=None,
-                       smd_method='unpooled',
-                       use_diff_std_means=False):
+    def metrics_helper(
+        human_scores,
+        system_scores,
+        population_human_score_sd=None,
+        population_system_score_sd=None,
+        population_human_score_mn=None,
+        population_system_score_mn=None,
+        smd_method="unpooled",
+        use_diff_std_means=False,
+    ):
         """
         Compute basic association metrics between system and human scores.
 
         Parameters
         ----------
         human_scores : pandas Series
             Series containing numeric human (reference) scores.
@@ -702,35 +739,29 @@
             - `h_max`: max human score
             - `h_mean`: mean human score (ddof=1)
             - `h_sd`: standard deviation of human scores (ddof=1)
             - `N`: total number of responses
         """
         # compute the kappas
         unweighted_kappa = kappa(human_scores, system_scores)
-        weighted_kappa = quadratic_weighted_kappa(human_scores,
-                                                  system_scores)
+        weighted_kappa = quadratic_weighted_kappa(human_scores, system_scores)
 
         # compute the agreement statistics
         human_system_agreement = agreement(human_scores, system_scores)
-        human_system_adjacent_agreement = agreement(human_scores,
-                                                    system_scores,
-                                                    tolerance=1)
+        human_system_adjacent_agreement = agreement(human_scores, system_scores, tolerance=1)
 
         # compute the Pearson correlation after removing
         # any cases where either of the scores are NaNs.
-        df = pd.DataFrame({'human': human_scores,
-                           'system': system_scores}).dropna(how='any')
+        df = pd.DataFrame({"human": human_scores, "system": system_scores}).dropna(how="any")
 
-        if (len(df) == 1 or
-                len(df['human'].unique()) == 1 or
-                len(df['system'].unique()) == 1):
+        if len(df) == 1 or len(df["human"].unique()) == 1 or len(df["system"].unique()) == 1:
             # set correlations to 1 if we have a single instance or zero variance
             correlations = np.nan
         else:
-            correlations = pearsonr(df['human'], df['system'])[0]
+            correlations = pearsonr(df["human"], df["system"])[0]
 
         # compute the min/max/mean/std. dev. for the system and human scores
         min_system_score = np.min(system_scores)
         min_human_score = np.min(human_scores)
 
         max_system_score = np.max(system_scores)
         max_human_score = np.max(human_scores)
@@ -740,66 +771,73 @@
 
         system_score_sd = np.std(system_scores, ddof=1)
         human_score_sd = np.std(human_scores, ddof=1)
 
         if use_diff_std_means:
 
             # calculate the difference of standardized means
-            smd_name = 'DSM'
-            smd = difference_of_standardized_means(human_scores,
-                                                   system_scores,
-                                                   population_human_score_mn,
-                                                   population_system_score_mn,
-                                                   population_human_score_sd,
-                                                   population_system_score_sd)
+            smd_name = "DSM"
+            smd = difference_of_standardized_means(
+                human_scores,
+                system_scores,
+                population_human_score_mn,
+                population_system_score_mn,
+                population_human_score_sd,
+                population_system_score_sd,
+            )
 
         else:
 
             # calculate the standardized mean difference
-            smd_name = 'SMD'
-            smd = standardized_mean_difference(human_scores,
-                                               system_scores,
-                                               population_human_score_sd,
-                                               population_system_score_sd,
-                                               method=smd_method)
+            smd_name = "SMD"
+            smd = standardized_mean_difference(
+                human_scores,
+                system_scores,
+                population_human_score_sd,
+                population_system_score_sd,
+                method=smd_method,
+            )
 
         # compute r2
         if len(df) == 1:
             r2 = np.nan
         else:
             r2 = r2_score(human_scores, system_scores)
 
         # compute MSE
         mse = mean_squared_error(human_scores, system_scores)
         rmse = np.sqrt(mse)
 
         # return everything as a series
-        metrics = pd.Series({'kappa': unweighted_kappa,
-                             'wtkappa': weighted_kappa,
-                             'exact_agr': human_system_agreement,
-                             'adj_agr': human_system_adjacent_agreement,
-                             smd_name: smd,
-                             'corr': correlations,
-                             'R2': r2,
-                             'RMSE': rmse,
-                             'sys_min': min_system_score,
-                             'sys_max': max_system_score,
-                             'sys_mean': mean_system_score,
-                             'sys_sd': system_score_sd,
-                             'h_min': min_human_score,
-                             'h_max': max_human_score,
-                             'h_mean': mean_human_score,
-                             'h_sd': human_score_sd,
-                             'N': len(system_scores)})
+        metrics = pd.Series(
+            {
+                "kappa": unweighted_kappa,
+                "wtkappa": weighted_kappa,
+                "exact_agr": human_system_agreement,
+                "adj_agr": human_system_adjacent_agreement,
+                smd_name: smd,
+                "corr": correlations,
+                "R2": r2,
+                "RMSE": rmse,
+                "sys_min": min_system_score,
+                "sys_max": max_system_score,
+                "sys_mean": mean_system_score,
+                "sys_sd": system_score_sd,
+                "h_min": min_human_score,
+                "h_max": max_human_score,
+                "h_mean": mean_human_score,
+                "h_sd": human_score_sd,
+                "N": len(system_scores),
+            }
+        )
 
         return metrics
 
     @staticmethod
-    def compute_disattenuated_correlations(human_system_corr,
-                                           human_human_corr):
+    def compute_disattenuated_correlations(human_system_corr, human_human_corr):
         """
         Compute disattenuated correlations between human and system scores.
 
         These are computed as the Pearson's correlation between the human score
         and the system score divided by the square root of correlation between
         two human raters.
 
@@ -817,41 +855,47 @@
         -------
         df_correlations: pandas DataFrame
             Data frame containing the human-system correlations, human-human
             correlations, and disattenuated correlations.
         """
         # if we only have a single value for human correlation and the index
         # is not in human-system values, we use the same HH value in all cases
-        if (len(human_human_corr) == 1 and
-                not human_human_corr.index[0] in human_system_corr.index):
-            human_human_corr = pd.Series(human_human_corr.values.repeat(len(human_system_corr)),
-                                         index=human_system_corr.index)
+        if len(human_human_corr) == 1 and not human_human_corr.index[0] in human_system_corr.index:
+            human_human_corr = pd.Series(
+                human_human_corr.values.repeat(len(human_system_corr)),
+                index=human_system_corr.index,
+            )
 
         # we now concatenate the two series on index
-        df_correlations = pd.concat([human_system_corr, human_human_corr],
-                                    axis=1,
-                                    sort=True,
-                                    keys=['corr_HM', 'corr_HH'])
+        df_correlations = pd.concat(
+            [human_system_corr, human_human_corr],
+            axis=1,
+            sort=True,
+            keys=["corr_HM", "corr_HH"],
+        )
 
         # if any of the HH correlations are negative, we will ignore these
         # and treat them as Nones
-        with np.errstate(invalid='ignore'):
-            df_correlations['sqrt_HH'] = np.sqrt(df_correlations['corr_HH'])
+        with np.errstate(invalid="ignore"):
+            df_correlations["sqrt_HH"] = np.sqrt(df_correlations["corr_HH"])
 
-        df_correlations['corr_disattenuated'] = (df_correlations['corr_HM'] /
-                                                 df_correlations['sqrt_HH'])
+        df_correlations["corr_disattenuated"] = (
+            df_correlations["corr_HM"] / df_correlations["sqrt_HH"]
+        )
 
         return df_correlations
 
-    def compute_correlations_by_group(self,
-                                      df,
-                                      selected_features,
-                                      target_variable,
-                                      grouping_variable,
-                                      include_length=False):
+    def compute_correlations_by_group(
+        self,
+        df,
+        selected_features,
+        target_variable,
+        grouping_variable,
+        include_length=False,
+    ):
         """
         Compute marginal and partial correlations against target variable.
 
         This method computes various marginal and partial correlations of the
         given columns in the given data frame against the target variable for
         all data and for each level of the grouping variable.
 
@@ -877,38 +921,37 @@
         df_output : pandas DataFrame
             Data frame containing the correlations.
         """
         df_desc = df.copy()
 
         columns = selected_features + [target_variable, grouping_variable]
         if include_length:
-            columns.append('length')
+            columns.append("length")
         df_desc = df_desc[columns]
 
         # create a duplicate data frame to compute correlations
         # over the whole data, i.e., across all grouping variables
         df_desc_all = df_desc.copy()
-        df_desc_all[grouping_variable] = 'All data'
+        df_desc_all[grouping_variable] = "All data"
 
         # combine the two data frames
         df_desc_combined = pd.concat([df_desc, df_desc_all], sort=True)
         df_desc_combined.reset_index(drop=True, inplace=True)
 
         # compute the various (marginal and partial) correlations with score
-        ret = self.correlation_helper(df_desc_combined,
-                                      target_variable,
-                                      grouping_variable,
-                                      include_length=include_length)
+        ret = self.correlation_helper(
+            df_desc_combined,
+            target_variable,
+            grouping_variable,
+            include_length=include_length,
+        )
 
         return ret
 
-    def filter_metrics(self,
-                       df_metrics,
-                       use_scaled_predictions=False,
-                       chosen_metric_dict=None):
+    def filter_metrics(self, df_metrics, use_scaled_predictions=False, chosen_metric_dict=None):
         """
         Filter data frame to retain only the given metrics.
 
         This method filters the data frame ``df_metrics`` -- containing
         all of the metric values by all score types (raw, raw_trim etc.)
         -- to retain only the metrics as defined in the given dictionary
         ``chosen_metric_dict``. This dictionary maps score types ("raw",
@@ -956,59 +999,66 @@
              "X_trim_round": ["sys_mean", "sys_sd", "kappa",
                                 "exact_agr", "adj_agr", "SMD"]}
 
         where X = "raw" or "scale" depending on whether
         ``use_scaled_predictions`` is ``False`` or ``True``, respectively.
         """
         # do we want the raw or the scaled metrics
-        score_prefix = 'scale' if use_scaled_predictions else 'raw'
+        score_prefix = "scale" if use_scaled_predictions else "raw"
 
         # what metrics are we choosing to include?
         if chosen_metric_dict:
             chosen_metrics = chosen_metric_dict
         else:
-            smd_name = 'DSM' if 'DSM' in df_metrics else 'SMD'
-            chosen_metrics = {'{}_trim'.format(score_prefix): ['N',
-                                                               'h_mean',
-                                                               'h_sd',
-                                                               'sys_mean',
-                                                               'sys_sd',
-                                                               'wtkappa',
-                                                               'corr',
-                                                               smd_name,
-                                                               'RMSE',
-                                                               'R2'],
-                              '{}_trim_round'.format(score_prefix): ['sys_mean',
-                                                                     'sys_sd',
-                                                                     'kappa',
-                                                                     'exact_agr',
-                                                                     'adj_agr',
-                                                                     smd_name]}
+            smd_name = "DSM" if "DSM" in df_metrics else "SMD"
+            chosen_metrics = {
+                f"{score_prefix}_trim": [
+                    "N",
+                    "h_mean",
+                    "h_sd",
+                    "sys_mean",
+                    "sys_sd",
+                    "wtkappa",
+                    "corr",
+                    smd_name,
+                    "RMSE",
+                    "R2",
+                ],
+                f"{score_prefix}_trim_round": [
+                    "sys_mean",
+                    "sys_sd",
+                    "kappa",
+                    "exact_agr",
+                    "adj_agr",
+                    smd_name,
+                ],
+            }
 
         # extract the metrics we need from the given metrics frame
         metricdict = {}
         for score_type in chosen_metrics:
             for metric in chosen_metrics[score_type]:
-                colname = (metric if metric in ['h_mean', 'h_sd', 'N']
-                           else '{}.{}'.format(metric, score_type))
+                colname = metric if metric in ["h_mean", "h_sd", "N"] else f"{metric}.{score_type}"
                 values = df_metrics[metric][score_type]
                 metricdict[colname] = values
 
         df_filtered_metrics = pd.DataFrame([metricdict])
         return df_filtered_metrics
 
-    def compute_metrics(self,
-                        df,
-                        compute_shortened=False,
-                        use_scaled_predictions=False,
-                        include_second_score=False,
-                        population_sd_dict=None,
-                        population_mn_dict=None,
-                        smd_method='unpooled',
-                        use_diff_std_means=False):
+    def compute_metrics(
+        self,
+        df,
+        compute_shortened=False,
+        use_scaled_predictions=False,
+        include_second_score=False,
+        population_sd_dict=None,
+        population_mn_dict=None,
+        smd_method="unpooled",
+        use_diff_std_means=False,
+    ):
         """
         Compute association metrics for scores in the given data frame.
 
         This function compute association metrics for all score types.
         If ``include_second_score`` is ``True``, then it is assumed that
         a column called `sc2` containing a second human score is available
         and it should be used to compute the human-human evaluation stats
@@ -1076,15 +1126,15 @@
             A shortened version of the first data frame but
             is empty if ``compute_shortened`` is ``False``.
         """
         # shorter variable name is easier to work with
         use_scaled = use_scaled_predictions
 
         # are we using DSM or SMD?
-        smd_name = 'DSM' if use_diff_std_means else 'SMD'
+        smd_name = "DSM" if use_diff_std_means else "SMD"
 
         # get the population standard deviations for SMD if none were supplied
         if not population_sd_dict:
             population_sd_dict = {col: None for col in df.columns}
 
         # get the population standard deviations for SMD if none were supplied
         if not population_mn_dict:
@@ -1094,108 +1144,152 @@
         # probably not available for all of the responses in the test
         # set and so we want to exclude 'sc2' from human-system metrics
         # computation. In addition, we also want to compute the human-human
         # metrics only on the data that is double scored.
         df_human_human = pd.DataFrame()
         if include_second_score:
 
-            df_single = df.drop('sc2', axis=1)
+            df_single = df.drop("sc2", axis=1)
 
-            df_human_system = df_single.apply(lambda s:
-                                              self.metrics_helper(df_single['sc1'],
-                                                                  s,
-                                                                  population_sd_dict['sc1'],
-                                                                  population_sd_dict[s.name],
-                                                                  population_mn_dict['sc1'],
-                                                                  population_mn_dict[s.name],
-                                                                  smd_method,
-                                                                  use_diff_std_means))
-            df_double = df[df['sc2'].notnull()][['sc1', 'sc2']]
-            df_human_human = df_double.apply(lambda s:
-                                             self.metrics_helper(df_double['sc1'],
-                                                                 s,
-                                                                 population_sd_dict['sc1'],
-                                                                 population_sd_dict[s.name],
-                                                                 population_mn_dict['sc1'],
-                                                                 population_mn_dict[s.name],
-                                                                 'pooled',
-                                                                 use_diff_std_means))
+            df_human_system = df_single.apply(
+                lambda s: self.metrics_helper(
+                    df_single["sc1"],
+                    s,
+                    population_sd_dict["sc1"],
+                    population_sd_dict[s.name],
+                    population_mn_dict["sc1"],
+                    population_mn_dict[s.name],
+                    smd_method,
+                    use_diff_std_means,
+                )
+            )
+            df_double = df[df["sc2"].notnull()][["sc1", "sc2"]]
+            df_human_human = df_double.apply(
+                lambda s: self.metrics_helper(
+                    df_double["sc1"],
+                    s,
+                    population_sd_dict["sc1"],
+                    population_sd_dict[s.name],
+                    population_mn_dict["sc1"],
+                    population_mn_dict[s.name],
+                    "pooled",
+                    use_diff_std_means,
+                )
+            )
             # drop the sc1 column from the human-human agreement frame
-            df_human_human = df_human_human.drop('sc1', axis=1)
+            df_human_human = df_human_human.drop("sc1", axis=1)
 
             # sort the rows in the correct order
-            df_human_human = df_human_human.reindex(['N', 'h_mean', 'h_sd',
-                                                          'h_min', 'h_max',
-                                                          'sys_mean', 'sys_sd',
-                                                          'sys_min', 'sys_max',
-                                                          'corr', 'wtkappa', 'R2',
-                                                          'kappa', 'exact_agr',
-                                                          'adj_agr', smd_name, 'RMSE'])
+            df_human_human = df_human_human.reindex(
+                [
+                    "N",
+                    "h_mean",
+                    "h_sd",
+                    "h_min",
+                    "h_max",
+                    "sys_mean",
+                    "sys_sd",
+                    "sys_min",
+                    "sys_max",
+                    "corr",
+                    "wtkappa",
+                    "R2",
+                    "kappa",
+                    "exact_agr",
+                    "adj_agr",
+                    smd_name,
+                    "RMSE",
+                ]
+            )
             # rename `h_*` -> `h1_*` and `sys_*` -> `h2_*`
-            df_human_human.rename(lambda c: c.replace('h_', 'h1_').replace('sys_', 'h2_'),
-                                  inplace=True)
+            df_human_human.rename(
+                lambda c: c.replace("h_", "h1_").replace("sys_", "h2_"), inplace=True
+            )
             # drop RMSE and R2 because they are not meaningful for human raters
-            df_human_human.drop(['R2', 'RMSE'], inplace=True)
+            df_human_human.drop(["R2", "RMSE"], inplace=True)
             df_human_human = df_human_human.transpose()
             # convert N to integer if it's not empty else set to 0
             try:
-                df_human_human['N'] = df_human_human['N'].astype(int)
+                df_human_human["N"] = df_human_human["N"].astype(int)
             except ValueError:
-                df_human_human['N'] = 0
-            df_human_human.index = ['']
+                df_human_human["N"] = 0
+            df_human_human.index = [""]
         else:
-            df_human_system = df.apply(lambda s: self.metrics_helper(df['sc1'],
-                                                                     s,
-                                                                     population_sd_dict['sc1'],
-                                                                     population_sd_dict[s.name],
-                                                                     population_mn_dict['sc1'],
-                                                                     population_mn_dict[s.name],
-                                                                     smd_method,
-                                                                     use_diff_std_means))
+            df_human_system = df.apply(
+                lambda s: self.metrics_helper(
+                    df["sc1"],
+                    s,
+                    population_sd_dict["sc1"],
+                    population_sd_dict[s.name],
+                    population_mn_dict["sc1"],
+                    population_mn_dict[s.name],
+                    smd_method,
+                    use_diff_std_means,
+                )
+            )
 
         # drop 'sc1' column from the human-system frame and transpose
-        df_human_system = df_human_system.drop('sc1', axis=1)
+        df_human_system = df_human_system.drop("sc1", axis=1)
         df_human_system = df_human_system.transpose()
 
         # sort the columns and rows in the correct order
-        df_human_system = df_human_system[['N',
-                                           'h_mean', 'h_sd',
-                                           'h_min', 'h_max',
-                                           'sys_mean', 'sys_sd',
-                                           'sys_min', 'sys_max',
-                                           'corr',
-                                           'wtkappa', 'R2', 'kappa',
-                                           'exact_agr', 'adj_agr',
-                                           smd_name, 'RMSE']]
+        df_human_system = df_human_system[
+            [
+                "N",
+                "h_mean",
+                "h_sd",
+                "h_min",
+                "h_max",
+                "sys_mean",
+                "sys_sd",
+                "sys_min",
+                "sys_max",
+                "corr",
+                "wtkappa",
+                "R2",
+                "kappa",
+                "exact_agr",
+                "adj_agr",
+                smd_name,
+                "RMSE",
+            ]
+        ]
 
         # make N column an integer if it's not NaN else set it to 0
-        df_human_system['N'] = df_human_system['N'].astype(int)
-        all_rows_order = ['raw', 'raw_trim', 'raw_trim_round',
-                          'scale', 'scale_trim', 'scale_trim_round']
+        df_human_system["N"] = df_human_system["N"].astype(int)
+        all_rows_order = [
+            "raw",
+            "raw_trim",
+            "raw_trim_round",
+            "scale",
+            "scale_trim",
+            "scale_trim_round",
+        ]
         existing_rows_index = [row for row in all_rows_order if row in df_human_system.index]
         df_human_system = df_human_system.reindex(existing_rows_index)
 
         # extract some default metrics for a shorter version of this data frame
         # if we were asked to do so
         if compute_shortened:
-            df_human_system_filtered = self.filter_metrics(df_human_system,
-                                                           use_scaled_predictions=use_scaled)
+            df_human_system_filtered = self.filter_metrics(
+                df_human_system, use_scaled_predictions=use_scaled
+            )
         else:
             df_human_system_filtered = pd.DataFrame()
 
         # return all data frames
-        return (df_human_system,
-                df_human_system_filtered,
-                df_human_human)
-
-    def compute_metrics_by_group(self,
-                                 df_test,
-                                 grouping_variable,
-                                 use_scaled_predictions=False,
-                                 include_second_score=False):
+        return (df_human_system, df_human_system_filtered, df_human_human)
+
+    def compute_metrics_by_group(
+        self,
+        df_test,
+        grouping_variable,
+        use_scaled_predictions=False,
+        include_second_score=False,
+    ):
         """
         Compute a subset of evaluation metrics by subgroups.
 
         This method computes a subset of evalution metrics for the scores
         in the given data frame by group specified in ``grouping_variable``.
         See ``filter_metrics()`` above for a description of the subset
         that is selected.
@@ -1223,79 +1317,88 @@
         df_human_human_by_group : pandas DataFrame
             Data frame that either contains the human-human
             statistics or is an empty data frame, depending
             on whether ``include_second_score`` is `True``.
         """
         # get the population standard deviation that we will need to compute SMD for all columns
         # other than id and subgroup
-        population_sd_dict = {col: df_test[col].std(ddof=1)
-                              for col in df_test.columns if col not in ['spkitemid',
-                                                                        grouping_variable]}
-
-        population_mn_dict = {col: df_test[col].mean()
-                              for col in df_test.columns if col not in ['spkitemid',
-                                                                        grouping_variable]}
+        population_sd_dict = {
+            col: df_test[col].std(ddof=1)
+            for col in df_test.columns
+            if col not in ["spkitemid", grouping_variable]
+        }
+
+        population_mn_dict = {
+            col: df_test[col].mean()
+            for col in df_test.columns
+            if col not in ["spkitemid", grouping_variable]
+        }
 
         # check if any of the standard deviations is zero and
         # tell user to expect to see many warnings.
-        zero_sd_scores = [score for (score, sd) in population_sd_dict.items() if
-                          np.isclose(sd, 0, atol=1e-07)]
+        zero_sd_scores = [
+            score for (score, sd) in population_sd_dict.items() if np.isclose(sd, 0, atol=1e-07)
+        ]
         if len(zero_sd_scores) > 0:
-            warnings.warn("The standard deviation for {} scores "
-                          "is zero (all values are the same). You "
-                          "will see multiple warnings about DSM computation "
-                          "since this metric is computed separately for "
-                          "each subgroup.".format(', '.join(zero_sd_scores)))
+            warnings.warn(
+                f"The standard deviation for {', '.join(zero_sd_scores)} "
+                f"scores is zero (all values are the same). You will see "
+                f"multiple warnings about DSM computation since this metric "
+                f"is computed separately for each subgroup."
+            )
 
         # create a duplicate data frame to compute evaluations
         # over the whole data, i.e., across groups
         df_preds_all = df_test.copy()
-        df_preds_all[grouping_variable] = 'All data'
+        df_preds_all[grouping_variable] = "All data"
 
         # combine the two data frames
         df_preds_combined = pd.concat([df_test, df_preds_all], sort=True)
         df_preds_combined.reset_index(drop=True, inplace=True)
 
         # group by the grouping_variable columns
         grouped = df_preds_combined.groupby(grouping_variable)
 
         df_human_system_by_group = pd.DataFrame()
         df_human_human_by_group = pd.DataFrame()
 
         for group, df_group in grouped:
             df_group = df_group.drop(grouping_variable, axis=1)
 
-            (df_human_system_metrics,
-             df_human_system_metrics_short,
-             df_human_human_metrics
-             ) = self.compute_metrics(df_group,
-                                      compute_shortened=True,
-                                      use_scaled_predictions=use_scaled_predictions,
-                                      include_second_score=include_second_score,
-                                      population_sd_dict=population_sd_dict,
-                                      population_mn_dict=population_mn_dict,
-                                      use_diff_std_means=True)
+            (
+                df_human_system_metrics,
+                df_human_system_metrics_short,
+                df_human_human_metrics,
+            ) = self.compute_metrics(
+                df_group,
+                compute_shortened=True,
+                use_scaled_predictions=use_scaled_predictions,
+                include_second_score=include_second_score,
+                population_sd_dict=population_sd_dict,
+                population_mn_dict=population_mn_dict,
+                use_diff_std_means=True,
+            )
 
             # we need to convert the shortened data frame to a series here
             df_human_system_by_group[group] = df_human_system_metrics_short.iloc[0]
 
             # update the by group human-human metrics frame if
             # we have the second score column available
             if include_second_score:
                 df_human_human_metrics.index = [group]
-                df_human_human_by_group = pd.concat([df_human_human_by_group, df_human_human_metrics])
+                df_human_human_by_group = pd.concat(
+                    [df_human_human_by_group, df_human_human_metrics]
+                )
 
         # transpose the by group human-system metrics frame
         df_human_system_by_group = df_human_system_by_group.transpose()
 
         return (df_human_system_by_group, df_human_human_by_group)
 
-    def compute_degradation_and_disattenuated_correlations(self,
-                                                           df,
-                                                           use_all_responses=True):
+    def compute_degradation_and_disattenuated_correlations(self, df, use_all_responses=True):
         """
         Compute the degradation in performance when using system score.
 
         This method computes the degradation in performance when using the
         system to predict the score instead of a second human and also the
         disattenuated correlations between human and system scores.
         These are computed as the Pearson's correlation between the human score
@@ -1324,39 +1427,44 @@
             Data frame containing the human-system correlations, human-human
             correlations and disattenuated correlation.
         """
         if use_all_responses:
             df_responses = df
         else:
             # use only double scored data
-            df_responses = df[df['sc2'].notnull()]
+            df_responses = df[df["sc2"].notnull()]
 
         # compute the human-system and human-human metrics
-        (df_human_system_eval,
-         _,
-         df_human_human_eval) = self.compute_metrics(df_responses,
-                                                     include_second_score=True)
+        (df_human_system_eval, _, df_human_human_eval) = self.compute_metrics(
+            df_responses, include_second_score=True
+        )
 
         # compute disattenuated correlations
-        df_correlations = self.compute_disattenuated_correlations(df_human_system_eval['corr'],
-                                                                  df_human_human_eval['corr'])
+        df_correlations = self.compute_disattenuated_correlations(
+            df_human_system_eval["corr"], df_human_human_eval["corr"]
+        )
 
         # Compute degradation. we only care about the degradation in these metrics
-        degradation_metrics = ['corr', 'kappa', 'wtkappa',
-                               'exact_agr', 'adj_agr', 'SMD']
+        degradation_metrics = [
+            "corr",
+            "kappa",
+            "wtkappa",
+            "exact_agr",
+            "adj_agr",
+            "SMD",
+        ]
         df_human_system_eval = df_human_system_eval[degradation_metrics]
         df_human_human_eval = df_human_human_eval[degradation_metrics]
-        df_degradation = df_human_system_eval.apply(lambda row:
-                                                    row - df_human_human_eval.loc[''], axis=1)
+        df_degradation = df_human_system_eval.apply(
+            lambda row: row - df_human_human_eval.loc[""], axis=1
+        )
 
         return (df_degradation, df_correlations)
 
-    def run_training_analyses(self,
-                              data_container,
-                              configuration):
+    def run_training_analyses(self, data_container, configuration):
         """
         Run all analyses on the training data.
 
         Parameters
         ----------
         data_container : container.DataContainer
             The DataContainer object. This container must include the following
@@ -1390,175 +1498,191 @@
             - margcor_score_by_*
             - pcor_score_by_*
             - pcor_score_no_length_by_*
 
         configuration : configuration_parser.Configuration
             A new Configuration object.
         """
-        frame_names = ['train_features', 'train_metadata',
-                       'train_preprocessed_features', 'train_length',
-                       'train_features']
+        frame_names = [
+            "train_features",
+            "train_metadata",
+            "train_preprocessed_features",
+            "train_length",
+            "train_features",
+        ]
 
-        param_names = ['length_column', 'subgroups', 'selected_features']
+        param_names = ["length_column", "subgroups", "selected_features"]
 
         self.check_frame_names(data_container, frame_names)
 
         self.check_param_names(configuration, param_names)
 
         # only use the features selected by the model but keep their order the same
         # as in the original file as ordering may affect the sign in pca
         df_train = data_container.train_features.copy()
         df_train_length = data_container.train_length.copy()
         df_train_metadata = data_container.train_metadata.copy()
         df_train_preprocessed_features = data_container.train_preprocessed_features.copy()
 
-        subgroups = configuration['subgroups']
-        selected_features = configuration['selected_features']
-
-        df_train_preprocessed = pd.merge(df_train_preprocessed_features,
-                                         df_train_metadata, on='spkitemid')
+        subgroups = configuration["subgroups"]
+        selected_features = configuration["selected_features"]
 
-        assert (len(df_train_preprocessed.index) ==
-                len(df_train_preprocessed_features.index) ==
-                len(df_train_metadata.index))
+        df_train_preprocessed = pd.merge(
+            df_train_preprocessed_features, df_train_metadata, on="spkitemid"
+        )
+
+        assert (
+            len(df_train_preprocessed.index)
+            == len(df_train_preprocessed_features.index)
+            == len(df_train_metadata.index)
+        )
 
         # get descriptives, percentiles and outliers for the original feature values
         df_descriptives = self.compute_basic_descriptives(df_train, selected_features)
         df_percentiles = self.compute_percentiles(df_train, selected_features)
         df_outliers = self.compute_outliers(df_train, selected_features)
 
         # set a general boolean flag indicating if we should include length
         include_length = not df_train_length.empty
 
         # include length if available
         if include_length:
-            columns = selected_features + ['sc1', 'length']
-            df_train_with_length = df_train.merge(df_train_length, on='spkitemid')
-            df_train_preprocess_length = df_train_preprocessed.merge(df_train_length,
-                                                                     on='spkitemid')
+            columns = selected_features + ["sc1", "length"]
+            df_train_with_length = df_train.merge(df_train_length, on="spkitemid")
+            df_train_preprocess_length = df_train_preprocessed.merge(
+                df_train_length, on="spkitemid"
+            )
         else:
-            columns = selected_features + ['sc1']
+            columns = selected_features + ["sc1"]
             df_train_with_length = df_train
             df_train_preprocess_length = df_train_preprocessed
 
         # get pairwise correlations against the original training features
         # as well as the pre-processed training features
-        df_pairwise_cors_orig = df_train_with_length[columns].corr(method='pearson')
-        df_pairwise_cors_preprocess = df_train_preprocess_length[columns].corr(method='pearson')
+        df_pairwise_cors_orig = df_train_with_length[columns].corr(method="pearson")
+        df_pairwise_cors_preprocess = df_train_preprocess_length[columns].corr(method="pearson")
 
         # get marginal and partial correlations against sc1 for all data
         # for partial correlations, we partial out all other features
         df_train_with_group_for_all = df_train_preprocess_length.copy()
         df_train_with_group_for_all = df_train_with_group_for_all[columns]
-        df_train_with_group_for_all['all_data'] = 'All data'
+        df_train_with_group_for_all["all_data"] = "All data"
 
-        (df_margcor_sc1,
-         df_pcor_sc1,
-         df_pcor_sc1_no_length) = self.correlation_helper(df_train_with_group_for_all,
-                                                          'sc1',
-                                                          'all_data',
-                                                          include_length=include_length)
+        (df_margcor_sc1, df_pcor_sc1, df_pcor_sc1_no_length) = self.correlation_helper(
+            df_train_with_group_for_all,
+            "sc1",
+            "all_data",
+            include_length=include_length,
+        )
 
         # get marginal and partial correlations against length for all data
         # if the length column is available
         df_margcor_length = pd.DataFrame()
         df_pcor_length = pd.DataFrame()
 
         if include_length:
 
             df_train_with_group_for_all = df_train_preprocess_length.copy()
-            columns = selected_features + ['length']
+            columns = selected_features + ["length"]
 
             df_train_with_group_for_all = df_train_with_group_for_all[columns]
-            df_train_with_group_for_all['all_data'] = 'All data'
+            df_train_with_group_for_all["all_data"] = "All data"
 
-            (df_margcor_length,
-             df_pcor_length,
-             _) = self.correlation_helper(df_train_with_group_for_all,
-                                          'length',
-                                          'all_data')
+            (df_margcor_length, df_pcor_length, _) = self.correlation_helper(
+                df_train_with_group_for_all, "length", "all_data"
+            )
 
         # get marginal and partial correlations against sc1 by group (preprocessed features)
         # also include partial correlations with length if length is available
         score_corr_by_group_dict = {}
-        include_length = 'length' in df_train_preprocess_length
+        include_length = "length" in df_train_preprocess_length
         for grouping_variable in subgroups:
 
-            corr_by_group = self.compute_correlations_by_group(df_train_preprocess_length,
-                                                               selected_features,
-                                                               'sc1',
-                                                               grouping_variable,
-                                                               include_length=include_length)
+            corr_by_group = self.compute_correlations_by_group(
+                df_train_preprocess_length,
+                selected_features,
+                "sc1",
+                grouping_variable,
+                include_length=include_length,
+            )
 
             score_corr_by_group_dict[grouping_variable] = corr_by_group
 
         # get marginal and partial correlations against sc1 by group (preprocessed features)
         length_corr_by_group_dict = {}
         if include_length:
             for grouping_variable in subgroups:
 
-                corr_by_group = self.compute_correlations_by_group(df_train_preprocess_length,
-                                                                   selected_features,
-                                                                   'length',
-                                                                   grouping_variable)
+                corr_by_group = self.compute_correlations_by_group(
+                    df_train_preprocess_length,
+                    selected_features,
+                    "length",
+                    grouping_variable,
+                )
 
                 length_corr_by_group_dict[grouping_variable] = corr_by_group
 
         # get PCA information
-        df_pca_components, df_pca_variance = self.compute_pca(df_train_preprocessed,
-                                                              selected_features)
+        df_pca_components, df_pca_variance = self.compute_pca(
+            df_train_preprocessed, selected_features
+        )
 
         # Datasets to add
-        datasets = [{'name': 'feature_descriptives', 'frame': df_descriptives},
-                    {'name': 'feature_descriptivesExtra', 'frame': df_percentiles},
-                    {'name': 'feature_outliers', 'frame': df_outliers},
-                    {'name': 'cors_orig', 'frame': df_pairwise_cors_orig},
-                    {'name': 'cors_processed', 'frame': df_pairwise_cors_preprocess},
-                    {'name': 'margcor_score_all_data', 'frame': df_margcor_sc1},
-                    {'name': 'pcor_score_all_data', 'frame': df_pcor_sc1},
-                    {'name': 'pcor_score_no_length_all_data', 'frame': df_pcor_sc1_no_length},
-                    {'name': 'margcor_length_all_data', 'frame': df_margcor_length},
-                    {'name': 'pcor_length_all_data', 'frame': df_pcor_length},
-                    {'name': 'pca', 'frame': df_pca_components},
-                    {'name': 'pcavar', 'frame': df_pca_variance}]
+        datasets = [
+            {"name": "feature_descriptives", "frame": df_descriptives},
+            {"name": "feature_descriptivesExtra", "frame": df_percentiles},
+            {"name": "feature_outliers", "frame": df_outliers},
+            {"name": "cors_orig", "frame": df_pairwise_cors_orig},
+            {"name": "cors_processed", "frame": df_pairwise_cors_preprocess},
+            {"name": "margcor_score_all_data", "frame": df_margcor_sc1},
+            {"name": "pcor_score_all_data", "frame": df_pcor_sc1},
+            {"name": "pcor_score_no_length_all_data", "frame": df_pcor_sc1_no_length},
+            {"name": "margcor_length_all_data", "frame": df_margcor_length},
+            {"name": "pcor_length_all_data", "frame": df_pcor_length},
+            {"name": "pca", "frame": df_pca_components},
+            {"name": "pcavar", "frame": df_pca_variance},
+        ]
 
         # Add length correlation by group datasets
         for group in length_corr_by_group_dict:
 
-            (length_marg_cors,
-             length_part_cors,
-             _) = length_corr_by_group_dict.get(group,
-                                                (pd.DataFrame(),
-                                                 pd.DataFrame(),
-                                                 pd.DataFrame()))
-
-            datasets.extend([{'name': 'margcor_length_by_{}'.format(group),
-                              'frame': length_marg_cors},
-                             {'name': 'pcor_length_by_{}'.format(group),
-                              'frame': length_part_cors}])
+            (length_marg_cors, length_part_cors, _) = length_corr_by_group_dict.get(
+                group, (pd.DataFrame(), pd.DataFrame(), pd.DataFrame())
+            )
+
+            datasets.extend(
+                [
+                    {"name": f"margcor_length_by_{group}", "frame": length_marg_cors},
+                    {"name": f"pcor_length_by_{group}", "frame": length_part_cors},
+                ]
+            )
 
         # Add score correlations by group datasets
         for group in score_corr_by_group_dict:
 
-            (sc1_marg_cors,
-             sc1_part_cors,
-             sc1_part_cors_no_length) = score_corr_by_group_dict[group]
-
-            datasets.extend([{'name': 'margcor_score_by_{}'.format(group),
-                              'frame': sc1_marg_cors},
-                             {'name': 'pcor_score_by_{}'.format(group),
-                              'frame': sc1_part_cors},
-                             {'name': 'pcor_score_no_length_by_{}'.format(group),
-                              'frame': sc1_part_cors_no_length}])
+            (
+                sc1_marg_cors,
+                sc1_part_cors,
+                sc1_part_cors_no_length,
+            ) = score_corr_by_group_dict[group]
+
+            datasets.extend(
+                [
+                    {"name": f"margcor_score_by_{group}", "frame": sc1_marg_cors},
+                    {"name": f"pcor_score_by_{group}", "frame": sc1_part_cors},
+                    {
+                        "name": f"pcor_score_no_length_by_{group}",
+                        "frame": sc1_part_cors_no_length,
+                    },
+                ]
+            )
 
         return configuration, DataContainer(datasets=datasets)
 
-    def run_prediction_analyses(self,
-                                data_container,
-                                configuration):
+    def run_prediction_analyses(self, data_container, configuration):
         """
         Run all analyses on the system scores (predictions).
 
         Parameters
         ----------
         data_container : container.DataContainer
             The DataContainer object. This container must include the following
@@ -1587,157 +1711,167 @@
             - consistency_by_*
             - disattenduated_correlations_by_*
             - true_score_eval
 
         configuration : configuration_parser.Configuration
             A new Configuration object.
         """
-        frame_names = ['pred_test', 'test_metadata', 'test_human_scores']
+        frame_names = ["pred_test", "test_metadata", "test_human_scores"]
 
-        param_names = ['subgroups',
-                       'second_human_score_column',
-                       'use_scaled_predictions']
+        param_names = [
+            "subgroups",
+            "second_human_score_column",
+            "use_scaled_predictions",
+        ]
 
         self.check_frame_names(data_container, frame_names)
 
         self.check_param_names(configuration, param_names)
 
         df_test = data_container.pred_test.copy()
         df_test_metadata = data_container.test_metadata.copy()
         df_test_human_scores = data_container.test_human_scores.copy()
 
-        subgroups = configuration['subgroups']
-        use_scaled_predictions = configuration['use_scaled_predictions']
+        subgroups = configuration["subgroups"]
+        use_scaled_predictions = configuration["use_scaled_predictions"]
 
-        df_preds = pd.merge(df_test, df_test_metadata, on='spkitemid')
+        df_preds = pd.merge(df_test, df_test_metadata, on="spkitemid")
 
         assert len(df_preds.index) == len(df_test.index) == len(df_test_metadata.index)
 
         # set a general boolean flag indicating if
         # we should include the second human score
         include_second_score = not df_test_human_scores.empty
 
         # extract the columns that contain predictions
-        prediction_columns = [column for column in df_test if column != 'spkitemid']
+        prediction_columns = [column for column in df_test if column != "spkitemid"]
 
         # if a second score is available, use it
         if include_second_score:
-            prediction_columns.append('sc2')
-            df_preds_second_score = df_preds.merge(df_test_human_scores[['spkitemid', 'sc2']],
-                                                   on='spkitemid')
+            prediction_columns.append("sc2")
+            df_preds_second_score = df_preds.merge(
+                df_test_human_scores[["spkitemid", "sc2"]], on="spkitemid"
+            )
         else:
             df_preds_second_score = df_preds
 
         # compute the evaluation metrics over the whole data set
-        (df_human_system,
-         df_human_system_short,
-         df_human_human) = self.compute_metrics(df_preds_second_score[prediction_columns],
-                                                compute_shortened=True,
-                                                use_scaled_predictions=use_scaled_predictions,
-                                                include_second_score=include_second_score)
+        (df_human_system, df_human_system_short, df_human_human) = self.compute_metrics(
+            df_preds_second_score[prediction_columns],
+            compute_shortened=True,
+            use_scaled_predictions=use_scaled_predictions,
+            include_second_score=include_second_score,
+        )
 
         # compute the evaluation metrics by group
         eval_by_group_dict = {}
         for group in subgroups:
             group_columns = prediction_columns + [group]
-            metrics = self.compute_metrics_by_group(df_preds_second_score[group_columns],
-                                                    group,
-                                                    use_scaled_predictions=use_scaled_predictions,
-                                                    include_second_score=include_second_score)
+            metrics = self.compute_metrics_by_group(
+                df_preds_second_score[group_columns],
+                group,
+                use_scaled_predictions=use_scaled_predictions,
+                include_second_score=include_second_score,
+            )
             eval_by_group_dict[group] = metrics
 
         # compute the degradation statistics and disattenuated correlations
         # if we have the second human score available
         df_degradation = pd.DataFrame()
         df_correlations = pd.DataFrame()
         if include_second_score:
-            (df_degradation,
-             df_correlations) = self.compute_degradation_and_disattenuated_correlations(df_preds_second_score[prediction_columns])
+            (
+                df_degradation,
+                df_correlations,
+            ) = self.compute_degradation_and_disattenuated_correlations(
+                df_preds_second_score[prediction_columns]
+            )
 
         # the following two evaluations require rounded human scores
         # we create a column for this
-        df_preds['sc1_round'] = np.round(df_preds['sc1'])
+        df_preds["sc1_round"] = np.round(df_preds["sc1"])
 
         # compute the confusion matrix as a data frame
-        score_type = 'scale' if use_scaled_predictions else 'raw'
-        human_scores = df_preds['sc1_round'].astype('int64')
-        system_scores = df_preds['{}_trim_round'.format(score_type)].astype('int64')
+        score_type = "scale" if use_scaled_predictions else "raw"
+        human_scores = df_preds["sc1_round"].astype("int64")
+        system_scores = df_preds[f"{score_type}_trim_round"].astype("int64")
         conf_matrix = confusion_matrix(human_scores, system_scores)
         labels = sorted(pd.concat([human_scores, system_scores]).unique())
         df_confmatrix = pd.DataFrame(conf_matrix, index=labels, columns=labels).transpose()
 
         # compute the score distributions of the rounded human and system scores
-        df_score_dist = df_preds[['sc1_round',
-                                  '{}_trim_round'
-                                  ''.format(score_type)]].apply(lambda s:
-                                                                (s.value_counts() /
-                                                                 len(df_test) * 100))
+        df_score_dist = df_preds[["sc1_round", f"{score_type}_trim_round"]].apply(
+            lambda s: s.value_counts() / len(df_test) * 100
+        )
 
         # Replace any NaNs, which we might get because our model never
         # predicts a particular score label, with zeros.
         df_score_dist.fillna(0, inplace=True)
 
-        df_score_dist.columns = ['human', 'sys_{}'.format(score_type)]
-        df_score_dist['difference'] = (df_score_dist['sys_{}'.format(score_type)] -
-                                       df_score_dist['human'])
-        df_score_dist['score'] = df_score_dist.index
-
-        df_score_dist = df_score_dist[['score', 'human',
-                                       'sys_{}'.format(score_type),
-                                       'difference']]
-        df_score_dist.sort_values(by='score', inplace=True)
-
-        datasets = [{'name': 'eval', 'frame': df_human_system},
-                    {'name': 'eval_short', 'frame': df_human_system_short},
-                    {'name': 'consistency', 'frame': df_human_human},
-                    {'name': 'degradation', 'frame': df_degradation},
-                    {'name': 'disattenuated_correlations', 'frame': df_correlations},
-                    {'name': 'confMatrix', 'frame': df_confmatrix},
-                    {'name': 'score_dist', 'frame': df_score_dist}]
+        df_score_dist.columns = ["human", f"sys_{score_type}"]
+        df_score_dist["difference"] = df_score_dist[f"sys_{score_type}"] - df_score_dist["human"]
+        df_score_dist["score"] = df_score_dist.index
+
+        df_score_dist = df_score_dist[["score", "human", f"sys_{score_type}", "difference"]]
+        df_score_dist.sort_values(by="score", inplace=True)
+
+        datasets = [
+            {"name": "eval", "frame": df_human_system},
+            {"name": "eval_short", "frame": df_human_system_short},
+            {"name": "consistency", "frame": df_human_human},
+            {"name": "degradation", "frame": df_degradation},
+            {"name": "disattenuated_correlations", "frame": df_correlations},
+            {"name": "confMatrix", "frame": df_confmatrix},
+            {"name": "score_dist", "frame": df_score_dist},
+        ]
 
         # compute true-score analyses if we have second score
         # or have been given rater error variance
         rater_error_variance = configuration.get_rater_error_variance()
 
         if include_second_score or rater_error_variance is not None:
-            system_score_columns = [col for col in prediction_columns
-                                    if col not in ['sc1', 'sc2']]
+            system_score_columns = [col for col in prediction_columns if col not in ["sc1", "sc2"]]
 
-            human_score_columns = [col for col in prediction_columns
-                                   if col in ['sc1', 'sc2']]
+            human_score_columns = [col for col in prediction_columns if col in ["sc1", "sc2"]]
 
-            df_prmse = get_true_score_evaluations(df_preds_second_score,
-                                                  system_score_columns,
-                                                  human_score_columns,
-                                                  rater_error_variance)
+            df_prmse = get_true_score_evaluations(
+                df_preds_second_score,
+                system_score_columns,
+                human_score_columns,
+                rater_error_variance,
+            )
 
-            datasets.extend([{'name': 'true_score_eval', 'frame': df_prmse}])
+            datasets.extend([{"name": "true_score_eval", "frame": df_prmse}])
 
         for group in eval_by_group_dict:
             eval_by_group, consistency_by_group = eval_by_group_dict[group]
 
             # compute disattenuated correlations if we have the second human score
             if include_second_score:
-                dis_corr_by_group = self.compute_disattenuated_correlations(eval_by_group['corr.{}_trim'.format(score_type)],
-                                                                            consistency_by_group['corr'])
+                dis_corr_by_group = self.compute_disattenuated_correlations(
+                    eval_by_group[f"corr.{score_type}_trim"],
+                    consistency_by_group["corr"],
+                )
             else:
                 dis_corr_by_group = pd.DataFrame()
 
-            datasets.extend([{'name': 'eval_by_{}'.format(group),
-                              'frame': eval_by_group},
-                             {'name': 'consistency_by_{}'.format(group),
-                              'frame': consistency_by_group},
-                             {'name': 'disattenuated_correlations_by_{}'.format(group),
-                              'frame': dis_corr_by_group}])
+            datasets.extend(
+                [
+                    {"name": f"eval_by_{group}", "frame": eval_by_group},
+                    {"name": f"consistency_by_{group}", "frame": consistency_by_group},
+                    {
+                        "name": f"disattenuated_correlations_by_{group}",
+                        "frame": dis_corr_by_group,
+                    },
+                ]
+            )
 
         return configuration, DataContainer(datasets=datasets)
 
-    def run_data_composition_analyses_for_rsmtool(self,
-                                                  data_container,
-                                                  configuration):
+    def run_data_composition_analyses_for_rsmtool(self, data_container, configuration):
         """
         Run all data composition analyses for RSMTool.
 
         Parameters
         ----------
         data_container : container.DataContainer
             The DataContainer object. This container must include the following
@@ -1757,86 +1891,108 @@
             - train_excluded_composition
             - data_composition
             - data_composition_by_*
 
         configuration : configuration_parser.Configuration
             A new Configuration object.
         """
-        frame_names = ['train_metadata', 'test_metadata',
-                       'train_excluded', 'test_excluded',
-                       'train_features']
-
-        param_names = ['candidate_column', 'subgroups',
-                       'exclude_zero_scores', 'exclude_listwise']
+        frame_names = [
+            "train_metadata",
+            "test_metadata",
+            "train_excluded",
+            "test_excluded",
+            "train_features",
+        ]
+
+        param_names = [
+            "candidate_column",
+            "subgroups",
+            "exclude_zero_scores",
+            "exclude_listwise",
+        ]
 
         self.check_frame_names(data_container, frame_names)
 
         self.check_param_names(configuration, param_names)
 
-        features = [column for column in data_container.train_features.columns
-                    if column not in ['spkitemid', 'sc1']]
-
-        exclude_scores = configuration['exclude_zero_scores']
-        exclude_listwise = configuration['exclude_listwise']
-
-        subgroups = configuration['subgroups']
-        candidate_column = configuration['candidate_column']
-
-        df_train_excluded = self.analyze_excluded_responses(data_container['train_excluded'],
-                                                            features,
-                                                            'Score/Features',
-                                                            exclude_zero_scores=exclude_scores,
-                                                            exclude_listwise=exclude_listwise)
-
-        df_test_excluded = self.analyze_excluded_responses(data_container['test_excluded'],
-                                                           features,
-                                                           'Score/Features',
-                                                           exclude_zero_scores=exclude_scores,
-                                                           exclude_listwise=exclude_listwise)
-
-        df_data_composition = self.analyze_used_responses(data_container['train_metadata'],
-                                                          data_container['test_metadata'],
-                                                          subgroups, candidate_column)
+        features = [
+            column
+            for column in data_container.train_features.columns
+            if column not in ["spkitemid", "sc1"]
+        ]
+
+        exclude_scores = configuration["exclude_zero_scores"]
+        exclude_listwise = configuration["exclude_listwise"]
+
+        subgroups = configuration["subgroups"]
+        candidate_column = configuration["candidate_column"]
+
+        df_train_excluded = self.analyze_excluded_responses(
+            data_container["train_excluded"],
+            features,
+            "Score/Features",
+            exclude_zero_scores=exclude_scores,
+            exclude_listwise=exclude_listwise,
+        )
+
+        df_test_excluded = self.analyze_excluded_responses(
+            data_container["test_excluded"],
+            features,
+            "Score/Features",
+            exclude_zero_scores=exclude_scores,
+            exclude_listwise=exclude_listwise,
+        )
+
+        df_data_composition = self.analyze_used_responses(
+            data_container["train_metadata"],
+            data_container["test_metadata"],
+            subgroups,
+            candidate_column,
+        )
 
         # do the analysis by subgroups
         # first create a joint data frame with both sets
-        df_train_metadata_with_set = data_container['train_metadata'].copy()
-        df_test_metadata_with_set = data_container['test_metadata'].copy()
+        df_train_metadata_with_set = data_container["train_metadata"].copy()
+        df_test_metadata_with_set = data_container["test_metadata"].copy()
 
-        df_train_metadata_with_set['set'] = 'Training set'
-        df_test_metadata_with_set['set'] = 'Evaluation set'
+        df_train_metadata_with_set["set"] = "Training set"
+        df_test_metadata_with_set["set"] = "Evaluation set"
 
-        df_both_metadata = pd.merge(df_train_metadata_with_set,
-                                    df_test_metadata_with_set,
-                                    how='outer')
+        df_both_metadata = pd.merge(
+            df_train_metadata_with_set, df_test_metadata_with_set, how="outer"
+        )
 
         # create contingency table for each subgroup
         data_composition_by_group_dict = {}
         for grouping_variable in subgroups:
-            df_crosstab_group = pd.crosstab(df_both_metadata[grouping_variable],
-                                            df_both_metadata['set'])
-            df_crosstab_group = df_crosstab_group[['Training set',
-                                                   'Evaluation set']]
+            df_crosstab_group = pd.crosstab(
+                df_both_metadata[grouping_variable], df_both_metadata["set"]
+            )
+            df_crosstab_group = df_crosstab_group[["Training set", "Evaluation set"]]
             df_crosstab_group.insert(0, grouping_variable, df_crosstab_group.index)
             data_composition_by_group_dict[grouping_variable] = df_crosstab_group
 
-        datasets = [{'name': 'test_excluded_composition', 'frame': df_test_excluded},
-                    {'name': 'train_excluded_composition', 'frame': df_train_excluded},
-                    {'name': 'data_composition', 'frame': df_data_composition}]
+        datasets = [
+            {"name": "test_excluded_composition", "frame": df_test_excluded},
+            {"name": "train_excluded_composition", "frame": df_train_excluded},
+            {"name": "data_composition", "frame": df_data_composition},
+        ]
 
         for group in data_composition_by_group_dict:
 
-            datasets.append({'name': 'data_composition_by_{}'.format(group),
-                             'frame': data_composition_by_group_dict[group]})
+            datasets.append(
+                {
+                    "name": f"data_composition_by_{group}",
+                    "frame": data_composition_by_group_dict[group],
+                }
+            )
 
         return configuration, DataContainer(datasets=datasets)
 
-    def run_data_composition_analyses_for_rsmeval(self,
-                                                  data_container,
-                                                  configuration):
+    def run_data_composition_analyses_for_rsmeval(self, data_container, configuration):
         """
         Run all data composition analyses for RSMEval.
 
         Parameters
         ----------
         data_container : container.DataContainer
             The DataContainer object. This container must include the following
@@ -1855,63 +2011,77 @@
             - test_excluded_composition
             - data_composition
             - data_composition_by_*
 
         configuration : configuration_parser.Configuration
             A new Configuration object.
         """
-        frame_names = ['test_metadata', 'test_excluded']
+        frame_names = ["test_metadata", "test_excluded"]
 
-        param_names = ['candidate_column', 'subgroups',
-                       'exclude_zero_scores', 'exclude_listwise']
+        param_names = [
+            "candidate_column",
+            "subgroups",
+            "exclude_zero_scores",
+            "exclude_listwise",
+        ]
 
         self.check_frame_names(data_container, frame_names)
 
         self.check_param_names(configuration, param_names)
 
-        exclude_scores = configuration['exclude_zero_scores']
-        exclude_listwise = configuration['exclude_listwise']
+        exclude_scores = configuration["exclude_zero_scores"]
+        exclude_listwise = configuration["exclude_listwise"]
 
-        subgroups = configuration['subgroups']
-        candidate_column = configuration['candidate_column']
+        subgroups = configuration["subgroups"]
+        candidate_column = configuration["candidate_column"]
 
         # analyze excluded responses
-        df_test_excluded = self.analyze_excluded_responses(data_container['test_excluded'],
-                                                           ['raw'],
-                                                           'Human/System',
-                                                           exclude_zero_scores=exclude_scores,
-                                                           exclude_listwise=exclude_listwise)
+        df_test_excluded = self.analyze_excluded_responses(
+            data_container["test_excluded"],
+            ["raw"],
+            "Human/System",
+            exclude_zero_scores=exclude_scores,
+            exclude_listwise=exclude_listwise,
+        )
 
         # rename the columns and index in the analysis data frame
-        df_test_excluded.rename(columns={'all features numeric':
-                                         'numeric system score',
-                                         'non-numeric feature values':
-                                         'non-numeric system score'},
-
-                                inplace=True)
-        df_data_composition = self.analyze_used_predictions(data_container['test_metadata'],
-                                                            subgroups,
-                                                            candidate_column)
+        df_test_excluded.rename(
+            columns={
+                "all features numeric": "numeric system score",
+                "non-numeric feature values": "non-numeric system score",
+            },
+            inplace=True,
+        )
+        df_data_composition = self.analyze_used_predictions(
+            data_container["test_metadata"], subgroups, candidate_column
+        )
 
         # create contingency table for each group
         data_composition_by_group_dict = {}
         for grouping_variable in subgroups:
-            series_crosstab_group = pd.pivot_table(data_container['test_metadata'],
-                                                   values='spkitemid',
-                                                   index=[grouping_variable],
-                                                   aggfunc=len)
+            series_crosstab_group = pd.pivot_table(
+                data_container["test_metadata"],
+                values="spkitemid",
+                index=[grouping_variable],
+                aggfunc=len,
+            )
 
             df_crosstab_group = pd.DataFrame(series_crosstab_group)
             df_crosstab_group.insert(0, grouping_variable, df_crosstab_group.index)
-            df_crosstab_group.rename(columns={'spkitemid': 'N responses'},
-                                     inplace=True)
+            df_crosstab_group.rename(columns={"spkitemid": "N responses"}, inplace=True)
             data_composition_by_group_dict[grouping_variable] = df_crosstab_group
 
-        datasets = [{'name': 'test_excluded_composition', 'frame': df_test_excluded},
-                    {'name': 'data_composition', 'frame': df_data_composition}]
+        datasets = [
+            {"name": "test_excluded_composition", "frame": df_test_excluded},
+            {"name": "data_composition", "frame": df_data_composition},
+        ]
 
         for group in data_composition_by_group_dict:
 
-            datasets.append({'name': 'data_composition_by_{}'.format(group),
-                             'frame': data_composition_by_group_dict[group]})
+            datasets.append(
+                {
+                    "name": f"data_composition_by_{group}",
+                    "frame": data_composition_by_group_dict[group],
+                }
+            )
 
         return configuration, DataContainer(datasets=datasets)
```

### Comparing `rsmtool-9.0.1/rsmtool/comparer.py` & `rsmtool-9.1.1/rsmtool/comparer.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,81 +16,83 @@
 import numpy as np
 import pandas as pd
 from scipy.stats import pearsonr
 
 from .reader import DataReader
 from .utils.files import get_output_directory_extension
 
-_df_eval_columns_existing_raw = ["N",
-                                 "h_mean",
-                                 "h_sd",
-                                 "sys_mean.raw_trim",
-                                 "sys_sd.raw_trim",
-                                 "corr.raw_trim",
-                                 "SMD.raw_trim",
-                                 "sys_mean.raw_trim_round",
-                                 "sys_sd.raw_trim_round",
-                                 "exact_agr.raw_trim_round",
-                                 "kappa.raw_trim_round",
-                                 "wtkappa.raw_trim",
-                                 "adj_agr.raw_trim_round",
-                                 "SMD.raw_trim_round",
-                                 "R2.raw_trim",
-                                 "RMSE.raw_trim"]
-
-_df_eval_columns_existing_scale = ["N",
-                                   "h_mean",
-                                   "h_sd",
-                                   "sys_mean.scale_trim",
-                                   "sys_sd.scale_trim",
-                                   "corr.scale_trim",
-                                   "SMD.scale_trim",
-                                   "sys_mean.scale_trim_round",
-                                   "sys_sd.scale_trim_round",
-                                   "exact_agr.scale_trim_round",
-                                   "kappa.scale_trim_round",
-                                   "wtkappa.scale_trim",
-                                   "adj_agr.scale_trim_round",
-                                   "SMD.scale_trim_round",
-                                   "R2.scale_trim",
-                                   "RMSE.scale_trim"]
-
-
-_df_eval_columns_renamed = ["N",
-                            "H1 mean",
-                            "H1 SD",
-                            "score mean(b)",
-                            "score SD(b)",
-                            "Pearson(b)",
-                            "SMD(b)",
-                            "score mean(br)",
-                            "score SD(br)",
-                            "Agmt.(br)",
-                            "K(br)",
-                            "QWK(b)",
-                            "Adj. Agmt.(br)",
-                            "SMD(br)",
-                            "R2(b)",
-                            "RMSE(b)"]
-
-raw_rename_dict = dict(zip(_df_eval_columns_existing_raw,
-                           _df_eval_columns_renamed))
-scale_rename_dict = dict(zip(_df_eval_columns_existing_scale,
-                             _df_eval_columns_renamed))
+_df_eval_columns_existing_raw = [
+    "N",
+    "h_mean",
+    "h_sd",
+    "sys_mean.raw_trim",
+    "sys_sd.raw_trim",
+    "corr.raw_trim",
+    "SMD.raw_trim",
+    "sys_mean.raw_trim_round",
+    "sys_sd.raw_trim_round",
+    "exact_agr.raw_trim_round",
+    "kappa.raw_trim_round",
+    "wtkappa.raw_trim",
+    "adj_agr.raw_trim_round",
+    "SMD.raw_trim_round",
+    "R2.raw_trim",
+    "RMSE.raw_trim",
+]
+
+_df_eval_columns_existing_scale = [
+    "N",
+    "h_mean",
+    "h_sd",
+    "sys_mean.scale_trim",
+    "sys_sd.scale_trim",
+    "corr.scale_trim",
+    "SMD.scale_trim",
+    "sys_mean.scale_trim_round",
+    "sys_sd.scale_trim_round",
+    "exact_agr.scale_trim_round",
+    "kappa.scale_trim_round",
+    "wtkappa.scale_trim",
+    "adj_agr.scale_trim_round",
+    "SMD.scale_trim_round",
+    "R2.scale_trim",
+    "RMSE.scale_trim",
+]
+
+
+_df_eval_columns_renamed = [
+    "N",
+    "H1 mean",
+    "H1 SD",
+    "score mean(b)",
+    "score SD(b)",
+    "Pearson(b)",
+    "SMD(b)",
+    "score mean(br)",
+    "score SD(br)",
+    "Agmt.(br)",
+    "K(br)",
+    "QWK(b)",
+    "Adj. Agmt.(br)",
+    "SMD(br)",
+    "R2(b)",
+    "RMSE(b)",
+]
+
+raw_rename_dict = dict(zip(_df_eval_columns_existing_raw, _df_eval_columns_renamed))
+scale_rename_dict = dict(zip(_df_eval_columns_existing_scale, _df_eval_columns_renamed))
 
 
 class Comparer:
     """Class to perform comparisons between two RSMTool experiments."""
 
     @staticmethod
-    def _modify_eval_columns_to_ensure_version_compatibilty(df,
-                                                            rename_dict,
-                                                            existing_eval_cols,
-                                                            short_metrics_list,
-                                                            raise_warnings=True):
+    def _modify_eval_columns_to_ensure_version_compatibilty(
+        df, rename_dict, existing_eval_cols, short_metrics_list, raise_warnings=True
+    ):
         """
         Ensure that column names in eval data frames are backwards compatible.
 
         This helper method ensures that the column names for eval data frames
         are forward and backward compatible. There are two major changes in
         RSMTool (7.0 or greater) that necessitate this: (1) for subgroup
         calculations, 'DSM' is now used instead of 'SMD', and (2) QWK
@@ -121,41 +123,46 @@
             The updated list of columns for the short metrics file.
         smd_name : str
             The SMD column name (either 'SMD' or 'DSM')
         """
         rename_dict_new = deepcopy(rename_dict)
         existing_eval_cols_new = deepcopy(existing_eval_cols)
         short_metrics_list_new = deepcopy(short_metrics_list)
-        smd_name = 'SMD'
+        smd_name = "SMD"
 
         # previously, the QWK metric used `trim_round` scores; now, we use just `trim` scores;
         # We check whether `trim_round` scores were used and
         # raise an error if this is the case
-        if any(col.endswith('trim_round') for col in df if col.startswith('wtkappa')):
-            raise ValueError("RSMTool (7.0 or greater) uses "
-                             "unrounded scores for weighted kappa calculations. At least one "
-                             "of your experiments was run "
-                             "using an older version of RSMTool that used  "
-                             "rounded scores instead. Please re-run "
-                             "the experiment with the latest version of RSMTool.")
+        if any(col.endswith("trim_round") for col in df if col.startswith("wtkappa")):
+            raise ValueError(
+                "RSMTool (7.0 or greater) uses "
+                "unrounded scores for weighted kappa calculations. At least one "
+                "of your experiments was run "
+                "using an older version of RSMTool that used  "
+                "rounded scores instead. Please re-run "
+                "the experiment with the latest version of RSMTool."
+            )
 
         # we check if DSM was calculated (which is what we expect for subgroup evals),
         # and if so, we update the rename dictionary and column lists accordingly; we
         # also set `smd_name` equal to 'DSM'
-        if any(col.startswith('DSM') for col in df):
-            smd_name = 'DSM'
-            existing_eval_cols_new = [col.replace('SMD', 'DSM')
-                                      for col in existing_eval_cols_new]
-            rename_dict_new = {key.replace('SMD', 'DSM'): val.replace('SMD', 'DSM')
-                               for key, val in rename_dict_new.items()}
-
-        return (rename_dict_new,
-                existing_eval_cols_new,
-                short_metrics_list_new,
-                smd_name)
+        if any(col.startswith("DSM") for col in df):
+            smd_name = "DSM"
+            existing_eval_cols_new = [col.replace("SMD", "DSM") for col in existing_eval_cols_new]
+            rename_dict_new = {
+                key.replace("SMD", "DSM"): val.replace("SMD", "DSM")
+                for key, val in rename_dict_new.items()
+            }
+
+        return (
+            rename_dict_new,
+            existing_eval_cols_new,
+            short_metrics_list_new,
+            smd_name,
+        )
 
     @staticmethod
     def make_summary_stat_df(df):
         """
         Compute summary statistics for the data in the given frame.
 
         Parameters
@@ -170,26 +177,25 @@
             in the input frame.
         """
         series = []
         for summary_func in [np.mean, np.std, np.median, np.min, np.max]:
 
             # apply function, but catch and ignore warnings
             with warnings.catch_warnings():
-                warnings.simplefilter('ignore')
+                warnings.simplefilter("ignore")
                 series.append(df.apply(summary_func))
 
         res = pd.concat(series, axis=1, sort=True)
-        res.columns = ['MEAN', 'SD', 'MEDIAN', 'MIN', 'MAX']
+        res.columns = ["MEAN", "SD", "MEDIAN", "MIN", "MAX"]
         return res
 
     @staticmethod
-    def compute_correlations_between_versions(df_old,
-                                              df_new,
-                                              human_score='sc1',
-                                              id_column='spkitemid'):
+    def compute_correlations_between_versions(
+        df_old, df_new, human_score="sc1", id_column="spkitemid"
+    ):
         """
         Compute correlations between old and new feature values.
 
         This method computes correlations between old and new feature values
         in the two given frames as well as the correlations between each
         feature value and the human score.
 
@@ -219,68 +225,78 @@
         ------
         ValueError
             If there are no shared features between the two sets.
         ValueError
             If there are no shared responses between the two sets.
         """
         # Only use features that appear in both datasets
-        features_old = [column for column in df_old
-                        if column not in [id_column, human_score]]
-        features_new = [column for column in df_new
-                        if column not in [id_column, human_score]]
+        features_old = [column for column in df_old if column not in [id_column, human_score]]
+        features_new = [column for column in df_new if column not in [id_column, human_score]]
 
         features = list(set(features_old).intersection(features_new))
 
         if len(features) == 0:
-            raise ValueError("There are no matching features "
-                             "in these two data sets.")
+            raise ValueError("There are no matching features " "in these two data sets.")
 
         columns = features + [id_column, human_score]
 
         # merge the two data sets and display a warning
         # if there are non-matching ids
-        df_merged = pd.merge(df_old[columns],
-                             df_new[columns],
-                             on=[id_column],
-                             suffixes=['%%%old', '%%%new'])
+        df_merged = pd.merge(
+            df_old[columns],
+            df_new[columns],
+            on=[id_column],
+            suffixes=["%%%old", "%%%new"],
+        )
 
         if len(df_merged) == 0:
             raise ValueError("There are no shared ids between these two datasets.")
 
         if len(df_merged) != len(df_old):
-            warnings.warn("Some responses from the old data "
-                          "were not present in the new data and therefore "
-                          "were excluded from the analysis.")
+            warnings.warn(
+                "Some responses from the old data "
+                "were not present in the new data and therefore "
+                "were excluded from the analysis."
+            )
 
         if len(df_merged) != len(df_new):
-            warnings.warn("Some responses from the new data "
-                          "were not present in the old data and therefore "
-                          "were excluded from the analysis.")
+            warnings.warn(
+                "Some responses from the new data "
+                "were not present in the old data and therefore "
+                "were excluded from the analysis."
+            )
 
         # compute correlations between each feature and human score.
         # we are using the same approach as used in analysis.py
         correlation_list = []
         for feature in features:
 
             # compute correlations
-            df_cor = pd.DataFrame({'Feature': [feature],
-                                   'N': len(df_merged),
-                                   'human_old': pearsonr(df_merged['{}%%%old'.format(human_score)],
-                                                         df_merged['{}%%%old'.format(feature)])[0],
-                                   'human_new': pearsonr(df_merged['{}%%%new'.format(human_score)],
-                                                         df_merged['{}%%%new'.format(feature)])[0],
-                                   'old_new': pearsonr(df_merged['{}%%%new'.format(feature)],
-                                                       df_merged['{}%%%old'.format(feature)])[0]})
+            df_cor = pd.DataFrame(
+                {
+                    "Feature": [feature],
+                    "N": len(df_merged),
+                    "human_old": pearsonr(
+                        df_merged[f"{human_score}%%%old"], df_merged[f"{feature}%%%old"]
+                    )[0],
+                    "human_new": pearsonr(
+                        df_merged[f"{human_score}%%%new"], df_merged[f"{feature}%%%new"]
+                    )[0],
+                    "old_new": pearsonr(
+                        df_merged[f"{feature}%%%new"], df_merged[f"{feature}%%%old"]
+                    )[0],
+                }
+            )
             correlation_list.append(df_cor)
 
         df_correlations = pd.concat(correlation_list, sort=True)
-        df_correlations.index = df_correlations['Feature']
+        df_correlations.index = df_correlations["Feature"]
         df_correlations.index.name = None
 
-        return(df_correlations)
+        return df_correlations
 
     @staticmethod
     def process_confusion_matrix(conf_matrix):
         """
         Add "human" and "machine" to column names in the confusion matrix.
 
         Parameters
@@ -291,16 +307,16 @@
         Returns
         -------
         conf_matrix_renamed : pandas DataFrame
             pandas Data Frame containing the confusion matrix
             with the columns renamed.
         """
         conf_matrix_renamed = conf_matrix.copy()
-        conf_matrix_renamed.index = ['machine {}'.format(n) for n in conf_matrix.index]
-        conf_matrix_renamed.columns = ['human {}'.format(x) for x in conf_matrix.columns]
+        conf_matrix_renamed.index = [f"machine {n}" for n in conf_matrix.index]
+        conf_matrix_renamed.columns = [f"human {x}" for x in conf_matrix.columns]
         return conf_matrix_renamed
 
     def load_rsmtool_output(self, filedir, figdir, experiment_id, prefix, groups_eval):
         """
         Load all of the outputs of an rsmtool experiment.
 
         For each type of output, we first check whether the file exists
@@ -331,305 +347,333 @@
         """
         file_format = get_output_directory_extension(filedir, experiment_id)
 
         files = defaultdict(pd.DataFrame)
         figs = {}
 
         # feature distributions and the inter-feature correlations
-        feature_train_file = join(filedir, '{}_train_features.{}'.format(experiment_id,
-                                                                         file_format))
+        feature_train_file = join(filedir, f"{experiment_id}_train_features.{file_format}")
         if exists(feature_train_file):
-            files['df_train_features'] = DataReader.read_from_file(feature_train_file)
+            files["df_train_features"] = DataReader.read_from_file(feature_train_file)
 
-        feature_distplots_file = join(figdir, '{}_distrib.svg'.format(experiment_id))
+        feature_distplots_file = join(figdir, f"{experiment_id}_distrib.svg")
         if exists(feature_distplots_file):
-            figs['feature_distplots'] = feature_distplots_file
+            figs["feature_distplots"] = feature_distplots_file
 
-        feature_cors_file = join(filedir, '{}_cors_processed.{}'.format(experiment_id,
-                                                                        file_format))
+        feature_cors_file = join(filedir, f"{experiment_id}_cors_processed.{file_format}")
         if exists(feature_cors_file):
-            files['df_feature_cors'] = DataReader.read_from_file(feature_cors_file, index_col=0)
+            files["df_feature_cors"] = DataReader.read_from_file(feature_cors_file, index_col=0)
 
         # df_scores
-        scores_file = join(filedir, '{}_pred_processed.{}'.format(experiment_id,
-                                                                  file_format))
+        scores_file = join(filedir, f"{experiment_id}_pred_processed.{file_format}")
         if exists(scores_file):
-            df_scores = DataReader.read_from_file(scores_file, converters={'spkitemid': str})
-            files['df_scores'] = df_scores[['spkitemid', 'sc1', prefix]]
+            df_scores = DataReader.read_from_file(scores_file, converters={"spkitemid": str})
+            files["df_scores"] = df_scores[["spkitemid", "sc1", prefix]]
 
         # model coefficients if present
-        betas_file = join(filedir, '{}_betas.{}'.format(experiment_id,
-                                                        file_format))
+        betas_file = join(filedir, f"{experiment_id}_betas.{file_format}")
         if exists(betas_file):
-            files['df_coef'] = DataReader.read_from_file(betas_file, index_col=0)
-            files['df_coef'].index.name = None
+            files["df_coef"] = DataReader.read_from_file(betas_file, index_col=0)
+            files["df_coef"].index.name = None
 
         # read in the model fit files if present
-        model_fit_file = join(filedir, '{}_model_fit.{}'.format(experiment_id,
-                                                                file_format))
+        model_fit_file = join(filedir, f"{experiment_id}_model_fit.{file_format}")
         if exists(model_fit_file):
-            files['df_model_fit'] = DataReader.read_from_file(model_fit_file)
+            files["df_model_fit"] = DataReader.read_from_file(model_fit_file)
 
         # human human agreement
-        consistency_file = join(filedir, '{}_consistency.{}'.format(experiment_id,
-                                                                    file_format))
+        consistency_file = join(filedir, f"{experiment_id}_consistency.{file_format}")
 
         # load if consistency file is present
         if exists(consistency_file):
             df_consistency = DataReader.read_from_file(consistency_file, index_col=0)
-            files['df_consistency'] = df_consistency
+            files["df_consistency"] = df_consistency
 
         # degradation
-        degradation_file = join(filedir, "{}_degradation.{}".format(experiment_id,
-                                                                    file_format))
+        degradation_file = join(filedir, f"{experiment_id}_degradation.{file_format}")
 
         # load if degradation file is present
         if exists(degradation_file):
             df_degradation = DataReader.read_from_file(degradation_file, index_col=0)
-            files['df_degradation'] = df_degradation
+            files["df_degradation"] = df_degradation
 
         # disattenuated correlations
-        dis_corr_file = join(filedir, "{}_disattenuated_correlations.{}".format(experiment_id,
-                                                                                file_format))
+        dis_corr_file = join(filedir, f"{experiment_id}_disattenuated_correlations.{file_format}")
 
         # load if disattenuated correlations is present
         if exists(dis_corr_file):
             df_dis_corr = DataReader.read_from_file(dis_corr_file, index_col=0)
             # we only use the row for raw_trim or scale_trim score
-            files['df_disattenuated_correlations'] = df_dis_corr.loc[['{}_trim'.format(prefix)]]
+            files["df_disattenuated_correlations"] = df_dis_corr.loc[[f"{prefix}_trim"]]
 
         # read in disattenuated correlations by group
         for group in groups_eval:
-            group_dis_corr_file = join(filedir,
-                                       '{}_disattenuated_correlations_by_{}.{}'.format(experiment_id,
-                                                                                       group,
-                                                                                       file_format))
+            group_dis_corr_file = join(
+                filedir,
+                f"{experiment_id}_disattenuated_correlations_by_{group}.{file_format}",
+            )
             if exists(group_dis_corr_file):
                 df_dis_cor_group = DataReader.read_from_file(group_dis_corr_file, index_col=0)
-                files['df_disattenuated_correlations_by_{}'.format(group)] = df_dis_cor_group
-                files['df_disattenuated_correlations_by_{}_overview'.format(group)] = self.make_summary_stat_df(df_dis_cor_group)
+                files[f"df_disattenuated_correlations_by_{group}"] = df_dis_cor_group
+                files[
+                    f"df_disattenuated_correlations_by_{group}_overview"
+                ] = self.make_summary_stat_df(df_dis_cor_group)
 
         # true score evaluations
-        true_score_eval_file = join(filedir, "{}_true_score_eval.{}".format(experiment_id,
-                                                                            file_format))
+        true_score_eval_file = join(filedir, f"{experiment_id}_true_score_eval.{file_format}")
 
         # load true score evaluations if present
         if exists(true_score_eval_file):
             df_true_score_eval = DataReader.read_from_file(true_score_eval_file, index_col=0)
             # we only use the row for raw_trim or scale_trim score
-            files['df_true_score_eval'] = df_true_score_eval.loc[['{}_trim'.format(prefix)]]
+            files["df_true_score_eval"] = df_true_score_eval.loc[[f"{prefix}_trim"]]
 
         # use the raw columns or the scale columns depending on the prefix
-        existing_eval_cols = (_df_eval_columns_existing_raw if prefix == 'raw'
-                              else _df_eval_columns_existing_scale)
-        rename_dict = raw_rename_dict if prefix == 'raw' else scale_rename_dict
+        existing_eval_cols = (
+            _df_eval_columns_existing_raw if prefix == "raw" else _df_eval_columns_existing_scale
+        )
+        rename_dict = raw_rename_dict if prefix == "raw" else scale_rename_dict
 
         # read in the short version of the evaluation metrics for all data
-        short_metrics_list = ["N", "Adj. Agmt.(br)", "Agmt.(br)", "K(br)",
-                              "Pearson(b)", "QWK(b)", "R2(b)", "RMSE(b)"]
-        eval_file_short = join(filedir, '{}_eval_short.{}'.format(experiment_id, file_format))
+        short_metrics_list = [
+            "N",
+            "Adj. Agmt.(br)",
+            "Agmt.(br)",
+            "K(br)",
+            "Pearson(b)",
+            "QWK(b)",
+            "R2(b)",
+            "RMSE(b)",
+        ]
+        eval_file_short = join(filedir, f"{experiment_id}_eval_short.{file_format}")
 
         if exists(eval_file_short):
             df_eval = DataReader.read_from_file(eval_file_short, index_col=0)
 
-            (rename_dict_new,
-             existing_eval_cols_new,
-             short_metrics_list_new,
-             _) = self._modify_eval_columns_to_ensure_version_compatibilty(df_eval,
-                                                                           rename_dict,
-                                                                           existing_eval_cols,
-                                                                           short_metrics_list)
+            (
+                rename_dict_new,
+                existing_eval_cols_new,
+                short_metrics_list_new,
+                _,
+            ) = self._modify_eval_columns_to_ensure_version_compatibilty(
+                df_eval, rename_dict, existing_eval_cols, short_metrics_list
+            )
 
             df_eval = df_eval[existing_eval_cols_new]
             df_eval = df_eval.rename(columns=rename_dict_new)
-            files['df_eval'] = df_eval[short_metrics_list_new]
-            files['df_eval'].index.name = None
+            files["df_eval"] = df_eval[short_metrics_list_new]
+            files["df_eval"].index.name = None
 
-        eval_file = join(filedir, '{}_eval.{}'.format(experiment_id, file_format))
+        eval_file = join(filedir, f"{experiment_id}_eval.{file_format}")
         if exists(eval_file):
-            files['df_eval_for_degradation'] = DataReader.read_from_file(eval_file, index_col=0)
+            files["df_eval_for_degradation"] = DataReader.read_from_file(eval_file, index_col=0)
 
         # read in the evaluation metrics by subgroup, if we are asked to
         for group in groups_eval:
-            group_eval_file = join(filedir, '{}_eval_by_{}.{}'.format(experiment_id,
-                                                                      group,
-                                                                      file_format))
+            group_eval_file = join(filedir, f"{experiment_id}_eval_by_{group}.{file_format}")
             if exists(group_eval_file):
                 df_eval = DataReader.read_from_file(group_eval_file, index_col=0)
 
-                (rename_dict_new,
-                 existing_eval_cols_new,
-                 short_metrics_list_new,
-                 smd_name
-                 ) = self._modify_eval_columns_to_ensure_version_compatibilty(df_eval,
-                                                                              rename_dict,
-                                                                              existing_eval_cols,
-                                                                              short_metrics_list,
-                                                                              raise_warnings=False)
+                (
+                    rename_dict_new,
+                    existing_eval_cols_new,
+                    short_metrics_list_new,
+                    smd_name,
+                ) = self._modify_eval_columns_to_ensure_version_compatibilty(
+                    df_eval,
+                    rename_dict,
+                    existing_eval_cols,
+                    short_metrics_list,
+                    raise_warnings=False,
+                )
 
                 df_eval = df_eval[existing_eval_cols_new]
                 df_eval = df_eval.rename(columns=rename_dict_new)
-                files['df_eval_by_{}'.format(group)] = df_eval[short_metrics_list_new]
-                files['df_eval_by_{}'.format(group)].index.name = None
+                files[f"df_eval_by_{group}"] = df_eval[short_metrics_list_new]
+                files[f"df_eval_by_{group}"].index.name = None
 
-                series = files['df_eval_by_{}'.format(group)]
-                files['df_eval_by_{}_overview'.format(group)] = self.make_summary_stat_df(series)
+                series = files[f"df_eval_by_{group}"]
+                files[f"df_eval_by_{group}_overview"] = self.make_summary_stat_df(series)
 
                 # set the ordering of mean/SD/SMD statistics
-                files['df_eval_by_{}_m_sd'.format(group)] = df_eval[['N', 'H1 mean',
-                                                                     'H1 SD', 'score mean(br)',
-                                                                     'score SD(br)',
-                                                                     'score mean(b)',
-                                                                     'score SD(b)',
-                                                                     '{}(br)'.format(smd_name),
-                                                                     '{}(b)'.format(smd_name)]]
-                files['df_eval_by_{}_m_sd'.format(group)].index.name = None
+                files[f"df_eval_by_{group}_m_sd"] = df_eval[
+                    [
+                        "N",
+                        "H1 mean",
+                        "H1 SD",
+                        "score mean(br)",
+                        "score SD(br)",
+                        "score mean(b)",
+                        "score SD(b)",
+                        f"{smd_name}(br)",
+                        f"{smd_name}(b)",
+                    ]
+                ]
+                files[f"df_eval_by_{group}_m_sd"].index.name = None
 
         # read in the partial correlations vs. score for all data
-        pcor_score_file = join(filedir, '{}_pcor_score_all_data.{}'.format(experiment_id,
-                                                                           file_format))
+        pcor_score_file = join(filedir, f"{experiment_id}_pcor_score_all_data.{file_format}")
         if exists(pcor_score_file):
-            files['df_pcor_sc1'] = DataReader.read_from_file(pcor_score_file, index_col=0)
-            files['df_pcor_sc1_overview'] = self.make_summary_stat_df(files['df_pcor_sc1'])
+            files["df_pcor_sc1"] = DataReader.read_from_file(pcor_score_file, index_col=0)
+            files["df_pcor_sc1_overview"] = self.make_summary_stat_df(files["df_pcor_sc1"])
 
         # read in the partial correlations by subgroups, if we are asked to
         for group in groups_eval:
-            group_pcor_file = join(filedir, '{}_pcor_score_by_{}.{}'.format(experiment_id,
-                                                                            group,
-                                                                            file_format))
+            group_pcor_file = join(filedir, f"{experiment_id}_pcor_score_by_{group}.{file_format}")
             if exists(group_pcor_file):
-                files['df_pcor_sc1_by_{}'
-                      ''.format(group)] = DataReader.read_from_file(group_pcor_file,
-                                                                    index_col=0)
+                files[f"df_pcor_sc1_by_{group}"] = DataReader.read_from_file(
+                    group_pcor_file, index_col=0
+                )
 
-                series = files['df_pcor_sc1_by_{}'.format(group)]
-                files['df_pcor_sc1_{}_overview'.format(group)] = self.make_summary_stat_df(series)
+                series = files[f"df_pcor_sc1_by_{group}"]
+                files[f"df_pcor_sc1_{group}_overview"] = self.make_summary_stat_df(series)
 
         # read in the marginal correlations vs. score for all data
-        mcor_score_file = join(filedir, '{}_margcor_score_all_data.{}'.format(experiment_id,
-                                                                              file_format))
+        mcor_score_file = join(filedir, f"{experiment_id}_margcor_score_all_data.{file_format}")
         if exists(mcor_score_file):
-            files['df_mcor_sc1'] = DataReader.read_from_file(mcor_score_file, index_col=0)
-            files['df_mcor_sc1_overview'] = self.make_summary_stat_df(files['df_mcor_sc1'])
+            files["df_mcor_sc1"] = DataReader.read_from_file(mcor_score_file, index_col=0)
+            files["df_mcor_sc1_overview"] = self.make_summary_stat_df(files["df_mcor_sc1"])
 
         # read in the partial correlations by subgroups, if we are asked to
         for group in groups_eval:
-            group_mcor_file = join(filedir,
-                                   '{}_margcor_score_by_{}.{}'.format(experiment_id,
-                                                                      group,
-                                                                      file_format))
+            group_mcor_file = join(
+                filedir, f"{experiment_id}_margcor_score_by_{group}.{file_format}"
+            )
             if exists(group_mcor_file):
-                files['df_mcor_sc1_by_{}'
-                      ''.format(group)] = DataReader.read_from_file(group_mcor_file,
-                                                                    index_col=0)
+                files[f"df_mcor_sc1_by_{group}"] = DataReader.read_from_file(
+                    group_mcor_file, index_col=0
+                )
 
-                series = files['df_mcor_sc1_by_{}'.format(group)]
-                files['df_mcor_sc1_{}_overview'.format(group)] = self.make_summary_stat_df(series)
+                series = files[f"df_mcor_sc1_by_{group}"]
+                files[f"df_mcor_sc1_{group}_overview"] = self.make_summary_stat_df(series)
 
-        pca_file = join(filedir, '{}_pca.{}'.format(experiment_id, file_format))
+        pca_file = join(filedir, f"{experiment_id}_pca.{file_format}")
         if exists(pca_file):
-            files['df_pca'] = DataReader.read_from_file(pca_file, index_col=0)
-            files['df_pcavar'] = DataReader.read_from_file(join(filedir,
-                                                                '{}_pcavar.{}'.format(experiment_id,
-                                                                                      file_format)),
-                                                           index_col=0)
+            files["df_pca"] = DataReader.read_from_file(pca_file, index_col=0)
+            files["df_pcavar"] = DataReader.read_from_file(
+                join(filedir, f"{experiment_id}_pcavar.{file_format}"), index_col=0
+            )
 
-        descriptives_file = join(filedir, '{}_feature_descriptives.{}'.format(experiment_id,
-                                                                              file_format))
+        descriptives_file = join(filedir, f"{experiment_id}_feature_descriptives.{file_format}")
         if exists(descriptives_file):
             # we read all files pertaining to the descriptive analysis together
             # since we merge the outputs
-            files['df_descriptives'] = DataReader.read_from_file(descriptives_file, index_col=0)
+            files["df_descriptives"] = DataReader.read_from_file(descriptives_file, index_col=0)
 
             # this df contains only the number of features. this is used later
             # for another two tables to show the number of features
-            df_features_n_values = files['df_descriptives'][['N', 'min', 'max']]
+            df_features_n_values = files["df_descriptives"][["N", "min", "max"]]
 
-            files['df_descriptives'] = files['df_descriptives'][['N', 'mean', 'std. dev.',
-                                                                 'skewness', 'kurtosis']]
+            files["df_descriptives"] = files["df_descriptives"][
+                ["N", "mean", "std. dev.", "skewness", "kurtosis"]
+            ]
 
-            outliers_file = join(filedir, '{}_feature_outliers.{}'.format(experiment_id,
-                                                                          file_format))
+            outliers_file = join(filedir, f"{experiment_id}_feature_outliers.{file_format}")
             df_outliers = DataReader.read_from_file(outliers_file, index_col=0)
-            df_outliers = df_outliers.rename(columns={'upper': 'Upper',
-                                                      'lower': 'Lower',
-                                                      'both': 'Both',
-                                                      'upperperc': 'Upper %',
-                                                      'lowerperc': 'Lower %',
-                                                      'bothperc': 'Both %'})
+            df_outliers = df_outliers.rename(
+                columns={
+                    "upper": "Upper",
+                    "lower": "Lower",
+                    "both": "Both",
+                    "upperperc": "Upper %",
+                    "lowerperc": "Lower %",
+                    "bothperc": "Both %",
+                }
+            )
             df_outliers_columns = df_outliers.columns.tolist()
-            files['df_outliers'] = df_outliers
+            files["df_outliers"] = df_outliers
 
             # join with df_features_n_values to get the value of N
-            files['df_outliers'] = pd.merge(files['df_outliers'], df_features_n_values,
-                                            left_index=True,
-                                            right_index=True)[['N'] + df_outliers_columns]
+            files["df_outliers"] = pd.merge(
+                files["df_outliers"],
+                df_features_n_values,
+                left_index=True,
+                right_index=True,
+            )[["N"] + df_outliers_columns]
 
             # join with df_features_n_values to get the value of N
-            percentiles_file = join(filedir, '{}_feature_descriptives'
-                                             'Extra.{}'.format(experiment_id,
-                                                               file_format))
-
-            files['df_percentiles'] = DataReader.read_from_file(percentiles_file,
-                                                                index_col=0)
-            files['df_percentiles'] = pd.merge(files['df_percentiles'],
-                                               df_features_n_values,
-                                               left_index=True,
-                                               right_index=True)
-
-            mild_outliers = (files['df_percentiles']["Mild outliers"] /
-                             files['df_percentiles']["N"].astype(float) * 100)
-
-            files['df_percentiles']["Mild outliers (%)"] = mild_outliers
-
-            extreme_outliers = (files['df_percentiles']["Extreme outliers"] /
-                                files['df_percentiles']["N"].astype(float) * 100)
-
-            files['df_percentiles']["Extreme outliers (%)"] = extreme_outliers
-
-            files['df_percentiles'] = files['df_percentiles'][['N', 'min', 'max',
-                                                               '1%', '5%', '25%',
-                                                               '50%', '75%', '95%',
-                                                               '99%', 'IQR', 'Mild outliers',
-                                                               'Mild outliers (%)',
-                                                               'Extreme outliers',
-                                                               'Extreme outliers (%)']]
+            percentiles_file = join(
+                filedir, f"{experiment_id}_feature_descriptivesExtra.{file_format}"
+            )
+
+            files["df_percentiles"] = DataReader.read_from_file(percentiles_file, index_col=0)
+            files["df_percentiles"] = pd.merge(
+                files["df_percentiles"],
+                df_features_n_values,
+                left_index=True,
+                right_index=True,
+            )
+
+            mild_outliers = (
+                files["df_percentiles"]["Mild outliers"]
+                / files["df_percentiles"]["N"].astype(float)
+                * 100
+            )
+
+            files["df_percentiles"]["Mild outliers (%)"] = mild_outliers
+
+            extreme_outliers = (
+                files["df_percentiles"]["Extreme outliers"]
+                / files["df_percentiles"]["N"].astype(float)
+                * 100
+            )
+
+            files["df_percentiles"]["Extreme outliers (%)"] = extreme_outliers
+
+            files["df_percentiles"] = files["df_percentiles"][
+                [
+                    "N",
+                    "min",
+                    "max",
+                    "1%",
+                    "5%",
+                    "25%",
+                    "50%",
+                    "75%",
+                    "95%",
+                    "99%",
+                    "IQR",
+                    "Mild outliers",
+                    "Mild outliers (%)",
+                    "Extreme outliers",
+                    "Extreme outliers (%)",
+                ]
+            ]
 
-        confmatrix_file = join(filedir, '{}_confMatrix.{}'.format(experiment_id, file_format))
+        confmatrix_file = join(filedir, f"{experiment_id}_confMatrix.{file_format}")
         if exists(confmatrix_file):
             conf_matrix = DataReader.read_from_file(confmatrix_file, index_col=0)
-            files['df_confmatrix'] = self.process_confusion_matrix(conf_matrix)
+            files["df_confmatrix"] = self.process_confusion_matrix(conf_matrix)
 
-        score_dist_file = join(filedir, '{}_score_dist.{}'.format(experiment_id, file_format))
+        score_dist_file = join(filedir, f"{experiment_id}_score_dist.{file_format}")
         if exists(score_dist_file):
             df_score_dist = DataReader.read_from_file(score_dist_file, index_col=1)
-            df_score_dist.rename(columns={'sys_{}'.format(prefix): 'sys'}, inplace=True)
-            files['df_score_dist'] = df_score_dist[['human', 'sys', 'difference']]
+            df_score_dist.rename(columns={f"sys_{prefix}": "sys"}, inplace=True)
+            files["df_score_dist"] = df_score_dist[["human", "sys", "difference"]]
 
         # read in the feature boxplots by subgroup, if we were asked to
         for group in groups_eval:
-            feature_boxplot_prefix = join(figdir,
-                                          '{}_feature_boxplot_by_{}'.format(experiment_id, group))
-            svg_file = join(feature_boxplot_prefix + '.svg')
-            png_file = join(feature_boxplot_prefix + '.png')
+            feature_boxplot_prefix = join(figdir, f"{experiment_id}_feature_boxplot_by_{group}")
+            svg_file = join(feature_boxplot_prefix + ".svg")
+            png_file = join(feature_boxplot_prefix + ".png")
             if exists(svg_file):
-                figs['feature_boxplots_by_{}_svg'.format(group)] = svg_file
+                figs[f"feature_boxplots_by_{group}_svg"] = svg_file
 
             elif exists(png_file):
-                figs['feature_boxplots_by_{}_png'.format(group)] = png_file
+                figs[f"feature_boxplots_by_{group}_png"] = png_file
 
         # read in the betas image if exists
-        betas_svg = join(figdir, '{}_betas.svg'.format(experiment_id))
+        betas_svg = join(figdir, f"{experiment_id}_betas.svg")
         if exists(betas_svg):
-            figs['betas'] = betas_svg
+            figs["betas"] = betas_svg
 
         # read in the evaluation barplots by subgroup, if we were asked to
         for group in groups_eval:
-            eval_barplot_svg_file = join(figdir, '{}_eval_by_{}.svg'.format(experiment_id, group))
+            eval_barplot_svg_file = join(figdir, f"{experiment_id}_eval_by_{group}.svg")
             if exists(eval_barplot_svg_file):
-                figs['eval_barplot_by_{}'.format(group)] = eval_barplot_svg_file
+                figs[f"eval_barplot_by_{group}"] = eval_barplot_svg_file
 
-        pca_svg_file = join(figdir, '{}_pca.svg'.format(experiment_id))
+        pca_svg_file = join(figdir, f"{experiment_id}_pca.svg")
         if exists(pca_svg_file):
-            figs['pca_scree_plot'] = pca_svg_file
+            figs["pca_scree_plot"] = pca_svg_file
 
         return (files, figs, file_format)
```

### Comparing `rsmtool-9.0.1/rsmtool/configuration_parser.py` & `rsmtool-9.1.1/rsmtool/configuration_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,21 +21,26 @@
 from os.path import abspath
 from pathlib import Path
 
 from skll.learner import Learner
 from skll.metrics import _SCORERS
 
 from . import HAS_RSMEXTRA
-from .utils.constants import BOOLEAN_FIELDS, CHECK_FIELDS, DEFAULTS, ID_FIELDS, LIST_FIELDS
+from .utils.constants import (
+    BOOLEAN_FIELDS,
+    CHECK_FIELDS,
+    DEFAULTS,
+    ID_FIELDS,
+    LIST_FIELDS,
+)
 from .utils.files import parse_json_with_comments
 from .utils.models import is_skll_model
 
 if HAS_RSMEXTRA:
-    from rsmextra.settings import (default_feature_subset_file, # noqa
-                                   default_feature_sign)
+    from rsmextra.settings import default_feature_sign, default_feature_subset_file
 
 
 def configure(context, config_file_or_obj_or_dict):
     """
     Create a Configuration object.
 
     Get the configuration for ``context`` from the input
@@ -78,16 +83,15 @@
         # Instantiate configuration parser object
         parser = ConfigurationParser(config_file_or_obj_or_dict)
         configuration = parser.parse(context=context)
 
     elif isinstance(config_file_or_obj_or_dict, dict):
 
         # directly instantiate the Configuration from the dictionary
-        configuration = Configuration(config_file_or_obj_or_dict,
-                                      context=context)
+        configuration = Configuration(config_file_or_obj_or_dict, context=context)
 
     elif isinstance(config_file_or_obj_or_dict, Configuration):
 
         # raise an error if we are passed a Configuration object
         # without a configdir attribute. This can only
         # happen if the object was constructed using an earlier version
         # of RSMTool and stored
@@ -95,36 +99,32 @@
             assert config_file_or_obj_or_dict.configdir is not None
         except AssertionError:
             raise AttributeError("Configuration object must have configdir attribute.")
         else:
             configuration = config_file_or_obj_or_dict
 
     else:
-        raise ValueError("The input to run_experiment must be "
-                         "a path to the file (str), a dictionary, "
-                         "or a configuration object. You passed "
-                         "{}.".format(type(config_file_or_obj_or_dict)))
+        raise ValueError(
+            f"The input to run_experiment must be a path to the file (str), "
+            f"a dictionary, or a configuration object. You passed "
+            f"{type(config_file_or_obj_or_dict)}."
+        )
 
     return configuration
 
 
 class Configuration:
     """
     Configuration class.
 
     Encapsulates all of the configuration parameters and methods to
     access these parameters.
     """
 
-    def __init__(self,
-                 configdict,
-                 *,
-                 configdir=None,
-                 context='rsmtool',
-                 logger=None):
+    def __init__(self, configdict, *, configdir=None, context="rsmtool", logger=None):
         """
         Create an object of the `Configuration` class.
 
         This method can be used to directly instantiate a Configuration
         object.
 
         Parameters
@@ -143,27 +143,27 @@
             "rsmpredict", "rsmsummarize"}.
             Defaults to "rsmtool".
         logger : logging object, optional
             A logging object. If ``None`` is passed, get logger from ``__name__``.
             Defaults to ``None``.
         """
         if not isinstance(configdict, dict):
-            raise TypeError('The input must be a dictionary.')
+            raise TypeError("The input must be a dictionary.")
 
         # create a logger instance
         self.logger = logger if logger else logging.getLogger(__name__)
 
         # process and validate the configuration dictionary
         configdict = ConfigurationParser.process_config(configdict)
         configdict = ConfigurationParser.validate_config(configdict, context=context)
 
         # set configdir to `cwd` if not given and let the user know
         if configdir is None:
             configdir = Path(getcwd())
-            self.logger.info("Configuration directory will be set to {}".format(configdir))
+            self.logger.info(f"Configuration directory will be set to {configdir}")
         else:
             configdir = Path(configdir).resolve()
 
         self._config = configdict
         self._configdir = configdir
         self._context = context
 
@@ -231,19 +231,20 @@
         -------
         config_string : str
             A string representation of the underlying configuration
             dictionary as encoded by ``json.dumps()``. It only
             includes the configuration options that can be set by
             the user.
         """
-        expected_fields = (CHECK_FIELDS[self._context]['required'] +
-                           CHECK_FIELDS[self._context]['optional'])
+        expected_fields = (
+            CHECK_FIELDS[self._context]["required"] + CHECK_FIELDS[self._context]["optional"]
+        )
 
         output_config = {k: v for k, v in self._config.items() if k in expected_fields}
-        return json.dumps(output_config, indent=4, separators=(',', ': '))
+        return json.dumps(output_config, indent=4, separators=(",", ": "))
 
     def __iter__(self):
         """
         Iterate through configuration object keys.
 
         Yields
         ------
@@ -419,23 +420,23 @@
             Defaults to ``None``.
         """
         # save a copy of the main config into the output directory
         if output_dir is None:
             output_dir = Path(getcwd())
 
         # Create output directory, if it does not exist
-        output_dir = Path(output_dir).resolve() / 'output'
+        output_dir = Path(output_dir).resolve() / "output"
         output_dir.mkdir(parents=True, exist_ok=True)
 
         id_field = ID_FIELDS[self._context]
         experiment_id = self._config[id_field]
         context = self._context
         outjson = output_dir / f"{experiment_id}_{context}.json"
 
-        with outjson.open(mode='w') as outfile:
+        with outjson.open(mode="w") as outfile:
             outfile.write(str(self))
 
     def check_exclude_listwise(self):
         """
         Check for candidate exclusion.
 
         Check if we are excluding candidates based on number of responses, and
@@ -443,21 +444,19 @@
 
         Returns
         -------
         exclude_listwise : bool
             Whether to exclude list-wise.
         """
         exclude_listwise = False
-        if self._config.get('min_items_per_candidate'):
+        if self._config.get("min_items_per_candidate"):
             exclude_listwise = True
         return exclude_listwise
 
-    def check_flag_column(self,
-                          flag_column='flag_column',
-                          partition='unknown'):
+    def check_flag_column(self, flag_column="flag_column", partition="unknown"):
         """
         Make sure the column name in ``flag_column`` is correctly specified.
 
         Get flag columns and values for filtering, if any, and convert single
         values to lists. Raises an exception if the column name in ``flag_column``
         is not correctly specified in the configuration file.
 
@@ -489,70 +488,68 @@
         ValueError
             If the value of ``partition`` does not match the ``flag_column``.
         """
         config = self._config
 
         new_filter_dict = {}
 
-        flag_message = {"train": "training",
-                        "test": "evaluating",
-                        "both": "training and evaluating",
-                        "unknown": "training and/or evaluating"}
+        flag_message = {
+            "train": "training",
+            "test": "evaluating",
+            "both": "training and evaluating",
+            "unknown": "training and/or evaluating",
+        }
 
         if partition not in flag_message:
-            raise ValueError("Unknown value for partition: {} "
-                             "This must be one of the following: {}."
-                             "".format(partition, ','.join(flag_message.keys())))
+            raise ValueError(
+                f"Unknown value for partition: {partition} This must "
+                f"be one of the following: {','.join(flag_message.keys())}."
+            )
 
         if flag_column == "flag_column_test":
             if partition in ["both", "train"]:
-                raise ValueError("Conditions specified in 'flag_column_test' "
-                                 "can only be applied to the evaluation partition.")
+                raise ValueError(
+                    "Conditions specified in 'flag_column_test' "
+                    "can only be applied to the evaluation partition."
+                )
 
         if config.get(flag_column):
 
             original_filter_dict = config[flag_column]
 
             # first check that the value is a dictionary
             if not isinstance(original_filter_dict, dict):
-                raise ValueError("`flag_column` must be a dictionary. "
-                                 "Please refer to the documentation for "
-                                 "further information.")
+                raise ValueError(
+                    "`flag_column` must be a dictionary. "
+                    "Please refer to the documentation for "
+                    "further information."
+                )
 
             for column in original_filter_dict:
 
                 # if we were given a single value, convert it to list
                 if not isinstance(original_filter_dict[column], list):
                     new_filter_dict[column] = [original_filter_dict[column]]
-                    self.logger.warning("The filtering condition {}"
-                                        " for column {} was converted "
-                                        "to list. Only responses where "
-                                        "{} == {} will be used for "
-                                        "{} the "
-                                        "model. You can ignore this "
-                                        "warning if this is the correct "
-                                        "interpretation of your "
-                                        "configuration settings"
-                                        ".".format(original_filter_dict[column],
-                                                   column,
-                                                   column,
-                                                   original_filter_dict[column],
-                                                   flag_message[partition])
-                                        )
+                    self.logger.warning(
+                        f"The filtering condition {original_filter_dict[column]} "
+                        f"for column {column} was converted to list. Only "
+                        f"responses where {column} == {original_filter_dict[column]} "
+                        f"will be used for {flag_message[partition]} the model. "
+                        f"You can ignore this warning if this is the correct "
+                        f"interpretation of your configuration settings."
+                    )
                 else:
                     new_filter_dict[column] = original_filter_dict[column]
 
-                    model_eval = ', '.join(map(str,
-                                               original_filter_dict[column]))
-                    self.logger.info("Only responses where "
-                                     "{} equals one of the following values "
-                                     "will be used for {} the model: "
-                                     "{}.".format(column,
-                                                  flag_message[partition],
-                                                  model_eval))
+                    model_eval = ", ".join(map(str, original_filter_dict[column]))
+                    self.logger.info(
+                        f"Only responses where {column} equals one of the "
+                        f"following values will be used for "
+                        f"{flag_message[partition]} the model: {model_eval}."
+                    )
         return new_filter_dict
 
     def get_trim_min_max_tolerance(self):
         """
         Get trim min, trim max, and tolerance values.
 
         Get the specified trim min and max, and trim_tolerance if any,
@@ -565,17 +562,17 @@
         spec_trim_max : float
             Specified trim max value.
         spec_trim_tolerance: float
             Specified trim tolerance value.
         """
         config = self._config
 
-        spec_trim_min = config.get('trim_min', None)
-        spec_trim_max = config.get('trim_max', None)
-        spec_trim_tolerance = config.get('trim_tolerance', None)
+        spec_trim_min = config.get("trim_min", None)
+        spec_trim_max = config.get("trim_max", None)
+        spec_trim_tolerance = config.get("trim_tolerance", None)
 
         if spec_trim_min:
             spec_trim_min = float(spec_trim_min)
         if spec_trim_max:
             spec_trim_max = float(spec_trim_max)
         if spec_trim_tolerance:
             spec_trim_tolerance = float(spec_trim_tolerance)
@@ -588,15 +585,15 @@
         Returns
         -------
         rater_error_variance : float
             Specified rater error variance.
         """
         config = self._config
 
-        rater_error_variance = config.get('rater_error_variance', None)
+        rater_error_variance = config.get("rater_error_variance", None)
 
         if rater_error_variance:
             rater_error_variance = float(rater_error_variance)
 
         return rater_error_variance
 
     def get_default_converter(self):
@@ -604,21 +601,21 @@
         Get default converter dictionary for data reader.
 
         Returns
         -------
         default_converter : dict
             The default converter for a train or test file.
         """
-        string_columns = [self._config['id_column']]
+        string_columns = [self._config["id_column"]]
 
-        candidate = self._config.get('candidate_column')
+        candidate = self._config.get("candidate_column")
         if candidate is not None:
             string_columns.append(candidate)
 
-        subgroups = self._config.get('subgroups')
+        subgroups = self._config.get("subgroups")
         if subgroups:
             string_columns.extend(subgroups)
 
         return dict([(column, str) for column in string_columns if column])
 
     def get_names_and_paths(self, keys, names):
         """
@@ -644,33 +641,35 @@
         ValueError
             If there are any duplicate keys or names.
         """
         assert len(keys) == len(names)
 
         # Make sure keys are not duplicated
         if not len(set(keys)) == len(keys):
-            raise ValueError('The ``keys`` must be unique. However, the '
-                             'following duplicate keys were found: {}.'
-                             ''.format(', '.join([key for key, val in Counter(keys).items()
-                                                  if val > 1])))
+            raise ValueError(
+                f"The ``keys`` must be unique. However, the following "
+                f"duplicate keys were found: "
+                f"{', '.join([key for key, val in Counter(keys).items() if val > 1])}."
+            )
         # Make sure names are not duplicated
         if not len(set(names)) == len(names):
-            raise ValueError('The``names`` must be unique. However, the '
-                             'following duplicate names were found: {}.'
-                             ''.format(', '.join([name for name, val in Counter(names).items()
-                                                  if val > 1])))
+            raise ValueError(
+                f"The``names`` must be unique. However, the following "
+                f"duplicate names were found: "
+                f"{', '.join([name for name, val in Counter(names).items() if val > 1])}."
+            )
         existing_names = []
         existing_paths = []
         for idx, key in enumerate(keys):
 
             path = self._config.get(key)
 
             # if the `features` field is a list,
             # do not include it in the container
-            if key == 'features':
+            if key == "features":
                 if isinstance(path, list):
                     continue
 
             if path is not None:
                 existing_paths.append(path)
                 existing_names.append(names[idx])
 
@@ -710,27 +709,26 @@
         """
         # if we passed in a string, convert it to a Path
         if isinstance(pathlike, str):
             pathlike = Path(pathlike)
 
         # raise an exception if the file does not exist
         if not pathlike.exists():
-            raise FileNotFoundError(f"The configuration file {pathlike} "
-                                    f"was not found.")
+            raise FileNotFoundError(f"The configuration file {pathlike} " f"was not found.")
 
         # raise an exception if the user specified a directory
         if not pathlike.is_file():
-            raise OSError(f"The given path {pathlike} should be a "
-                          f"file, not a directory.")
+            raise OSError(f"The given path {pathlike} should be a " f"file, not a directory.")
 
         # make sure we have a file that ends in ".json"
         extension = pathlike.suffix.lower()
-        if extension != '.json':
-            raise ValueError(f"The configuration file must be in `.json` "
-                             f"format. You specified: {extension}.")
+        if extension != ".json":
+            raise ValueError(
+                f"The configuration file must be in `.json` " f"format. You specified: {extension}."
+            )
 
         # set the various attributes to None
         self._filename = pathlike.name
         self._configdir = pathlike.resolve().parent
 
         # set the `logger` class attribute to the given logger, if provided
         # or else create a new logger
@@ -750,16 +748,16 @@
             A string to be reformatted for JSON parsing.
 
         Return
         ------
         json_string : str
             The updated string.
         """
-        json_string = json_string.replace('True', 'true')
-        json_string = json_string.replace('False', 'false')
+        json_string = json_string.replace("True", "true")
+        json_string = json_string.replace("False", "false")
         json_string = json_string.replace("'", '"')
         return json_string
 
     def _parse_json_file(self, filepath):
         """
         Parse the configuration JSON.
 
@@ -782,23 +780,24 @@
         ------
         ValueError
             If the JSON file could not be parsed.
         """
         try:
             configdict = parse_json_with_comments(filepath)
         except ValueError:
-            raise ValueError('The main configuration file `{}` exists but '
-                             'is formatted incorrectly. Please check that '
-                             'each line ends with a comma, there is no comma '
-                             'at the end of the last line, and that all quotes '
-                             'match.'.format(filepath))
+            raise ValueError(
+                f"The main configuration file `{filepath}` exists but "
+                f"is formatted incorrectly. Please check that each "
+                f"line ends with a comma, there is no comma at the end "
+                f"of the last line, and that all quotes match."
+            )
 
         return configdict
 
-    def parse(self, context='rsmtool'):
+    def parse(self, context="rsmtool"):
         """
         Parse configuration file.
 
         Parse the configuration file for which this parser was
         instantiated.
 
         Parameters
@@ -817,20 +816,18 @@
         """
         filepath = self._configdir / self._filename
         configdict = self._parse_json_file(filepath)
 
         # create a new Configuration object which will automatically
         # process and validate the configuration
         # dictionary being passed in
-        return Configuration(configdict,
-                             configdir=self._configdir,
-                             context=context)
+        return Configuration(configdict, configdir=self._configdir, context=context)
 
     @classmethod
-    def validate_config(cls, config, context='rsmtool'):
+    def validate_config(cls, config, context="rsmtool"):
         """
         Validate configuration file.
 
         Ensure that all required fields are specified, add default values
         values for all unspecified fields, and ensure that all specified
         fields are valid.
 
@@ -856,200 +853,221 @@
         ValueError
             If config does not exist, and no config passed.
         """
         # make a copy of the given parameter dictionary
         new_config = deepcopy(config)
 
         # 1. Check to make sure all required fields are specified
-        required_fields = CHECK_FIELDS[context]['required']
+        required_fields = CHECK_FIELDS[context]["required"]
 
         for field in required_fields:
             if field not in new_config:
-                raise ValueError("The config file must "
-                                 "specify '{}'".format(field))
+                raise ValueError(f"The config file must specify '{field}'")
 
         # 2. Add default values for unspecified optional fields
         # for given RSMTool context
         defaults = DEFAULTS
 
         for field in defaults:
             if field not in new_config:
                 new_config[field] = defaults[field]
 
         # 3. Check to make sure no unrecognized fields are specified
         for field in new_config:
             if field not in defaults and field not in required_fields:
-                raise ValueError("Unrecognized field '{}'"
-                                 " in json file".format(field))
+                raise ValueError(f"Unrecognized field '{field}' in json file")
 
         # 4. Check to make sure that the ID fields that will be
         # used as part of filenames are formatted correctly
         # i.e., they do not contain any spaces and are < 200 characters
         id_field = ID_FIELDS[context]
         id_field_values = {id_field: new_config[id_field]}
 
         for id_field, id_field_value in id_field_values.items():
             if len(id_field_value) > 200:
-                raise ValueError("{} is too long (must be "
-                                 "<=200 characters)".format(id_field))
+                raise ValueError(f"{id_field} is too long (must be <=200 characters)")
 
-            if re.search(r'\s', id_field_value):
-                raise ValueError("{} cannot contain any "
-                                 "spaces".format(id_field))
+            if re.search(r"\s", id_field_value):
+                raise ValueError(f"{id_field} cannot contain any spaces")
 
         # 5. Check that the feature file and feature subset/subset file are not
         # specified together
-        msg = ("You cannot specify BOTH \"features\" and \"{}\". "
-               "Please refer to the \"Selecting Feature Columns\" "
-               "section in the documentation for more details.")
-        if new_config['features'] and new_config['feature_subset_file']:
+        msg = (
+            'You cannot specify BOTH "features" and "{}". '
+            'Please refer to the "Selecting Feature Columns" '
+            "section in the documentation for more details."
+        )
+        if new_config["features"] and new_config["feature_subset_file"]:
             msg = msg.format("feature_subset_file")
             raise ValueError(msg)
-        if new_config['features'] and new_config['feature_subset']:
+        if new_config["features"] and new_config["feature_subset"]:
             msg = msg.format("feature_subset")
             raise ValueError(msg)
 
         # 6. Check for fields that require feature_subset_file and try
         # to use the default feature file
-        if (new_config['feature_subset'] and
-                not new_config['feature_subset_file']):
+        if new_config["feature_subset"] and not new_config["feature_subset_file"]:
 
             # Check if we have the default subset file from rsmextra
             if HAS_RSMEXTRA:
                 default_basename = Path(default_feature_subset_file).name
-                new_config['feature_subset_file'] = default_feature_subset_file
-                cls.logger.warning("You requested feature subsets but did not "
-                                   "specify any feature file. "
-                                   "The tool will use the default "
-                                   "feature file {} available via "
-                                   "rsmextra".format(default_basename))
+                new_config["feature_subset_file"] = default_feature_subset_file
+                cls.logger.warning(
+                    f"You requested feature subsets but did not specify "
+                    f"any feature file. The tool will use the default "
+                    f"feature file {default_basename} available via rsmextra."
+                )
             else:
-                raise ValueError("If you want to use feature subsets, you "
-                                 "must specify a feature subset file")
+                raise ValueError(
+                    "If you want to use feature subsets, you " "must specify a feature subset file"
+                )
 
-        if new_config['sign'] and not new_config['feature_subset_file']:
+        if new_config["sign"] and not new_config["feature_subset_file"]:
 
             # Check if we have the default subset file from rsmextra
             if HAS_RSMEXTRA:
                 default_basename = Path(default_feature_subset_file).name
-                new_config['feature_subset_file'] = default_feature_subset_file
-                cls.logger.warning("You specified the expected sign of "
-                                   "correlation but did not specify a feature "
-                                   "subset file. The tool will use "
-                                   "the default feature subset file {} "
-                                   "available via "
-                                   "rsmextra".format(default_basename))
+                new_config["feature_subset_file"] = default_feature_subset_file
+                cls.logger.warning(
+                    f"You specified the expected sign of correlation "
+                    f"but did not specify a feature subset file. The "
+                    f"tool will use the default feature subset file "
+                    f"{default_basename} available via rsmextra."
+                )
             else:
-                raise ValueError("If you want to specify the expected sign of "
-                                 " correlation for each feature, you must "
-                                 "specify a feature subset file")
+                raise ValueError(
+                    "If you want to specify the expected sign of "
+                    " correlation for each feature, you must "
+                    "specify a feature subset file"
+                )
 
         # Use the default sign if we are using the default feature file
         # and sign has not been specified in the config file
         if HAS_RSMEXTRA:
             default_feature = default_feature_subset_file
-            if (new_config['feature_subset_file'] == default_feature and
-                    not new_config['sign']):
-                new_config['sign'] = default_feature_sign
+            if new_config["feature_subset_file"] == default_feature and not new_config["sign"]:
+                new_config["sign"] = default_feature_sign
 
         # 7. Check for fields that must be specified together
-        if (new_config['min_items_per_candidate'] and
-                not new_config['candidate_column']):
-            raise ValueError("If you want to filter out candidates with "
-                             "responses to less than X items, you need "
-                             "to specify the name of the column which "
-                             "contains candidate IDs.")
+        if new_config["min_items_per_candidate"] and not new_config["candidate_column"]:
+            raise ValueError(
+                "If you want to filter out candidates with "
+                "responses to less than X items, you need "
+                "to specify the name of the column which "
+                "contains candidate IDs."
+            )
 
         # 8. Check that if "skll_objective" is specified, it's
         # one of the metrics that SKLL allows for AND that it is
         # specified for a SKLL model and _not_ a built-in
         # linear regression model
-        if new_config['skll_objective']:
-            if not is_skll_model(new_config['model']):
-                warnings.warn("You specified a custom SKLL objective but also chose a "
-                              "non-SKLL model. The objective will be ignored.")
+        if new_config["skll_objective"]:
+            if not is_skll_model(new_config["model"]):
+                warnings.warn(
+                    "You specified a custom SKLL objective but also chose a "
+                    "non-SKLL model. The objective will be ignored."
+                )
             else:
-                if new_config['skll_objective'] not in _SCORERS:
-                    raise ValueError("Invalid SKLL objective. Please refer to the SKLL "
-                                     "documentation and choose a valid tuning objective.")
+                if new_config["skll_objective"] not in _SCORERS:
+                    raise ValueError(
+                        "Invalid SKLL objective. Please refer to the SKLL "
+                        "documentation and choose a valid tuning objective."
+                    )
 
         # 9. Check that if "skll_fixed_parameters" is specified,
         # it's specified for SKLL model and _not_ a built-in linear
         # regression model; we cannot check whether the parameters
         # are valid at parse time but SKLL will raise an error
         # at run time for any invalid parameters
-        if new_config['skll_fixed_parameters']:
-            if not is_skll_model(new_config['model']):
-                warnings.warn("You specified custom SKLL fixed parameters but "
-                              "also chose a non-SKLL model. The parameters will "
-                              "be ignored.")
+        if new_config["skll_fixed_parameters"]:
+            if not is_skll_model(new_config["model"]):
+                warnings.warn(
+                    "You specified custom SKLL fixed parameters but "
+                    "also chose a non-SKLL model. The parameters will "
+                    "be ignored."
+                )
 
         # 10. Check that if we are running rsmtool to ask for
         # expected scores then the SKLL model type must actually
         # support probabilistic classification. If it's not a SKLL
         # model at all, we just treat it as a LinearRegression model
         # which is basically what they all are in the end.
-        if context == 'rsmtool' and new_config['predict_expected_scores']:
-            model_name = new_config['model']
-            dummy_learner = Learner(model_name) if is_skll_model(model_name) else Learner('LinearRegression')
-            if not hasattr(dummy_learner.model_type, 'predict_proba'):
-                raise ValueError("{} does not support expected scores "
-                                 "since it is not a probablistic classifier.".format(model_name))
+        if context == "rsmtool" and new_config["predict_expected_scores"]:
+            model_name = new_config["model"]
+            dummy_learner = (
+                Learner(model_name) if is_skll_model(model_name) else Learner("LinearRegression")
+            )
+            if not hasattr(dummy_learner.model_type, "predict_proba"):
+                raise ValueError(
+                    f"{model_name} does not support expected scores "
+                    f"since it is not a probablistic classifier."
+                )
             del dummy_learner
 
         # 11. Check the fields that requires rsmextra
         if not HAS_RSMEXTRA:
-            if new_config['special_sections']:
-                raise ValueError("Special sections are only available to ETS"
-                                 " users by installing the rsmextra package.")
+            if new_config["special_sections"]:
+                raise ValueError(
+                    "Special sections are only available to ETS"
+                    " users by installing the rsmextra package."
+                )
 
         # 12. Raise a warning if we are specifiying a feature file but also
         # telling the system to automatically select transformations
-        if new_config['features'] and new_config['select_transformations']:
+        if new_config["features"] and new_config["select_transformations"]:
             # Show a warning unless a user passed a list of features.
-            if not isinstance(new_config['features'], list):
-                warnings.warn("You specified a feature file but also set "
-                              "`select_transformations` to True. Any "
-                              "transformations or signs specified in "
-                              "the feature file will be overwritten by "
-                              "the automatically selected transformations "
-                              "and signs.")
+            if not isinstance(new_config["features"], list):
+                warnings.warn(
+                    "You specified a feature file but also set "
+                    "`select_transformations` to True. Any "
+                    "transformations or signs specified in "
+                    "the feature file will be overwritten by "
+                    "the automatically selected transformations "
+                    "and signs."
+                )
 
         # 13. If we have `experiment_names`, check that the length of the list
         # matches the list of experiment_dirs.
-        if context == 'rsmsummarize' and new_config['experiment_names']:
-            if len(new_config['experiment_names']) != len(new_config['experiment_dirs']):
-                raise ValueError("The number of specified experiment names should be the same"
-                                 " as the number of specified experiment directories.")
+        if context == "rsmsummarize" and new_config["experiment_names"]:
+            if len(new_config["experiment_names"]) != len(new_config["experiment_dirs"]):
+                raise ValueError(
+                    "The number of specified experiment names should be the same"
+                    " as the number of specified experiment directories."
+                )
 
         # 14. Check that if the user specified min_n_per_group, they also
         # specified subgroups. If they supplied a dictionary, make
         # sure the keys match
-        if new_config['min_n_per_group']:
+        if new_config["min_n_per_group"]:
             # make sure we have subgroups
-            if 'subgroups' not in new_config:
-                raise ValueError("You must specify a list of subgroups in "
-                                 "in the `subgroups` field if "
-                                 "you want to use the `min_n_per_group` field")
+            if "subgroups" not in new_config:
+                raise ValueError(
+                    "You must specify a list of subgroups in "
+                    "in the `subgroups` field if "
+                    "you want to use the `min_n_per_group` field"
+                )
             # if we got dictionary, make sure the keys match
-            elif isinstance(new_config['min_n_per_group'], dict):
-                if sorted(new_config['min_n_per_group'].keys()) != sorted(new_config['subgroups']):
-                    raise ValueError("The keys in `min_n_per_group` must "
-                                     "match the subgroups in `subgroups` field")
+            elif isinstance(new_config["min_n_per_group"], dict):
+                if sorted(new_config["min_n_per_group"].keys()) != sorted(new_config["subgroups"]):
+                    raise ValueError(
+                        "The keys in `min_n_per_group` must "
+                        "match the subgroups in `subgroups` field"
+                    )
             # else convert to dictionary
             else:
-                new_config['min_n_per_group'] = {group: new_config['min_n_per_group']
-                                                 for group in new_config['subgroups']}
+                new_config["min_n_per_group"] = {
+                    group: new_config["min_n_per_group"] for group in new_config["subgroups"]
+                }
 
         # 15. Clean up config dict to keep only context-specific fields
-        context_relevant_fields = (CHECK_FIELDS[context]['optional'] +
-                                   CHECK_FIELDS[context]['required'])
+        context_relevant_fields = (
+            CHECK_FIELDS[context]["optional"] + CHECK_FIELDS[context]["required"]
+        )
 
-        new_config = {k: v for k, v in new_config.items()
-                      if k in context_relevant_fields}
+        new_config = {k: v for k, v in new_config.items() if k in context_relevant_fields}
 
         return new_config
 
     @classmethod
     def process_config(cls, config):
         """
         Process configuration file.
@@ -1082,28 +1100,26 @@
         # Get the parameter dictionary
         new_config = deepcopy(config)
 
         # convert multiple values into lists
         for field in LIST_FIELDS:
             if field in new_config and new_config[field] is not None:
                 if not isinstance(new_config[field], list):
-                    new_config[field] = new_config[field].split(',')
-                    new_config[field] = [prefix.strip() for prefix
-                                         in new_config[field]]
+                    new_config[field] = new_config[field].split(",")
+                    new_config[field] = [prefix.strip() for prefix in new_config[field]]
 
         # make sure all boolean values are boolean
         for field in BOOLEAN_FIELDS:
-            error_message = ('Field {} can only be set to '
-                             'True or False.'.format(field))
+            error_message = f"Field {field} can only be set to True or False."
             if field in new_config and new_config[field] is not None:
                 if not isinstance(new_config[field], bool):
                     # we first convert the value to string to avoid
                     # attribute errors in case the user supplied an integer.
                     given_value = str(new_config[field]).strip()
-                    m = re.match(r'^(true|false)$', given_value, re.I)
+                    m = re.match(r"^(true|false)$", given_value, re.I)
                     if not m:
                         raise ValueError(error_message)
                     else:
                         bool_value = json.loads(m.group().lower())
                         new_config[field] = bool_value
 
         return new_config
```

### Comparing `rsmtool-9.0.1/rsmtool/container.py` & `rsmtool-9.1.1/rsmtool/container.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         Return a string representation of the container.
 
         Returns
         -------
         container_names : str
             A comma-separated list of dataset names from the container.
         """
-        return ', '.join(self._names)
+        return ", ".join(self._names)
 
     def __add__(self, other):
         """
         Add another container object to instance.
 
         Return a new container object with datasets included
         in either of the two containers.
@@ -125,22 +125,20 @@
         KeyError
             If there are duplicate keys in the two containers.
         ValueError
             If the object being added is not a container.
 
         """
         if not isinstance(other, DataContainer):
-            raise ValueError('Object must be a `DataContainer`, '
-                             'not {}.'.format(type(other)))
+            raise ValueError(f"Object must be a `DataContainer`, not {type(other)}.")
 
         # Make sure there are no duplicate keys
         common_keys = set(other._names).intersection(self._names)
         if common_keys:
-            raise KeyError('The key(s) `{}` already exist in the '
-                           'container.'.format(', '.join(common_keys)))
+            raise KeyError(f"The key(s) `{', '.join(common_keys)}` already exist in the container.")
 
         dicts = DataContainer.to_datasets(self)
         dicts.extend(DataContainer.to_datasets(other))
         return DataContainer(dicts)
 
     def __iter__(self):
         """
@@ -170,17 +168,19 @@
         Returns
         -------
         datasets_dict : list of dicts
             A list of dataset dictionaries.
         """
         dataset_dicts = []
         for name in data_container.keys():
-            dataset_dict = {'name': name,
-                            'path': data_container.get_path(name),
-                            'frame': data_container.get_frame(name)}
+            dataset_dict = {
+                "name": name,
+                "path": data_container.get_path(name),
+                "frame": data_container.get_frame(name),
+            }
             dataset_dicts.append(dataset_dict)
         return dataset_dicts
 
     def add_dataset(self, dataset_dict, update=False):
         """
         Add a new dataset (or update an existing one).
 
@@ -189,22 +189,21 @@
         dataset_dict : dict
             The dataset dictionary to add or update
             with the "name", "frame", and "path" keys.
         update : bool, optional
             Update an existing DataFrame, if ``True``.
             Defaults to ``False``.
         """
-        name = dataset_dict['name']
-        data_frame = dataset_dict['frame']
-        path = dataset_dict.get('path')
+        name = dataset_dict["name"]
+        data_frame = dataset_dict["frame"]
+        path = dataset_dict.get("path")
 
         if not update:
             if name in self._names:
-                raise KeyError('The name {} already exists in the '
-                               'container dictionary.'.format(name))
+                raise KeyError(f"The name {name} already exists in the container dictionary.")
 
         if name not in self._names:
             self._names.append(name)
 
         self._dataframes[name] = data_frame
         self._data_paths[name] = path
 
@@ -273,22 +272,24 @@
         -------
         frames : dict
             A dictionary with the data frames that contain the specified
             prefix and/or suffix in their corresponding names. The names
             are the keys and the frames are the values.
         """
         if prefix is None:
-            prefix = ''
+            prefix = ""
 
         if suffix is None:
-            suffix = ''
+            suffix = ""
 
-        names = [name for name in self._names if
-                 name.lower().startswith(prefix) and
-                 name.lower().endswith(suffix)]
+        names = [
+            name
+            for name in self._names
+            if name.lower().startswith(prefix) and name.lower().endswith(suffix)
+        ]
 
         frames = {}
         for name in names:
             frames[name] = self._dataframes[name]
         return frames
 
     def keys(self):  # noqa: D402
@@ -334,17 +335,17 @@
             The name of the dataset to drop.
 
         Returns
         -------
         self
         """
         if name not in self:
-            warnings.warn('The name `{}` is not in the '
-                          'container. No datasets will '
-                          'be dropped.'.format(name))
+            warnings.warn(
+                f"The name `{name}` is not in the container. " f"No datasets will be dropped."
+            )
         else:
             self._names.remove(name)
             self._dataframes.pop(name)
             self._data_paths.pop(name)
         return self
 
     def rename(self, name, new_name):
@@ -359,22 +360,19 @@
             The new name for the dataset in the container object.
 
         Returns
         -------
         self
         """
         if name not in self:
-            warnings.warn('The name `{}` is not in the '
-                          'container and cannot '
-                          'be renamed.'.format(name))
+            warnings.warn(f"The name `{name}` is not in the container and cannot be renamed.")
         else:
             frame = self._dataframes[name]
             path = self._data_paths[name]
-            self.add_dataset({'name': new_name, 'frame': frame, 'path': path},
-                             update=True)
+            self.add_dataset({"name": new_name, "frame": frame, "path": path}, update=True)
             self.drop(name)
         return self
 
     def copy(self, deep=True):
         """
         Return a copy of the container object.
```

### Comparing `rsmtool-9.0.1/rsmtool/convert_feature_json.py` & `rsmtool-9.1.1/rsmtool/convert_feature_json.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,56 +35,55 @@
     ------
     RuntimeError
         If the given input file is not a valid feature JSON file.
     RuntimeError
         If the output file has an unsupported extension.
     """
     # make sure the input file is a valid feature JSON file
-    json_dict = json.load(open(json_file, 'r'))
-    if not list(json_dict.keys()) == ['features']:
-        raise RuntimeError("{} is not a valid feature JSON "
-                           "file".format(json_file))
+    json_dict = json.load(open(json_file, "r"))
+    if not list(json_dict.keys()) == ["features"]:
+        raise RuntimeError(f"{json_file} is not a valid feature JSON file")
 
     # convert to tabular format
-    df_feature = pd.DataFrame(json_dict['features'])
+    df_feature = pd.DataFrame(json_dict["features"])
 
     # make sure the output file is in a supported format
     output_extension = splitext(output_file)[1].lower()
-    if output_extension not in ['.csv', '.tsv', '.xlsx']:
-        raise RuntimeError("The output file {} has an unsupported "
-                           "extension. It must be a CSV/TSV/XLSX "
-                           "file. RSMTool no longer supports .xls "
-                           "files".format(output_file))
+    if output_extension not in [".csv", ".tsv", ".xlsx"]:
+        raise RuntimeError(
+            f"The output file {output_file} has an unsupported extension. "
+            f"It must be a CSV/TSV/XLSX file. RSMTool no longer supports "
+            f".xls files."
+        )
 
-    if output_extension == '.csv':
+    if output_extension == ".csv":
         df_feature.to_csv(output_file, index=False)
-    elif output_extension == '.tsv':
-        df_feature.to_csv(output_file, sep='\t', index=False)
-    elif output_extension == '.xlsx':
-        df_feature.to_excel(output_file, sheet_name='features', index=False)
+    elif output_extension == ".tsv":
+        df_feature.to_csv(output_file, sep="\t", index=False)
+    elif output_extension == ".xlsx":
+        df_feature.to_excel(output_file, sheet_name="features", index=False)
 
     if delete:
         os.unlink(json_file)
 
 
 def main():  # noqa: D103
-    parser = argparse.ArgumentParser(prog='convert_feature_json')
-    parser.add_argument('json_file',
-                        help="The feature JSON file to convert "
-                             "to tabular format.")
-    parser.add_argument('output_file',
-                        help="The output file containing the features "
-                             "in tabular format.")
-    parser.add_argument('--delete',
-                        help="Delete original JSON file after conversion.",
-                        default=False,
-                        required=False,
-                        action="store_true")
+    parser = argparse.ArgumentParser(prog="convert_feature_json")
+    parser.add_argument("json_file", help="The feature JSON file to convert " "to tabular format.")
+    parser.add_argument(
+        "output_file",
+        help="The output file containing the features " "in tabular format.",
+    )
+    parser.add_argument(
+        "--delete",
+        help="Delete original JSON file after conversion.",
+        default=False,
+        required=False,
+        action="store_true",
+    )
 
     args = parser.parse_args()
-    convert_feature_json_file(args.json_file,
-                              args.output_file,
-                              delete=args.delete)
+    convert_feature_json_file(args.json_file, args.output_file, delete=args.delete)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `rsmtool-9.0.1/rsmtool/fairness_utils.py` & `rsmtool-9.1.1/rsmtool/fairness_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,23 @@
 :author: Jeremy Biggs (jbiggs@ets.org)
 :author: Nitin Madnani (nmadnani@ets.org)
 
 :organization: ETS
 """
 
 import pickle
+import warnings
 from os.path import join
 
-import numpy as np
 import pandas as pd
 import statsmodels.formula.api as smf
+from statsmodels.stats.anova import anova_lm
+
 from rsmtool.container import DataContainer
 from rsmtool.writer import DataWriter
-from statsmodels.stats.anova import anova_lm
 
 
 def convert_to_ordered_category(group_values, base_group=None):
     """
     Convert given series to an ordered category.
 
     The levels are ordered by category size. If multiple
@@ -50,33 +51,35 @@
     # get ordered list by size
 
     # To get the ordered list by size, we convert the value counts to data
     # frame to allow for multilevel sorting. This ensures that the order
     # is consistent and reproducible across runs when there is more than
     # one group with the maximum number of occurrences
     df_groups_by_size = pd.DataFrame(group_values.value_counts()).reset_index()
-    df_groups_by_size.columns = ['group_name', 'count']
-    df_groups_by_size_sorted = df_groups_by_size.sort_values(['count', 'group_name'],
-                                                             ascending=[False, True])
-    groups_by_size = df_groups_by_size_sorted['group_name'].tolist()
+    df_groups_by_size.columns = ["group_name", "count"]
+    df_groups_by_size_sorted = df_groups_by_size.sort_values(
+        ["count", "group_name"], ascending=[False, True]
+    )
+    groups_by_size = df_groups_by_size_sorted["group_name"].tolist()
 
     if base_group is not None:
         # if we have user-supplied base group, check that it's actually in the data
         if base_group not in group_values.values:
-            raise ValueError("The reference group {} must be one of the existing "
-                             "values for this group".format(base_group))
+            raise ValueError(
+                f"The reference group {base_group} must be one of the "
+                f"existing values for this group"
+            )
         else:
             # move the supplied reference group to the beginning of the list
             base_index = groups_by_size.index(base_group)
             groups_by_size.insert(0, groups_by_size.pop(base_index))
 
     # convert to category and reorder
     group_category = group_values.astype("category")
-    group_ordered_category = group_category.cat.reorder_categories(groups_by_size,
-                                                                   ordered=True)
+    group_ordered_category = group_category.cat.reorder_categories(groups_by_size, ordered=True)
     return group_ordered_category
 
 
 def get_coefficients(fit, base_category):
     """
     Extract estimates, significance, and confidence intervals for a given group.
 
@@ -101,36 +104,33 @@
         - "P>[t]"
         - "0.025" (lower end for 95% confidence interval)
         - "0.975" (upper end of 95% confidence interval)
     """
     # extract the data we need
     df_results = pd.concat([fit.params, fit.pvalues, fit.conf_int()], axis=1)
 
-    df_results.columns = ['estimate', 'P>[t]', '[0.025', '0.975]']
+    df_results.columns = ["estimate", "P>[t]", "[0.025", "0.975]"]
 
     # identify the rows we are interested in
-    groups = ['Intercept'] + [v for v in df_results.index if 'group' in v]
+    groups = ["Intercept"] + [v for v in df_results.index if "group" in v]
 
     df_results = df_results.loc[groups]
 
     # rename the rows
-    df_results.index = [v.split('.')[1].strip(']')
-                        if not v == 'Intercept'
-                        else 'Intercept ({})'.format(base_category)
-                        for v in df_results.index]
+    df_results.index = [
+        v.split(".")[1].strip("]") if not v == "Intercept" else f"Intercept ({base_category})"
+        for v in df_results.index
+    ]
 
     return df_results
 
 
-def write_fairness_results(fit_dictionary,
-                           fairness_container,
-                           group,
-                           output_dir,
-                           experiment_id,
-                           file_format):
+def write_fairness_results(
+    fit_dictionary, fairness_container, group, output_dir, experiment_id, file_format
+):
     """
     Save the results of fairness analysis to disk.
 
     Parameters
     ----------
     fit_dictionary: dict
         A dictionary of fitted models generated by ``get_fairness_analyses()``.
@@ -146,39 +146,32 @@
     file_format: str
         File format to use for data files.
     """
     # let's first save model files and summaries
     for model in fit_dictionary:
         fit = fit_dictionary[model]
 
-        ols_file = join(output_dir, '{}_{}_by_{}.ols'.format(experiment_id,
-                                                             model,
-                                                             group))
-        summary_file = join(output_dir, '{}_{}_by_{}_ols_summary.txt'.format(experiment_id,
-                                                                             model,
-                                                                             group))
-        with open(ols_file, 'wb') as olsf, open(summary_file, 'w') as summf:
+        ols_file = join(output_dir, f"{experiment_id}_{model}_by_{group}.ols")
+        summary_file = join(output_dir, f"{experiment_id}_{model}_by_{group}_ols_summary.txt")
+        with open(ols_file, "wb") as olsf, open(summary_file, "w") as summf:
             pickle.dump(fit, olsf)
             summf.write(str(fit.summary()))
 
     # Now let's write out the content of the data container
     writer = DataWriter(experiment_id)
-    writer.write_experiment_output(output_dir,
-                                   fairness_container,
-                                   file_format=file_format,
-                                   index=True)
+    writer.write_experiment_output(
+        output_dir, fairness_container, file_format=file_format, index=True
+    )
 
 
-def get_fairness_analyses(df,
-                          group,
-                          system_score_column,
-                          human_score_column='sc1',
-                          base_group=None):
+def get_fairness_analyses(
+    df, group, system_score_column, human_score_column="sc1", base_group=None
+):
     """
-    Compute fairness analyses described in `Loukina et al. 2019 <https://www.aclweb.org/anthology/W19-4401/>`_.
+    Compute analyses from `Loukina et al. 2019 <https://www.aclweb.org/anthology/W19-4401/>`_.
 
     The function computes how much variance group membership explains in
     overall score accuracy (osa), overall score difference (osd),
     and conditional score difference (csd). See the paper for more
     details.
 
     Parameters
@@ -210,98 +203,94 @@
          - "estimates_<METRIC>_by_<GROUP>" where "<GROUP>" corresponds to
            the given group and "<METRIC>" can be "osa", "osd" and "csd" estimates
            for each group computed by the respective models.
          - "fairness_metrics_by_<GROUP>" - a summary of model fits (R2 and
            p values).
     """
     # compute error and squared error
-    df['error'] = df[system_score_column] - df[human_score_column]
-    df['SE'] = df['error']**2
+    df["error"] = df[system_score_column] - df[human_score_column]
+    df["SE"] = df["error"] ** 2
 
     # convert group values to category and reorder them using
     # the largest category as reference
 
-    df['group'] = convert_to_ordered_category(df[group], base_group=base_group)
-    base_group = df['group'].cat.categories[0]
+    df["group"] = convert_to_ordered_category(df[group], base_group=base_group)
+    base_group = df["group"].cat.categories[0]
 
-    df['sc1_cat'] = convert_to_ordered_category(df[human_score_column])
+    df["sc1_cat"] = convert_to_ordered_category(df[human_score_column])
 
     # Overall score accuracy (OSA)
     # Variance in squared error explained by L1
 
     # fit the model
-    osa_model = smf.ols(formula='SE ~ group', data=df)
+    osa_model = smf.ols(formula="SE ~ group", data=df)
     osa_fit = osa_model.fit()
 
     # collect the results
-    osa_dict = {'R2': osa_fit.rsquared_adj,
-                'sig': osa_fit.f_pvalue}
+    osa_dict = {"R2": osa_fit.rsquared_adj, "sig": osa_fit.f_pvalue}
 
-    osa_results = pd.Series(osa_dict, name='Overall score accuracy')
+    osa_results = pd.Series(osa_dict, name="Overall score accuracy")
 
     df_coefficients_osa = get_coefficients(osa_fit, base_group)
 
     # Overall score difference (OSD)
     # variance in signed residuals (raw error) explained by L1
 
     # fit the model
-    osd_model = smf.ols(formula='error ~ group', data=df)
+    osd_model = smf.ols(formula="error ~ group", data=df)
     osd_fit = osd_model.fit()
 
     # collect the results
-    osd_dict = {'R2': osd_fit.rsquared_adj,
-                'sig': osd_fit.f_pvalue}
+    osd_dict = {"R2": osd_fit.rsquared_adj, "sig": osd_fit.f_pvalue}
 
-    osd_results = pd.Series(osd_dict, name='Overall score difference')
+    osd_results = pd.Series(osd_dict, name="Overall score difference")
 
     df_coefficients_osd = get_coefficients(osd_fit, base_group)
 
     # conditional score difference CSD
     # Variance in score difference conditioned on Native language
 
     # fit "null" model with human score only
-    csd_null_mod = smf.ols(formula='error ~ sc1_cat', data=df)
+    csd_null_mod = smf.ols(formula="error ~ sc1_cat", data=df)
     csd_null_fit = csd_null_mod.fit()
 
     # fit model with both human score and group
-    csd_mod = smf.ols(formula='error ~ group + sc1_cat', data=df)
+    csd_mod = smf.ols(formula="error ~ group + sc1_cat", data=df)
     csd_fit = csd_mod.fit()
 
     # compare the two models using anova_lm
     # we filter warnings for this function because we get
     # runtime warning due to NaNs in the data.
     # these seem to be by design: https://groups.google.com/forum/#!topic/pystatsmodels/-flY0cNnb3k
-    np.warnings.filterwarnings('ignore')
+    warnings.filterwarnings("ignore")
     anova_results = anova_lm(csd_null_fit, csd_fit)
     # we reset warnings
-    np.warnings.resetwarnings()
+    warnings.resetwarnings()
 
     # collect the results. Note that R2 in this case is a difference
     # in R2 between the two models and significance is obtained from anova
-    csd_dict = {'R2': csd_fit.rsquared_adj - csd_null_fit.rsquared_adj,
-                'sig': anova_results.values[1][-1]}
-    csd_results = pd.Series(csd_dict, name='Conditional score difference')
+    csd_dict = {
+        "R2": csd_fit.rsquared_adj - csd_null_fit.rsquared_adj,
+        "sig": anova_results.values[1][-1],
+    }
+    csd_results = pd.Series(csd_dict, name="Conditional score difference")
 
     df_coefficients_csd = get_coefficients(csd_fit, base_group)
 
     # create a summary table
 
     df_r2_all = pd.concat([osa_results, osd_results, csd_results], axis=1, sort=True)
-    df_r2_all['base_category'] = base_group
+    df_r2_all["base_category"] = base_group
 
     # assemble all datasets into a DataContainer
 
-    datasets = [{'name': 'estimates_osa_by_{}'.format(group),
-                 'frame': df_coefficients_osa},
-                {'name': 'estimates_osd_by_{}'.format(group),
-                 'frame': df_coefficients_osd},
-                {'name': 'estimates_csd_by_{}'.format(group),
-                 'frame': df_coefficients_csd},
-                {'name': 'fairness_metrics_by_{}'.format(group),
-                 'frame': df_r2_all}]
+    datasets = [
+        {"name": f"estimates_osa_by_{group}", "frame": df_coefficients_osa},
+        {"name": f"estimates_osd_by_{group}", "frame": df_coefficients_osd},
+        {"name": f"estimates_csd_by_{group}", "frame": df_coefficients_csd},
+        {"name": f"fairness_metrics_by_{group}", "frame": df_r2_all},
+    ]
 
     # assemble all models into a dictionary
-    model_dict = {'osa': osa_fit,
-                  'osd': osd_fit,
-                  'csd': csd_fit}
+    model_dict = {"osa": osa_fit, "osd": osd_fit, "csd": csd_fit}
 
     return model_dict, DataContainer(datasets=datasets)
```

### Comparing `rsmtool-9.0.1/rsmtool/modeler.py` & `rsmtool-9.1.1/rsmtool/modeler.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,15 @@
 from .preprocessor import FeaturePreprocessor
 from .utils.metrics import compute_expected_scores_from_model
 from .utils.models import is_skll_model
 from .writer import DataWriter
 
 
 class Modeler:
-    """
-    Class to train model and generate predictions with built-in or SKLL models.
-    """
+    """Class to train model and generate predictions with built-in or SKLL models."""
 
     def __init__(self, logger=None):
         """Instantiate empty instance with no learner and given logger, if any."""
         self.learner = None
         self.logger = logger if logger else logging.getLogger(__name__)
 
     @classmethod
@@ -56,18 +54,19 @@
             A Modeler instance.
 
         Raises
         ------
         ValueError
             If ``model_path`` does not end with ".model".
         """
-        if not model_path.lower().endswith('.model'):
-            raise ValueError('The file `{}` does not end with the '
-                             'proper extension. Please make sure that '
-                             'it is a `.model` file.'.format(model_path))
+        if not model_path.lower().endswith(".model"):
+            raise ValueError(
+                f"The file `{model_path}` does not end with the proper "
+                f"extension. Please make sure that it is a `.model` file."
+            )
 
         # Create SKLL learner from file
         learner = Learner.from_file(model_path)
         return cls.load_from_learner(learner)
 
     @classmethod
     def load_from_learner(cls, learner):
@@ -86,17 +85,18 @@
 
         Raises
         ------
         TypeError
             If ``learner`` is not a SKLL Learner instance.
         """
         if not isinstance(learner, Learner):
-            raise TypeError('The `learner` argument must be a '
-                            '` SKLL Learner` instance, not `{}`.'
-                            ''.format(type(learner)))
+            raise TypeError(
+                f"The `learner` argument must be a ` SKLL Learner` instance, "
+                f"not `{type(learner)}`."
+            )
 
         # Create Modeler instance
         modeler = Modeler()
         modeler.learner = learner
         return modeler
 
     @staticmethod
@@ -112,17 +112,17 @@
 
         Returns
         -------
         df_fit : pandas DataFrame
             The output data frame with the main model fit metrics.
         """
         df_fit = pd.DataFrame({"N responses": [int(fit.nobs)]})
-        df_fit['N features'] = int(fit.df_model)
-        df_fit['R2'] = fit.rsquared
-        df_fit['R2_adjusted'] = fit.rsquared_adj
+        df_fit["N features"] = int(fit.df_model)
+        df_fit["R2"] = fit.rsquared
+        df_fit["R2_adjusted"] = fit.rsquared_adj
         return df_fit
 
     @staticmethod
     def ols_coefficients_to_dataframe(coefs):
         """
         Convert series containing OLS coefficients to a data frame.
 
@@ -141,30 +141,30 @@
 
         Note
         ----
         The first row in the output data frame is always for the intercept
         and the rest are sorted by feature name.
         """
         # first create a sorted data frame for all the non-intercept features
-        non_intercept_columns = [c for c in coefs.index if c != 'const']
-        df_non_intercept = pd.DataFrame(coefs.filter(non_intercept_columns),
-                                        columns=['coefficient'])
-        df_non_intercept.index.name = 'feature'
+        non_intercept_columns = [c for c in coefs.index if c != "const"]
+        df_non_intercept = pd.DataFrame(
+            coefs.filter(non_intercept_columns), columns=["coefficient"]
+        )
+        df_non_intercept.index.name = "feature"
         df_non_intercept = df_non_intercept.sort_index()
         df_non_intercept.reset_index(inplace=True)
 
         # now create a data frame that just has the intercept
-        df_intercept = pd.DataFrame([{'feature': 'Intercept',
-                                      'coefficient': coefs['const']}])
+        df_intercept = pd.DataFrame([{"feature": "Intercept", "coefficient": coefs["const"]}])
 
         # append the non-intercept frame to the intercept one
         df_coef = pd.concat([df_intercept, df_non_intercept], sort=True, ignore_index=True)
 
         # we always want to have the feature column first
-        df_coef = df_coef[['feature', 'coefficient']]
+        df_coef = df_coef[["feature", "coefficient"]]
 
         return df_coef
 
     @staticmethod
     def skll_learner_params_to_dataframe(learner):
         """
         Extract parameters from the given SKLL learner into a data frame.
@@ -188,30 +188,28 @@
            do not want.
         2. The first row in the output data frame is always for the intercept
            and the rest are sorted by feature name.
         """
         # get the intercept, coefficients, and feature names
         intercept = learner.model.intercept_
         coefficients = learner.model.coef_
-        feature_names = learner.feat_vectorizer.get_feature_names()
+        feature_names = learner.feat_vectorizer.get_feature_names_out()
 
         # first create a sorted data frame for all the non-intercept features
-        df_non_intercept = pd.DataFrame({'feature': feature_names,
-                                         'coefficient': coefficients})
-        df_non_intercept = df_non_intercept.sort_values(by=['feature'])
+        df_non_intercept = pd.DataFrame({"feature": feature_names, "coefficient": coefficients})
+        df_non_intercept = df_non_intercept.sort_values(by=["feature"])
 
         # now create a data frame that just has the intercept
-        df_intercept = pd.DataFrame([{'feature': 'Intercept',
-                                      'coefficient': intercept}])
+        df_intercept = pd.DataFrame([{"feature": "Intercept", "coefficient": intercept}])
 
         # append the non-intercept frame to the intercept one
         df_coef = pd.concat([df_intercept, df_non_intercept], sort=True, ignore_index=True)
 
         # we always want to have the feature column first
-        df_coef = df_coef[['feature', 'coefficient']]
+        df_coef = df_coef[["feature", "coefficient"]]
 
         return df_coef
 
     def create_fake_skll_learner(self, df_coefficients):
         """
         Create a fake SKLL linear regression learner from given coefficients.
 
@@ -229,32 +227,33 @@
         """
         # initialize a random number generator
         randgen = RandomState(1234567890)
 
         # iterate over the coefficients
         coefdict = {}
         for feature, coefficient in df_coefficients.itertuples(index=False):
-            if feature == 'Intercept':
+            if feature == "Intercept":
                 intercept = coefficient
             else:
                 # exclude NA coefficients
                 if coefficient == np.nan:
-                    self.logger.warning("No coefficient was estimated for "
-                                        "{}. This is likely due to exact "
-                                        "collinearity in the model. This "
-                                        "feature will not be used for model "
-                                        "building".format(feature))
+                    self.logger.warning(
+                        f"No coefficient was estimated for {feature}. "
+                        f"This is likely due to exact collinearity in "
+                        f"the model. This feature will not be used for "
+                        f"model building"
+                    )
                 else:
                     coefdict[feature] = coefficient
 
-        learner = Learner('LinearRegression')
+        learner = Learner("LinearRegression")
         num_features = len(coefdict)  # excluding the intercept
         fake_feature_values = randgen.rand(num_features)
         fake_features = [dict(zip(coefdict, fake_feature_values))]
-        fake_fs = FeatureSet('fake', ids=['1'], labels=[1.0], features=fake_features)
+        fake_fs = FeatureSet("fake", ids=["1"], labels=[1.0], features=fake_features)
         learner.train(fake_fs, grid_search=False)
 
         # now create its parameters from the coefficients from the built-in model
         learner.model.coef_ = learner.feat_vectorizer.transform(coefdict).toarray()[0]
         learner.model.intercept_ = intercept
         return learner
 
@@ -286,15 +285,15 @@
         # get the feature columns
         X = df_train[feature_columns]
 
         # add the intercept
         X = sm.add_constant(X)
 
         # fit the model
-        fit = sm.OLS(df_train['sc1'], X).fit()
+        fit = sm.OLS(df_train["sc1"], X).fit()
         df_coef = self.ols_coefficients_to_dataframe(fit.params)
         learner = self.create_fake_skll_learner(df_coef)
 
         # we used all the features
         used_features = feature_columns
 
         return learner, fit, df_coef, used_features
@@ -322,33 +321,31 @@
         df_coef : pandas DataFrame
             Data frame containing the model coefficients.
         used_features : list of str
             A list of features used in the final model.
         """
         # we first compute a single feature that is simply the sum of all features
         df_train_eqwt = df_train.copy()
-        df_train_eqwt['sumfeature'] = df_train_eqwt[feature_columns].apply(np.sum,
-                                                                           axis=1)
+        df_train_eqwt["sumfeature"] = df_train_eqwt[feature_columns].apply(np.sum, axis=1)
 
         # train a plain Linear Regression model
-        X = df_train_eqwt['sumfeature']
+        X = df_train_eqwt["sumfeature"]
         X = sm.add_constant(X)
-        fit = sm.OLS(df_train_eqwt['sc1'], X).fit()
+        fit = sm.OLS(df_train_eqwt["sc1"], X).fit()
 
         # get the coefficient for the summed feature and the intercept
-        coef = fit.params['sumfeature']
-        const = fit.params['const']
+        coef = fit.params["sumfeature"]
+        const = fit.params["const"]
 
         # now we need to assign this coefficient to all of the original
         # features and create a fake SKLL learner with these weights
-        original_features = [c for c in df_train_eqwt.columns if c not in ['sc1',
-                                                                           'sumfeature',
-                                                                           'spkitemid']]
-        coefs = pd.Series(dict([(origf, coef)
-                                for origf in original_features] + [('const', const)]))
+        original_features = [
+            c for c in df_train_eqwt.columns if c not in ["sc1", "sumfeature", "spkitemid"]
+        ]
+        coefs = pd.Series(dict([(origf, coef) for origf in original_features] + [("const", const)]))
         df_coef = self.ols_coefficients_to_dataframe(coefs)
 
         # create fake SKLL learner with these coefficients
         learner = self.create_fake_skll_learner(df_coef)
 
         # we used all the features
         used_features = feature_columns
@@ -380,46 +377,48 @@
              Data frame containing the model coefficients.
         used_features : list of str
             A list of features used in the final model.
         """
         # train a plain Linear Regression model
         X = df_train[feature_columns]
         X = sm.add_constant(X)
-        fit = sm.OLS(df_train['sc1'], X).fit()
+        fit = sm.OLS(df_train["sc1"], X).fit()
 
         # convert the model parameters into a data frame
         df_params = self.ols_coefficients_to_dataframe(fit.params)
-        df_params = df_params.set_index('feature')
+        df_params = df_params.set_index("feature")
 
         # compute the betas for the non-intercept coefficients
         df_weights = df_params.loc[feature_columns]
         df_betas = df_weights.copy()
 
         df_train_std = df_train[feature_columns].std()
-        df_betas['coefficient'] = (df_weights['coefficient'].multiply(df_train_std,
-                                                                      axis='index') /
-                                   df_train['sc1'].std())
+        df_betas["coefficient"] = (
+            df_weights["coefficient"].multiply(df_train_std, axis="index") / df_train["sc1"].std()
+        )
 
         # replace each negative beta with delta and adjust
         # all the positive betas to account for this
         RT = 0.05
-        df_positive_betas = df_betas[df_betas['coefficient'] > 0]
-        df_negative_betas = df_betas[df_betas['coefficient'] < 0]
-        delta = np.sum(df_positive_betas['coefficient']) * RT / len(df_negative_betas)
-        df_betas['coefficient'] = df_betas.apply(lambda row: row['coefficient'] * (1 - RT)
-                                                 if row['coefficient'] > 0 else delta, axis=1)
+        df_positive_betas = df_betas[df_betas["coefficient"] > 0]
+        df_negative_betas = df_betas[df_betas["coefficient"] < 0]
+        delta = np.sum(df_positive_betas["coefficient"]) * RT / len(df_negative_betas)
+        df_betas["coefficient"] = df_betas.apply(
+            lambda row: row["coefficient"] * (1 - RT) if row["coefficient"] > 0 else delta,
+            axis=1,
+        )
 
         # rescale the adjusted betas to get the new coefficients
-        df_coef = df_betas['coefficient'] * df_train['sc1'].std()
-        df_coef = df_coef.divide(df_train[feature_columns].std(), axis='index')
+        df_coef = df_betas["coefficient"] * df_train["sc1"].std()
+        df_coef = df_coef.divide(df_train[feature_columns].std(), axis="index")
 
         # add the intercept back to the new coefficients
-        df_coef['Intercept'] = df_params.loc['Intercept'].coefficient
+        df_coef["Intercept"] = df_params.loc["Intercept"].coefficient
         df_coef = df_coef.sort_index().reset_index()
-        df_coef.columns = ['feature', 'coefficient']
+        df_coef.columns = ["feature", "coefficient"]
 
         # create fake SKLL learner with these coefficients
         learner = self.create_fake_skll_learner(df_coef)
 
         # we used all the features
         used_features = feature_columns
 
@@ -452,31 +451,31 @@
         used_features : list of str
             A list of features used in the final model.
         """
         # train a Lasso Regression model with this featureset with a preset lambda
         p_lambda = sqrt(len(df_train) * log10(len(feature_columns)))
 
         # create a SKLL FeatureSet instance from the given data frame
-        fs_train = FeatureSet.from_data_frame(df_train[feature_columns + ['sc1']],
-                                              'train',
-                                              labels_column='sc1')
+        fs_train = FeatureSet.from_data_frame(
+            df_train[feature_columns + ["sc1"]], "train", labels_column="sc1"
+        )
 
         # note that 'alpha' in sklearn is different from this lambda
         # so we need to normalize looking at the sklearn objective equation
         p_alpha = p_lambda / len(df_train)
-        l_lasso = Learner('Lasso', model_kwargs={'alpha': p_alpha, 'positive': True})
+        l_lasso = Learner("Lasso", model_kwargs={"alpha": p_alpha, "positive": True})
         l_lasso.train(fs_train, grid_search=False)
 
         # get the feature names that have the non-zero coefficients
         non_zero_features = list(l_lasso.model_params[0].keys())
 
         # now train a new vanilla linear regression with just the non-zero features
         X = df_train[non_zero_features]
         X = sm.add_constant(X)
-        fit = sm.OLS(df_train['sc1'], X).fit()
+        fit = sm.OLS(df_train["sc1"], X).fit()
 
         # get the coefficients data frame
         df_coef = self.ols_coefficients_to_dataframe(fit.params)
 
         # create fake SKLL learner with these coefficients
         learner = self.create_fake_skll_learner(df_coef)
 
@@ -510,28 +509,28 @@
         df_coef : pandas DataFrame
             Data frame containing the model coefficients.
         used_features : list of str
             A list of features used in the final model.
         """
         # train a LassoCV outside of SKLL since it's not exposed there
         X = df_train[feature_columns].values
-        y = df_train['sc1'].values
+        y = df_train["sc1"].values
         clf = LassoCV(cv=10, positive=True, random_state=1234567890)
         model = clf.fit(X, y)
 
         # get the non-zero features from this model
         non_zero_features = []
         for feature, coefficient in zip(feature_columns, model.coef_):
             if coefficient != 0:
                 non_zero_features.append(feature)
 
         # now train a new linear regression with just these non-zero features
         X = df_train[non_zero_features]
         X = sm.add_constant(X)
-        fit = sm.OLS(df_train['sc1'], X).fit()
+        fit = sm.OLS(df_train["sc1"], X).fit()
 
         # convert the model parameters into a data frame
         df_coef = self.ols_coefficients_to_dataframe(fit.params)
 
         # create fake SKLL learner with these coefficients
         learner = self.create_fake_skll_learner(df_coef)
 
@@ -571,15 +570,15 @@
         used_features : list of str
             A list of features used in the final model.
         """
         # add an intercept to the features manually
         X = df_train[feature_columns].values
         intercepts = np.ones((len(df_train), 1))
         X_plus_intercept = np.concatenate([intercepts, X], axis=1)
-        y = df_train['sc1'].values
+        y = df_train["sc1"].values
 
         # fit an NNLS model on this data
         coefs, rnorm = nnls(X_plus_intercept, y)
 
         # check whether the intercept is set to 0 and if so then we need
         # to flip the sign and refit the model to ensure that it is always
         # kept in the model
@@ -597,15 +596,15 @@
         for feature, coefficient in zip(feature_columns, coefficients):
             if coefficient != 0:
                 non_zero_features.append(feature)
 
         # now train a new linear regression with just these non-zero features
         X = df_train[non_zero_features]
         X = sm.add_constant(X)
-        fit = sm.OLS(df_train['sc1'], X).fit()
+        fit = sm.OLS(df_train["sc1"], X).fit()
 
         # convert this model's parameters to a data frame
         df_coef = self.ols_coefficients_to_dataframe(fit.params)
 
         # create fake SKLL learner with these coefficients
         learner = self.create_fake_skll_learner(df_coef)
 
@@ -644,33 +643,33 @@
             Data frame containing the model coefficients.
         used_features : list of str
             A list of features used in the final model.
         """
         X = df_train[feature_columns]
         X = sm.add_constant(X)
 
-        y = df_train['sc1']
+        y = df_train["sc1"]
 
         fit = sm.OLS(y, X).fit()
 
         positive_features = []
         for name, value in fit.params.items():
-            if value >= 0 and name != 'const':
+            if value >= 0 and name != "const":
                 positive_features.append(name)
 
         X = df_train[positive_features]
         X = sm.add_constant(X)
 
         fit = sm.OLS(y, X).fit()
 
         # if any parameters are still negative, set them to zero
         params = fit.params.copy()
-        params = params.drop('const')
+        params = params.drop("const")
         if not (params >= 0).all():
-            fit.params[(fit.params < 0) & (fit.params.index != 'const')] = 0
+            fit.params[(fit.params < 0) & (fit.params.index != "const")] = 0
 
         # convert this model's parameters to a data frame
         df_coef = self.ols_coefficients_to_dataframe(fit.params)
 
         # create fake SKLL learner with these coefficients
         learner = self.create_fake_skll_learner(df_coef)
 
@@ -705,33 +704,33 @@
         used_features : list of str
             A list of features used in the final model.
         """
         # train a Lasso Regression model with a preset lambda
         p_lambda = sqrt(len(df_train) * log10(len(feature_columns)))
 
         # create a SKLL FeatureSet instance from the given data frame
-        fs_train = FeatureSet.from_data_frame(df_train[feature_columns + ['sc1']],
-                                              'train',
-                                              labels_column='sc1')
+        fs_train = FeatureSet.from_data_frame(
+            df_train[feature_columns + ["sc1"]], "train", labels_column="sc1"
+        )
 
         # note that 'alpha' in sklearn is different from this lambda
         # so we need to normalize looking at the sklearn objective equation
         p_alpha = p_lambda / len(df_train)
-        l_lasso = Learner('Lasso', model_kwargs={'alpha': p_alpha, 'positive': True})
+        l_lasso = Learner("Lasso", model_kwargs={"alpha": p_alpha, "positive": True})
         l_lasso.train(fs_train, grid_search=False)
 
         # get the feature names that have the non-zero coefficients
         non_zero_features = list(l_lasso.model_params[0].keys())
 
         # now train an NNLS regression using these non-zero features
         # first add an intercept to the features manually
         X = df_train[feature_columns].values
         intercepts = np.ones((len(df_train), 1))
         X_plus_intercept = np.concatenate([intercepts, X], axis=1)
-        y = df_train['sc1'].values
+        y = df_train["sc1"].values
 
         # fit an NNLS model on this data
         coefs, rnorm = nnls(X_plus_intercept, y)
 
         # check whether the intercept is set to 0 and if so then we need
         # to flip the sign and refit the model to ensure that it is always
         # kept in the model
@@ -751,15 +750,15 @@
         for feature, coefficient in zip(feature_columns, coefficients):
             if coefficient != 0:
                 non_zero_features.append(feature)
 
         # now train a new linear regression with just these non-zero features
         X = df_train[non_zero_features]
         X = sm.add_constant(X)
-        fit = sm.OLS(df_train['sc1'], X).fit()
+        fit = sm.OLS(df_train["sc1"], X).fit()
 
         # convert this model's parameters into a data frame
         df_coef = self.ols_coefficients_to_dataframe(fit.params)
 
         # create fake SKLL learner with these coefficients
         learner = self.create_fake_skll_learner(df_coef)
 
@@ -794,22 +793,22 @@
         used_features : list of str
             A list of features used in the final model.
         """
         # train a Lasso Regression model with a preset lambda
         p_lambda = sqrt(len(df_train) * log10(len(feature_columns)))
 
         # create a SKLL FeatureSet instance from the given data frame
-        fs_train = FeatureSet.from_data_frame(df_train[feature_columns + ['sc1']],
-                                              'train',
-                                              labels_column='sc1')
+        fs_train = FeatureSet.from_data_frame(
+            df_train[feature_columns + ["sc1"]], "train", labels_column="sc1"
+        )
 
         # note that 'alpha' in sklearn is different from this lambda
         # so we need to normalize looking at the sklearn objective equation
         alpha = p_lambda / len(df_train)
-        learner = Learner('Lasso', model_kwargs={'alpha': alpha, 'positive': True})
+        learner = Learner("Lasso", model_kwargs={"alpha": alpha, "positive": True})
         learner.train(fs_train, grid_search=False)
 
         # convert this model's parameters to a data frame
         df_coef = self.skll_learner_params_to_dataframe(learner)
 
         # there's no OLS fit object in this case
         fit = None
@@ -845,30 +844,32 @@
         df_coef : pandas DataFrame
             Data frame containing the model coefficients.
         used_features : list of str
             A list of features used in the final model.
         """
         # train a LassoCV outside of SKLL since it's not exposed there
         X = df_train[feature_columns].values
-        y = df_train['sc1'].values
+        y = df_train["sc1"].values
         clf = LassoCV(cv=10, positive=True, random_state=1234567890)
         model = clf.fit(X, y)
 
         # save the non-zero model coefficients and intercept to a data frame
         non_zero_features, non_zero_feature_values = [], []
         for feature, coefficient in zip(feature_columns, model.coef_):
             if coefficient != 0:
                 non_zero_features.append(feature)
                 non_zero_feature_values.append(coefficient)
 
         # initialize the coefficient data frame with just the intercept
-        df_coef = pd.DataFrame([('Intercept', model.intercept_)])
-        df_coef = pd.concat([df_coef, pd.DataFrame(zip(non_zero_features, non_zero_feature_values))],
-                            ignore_index=True)
-        df_coef.columns = ['feature', 'coefficient']
+        df_coef = pd.DataFrame([("Intercept", model.intercept_)])
+        df_coef = pd.concat(
+            [df_coef, pd.DataFrame(zip(non_zero_features, non_zero_feature_values))],
+            ignore_index=True,
+        )
+        df_coef.columns = ["feature", "coefficient"]
 
         # create a fake SKLL learner with these non-zero weights
         learner = self.create_fake_skll_learner(df_coef)
 
         # there's no OLS fit object in this case
         fit = None
 
@@ -908,37 +909,34 @@
         X = df_train[feature_columns]
 
         # add the intercept
         X = sm.add_constant(X)
 
         # define the weights as inverse proportion of total
         # number of data points for each score
-        score_level_dict = df_train['sc1'].value_counts()
+        score_level_dict = df_train["sc1"].value_counts()
         expected_proportion = 1 / len(score_level_dict)
-        score_weights_dict = {sc1: expected_proportion / count
-                              for sc1, count in score_level_dict.items()}
-        weights = [score_weights_dict[sc1] for sc1 in df_train['sc1']]
+        score_weights_dict = {
+            sc1: expected_proportion / count for sc1, count in score_level_dict.items()
+        }
+        weights = [score_weights_dict[sc1] for sc1 in df_train["sc1"]]
 
         # fit the model
-        fit = sm.WLS(df_train['sc1'], X, weights=weights).fit()
+        fit = sm.WLS(df_train["sc1"], X, weights=weights).fit()
         df_coef = self.ols_coefficients_to_dataframe(fit.params)
         learner = self.create_fake_skll_learner(df_coef)
 
         # we used all the features
         used_features = feature_columns
 
         return learner, fit, df_coef, used_features
 
-    def train_builtin_model(self,
-                            model_name,
-                            df_train,
-                            experiment_id,
-                            filedir,
-                            figdir,
-                            file_format='csv'):
+    def train_builtin_model(
+        self, model_name, df_train, experiment_id, filedir, figdir, file_format="csv"
+    ):
         """
         Train one of the :ref:`built-in linear regression models <builtin_models>`.
 
         Parameters
         ----------
         model_name : str
             Name of the built-in model to train.
@@ -956,121 +954,123 @@
         file_format : str, optional
             The format in which to save files. One of {"csv", "tsv", "xlsx"}.
             Defaults to "csv".
 
         Returns
         -------
         learner : skll.learner.Learner
-            SKLL ``LinearRegression`` `Learner <https://skll.readthedocs.io/en/latest/api/learner.html#skll.learner.Learner>`_
-            object containing the coefficients learned by training
-            the built-in model.
+            SKLL ``LinearRegression`` Learner object containing the coefficients
+            learned by training the built-in model.
         """
         # get the columns that actually contain the feature values
-        feature_columns = [c for c in df_train.columns if c not in ['spkitemid', 'sc1']]
+        feature_columns = [c for c in df_train.columns if c not in ["spkitemid", "sc1"]]
 
         # LinearRegression
-        if model_name == 'LinearRegression':
+        if model_name == "LinearRegression":
             result = self.train_linear_regression(df_train, feature_columns)
 
         # EqualWeightsLR
-        elif model_name == 'EqualWeightsLR':
+        elif model_name == "EqualWeightsLR":
             result = self.train_equal_weights_lr(df_train, feature_columns)
 
         # RebalancedLR
-        elif model_name == 'RebalancedLR':
+        elif model_name == "RebalancedLR":
             result = self.train_rebalanced_lr(df_train, feature_columns)
 
         # LassoFixedLambdaThenLR
-        elif model_name == 'LassoFixedLambdaThenLR':
+        elif model_name == "LassoFixedLambdaThenLR":
             result = self.train_lasso_fixed_lambda_then_lr(df_train, feature_columns)
 
         # PositiveLassoCVThenLR
-        elif model_name == 'PositiveLassoCVThenLR':
+        elif model_name == "PositiveLassoCVThenLR":
             result = self.train_positive_lasso_cv_then_lr(df_train, feature_columns)
 
         # NNLR
-        elif model_name == 'NNLR':
+        elif model_name == "NNLR":
             result = self.train_non_negative_lr(df_train, feature_columns)
 
         # NNLRIterative
-        elif model_name == 'NNLRIterative':
+        elif model_name == "NNLRIterative":
             result = self.train_non_negative_lr_iterative(df_train, feature_columns)
 
         # LassoFixedLambdaThenNNLR
-        elif model_name == 'LassoFixedLambdaThenNNLR':
+        elif model_name == "LassoFixedLambdaThenNNLR":
             result = self.train_lasso_fixed_lambda_then_non_negative_lr(df_train, feature_columns)
 
         # LassoFixedLambda
-        elif model_name == 'LassoFixedLambda':
+        elif model_name == "LassoFixedLambda":
             result = self.train_lasso_fixed_lambda(df_train, feature_columns)
 
         # PositiveLassoCV
-        elif model_name == 'PositiveLassoCV':
+        elif model_name == "PositiveLassoCV":
             result = self.train_positive_lasso_cv(df_train, feature_columns)
 
         # ScoreWeightedLR
-        elif model_name == 'ScoreWeightedLR':
+        elif model_name == "ScoreWeightedLR":
             result = self.train_score_weighted_lr(df_train, feature_columns)
 
         writer = DataWriter(experiment_id)
         frames = []
 
         # unpack all results
         learner, fit, df_coef, used_features = result
 
         # add raw coefficients to frame list
-        frames.append({'name': 'coefficients', 'frame': df_coef})
+        frames.append({"name": "coefficients", "frame": df_coef})
 
         # compute the standardized and relative coefficients (betas) for the
         # non-intercept features and save to a file
-        df_betas = df_coef.set_index('feature').loc[used_features]
-        df_betas = df_betas.multiply(df_train[used_features].std(),
-                                     axis='index') / df_train['sc1'].std()
-        df_betas.columns = ['standardized']
-        df_betas['relative'] = df_betas / sum(abs(df_betas['standardized']))
+        df_betas = df_coef.set_index("feature").loc[used_features]
+        df_betas = (
+            df_betas.multiply(df_train[used_features].std(), axis="index") / df_train["sc1"].std()
+        )
+        df_betas.columns = ["standardized"]
+        df_betas["relative"] = df_betas / sum(abs(df_betas["standardized"]))
         df_betas.reset_index(inplace=True)
 
         # add betas to frame list
-        frames.append({'name': 'betas', 'frame': df_betas})
+        frames.append({"name": "betas", "frame": df_betas})
 
         # save the OLS fit object and its summary to files
         if fit:
-            ols_file = join(filedir, '{}.ols'.format(experiment_id))
-            summary_file = join(filedir, '{}_ols_summary.txt'.format(experiment_id))
-            with open(ols_file, 'wb') as olsf, open(summary_file, 'w') as summf:
+            ols_file = join(filedir, f"{experiment_id}.ols")
+            summary_file = join(filedir, f"{experiment_id}_ols_summary.txt")
+            with open(ols_file, "wb") as olsf, open(summary_file, "w") as summf:
                 pickle.dump(fit, olsf)
                 summf.write(str(fit.summary()))
 
             # create a data frame with main model fit metrics and save to the file
             df_model_fit = self.model_fit_to_dataframe(fit)
 
             # add model_fit to frame list
-            frames.append({'name': 'model_fit', 'frame': df_model_fit})
+            frames.append({"name": "model_fit", "frame": df_model_fit})
 
         # save the SKLL model to a file
-        model_file = join(filedir, '{}.model'.format(experiment_id))
+        model_file = join(filedir, f"{experiment_id}.model")
         learner.save(model_file)
 
         container = DataContainer(frames)
         writer.write_experiment_output(filedir, container, file_format=file_format)
 
         self.learner = learner
 
         return learner
 
-    def train_skll_model(self,
-                         model_name,
-                         df_train,
-                         experiment_id,
-                         filedir,
-                         figdir,
-                         file_format='csv',
-                         custom_fixed_parameters=None,
-                         custom_objective=None,
-                         predict_expected_scores=False):
+    def train_skll_model(
+        self,
+        model_name,
+        df_train,
+        experiment_id,
+        filedir,
+        figdir,
+        file_format="csv",
+        custom_fixed_parameters=None,
+        custom_objective=None,
+        predict_expected_scores=False,
+    ):
         """
         Train a SKLL classification or regression model.
 
         Parameters
         ----------
         model_name : str
             Name of the SKLL model to train.
@@ -1106,55 +1106,50 @@
         learner_and_objective : tuple
             A 2-tuple containing a SKLL Learner object of the appropriate type
             and the chosen tuning objective.
         """
         # Instantiate the given SKLL learner and set its probability value
         # and fixed parameters appropriately
         model_kwargs = custom_fixed_parameters if custom_fixed_parameters is not None else {}
-        learner = Learner(model_name,
-                          model_kwargs=model_kwargs,
-                          probability=predict_expected_scores)
+        learner = Learner(
+            model_name, model_kwargs=model_kwargs, probability=predict_expected_scores
+        )
 
         # get the features, IDs, and labels from the given data frame
-        feature_columns = [c for c in df_train.columns if c not in ['spkitemid', 'sc1']]
-        features = df_train[feature_columns].to_dict(orient='records')
-        ids = df_train['spkitemid'].tolist()
-        labels = df_train['sc1'].tolist()
+        feature_columns = [c for c in df_train.columns if c not in ["spkitemid", "sc1"]]
+        features = df_train[feature_columns].to_dict(orient="records")
+        ids = df_train["spkitemid"].tolist()
+        labels = df_train["sc1"].tolist()
 
         # create a FeatureSet and train the model
-        fs = FeatureSet('train', ids=ids, labels=labels, features=features)
+        fs = FeatureSet("train", ids=ids, labels=labels, features=features)
 
         # If we are training a SKLL regressor, then we want to use either the
         # user-specified objective or `neg_mean_squared_error`. If it's SKLL
         # classifier, then the choice is between the user-specified objective
         # and `f1_score_micro`.
-        if learner.model_type._estimator_type == 'regressor':
-            objective = 'neg_mean_squared_error' if not custom_objective else custom_objective
+        if learner.model_type._estimator_type == "regressor":
+            objective = "neg_mean_squared_error" if not custom_objective else custom_objective
         else:
-            objective = 'f1_score_micro' if not custom_objective else custom_objective
+            objective = "f1_score_micro" if not custom_objective else custom_objective
 
         learner.train(fs, grid_search=True, grid_objective=objective, grid_jobs=1)
 
         # TODO: compute betas for linear SKLL models?
 
         # save the SKLL model to disk with the given model name prefix
-        model_file = join(filedir, '{}.model'.format(experiment_id))
+        model_file = join(filedir, f"{experiment_id}.model")
         learner.save(model_file)
 
         self.learner = learner
 
         # return the SKLL learner object and the chosen objective
         return learner, objective
 
-    def train(self,
-              configuration,
-              data_container,
-              filedir,
-              figdir,
-              file_format='csv'):
+    def train(self, configuration, data_container, filedir, figdir, file_format="csv"):
         """
         Train the given model on the given data and save the results.
 
         The main driver function to train the given model on the given
         data and save the results in the given directories using the
         given experiment ID as the prefix.
 
@@ -1174,108 +1169,124 @@
             The format in which to save files. One of {"csv", "tsv", "xlsx"}.
             Defaults to "csv".
 
         Returns
         -------
         name : SKLL Learner object
         """
-        Analyzer.check_param_names(configuration, ['model_name', 'experiment_id'])
-        Analyzer.check_frame_names(data_container, ['train_preprocessed_features'])
+        Analyzer.check_param_names(configuration, ["model_name", "experiment_id"])
+        Analyzer.check_frame_names(data_container, ["train_preprocessed_features"])
 
-        model_name = configuration['model_name']
-        experiment_id = configuration['experiment_id']
+        model_name = configuration["model_name"]
+        experiment_id = configuration["experiment_id"]
 
-        df_train = data_container['train_preprocessed_features']
+        df_train = data_container["train_preprocessed_features"]
 
         args = [model_name, df_train, experiment_id, filedir, figdir]
-        kwargs = {'file_format': file_format}
+        kwargs = {"file_format": file_format}
 
         # add user-specified SKLL objective to the arguments if we are
         # training a SKLL model
         if is_skll_model(model_name):
-            kwargs.update({'custom_fixed_parameters': configuration['skll_fixed_parameters'],
-                           'custom_objective': configuration['skll_objective'],
-                           'predict_expected_scores': configuration['predict_expected_scores']})
+            kwargs.update(
+                {
+                    "custom_fixed_parameters": configuration["skll_fixed_parameters"],
+                    "custom_objective": configuration["skll_objective"],
+                    "predict_expected_scores": configuration["predict_expected_scores"],
+                }
+            )
             model, chosen_objective = self.train_skll_model(*args, **kwargs)
-            configuration['skll_objective'] = chosen_objective
+            configuration["skll_objective"] = chosen_objective
         else:
             model = self.train_builtin_model(*args, **kwargs)
 
         return model
 
-    def predict(self, df, min_score, max_score, predict_expected=False):
+    def predict(self, df, min_score=None, max_score=None, predict_expected=False):
         """
         Get raw predictions from given SKLL model on data in given data frame.
 
         Parameters
         ----------
         df : pandas DataFrame
             Data frame containing features on which to make the predictions.
             The data must contain pre-processed feature values, an ID column
             named "spkitemid", and a label column named "sc1".
-        min_score : int
+        min_score : int, optional
             Minimum score level to be used if computing expected scores.
-        max_score : int
+            If ``None``, trying to compute expected scores will raise an
+            exception.
+            Defaults to ``None``.
+        max_score : int, optional
             Maximum score level to be used if computing expected scores.
+            If ``None``, trying to compute expected scores will raise an
+            exception.
+            Defaults to ``None``.
         predict_expected : bool, optional
             Predict expected scores for classifiers that return probability
             distributions over score. This will be ignored with a warning
             if the specified model does not support probability distributions.
             Note also that this assumes that the score range consists of
             contiguous integers - starting at ``min_score`` and ending at
-            ``max_score``. Defaults to ``False``.
+            ``max_score``.
+            Defaults to ``False``.
 
         Returns
         -------
         df_predictions : pandas DataFrame
             Data frame containing the raw predictions, the IDs, and the
             human scores.
 
         Raises
         ------
         ValueError
             If the model cannot predict probability distributions and
             ``predict_expected`` is set to ``True``.
         ValueError
-            If  the score range specified by ``min_score`` and ``max_score``
+            If the score range specified by ``min_score`` and ``max_score``
             does not match what the model predicts in its probability
             distribution.
+        ValueError
+            If ``predict_expected`` is ``True`` but ``min_score`` and
+            ``max_score`` are not specified.
         """
+        # expected scores require specifying ``trim_min`` and ``trim_max``
+        if predict_expected and not (min_score and max_score):
+            raise ValueError("Must specify 'min_score' and 'max_score' for expected scores.")
+
         model = self.learner
 
-        feature_columns = [c for c in df.columns if c not in ['spkitemid', 'sc1']]
-        features = df[feature_columns].to_dict(orient='records')
-        ids = df['spkitemid'].tolist()
+        feature_columns = [c for c in df.columns if c not in ["spkitemid", "sc1"]]
+        features = df[feature_columns].to_dict(orient="records")
+        ids = df["spkitemid"].tolist()
 
         # if we have the labels, save them in the featureset
         labels = None
-        if 'sc1' in df:
-            labels = df['sc1'].tolist()
+        if "sc1" in df:
+            labels = df["sc1"].tolist()
 
-        fs = FeatureSet('data', ids=ids, labels=labels, features=features)
+        fs = FeatureSet("data", ids=ids, labels=labels, features=features)
         # if we are predicting expected scores, then call a different function
-        predictions = compute_expected_scores_from_model(model,
-                                                         fs,
-                                                         min_score,
-                                                         max_score) if predict_expected else model.predict(fs)
+        predictions = (
+            compute_expected_scores_from_model(model, fs, min_score, max_score)
+            if predict_expected
+            else model.predict(fs)
+        )
 
         df_predictions = pd.DataFrame()
-        df_predictions['spkitemid'] = ids
-        df_predictions['raw'] = predictions
+        df_predictions["spkitemid"] = ids
+        df_predictions["raw"] = predictions
 
         # save the labels in the dataframe if they existed in the first place
         if labels:
-            df_predictions['sc1'] = labels
+            df_predictions["sc1"] = labels
 
         return df_predictions
 
-    def predict_train_and_test(self,
-                               df_train,
-                               df_test,
-                               configuration):
+    def predict_train_and_test(self, df_train, df_test, configuration):
         """
         Generate raw, scaled, and trimmed predictions on given data.
 
         Parameters
         ----------
         df_train : pandas DataFrame
             Data frame containing the pre-processed training
@@ -1288,79 +1299,97 @@
             and "trim_min" keys.
 
         Returns
         -------
         List of data frames containing predictions and other
         information.
         """
-        Analyzer.check_param_names(configuration, ['trim_max',
-                                                   'trim_min',
-                                                   'trim_tolerance'])
-
-        (trim_min,
-         trim_max,
-         trim_tolerance) = configuration.get_trim_min_max_tolerance()
-
-        predict_expected_scores = configuration['predict_expected_scores']
-
-        df_train_predictions = self.predict(df_train,
-                                            int(trim_min),
-                                            int(trim_max),
-                                            predict_expected=predict_expected_scores)
-        df_test_predictions = self.predict(df_test,
-                                           int(trim_min),
-                                           int(trim_max),
-                                           predict_expected=predict_expected_scores)
+        Analyzer.check_param_names(configuration, ["trim_max", "trim_min", "trim_tolerance"])
+
+        (
+            trim_min,
+            trim_max,
+            trim_tolerance,
+        ) = configuration.get_trim_min_max_tolerance()
+
+        predict_expected_scores = configuration["predict_expected_scores"]
+
+        df_train_predictions = self.predict(
+            df_train,
+            min_score=int(trim_min),
+            max_score=int(trim_max),
+            predict_expected=predict_expected_scores,
+        )
+        df_test_predictions = self.predict(
+            df_test,
+            min_score=int(trim_min),
+            max_score=int(trim_max),
+            predict_expected=predict_expected_scores,
+        )
 
         # get the mean and SD of the training set predictions
-        train_predictions_mean = df_train_predictions['raw'].mean()
-        train_predictions_sd = df_train_predictions['raw'].std()
+        train_predictions_mean = df_train_predictions["raw"].mean()
+        train_predictions_sd = df_train_predictions["raw"].std()
 
         # get the mean and SD of the human labels
-        human_labels_mean = df_train['sc1'].mean()
-        human_labels_sd = df_train['sc1'].std()
+        human_labels_mean = df_train["sc1"].mean()
+        human_labels_sd = df_train["sc1"].std()
 
-        self.logger.info('Processing train set predictions.')
+        self.logger.info("Processing train set predictions.")
         feature_preprocessor = FeaturePreprocessor()
-        df_train_predictions = feature_preprocessor.process_predictions(df_train_predictions,
-                                                                        train_predictions_mean,
-                                                                        train_predictions_sd,
-                                                                        human_labels_mean,
-                                                                        human_labels_sd,
-                                                                        trim_min,
-                                                                        trim_max,
-                                                                        trim_tolerance)
-
-        self.logger.info('Processing test set predictions.')
-        df_test_predictions = feature_preprocessor.process_predictions(df_test_predictions,
-                                                                       train_predictions_mean,
-                                                                       train_predictions_sd,
-                                                                       human_labels_mean,
-                                                                       human_labels_sd,
-                                                                       trim_min,
-                                                                       trim_max,
-                                                                       trim_tolerance)
-
-        df_postproc_params = pd.DataFrame([{'trim_min': trim_min,
-                                            'trim_max': trim_max,
-                                            'trim_tolerance': trim_tolerance,
-                                            'h1_mean': human_labels_mean,
-                                            'h1_sd': human_labels_sd,
-                                            'train_predictions_mean': train_predictions_mean,
-                                            'train_predictions_sd': train_predictions_sd}])
-
-        datasets = [{'name': 'pred_train', 'frame': df_train_predictions},
-                    {'name': 'pred_test', 'frame': df_test_predictions},
-                    {'name': 'postprocessing_params', 'frame': df_postproc_params}]
+        df_train_predictions = feature_preprocessor.process_predictions(
+            df_train_predictions,
+            train_predictions_mean,
+            train_predictions_sd,
+            human_labels_mean,
+            human_labels_sd,
+            trim_min,
+            trim_max,
+            trim_tolerance,
+        )
+
+        self.logger.info("Processing test set predictions.")
+        df_test_predictions = feature_preprocessor.process_predictions(
+            df_test_predictions,
+            train_predictions_mean,
+            train_predictions_sd,
+            human_labels_mean,
+            human_labels_sd,
+            trim_min,
+            trim_max,
+            trim_tolerance,
+        )
+
+        df_postproc_params = pd.DataFrame(
+            [
+                {
+                    "trim_min": trim_min,
+                    "trim_max": trim_max,
+                    "trim_tolerance": trim_tolerance,
+                    "h1_mean": human_labels_mean,
+                    "h1_sd": human_labels_sd,
+                    "train_predictions_mean": train_predictions_mean,
+                    "train_predictions_sd": train_predictions_sd,
+                }
+            ]
+        )
+
+        datasets = [
+            {"name": "pred_train", "frame": df_train_predictions},
+            {"name": "pred_test", "frame": df_test_predictions},
+            {"name": "postprocessing_params", "frame": df_postproc_params},
+        ]
 
         # configuration options that are entirely for internal use
-        internal_options_dict = {'train_predictions_mean': train_predictions_mean,
-                                 'train_predictions_sd': train_predictions_sd,
-                                 'human_labels_mean': human_labels_mean,
-                                 'human_labels_sd': human_labels_sd}
+        internal_options_dict = {
+            "train_predictions_mean": train_predictions_mean,
+            "train_predictions_sd": train_predictions_sd,
+            "human_labels_mean": human_labels_mean,
+            "human_labels_sd": human_labels_sd,
+        }
 
         new_configuration = configuration.copy()
         for key, value in internal_options_dict.items():
             new_configuration[key] = value
 
         return new_configuration, DataContainer(datasets=datasets)
 
@@ -1426,21 +1455,22 @@
 
         Raises
         ------
         RuntimeError
             If the model is non-linear and no coefficients
             are available.
         """
-        Analyzer.check_param_names(configuration, ['train_predictions_mean',
-                                                   'train_predictions_sd',
-                                                   'human_labels_sd'])
-
-        train_predictions_mean = configuration['train_predictions_mean']
-        train_predictions_sd = configuration['train_predictions_sd']
-        h1_sd = configuration['human_labels_sd']
+        Analyzer.check_param_names(
+            configuration,
+            ["train_predictions_mean", "train_predictions_sd", "human_labels_sd"],
+        )
+
+        train_predictions_mean = configuration["train_predictions_mean"]
+        train_predictions_sd = configuration["train_predictions_sd"]
+        h1_sd = configuration["human_labels_sd"]
 
         feature_names = self.get_feature_names()
 
         # try to get the model coefficients, if available
         try:
             coefficients = self.get_coefficients()
         except AttributeError:
@@ -1452,19 +1482,22 @@
         scaled_coefficients = coefficients * h1_sd / train_predictions_sd
 
         # adjust the intercept to set the mean predicted score
         # to the mean of the training variable
         new_intercept = intercept * (h1_sd / train_predictions_sd)
         new_intercept += train_predictions_mean * (1 - h1_sd / train_predictions_sd)
 
-        intercept_and_feature_names = ['Intercept'] + feature_names
+        intercept_and_feature_names = ["Intercept"] + feature_names
         intercept_and_feature_values = [new_intercept] + list(scaled_coefficients)
 
         # create a data frame with new values
-        df_scaled_coefficients = pd.DataFrame({'feature': intercept_and_feature_names,
-                                               'coefficient': intercept_and_feature_values},
-                                              columns=['feature', 'coefficient'])
+        df_scaled_coefficients = pd.DataFrame(
+            {
+                "feature": intercept_and_feature_names,
+                "coefficient": intercept_and_feature_values,
+            },
+            columns=["feature", "coefficient"],
+        )
 
-        scaled_dataset = [{'name': 'coefficients_scaled',
-                           'frame': df_scaled_coefficients}]
+        scaled_dataset = [{"name": "coefficients_scaled", "frame": df_scaled_coefficients}]
 
         return DataContainer(datasets=scaled_dataset)
```

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/builtin_model.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/builtin_model.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/consistency.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/consistency.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/evaluation.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/feature_descriptives.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/feature_descriptives.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/features_by_group.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/features_by_group.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/footer.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/footer.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/header.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/header.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/model.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/model.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/notes.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/notes.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/pca.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/pca.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/preprocessed_features.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/preprocessed_features.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/preprocessed_features_by_group.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/preprocessed_features_by_group.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/score_distributions.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/score_distributions.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/sysinfo.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/sysinfo.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/comparison/true_score_evaluation.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/comparison/true_score_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/consistency.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/consistency.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/data_description.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/data_description.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/data_description_by_group.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/data_description_by_group.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/dff_by_group.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/dff_by_group.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/evaluation.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/evaluation_by_group.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/evaluation_by_group.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/fairness_analyses.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/fairness_analyses.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/feature_descriptives.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/feature_descriptives.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/features_by_group.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/features_by_group.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/footer.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/footer.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/header.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/header.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/intermediate_file_paths.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/intermediate_file_paths.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/javascript/sort.js` & `rsmtool-9.1.1/rsmtool/notebooks/javascript/sort.js`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/pca.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/pca.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/preprocessed_features.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/preprocessed_features.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/skll_model.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/skll_model.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/summary/evaluation.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/summary/evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/summary/footer.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/summary/footer.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/summary/header.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/summary/header.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/summary/intermediate_file_paths.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/summary/intermediate_file_paths.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/summary/model.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/summary/model.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/summary/preprocessed_features.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/summary/preprocessed_features.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/summary/sysinfo.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/summary/sysinfo.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/summary/true_score_evaluation.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/summary/true_score_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/sysinfo.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/sysinfo.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/notebooks/true_score_evaluation.ipynb` & `rsmtool-9.1.1/rsmtool/notebooks/true_score_evaluation.ipynb`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/preprocessor.py` & `rsmtool-9.1.1/rsmtool/preprocessor.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from .utils.models import is_built_in_model, is_skll_model
 
 
 class FeatureSubsetProcessor:
     """Class to encapsulate feature sub-setting methods."""
 
     def __init__(self, logger=None):
+        """Initialize the FeatureSubsetProcessor object."""
         self.logger = logger if logger else logging.getLogger(__name__)
 
     def select_by_subset(self, feature_columns, feature_subset_specs, subset):
         """
         Select feature columns using feature subset specifications.
 
         Parameters
@@ -43,34 +44,35 @@
             The column to subset.
 
         Returns
         -------
         feature_names : list of str
             A list of feature names to include.
         """
-        feature_subset = feature_subset_specs[feature_subset_specs[subset] == 1]['Feature']
-        feature_names = [feature for feature in feature_columns
-                         if feature in feature_subset.values]
+        feature_subset = feature_subset_specs[feature_subset_specs[subset] == 1]["Feature"]
+        feature_names = [feature for feature in feature_columns if feature in feature_subset.values]
 
         # check whether there are any features in the data file and raise warning
         if len(feature_columns) != len(feature_names):
-            feature_subset_specs_set = set(feature_subset_specs['Feature'])
+            feature_subset_specs_set = set(feature_subset_specs["Feature"])
             extra_columns = set(feature_columns).difference(feature_subset_specs_set)
             if extra_columns:
-                self.logger.warning("No subset information was available for the "
-                                    "following columns in the input file. These "
-                                    "columns will not be used in the model: "
-                                    "{}".format(', '.join(extra_columns)))
+                self.logger.warning(
+                    f"No subset information was available for the following "
+                    f"columns in the input file. These columns will not be "
+                    f"used in the model: {', '.join(extra_columns)}"
+                )
         if len(feature_subset) != len(feature_names):
             extra_subset_features = set(feature_subset).difference(set(feature_names))
             if extra_subset_features:
-                self.logger.warning("The following features were included into the {} "
-                                    "subset in the feature_subset_file but were not "
-                                    "specified in the input data: "
-                                    "{}".format(subset, ', '.join(extra_subset_features)))
+                self.logger.warning(
+                    f"The following features were included into the {subset} "
+                    f"subset in the feature_subset_file but were not specified "
+                    f"in the input data: {', '.join(extra_subset_features)}"
+                )
         return feature_names
 
     def check_feature_subset_file(self, df, subset=None, sign=None):
         """
         Check that feature subset file is complete and in the correct format.
 
         Raises an exception if it finds any errors but otherwise
@@ -94,52 +96,52 @@
         ValueError
             If any of the columns contain invalid values.
         """
         # we want to allow title-cased names of columns for historical reasons
         # e.g., `Feature` instead of `feature` etc.
         df_feature_specs = df.copy()
 
-        if ('feature' not in df_feature_specs and
-                'Feature' not in df_feature_specs):
-            raise ValueError("The feature_subset_file must contain "
-                             "a column named 'feature' "
-                             "containing the feature names.")
+        if "feature" not in df_feature_specs and "Feature" not in df_feature_specs:
+            raise ValueError(
+                "The feature_subset_file must contain "
+                "a column named 'feature' "
+                "containing the feature names."
+            )
         if subset:
             if subset not in df_feature_specs:
-                raise ValueError("Unknown value for feature_subset: {}".format(subset))
+                raise ValueError(f"Unknown value for feature_subset: {subset}")
 
             if not df_feature_specs[subset].isin([0, 1]).all():
-                raise ValueError("The subset columns in feature "
-                                 "file can only contain 0 or 1")
+                raise ValueError("The subset columns in feature " "file can only contain 0 or 1")
 
         if sign:
-            possible_sign_columns = ['sign_{}'.format(sign),
-                                     'Sign_{}'.format(sign)]
-            existing_sign_columns = [c for c in possible_sign_columns
-                                     if c in df_feature_specs]
+            possible_sign_columns = [f"sign_{sign}", f"Sign_{sign}"]
+            existing_sign_columns = [c for c in possible_sign_columns if c in df_feature_specs]
             if len(existing_sign_columns) > 1:
-                raise ValueError("The feature_subset_file contains "
-                                 "multiple columns for sign: "
-                                 "{}".format(' ,'.join(existing_sign_columns)))
+                raise ValueError(
+                    f"The feature_subset_file contains multiple columns "
+                    f"for sign: {' ,'.join(existing_sign_columns)}"
+                )
             elif len(existing_sign_columns) == 0:
-                raise ValueError("The feature_subset_file must "
-                                 "contain the requested "
-                                 "sign column 'sign_{}'".format(sign))
+                raise ValueError(
+                    f"The feature_subset_file must contain the requested "
+                    f"sign column 'sign_{sign}'"
+                )
             else:
                 sign_column = existing_sign_columns[0]
 
-            if not df_feature_specs[sign_column].isin(['-', '+']).all():
-                raise ValueError("The sign columns in feature "
-                                 "file can only contain - or +")
+            if not df_feature_specs[sign_column].isin(["-", "+"]).all():
+                raise ValueError("The sign columns in feature " "file can only contain - or +")
 
 
 class FeatureSpecsProcessor:
     """Encapsulate feature file processing methods."""
 
     def __init__(self, logger=None):
+        """Initialize the FeatureSpecsProcessor object."""
         self.logger = logger if logger else logging.getLogger(__name__)
 
     def generate_default_specs(self, feature_names):
         """
         Generate default feature "specifications" for given feature names.
 
         The specifications are stored as a data frame with three columns
@@ -158,17 +160,17 @@
 
         Note
         ----
         Since these are default specifications, the values for the
         "transform" column for each feature will be "raw" and the
         value for the "sign" column will be ``1``.
         """
-        df_feature_specs = pd.DataFrame({'feature': feature_names})
-        df_feature_specs['transform'] = 'raw'
-        df_feature_specs['sign'] = 1.0
+        df_feature_specs = pd.DataFrame({"feature": feature_names})
+        df_feature_specs["transform"] = "raw"
+        df_feature_specs["sign"] = 1.0
         return df_feature_specs
 
     def find_feature_sign(self, feature, sign_dict):
         """
         Get the feature sign from the feature CSV file.
 
         Parameters
@@ -180,21 +182,23 @@
 
         Returns
         -------
         feature_sign_numeric : float
             The signed feature.
         """
         if feature not in sign_dict.keys():
-            self.logger.warning("No information about sign is available "
-                                "for feature {}. The feature will be assigned "
-                                "the default positive weight.".format(feature))
+            self.logger.warning(
+                f"No information about sign is available for feature "
+                f"{feature}. The feature will be assigned the default "
+                f"positive weight."
+            )
             feature_sign_numeric = 1.0
         else:
             feature_sign_string = sign_dict[feature]
-            feature_sign_numeric = -1.0 if feature_sign_string == '-' else 1.0
+            feature_sign_numeric = -1.0 if feature_sign_string == "-" else 1.0
         return feature_sign_numeric
 
     def validate_feature_specs(self, df, use_truncations=False):
         """
         Validate given feature specifications.
 
         Check given feature specifications to make sure that there are no duplicate
@@ -227,67 +231,67 @@
         ValueError
             If ``use_truncations`` is set to ``True``, and no
             "min" and "max" columns exist in the data set.
         """
         df_specs_org = df
         df_specs_new = df_specs_org.copy()
 
-        expected_columns = ['feature', 'sign', 'transform']
+        expected_columns = ["feature", "sign", "transform"]
 
         # we allow internally the use of 'Feature' since
         # this is the column name in subset_feature_file.
-        if 'Feature' in df_specs_org:
-            df_specs_new['feature'] = df_specs_org['Feature']
+        if "Feature" in df_specs_org:
+            df_specs_new["feature"] = df_specs_org["Feature"]
 
         # check that we have a column named `feature`
-        if 'feature' not in df_specs_new:
-            raise KeyError("The feature file must contain a "
-                           "column named 'feature'")
+        if "feature" not in df_specs_new:
+            raise KeyError("The feature file must contain a " "column named 'feature'")
 
         # check to make sure that there are no duplicate feature names
-        feature_name_count = df_specs_new['feature'].value_counts()
+        feature_name_count = df_specs_new["feature"].value_counts()
         duplicate_features = feature_name_count[feature_name_count > 1]
         if len(duplicate_features) > 0:
-            raise ValueError("The following feature names "
-                             " are duplicated in the feature "
-                             "file: {}".format(duplicate_features.index))
+            raise ValueError(
+                f"The following feature names are duplicated in "
+                f"the feature file: {duplicate_features.index}"
+            )
 
         # if we have `sign` column, check that it can be converted to float
-        if 'sign' in df_specs_new:
+        if "sign" in df_specs_new:
             try:
-                df_specs_new['sign'] = df_specs_new['sign'].astype(float)
-                assert np.all(df_specs_new['sign'].isin([-1, 1]))
+                df_specs_new["sign"] = df_specs_new["sign"].astype(float)
+                assert np.all(df_specs_new["sign"].isin([-1, 1]))
             except (ValueError, AssertionError):
-                raise ValueError("The `sign` column in the feature"
-                                 "file can only contain '1' or '-1'")
+                raise ValueError(
+                    "The `sign` column in the feature" "file can only contain '1' or '-1'"
+                )
         else:
-            df_specs_new['sign'] = 1
+            df_specs_new["sign"] = 1
 
-        if 'transform' not in df_specs_new:
-            df_specs_new['transform'] = 'raw'
+        if "transform" not in df_specs_new:
+            df_specs_new["transform"] = "raw"
 
         if use_truncations:
-            if not all(col in df_specs_new for col in ['min', 'max']):
-                raise ValueError('The ``use_truncation_thresholds`` configuration option '
-                                 'was specified, but no ``min`` or ``max`` columns exist '
-                                 'in the feature file.')
+            if not all(col in df_specs_new for col in ["min", "max"]):
+                raise ValueError(
+                    "The ``use_truncation_thresholds`` configuration option "
+                    "was specified, but no ``min`` or ``max`` columns exist "
+                    "in the feature file."
+                )
 
             # add ``min`` and ``max`` to the
             # list of expected columns
-            expected_columns.extend(['min', 'max'])
+            expected_columns.extend(["min", "max"])
 
         df_specs_new = df_specs_new[expected_columns]
         return df_specs_new
 
-    def generate_specs(self,
-                       df,
-                       feature_names,
-                       train_label,
-                       feature_subset=None,
-                       feature_sign=None):
+    def generate_specs(
+        self, df, feature_names, train_label, feature_subset=None, feature_sign=None
+    ):
         """
         Generate feature specifications using the feature CSV file.
 
         Compute the specifications for "sign" and the correlation with score
         to identify the best transformation.
 
         Parameters
@@ -309,45 +313,45 @@
         -------
         df_feature_specs : pandas DataFrame
             The output data frame containing the feature specifications.
         """
         # get feature sign information, if available
         if feature_sign:
             # Convert to dictionary {feature:sign}
-            sign_dict = dict(zip(feature_subset.Feature,
-                                 feature_subset['Sign_{}'.format(feature_sign)]))
+            sign_dict = dict(zip(feature_subset.Feature, feature_subset[f"Sign_{feature_sign}"]))
         # else create an empty dictionary
         else:
             sign_dict = {}
 
         feature_specs = []
         feature_dict = {}
         for feature in feature_names:
-            feature_dict['feature'] = feature
-            feature_dict['transform'] = FeatureTransformer().find_feature_transform(feature,
-                                                                                    df[feature],
-                                                                                    df[train_label])
+            feature_dict["feature"] = feature
+            feature_dict["transform"] = FeatureTransformer().find_feature_transform(
+                feature, df[feature], df[train_label]
+            )
 
-            feature_dict['sign'] = self.find_feature_sign(feature, sign_dict)
+            feature_dict["sign"] = self.find_feature_sign(feature, sign_dict)
 
             # Change the sign for inverse and addOneInv transformations
-            if feature_dict['transform'] in ['inv', 'addOneInv']:
-                feature_dict['sign'] = feature_dict['sign'] * -1
+            if feature_dict["transform"] in ["inv", "addOneInv"]:
+                feature_dict["sign"] = feature_dict["sign"] * -1
 
             feature_specs.append(feature_dict)
             feature_dict = {}
 
         df_feature_specs = pd.DataFrame(feature_specs)
         return df_feature_specs
 
 
 class FeaturePreprocessor:
     """Class to preprocess features in training and testing sets."""
 
     def __init__(self, logger=None):
+        """Initialize the FeaturePreprocessor object."""
         self.logger = logger if logger else logging.getLogger(__name__)
 
     def check_model_name(self, model_name):
         """
         Check that the given model name is valid and determine its type.
 
         Parameters
@@ -362,29 +366,25 @@
 
         Raises
         ------
         ValueError
             If the model is not supported.
         """
         if is_built_in_model(model_name):
-            model_type = 'BUILTIN'
+            model_type = "BUILTIN"
         elif is_skll_model(model_name):
-            model_type = 'SKLL'
+            model_type = "SKLL"
         else:
-            raise ValueError("The specified model {} "
-                             "was not found. Please "
-                             "check the spelling.".format(model_name))
+            raise ValueError(
+                f"The specified model {model_name} was not found. " f"Please check the spelling."
+            )
 
         return model_type
 
-    def trim(self,
-             values,
-             trim_min,
-             trim_max,
-             tolerance=0.4998):
+    def trim(self, values, trim_min, trim_max, tolerance=0.4998):
         """
         Trim values in given numpy array.
 
         The trimming uses ``trim_min`` - ``tolerance`` as the floor and
         ``trim_max`` + ``tolerance`` as the ceiling.
 
         Parameters
@@ -414,18 +414,15 @@
         new_min = trim_min - tolerance
         trimmed_values = values.copy()
         trimmed_values[trimmed_values > new_max] = new_max
         trimmed_values[trimmed_values < new_min] = new_min
         return trimmed_values
 
     @staticmethod
-    def remove_outliers(values,
-                        mean=None,
-                        sd=None,
-                        sd_multiplier=4):  # noqa: D301
+    def remove_outliers(values, mean=None, sd=None, sd_multiplier=4):  # noqa: D301
         """
         Remove outliers from given array of values by clamping them.
 
         Clamp any given values that are
         ± ``sd_multiplier`` (:math:`m`) standard deviations (:math:`\\sigma`)
         away from the mean (:math:`\\mu`). Use given ``mean`` and ``sd``
         instead of computing :math:`\\sigma` and :math:`\\mu`, if specified.
@@ -468,18 +465,15 @@
         floor = mean - sd_multiplier * sd
         ceiling = mean + sd_multiplier * sd
 
         new_values[new_values > ceiling] = ceiling
         new_values[new_values < floor] = floor
         return new_values
 
-    def remove_outliers_using_truncations(self,
-                                          values,
-                                          feature_name,
-                                          truncations):
+    def remove_outliers_using_truncations(self, values, feature_name, truncations):
         """
         Remove outliers using pre-specified truncation groups.
 
         This is different from ``remove_outliers()`` which calculates the
         outliers based on the training set.
 
         Parameters
@@ -497,25 +491,22 @@
         -------
         new_values : numpy array
             Numpy array with the outliers clamped.
         """
         # convert data to a numpy float array before doing any clamping
         new_values = np.array(values, dtype=np.float64)
 
-        minimum = truncations.loc[feature_name, 'min']
-        maximum = truncations.loc[feature_name, 'max']
+        minimum = truncations.loc[feature_name, "min"]
+        maximum = truncations.loc[feature_name, "max"]
 
         new_values[new_values > maximum] = maximum
         new_values[new_values < minimum] = minimum
         return new_values
 
-    def select_candidates(self,
-                          df,
-                          N,
-                          candidate_col='candidate'):
+    def select_candidates(self, df, N, candidate_col="candidate"):
         """
         Select candidates which have responses to N or more items.
 
         Parameters
         ----------
         df : pandas DataFrame
             The data frame from which to select candidates with N or more items.
@@ -542,16 +533,15 @@
         df_included = df[df[candidate_col].isin(selected_candidates)].copy()
         df_excluded = df[~df[candidate_col].isin(selected_candidates)].copy()
 
         # reset indices
         df_included.reset_index(drop=True, inplace=True)
         df_excluded.reset_index(drop=True, inplace=True)
 
-        return (df_included,
-                df_excluded)
+        return (df_included, df_excluded)
 
     def check_subgroups(self, df, subgroups):
         """
         Validate subgroup names in the given data.
 
         Check that all subgroups, if specified, correspond to columns in the
         provided data frame, and replace all NaNs in subgroups values with
@@ -574,39 +564,39 @@
         Raises
         ------
         KeyError
             If the data does not contain columns for all specified subgroups.
         """
         missing_sub_cols = set(subgroups).difference(df.columns)
         if missing_sub_cols:
-            raise KeyError("The data does not contain columns "
-                           "for all subgroups specified in the "
-                           "configuration file. Please check for "
-                           "capitalization and other spelling "
-                           "errors and make sure the subgroup "
-                           "names do not contain hyphens. "
-                           "The data does not have columns "
-                           "for the following "
-                           "subgroups: {}".format(', '.join(missing_sub_cols)))
+            raise KeyError(
+                f"The data does not contain columns for all subgroups "
+                f"specified in the configuration file. Please check "
+                f"for capitalization and other spelling errors and make "
+                f"sure the subgroup names do not contain hyphens. The "
+                f"data does not have columns for the following "
+                f"subgroups: {', '.join(missing_sub_cols)}"
+            )
 
         # replace any empty values in subgroups values by "No info"
         empty_value = re.compile(r"^\s*$")
-        df[subgroups] = df[subgroups].replace(to_replace=empty_value,
-                                              value='No info')
+        df[subgroups] = df[subgroups].replace(to_replace=empty_value, value="No info")
         return df
 
-    def rename_default_columns(self,
-                               df,
-                               requested_feature_names,
-                               id_column,
-                               first_human_score_column,
-                               second_human_score_column,
-                               length_column,
-                               system_score_column,
-                               candidate_column):
+    def rename_default_columns(
+        self,
+        df,
+        requested_feature_names,
+        id_column,
+        first_human_score_column,
+        second_human_score_column,
+        length_column,
+        system_score_column,
+        candidate_column,
+    ):
         """
         Standardize column names and rename columns with reserved column names.
 
         RSMTool reserves some column names for internal use, e.g., "sc1",
         "spkitemid" etc. If the given data already contains columns with
         these names, then they must be renamed to prevent conflict. This
         method renames such columns to "##NAME##", e.g., an existing column
@@ -642,70 +632,72 @@
         -------
         df : pandas DataFrame
             Modified input data frame with all the approximate
             re-namings.
         """
         df = df.copy()
 
-        columns = [id_column,
-                   first_human_score_column,
-                   second_human_score_column,
-                   length_column,
-                   system_score_column,
-                   candidate_column]
+        columns = [
+            id_column,
+            first_human_score_column,
+            second_human_score_column,
+            length_column,
+            system_score_column,
+            candidate_column,
+        ]
 
-        defaults = ['spkitemid', 'sc1', 'sc2', 'length', 'raw', 'candidate']
+        defaults = ["spkitemid", "sc1", "sc2", "length", "raw", "candidate"]
 
         # create a dictionary of name mapping for used columns
-        name_mapping = dict(filter(lambda t: t[0] is not None, zip(columns,
-                                                                   defaults)))
+        name_mapping = dict(filter(lambda t: t[0] is not None, zip(columns, defaults)))
 
         # find the columns where the names match the default names
-        correct_defaults = [column for (column, default)
-                            in name_mapping.items()
-                            if column == default]
+        correct_defaults = [
+            column for (column, default) in name_mapping.items() if column == default
+        ]
 
         # find the columns with default names reserved for other columns
         # which are not used as features in the model
-        columns_with_incorrect_default_names = [column for column in df.columns
-                                                if (column in defaults and
-                                                    column not in correct_defaults and
-                                                    column not in requested_feature_names)]
+        columns_with_incorrect_default_names = [
+            column
+            for column in df.columns
+            if (
+                column in defaults
+                and column not in correct_defaults
+                and column not in requested_feature_names
+            )
+        ]
         # rename these columns
         if columns_with_incorrect_default_names:
-            new_column_names = ['##{}##'.format(column) for column
-                                in columns_with_incorrect_default_names]
-            df.rename(columns=dict(zip(columns_with_incorrect_default_names,
-                                       new_column_names)),
-                      inplace=True)
+            new_column_names = [f"##{column}##" for column in columns_with_incorrect_default_names]
+            df.rename(
+                columns=dict(zip(columns_with_incorrect_default_names, new_column_names)),
+                inplace=True,
+            )
 
         # find the columns where the names do not match the default
-        columns_with_custom_names = [column for column in name_mapping
-                                     if column not in correct_defaults]
+        columns_with_custom_names = [
+            column for column in name_mapping if column not in correct_defaults
+        ]
 
         # rename the custom-named columns to default values
         for column in columns_with_custom_names:
 
             # if the column has already been renamed because it used a
             # default name, then use the updated name
             if column in columns_with_incorrect_default_names:
-                df.rename(columns={'##{}##'.format(column): name_mapping[column]},
-                          inplace=True)
+                df.rename(columns={f"##{column}##": name_mapping[column]}, inplace=True)
             else:
-                df.rename(columns={column: name_mapping[column]},
-                          inplace=True)
+                df.rename(columns={column: name_mapping[column]}, inplace=True)
 
         return df
 
-    def filter_on_column(self,
-                         df,
-                         column,
-                         id_column,
-                         exclude_zeros=False,
-                         exclude_zero_sd=False):  # noqa: D301
+    def filter_on_column(
+        self, df, column, id_column, exclude_zeros=False, exclude_zero_sd=False
+    ):  # noqa: D301
         """
         Filter out rows containing non-numeric values.
 
         Filter out the rows in the given data frame that contain non-numeric
         (or zero, if specified) values in the specified column. Additionally,
         it may exclude any columns if they have a standard deviation
         (:math:`\\sigma`) of 0.
@@ -749,29 +741,30 @@
         # return a copy of the original data frame if
         # the given column does not exist at all
         if column not in df.columns:
             return df_filter
 
         # Force convert the label column to numeric and
         # convert whatever can't be converted to a NaN
-        df_filter[column] = pd.to_numeric(df_filter[column],
-                                          errors='coerce').astype(float)
+        df_filter[column] = pd.to_numeric(df_filter[column], errors="coerce").astype(float)
 
         # Save the values that have been converted to NaNs
         # as a separate data frame. We want to keep them as NaNs
         # to do more analyses later. We also filter out inf values.
         # Since these can only be generated during transformations,
         # we include them with NaNs for consistency.
         bad_rows = df_filter[column].isnull() | np.isinf(df_filter[column])
         df_bad_rows = df_filter[bad_rows]
 
         # if the column contained only non-numeric values, we need to drop it
         if len(df_bad_rows) == len(df_filter):
-            self.logger.info(f"Feature {column} was excluded from the model "
-                             f"because it only contains non-numeric values.")
+            self.logger.info(
+                f"Feature {column} was excluded from the model "
+                f"because it only contains non-numeric values."
+            )
             drop_column = True
 
         # now drop the above bad rows containing NaNs from our data frame
         df_filter = df_filter[~bad_rows]
 
         # exclude zeros if specified
         if exclude_zeros:
@@ -793,36 +786,40 @@
         # for training set sd == 0 will break normalization.
         # We set the tolerance level to the 6th digit
         # to account for the possibility that the exact value
         # computed by `std()` is not 0
         if exclude_zero_sd is True:
             feature_sd = df_filter[column].std()
             if np.isclose(feature_sd, 0, atol=1e-07):
-                self.logger.info(f"Feature {column} was excluded from the model "
-                                 f"because its standard deviation in the "
-                                 f"training set is equal to 0.")
+                self.logger.info(
+                    f"Feature {column} was excluded from the model "
+                    f"because its standard deviation in the "
+                    f"training set is equal to 0."
+                )
                 drop_column = True
 
         # if `drop_column` is true, then we need to drop the column
         if drop_column:
             df_filter = df_filter.drop(column, axis=1)
             df_exclude = df_exclude.drop(column, axis=1)
 
         # return the filtered rows and the new data frame
         return (df_filter, df_exclude)
 
-    def process_predictions(self,
-                            df_test_predictions,
-                            train_predictions_mean,
-                            train_predictions_sd,
-                            human_labels_mean,
-                            human_labels_sd,
-                            trim_min,
-                            trim_max,
-                            trim_tolerance=0.4998):
+    def process_predictions(
+        self,
+        df_test_predictions,
+        train_predictions_mean,
+        train_predictions_sd,
+        human_labels_mean,
+        human_labels_sd,
+        trim_min,
+        trim_max,
+        trim_tolerance=0.4998,
+    ):
         """
         Process predictions to create scaled, trimmed and rounded predictions.
 
         Parameters
         ----------
         df_test_predictions : pandas DataFrame
             Data frame containing the test set predictions.
@@ -851,43 +848,40 @@
         -------
         df_pred_processed : pandas DataFrame
             Data frame containing the various trimmed
             and rounded predictions.
         """
         # rescale the test set predictions by boosting
         # them to match the human mean and SD
-        scaled_test_predictions = (df_test_predictions['raw'] -
-                                   train_predictions_mean) / train_predictions_sd
+        scaled_test_predictions = (
+            df_test_predictions["raw"] - train_predictions_mean
+        ) / train_predictions_sd
         scaled_test_predictions = scaled_test_predictions * human_labels_sd + human_labels_mean
 
         df_pred_process = df_test_predictions.copy()
-        df_pred_process['scale'] = scaled_test_predictions
+        df_pred_process["scale"] = scaled_test_predictions
 
         # trim and round the predictions before running the analyses
-        df_pred_process['raw_trim'] = self.trim(df_pred_process['raw'],
-                                                trim_min,
-                                                trim_max,
-                                                trim_tolerance)
-
-        df_pred_process['raw_trim_round'] = np.rint(df_pred_process['raw_trim'])
-        df_pred_process['raw_trim_round'] = df_pred_process['raw_trim_round'].astype('int64')
-
-        df_pred_process['scale_trim'] = self.trim(df_pred_process['scale'],
-                                                  trim_min,
-                                                  trim_max,
-                                                  trim_tolerance)
+        df_pred_process["raw_trim"] = self.trim(
+            df_pred_process["raw"], trim_min, trim_max, trim_tolerance
+        )
+
+        df_pred_process["raw_trim_round"] = np.rint(df_pred_process["raw_trim"])
+        df_pred_process["raw_trim_round"] = df_pred_process["raw_trim_round"].astype("int64")
+
+        df_pred_process["scale_trim"] = self.trim(
+            df_pred_process["scale"], trim_min, trim_max, trim_tolerance
+        )
 
-        df_pred_process['scale_trim_round'] = np.rint(df_pred_process['scale_trim'])
-        df_pred_process['scale_trim_round'] = df_pred_process['scale_trim_round'].astype('int64')
+        df_pred_process["scale_trim_round"] = np.rint(df_pred_process["scale_trim"])
+        df_pred_process["scale_trim_round"] = df_pred_process["scale_trim_round"].astype("int64")
 
         return df_pred_process
 
-    def filter_on_flag_columns(self,
-                               df,
-                               flag_column_dict):
+    def filter_on_flag_columns(self, df, flag_column_dict):
         """
         Filter based on specific flag columns.
 
         Check that all flag_columns are present in the given
         data frame, convert these columns to strings and filter
         out the values which do not match the condition in
         ``flag_column_dict``.
@@ -924,32 +918,32 @@
 
         if not flag_columns:
             return df.copy(), pd.DataFrame(columns=df.columns)
         else:
             # check that all columns are present
             missing_flag_columns = set(flag_columns).difference(df.columns)
             if missing_flag_columns:
-                raise KeyError("The data does not contain columns "
-                               "for all flag columns specified in the "
-                               "configuration file. Please check for "
-                               "capitalization and other spelling "
-                               "errors and make sure the flag column "
-                               "names do not contain hyphens. "
-                               "The data does not have the following columns: "
-                               "{}".format(', '.join(missing_flag_columns)))
+                raise KeyError(
+                    f"The data does not contain columns for all flag columns "
+                    f"specified in the configuration file. Please check for "
+                    f"capitalization and other spelling errors and make sure "
+                    f"the flag column names do not contain hyphens. The data "
+                    f"does not have the following "
+                    f"columns: {', '.join(missing_flag_columns)}"
+                )
 
             # since flag column may be a mix of strings and numeric values
             # we convert all strings and integers to floats such that, for
             # example, “1”, 1, and “1.0" all map to 1.0. To do this, we will
             # first convert all the strings to numbers and then convert
             # all the integers to floats.
 
-            flag_column_dict_to_float = {key: list(map(convert_to_float, value))
-                                         for (key, value)
-                                         in flag_column_dict.items()}
+            flag_column_dict_to_float = {
+                key: list(map(convert_to_float, value)) for (key, value) in flag_column_dict.items()
+            }
 
             # and now convert the the values in the feature column
             # in the data frame
             df_new = df[flag_columns].copy()
             df_new = df_new.applymap(convert_to_float)
 
             # identify responses with values which satisfy the condition
@@ -959,32 +953,29 @@
             # return the columns from the original frame that was passed in
             # so that all data types remain the same and are not changed
             df_responses_with_requested_flags = df[flag_mask].copy()
             df_responses_with_excluded_flags = df[~flag_mask].copy()
 
             # make sure that the remaining data frame is not empty
             if len(df_responses_with_requested_flags) == 0:
-                raise ValueError("No responses remaining after filtering "
-                                 "on flag columns. No further analysis can "
-                                 "be run.")
+                raise ValueError(
+                    "No responses remaining after filtering "
+                    "on flag columns. No further analysis can "
+                    "be run."
+                )
             # reset the index
-            df_responses_with_requested_flags.reset_index(drop=True,
-                                                          inplace=True)
+            df_responses_with_requested_flags.reset_index(drop=True, inplace=True)
 
-            df_responses_with_excluded_flags.reset_index(drop=True,
-                                                         inplace=True)
+            df_responses_with_excluded_flags.reset_index(drop=True, inplace=True)
 
-            return (df_responses_with_requested_flags,
-                    df_responses_with_excluded_flags)
+            return (df_responses_with_requested_flags, df_responses_with_excluded_flags)
 
-    def generate_feature_names(self,
-                               df,
-                               reserved_column_names,
-                               feature_subset_specs,
-                               feature_subset):
+    def generate_feature_names(
+        self, df, reserved_column_names, feature_subset_specs, feature_subset
+    ):
         """
         Generate feature names from column names in data frame.
 
         This method also selects the specified subset of features.
 
         Parameters
         ----------
@@ -1001,37 +992,40 @@
         -------
         feature_names : list of str
             A list of features names.
         """
         df = df.copy()
 
         # Exclude the reserved names
-        possible_feature_names = [cname for cname in df.columns
-                                  if cname not in reserved_column_names]
+        possible_feature_names = [
+            cname for cname in df.columns if cname not in reserved_column_names
+        ]
 
         # Select the features by subset.
         # In the future, we may add option to select
         # by other methods, if needed.
         if feature_subset is not None:
-            feature_names = FeatureSubsetProcessor().select_by_subset(possible_feature_names,
-                                                                      feature_subset_specs,
-                                                                      feature_subset)
+            feature_names = FeatureSubsetProcessor().select_by_subset(
+                possible_feature_names, feature_subset_specs, feature_subset
+            )
         else:
             feature_names = possible_feature_names
         return feature_names
 
-    def preprocess_feature(self,
-                           values,
-                           feature_name,
-                           feature_transform,
-                           feature_mean,
-                           feature_sd,
-                           exclude_zero_sd=False,
-                           raise_error=True,
-                           truncations=None):
+    def preprocess_feature(
+        self,
+        values,
+        feature_name,
+        feature_transform,
+        feature_mean,
+        feature_sd,
+        exclude_zero_sd=False,
+        raise_error=True,
+        truncations=None,
+    ):
         """
         Remove outliers and transform the values in given numpy array.
 
         Use the given outlier and transformation parameters.
 
         Parameters
         ----------
@@ -1068,52 +1062,55 @@
         ------
         ValueError
             If the preprocessed feature values have zero standard deviation
             and ``exclude_zero_sd`` is set to ``True``.
         """
         if truncations is not None:
             # clamp outlier values using the truncations set
-            features_no_outliers = self.remove_outliers_using_truncations(values,
-                                                                          feature_name,
-                                                                          truncations)
+            features_no_outliers = self.remove_outliers_using_truncations(
+                values, feature_name, truncations
+            )
 
         else:
             # clamp any outlier values that are 4 standard deviations
             # away from the mean
-            features_no_outliers = self.remove_outliers(values,
-                                                        mean=feature_mean,
-                                                        sd=feature_sd)
+            features_no_outliers = self.remove_outliers(values, mean=feature_mean, sd=feature_sd)
 
         # apply the requested transformation to the feature
-        transformed_feature = FeatureTransformer().transform_feature(features_no_outliers,
-                                                                     feature_name,
-                                                                     feature_transform,
-                                                                     raise_error=raise_error)
+        transformed_feature = FeatureTransformer().transform_feature(
+            features_no_outliers,
+            feature_name,
+            feature_transform,
+            raise_error=raise_error,
+        )
 
         # check the standard deviation of the transformed feature
         # we set ddof to 1 so that np.std gave the same result as pandas .std
         # we also set the tolerance limit to account for cases where std
         # is computed as a very low decimal rather than 0
         # We only do this for the training set.
         if exclude_zero_sd:
             feature_sd = np.std(transformed_feature, ddof=1)
             if np.isclose(feature_sd, 0, atol=1e-07):
-                raise ValueError("The standard deviation for "
-                                 "feature {} is 0 after pre-processing. "
-                                 "Please exclude this feature and re-run "
-                                 "the experiment.".format(feature_name))
+                raise ValueError(
+                    f"The standard deviation for feature {feature_name} "
+                    f"is 0 after pre-processing. Please exclude this "
+                    f"feature and re-run the experiment."
+                )
 
         return transformed_feature
 
-    def preprocess_features(self,
-                            df_train,
-                            df_test,
-                            df_feature_specs,
-                            standardize_features=True,
-                            use_truncations=False):
+    def preprocess_features(
+        self,
+        df_train,
+        df_test,
+        df_feature_specs,
+        standardize_features=True,
+        use_truncations=False,
+    ):
         """
         Preprocess features in given data using corresponding specifications.
 
         Preprocess the feature values in the training and testing data
         frames whose specifications are contained in ``df_feature_specs``.
         Also returns a third data frame containing the feature specifications
         and other information.
@@ -1152,110 +1149,116 @@
         df_test_preprocessed = df_test.copy()
 
         # we also need to create a data frame that includes
         # all relevant information about each feature
         df_feature_info = pd.DataFrame()
 
         # make feature the index of df_feature_specs
-        df_feature_specs.index = df_feature_specs['feature']
+        df_feature_specs.index = df_feature_specs["feature"]
 
         # if we are should be using truncations, then we create the truncations
         # set from the feature specifications
         if use_truncations:
-            truncations = df_feature_specs[['feature', 'min', 'max']].set_index('feature')
+            truncations = df_feature_specs[["feature", "min", "max"]].set_index("feature")
         else:
             truncations = None
 
         # now iterate over each feature
-        for feature_name in df_feature_specs['feature']:
+        for feature_name in df_feature_specs["feature"]:
 
-            feature_transformation = df_feature_specs.at[feature_name, 'transform']
-            feature_sign = df_feature_specs.at[feature_name, 'sign']
+            feature_transformation = df_feature_specs.at[feature_name, "transform"]
+            feature_sign = df_feature_specs.at[feature_name, "sign"]
 
             train_feature_mean = df_train[feature_name].mean()
             train_feature_sd = df_train[feature_name].std()
 
             training_feature_values = df_train[feature_name].values
-            df_train_preprocessed[feature_name] = self.preprocess_feature(training_feature_values,
-                                                                          feature_name,
-                                                                          feature_transformation,
-                                                                          train_feature_mean,
-                                                                          train_feature_sd,
-                                                                          exclude_zero_sd=True,
-                                                                          truncations=truncations)
+            df_train_preprocessed[feature_name] = self.preprocess_feature(
+                training_feature_values,
+                feature_name,
+                feature_transformation,
+                train_feature_mean,
+                train_feature_sd,
+                exclude_zero_sd=True,
+                truncations=truncations,
+            )
 
             testing_feature_values = df_test[feature_name].values
-            df_test_preprocessed[feature_name] = self.preprocess_feature(testing_feature_values,
-                                                                         feature_name,
-                                                                         feature_transformation,
-                                                                         train_feature_mean,
-                                                                         train_feature_sd,
-                                                                         truncations=truncations)
+            df_test_preprocessed[feature_name] = self.preprocess_feature(
+                testing_feature_values,
+                feature_name,
+                feature_transformation,
+                train_feature_mean,
+                train_feature_sd,
+                truncations=truncations,
+            )
 
             # Standardize the features using the mean and sd computed on the
             # training set. These are computed separately because we need to
             # get the mean of transformed feature before standardization.
             train_transformed_mean = df_train_preprocessed[feature_name].mean()
             train_transformed_sd = df_train_preprocessed[feature_name].std()
 
             if standardize_features:
 
-                df_train_without_mean = (df_train_preprocessed[feature_name] -
-                                         train_transformed_mean)
+                df_train_without_mean = df_train_preprocessed[feature_name] - train_transformed_mean
                 df_train_preprocessed[feature_name] = df_train_without_mean / train_transformed_sd
 
-                df_test_without_mean = (df_test_preprocessed[feature_name] -
-                                        train_transformed_mean)
+                df_test_without_mean = df_test_preprocessed[feature_name] - train_transformed_mean
                 df_test_preprocessed[feature_name] = df_test_without_mean / train_transformed_sd
 
             # Multiply both train and test feature by sign.
-            df_train_preprocessed[feature_name] = (df_train_preprocessed[feature_name] *
-                                                   feature_sign)
-            df_test_preprocessed[feature_name] = (df_test_preprocessed[feature_name] *
-                                                  feature_sign)
+            df_train_preprocessed[feature_name] = df_train_preprocessed[feature_name] * feature_sign
+            df_test_preprocessed[feature_name] = df_test_preprocessed[feature_name] * feature_sign
 
             # update the feature preprocessing metadata frame
-            df_feature = pd.DataFrame([{"feature": feature_name,
-                                        "transform": feature_transformation,
-                                        "sign": feature_sign,
-                                        "train_mean": train_feature_mean,
-                                        "train_sd": train_feature_sd,
-                                        "train_transformed_mean": train_transformed_mean,
-                                        "train_transformed_sd": train_transformed_sd}])
+            df_feature = pd.DataFrame(
+                [
+                    {
+                        "feature": feature_name,
+                        "transform": feature_transformation,
+                        "sign": feature_sign,
+                        "train_mean": train_feature_mean,
+                        "train_sd": train_feature_sd,
+                        "train_transformed_mean": train_transformed_mean,
+                        "train_transformed_sd": train_transformed_sd,
+                    }
+                ]
+            )
 
             df_feature_info = pd.concat([df_feature_info, df_feature])
 
         # reset the index for the feature metadata frame
         # since we built it up row by row
-        df_feature_info = df_feature_info.reset_index().drop('index', axis=1)
+        df_feature_info = df_feature_info.reset_index().drop("index", axis=1)
 
         # return the three data frames
-        return (df_train_preprocessed,
-                df_test_preprocessed,
-                df_feature_info)
-
-    def filter_data(self,
-                    df,
-                    label_column,
-                    id_column,
-                    length_column,
-                    second_human_score_column,
-                    candidate_column,
-                    requested_feature_names,
-                    reserved_column_names,
-                    given_trim_min,
-                    given_trim_max,
-                    flag_column_dict,
-                    subgroups,
-                    exclude_zero_scores=True,
-                    exclude_zero_sd=False,
-                    feature_subset_specs=None,
-                    feature_subset=None,
-                    min_candidate_items=None,
-                    use_fake_labels=False):
+        return (df_train_preprocessed, df_test_preprocessed, df_feature_info)
+
+    def filter_data(
+        self,
+        df,
+        label_column,
+        id_column,
+        length_column,
+        second_human_score_column,
+        candidate_column,
+        requested_feature_names,
+        reserved_column_names,
+        given_trim_min,
+        given_trim_max,
+        flag_column_dict,
+        subgroups,
+        exclude_zero_scores=True,
+        exclude_zero_sd=False,
+        feature_subset_specs=None,
+        feature_subset=None,
+        min_candidate_items=None,
+        use_fake_labels=False,
+    ):
         """
         Filter rows with zero/non-numeric values for ``label_column``.
 
         Check whether any features that are specifically requested in
         ``requested_feature_names`` are missing from the data. If no
         feature names are requested, the feature list is generated based
         on column names and subset information, if available. The function
@@ -1350,241 +1353,260 @@
             columns_to_check.append(second_human_score_column)
 
         if candidate_column:
             columns_to_check.append(candidate_column)
 
         missing_columns = set(columns_to_check).difference(df.columns)
         if missing_columns:
-            raise KeyError("Columns {} from the config file "
-                           "do not exist in the data.".format(missing_columns))
+            raise KeyError(
+                f"Columns {missing_columns} from the config file do not " f"exist in the data."
+            )
 
         # it is possible for the `id_column` and `candidate_column` to be
         # set to the same column name in the CSV file, e.g., if there is
         # only one response per candidate. If this happens, we neeed to
         # create a duplicate column for candidates or id for the downstream
         # processing to work as usual.
         if id_column == candidate_column:
             # if the name for both columns is `candidate`, we need to
             # create a separate id_column name
-            if id_column == 'candidate':
-                df['spkitemid'] = df['candidate'].copy()
-                id_column = 'spkitemid'
+            if id_column == "candidate":
+                df["spkitemid"] = df["candidate"].copy()
+                id_column = "spkitemid"
             # else we create a separate `candidate` column
             else:
-                df['candidate'] = df[id_column].copy()
-                candidate_column = 'candidate'
+                df["candidate"] = df[id_column].copy()
+                candidate_column = "candidate"
 
-        df = self.rename_default_columns(df,
-                                         requested_feature_names,
-                                         id_column,
-                                         label_column,
-                                         second_human_score_column,
-                                         length_column,
-                                         None,
-                                         candidate_column)
+        df = self.rename_default_columns(
+            df,
+            requested_feature_names,
+            id_column,
+            label_column,
+            second_human_score_column,
+            length_column,
+            None,
+            candidate_column,
+        )
 
         # check that the id_column contains unique values
-        if df['spkitemid'].size != df['spkitemid'].unique().size:
-            raise ValueError("The data contains duplicate response IDs in "
-                             "'{}'. Please make sure all response IDs are "
-                             "unique and re-run the tool.".format(id_column))
+        if df["spkitemid"].size != df["spkitemid"].unique().size:
+            raise ValueError(
+                f"The data contains duplicate response IDs in '{id_column}'. "
+                f"Please make sure all response IDs are unique and re-run the tool."
+            )
 
         # Generate feature names if no specific features were requested by the user
         if len(requested_feature_names) == 0:
-            feature_names = self.generate_feature_names(df,
-                                                        reserved_column_names,
-                                                        feature_subset_specs=feature_subset_specs,
-                                                        feature_subset=feature_subset)
+            feature_names = self.generate_feature_names(
+                df,
+                reserved_column_names,
+                feature_subset_specs=feature_subset_specs,
+                feature_subset=feature_subset,
+            )
         else:
             feature_names = requested_feature_names
 
         # make sure that feature names do not contain reserved column names
         illegal_feature_names = set(feature_names).intersection(reserved_column_names)
         if illegal_feature_names:
-            raise ValueError("The following reserved "
-                             "column names cannot be "
-                             "used as feature names: '{}'. "
-                             "Please rename these columns "
-                             "and re-run the "
-                             "experiment.".format(', '.join(illegal_feature_names)))
+            raise ValueError(
+                f"The following reserved column names cannot be used as "
+                f"feature names: '{', '.join(illegal_feature_names)}'. "
+                f"Please rename these columns and re-run the experiment."
+            )
 
         # check to make sure that the subgroup columns are all present
         df = self.check_subgroups(df, subgroups)
 
         # filter out the responses based on flag columns
-        (df_responses_with_requested_flags,
-         df_responses_with_excluded_flags) = self.filter_on_flag_columns(df, flag_column_dict)
+        (
+            df_responses_with_requested_flags,
+            df_responses_with_excluded_flags,
+        ) = self.filter_on_flag_columns(df, flag_column_dict)
 
         # filter out the rows that have non-numeric or zero labels
         # unless we are going to generate fake labels in the first place
         if not use_fake_labels:
-            (df_filtered,
-             df_excluded) = self.filter_on_column(df_responses_with_requested_flags,
-                                                  'sc1',
-                                                  'spkitemid',
-                                                  exclude_zeros=exclude_zero_scores)
+            (df_filtered, df_excluded) = self.filter_on_column(
+                df_responses_with_requested_flags,
+                "sc1",
+                "spkitemid",
+                exclude_zeros=exclude_zero_scores,
+            )
 
             # make sure that the remaining data frame is not empty
             if len(df_filtered) == 0:
-                raise ValueError("No responses remaining after filtering out "
-                                 "non-numeric human scores. No further analysis "
-                                 "can be run. ")
+                raise ValueError(
+                    "No responses remaining after filtering out "
+                    "non-numeric human scores. No further analysis "
+                    "can be run. "
+                )
 
-            trim_min = given_trim_min if given_trim_min else df_filtered['sc1'].min()
-            trim_max = given_trim_max if given_trim_max else df_filtered['sc1'].max()
+            trim_min = given_trim_min if given_trim_min else df_filtered["sc1"].min()
+            trim_max = given_trim_max if given_trim_max else df_filtered["sc1"].max()
         else:
             df_filtered = df_responses_with_requested_flags.copy()
             trim_min = given_trim_min if given_trim_min else 1
             trim_max = given_trim_max if given_trim_max else 10
-            self.logger.info("Generating labels randomly "
-                             "from [{}, {}]".format(trim_min, trim_max))
+            self.logger.info(f"Generating labels randomly from [{trim_min}, {trim_max}]")
             randgen = RandomState(seed=1234567890)
-            df_filtered[label_column] = randgen.random_integers(trim_min,
-                                                                trim_max,
-                                                                size=len(df_filtered))
+            df_filtered[label_column] = randgen.random_integers(
+                trim_min, trim_max, size=len(df_filtered)
+            )
 
         # make sure there are no missing features in the data
         missing_features = set(feature_names).difference(df_filtered.columns)
         if not missing_features:
             # make sure all features selected for model building are numeric
             # and also replace any non-numeric feature values in already
             # excluded data with NaNs for consistency
             for feat in feature_names:
-                df_excluded[feat] = pd.to_numeric(df_excluded[feat],
-                                                  errors='coerce').astype(float)
-                newdf, newdf_excluded = self.filter_on_column(df_filtered,
-                                                              feat,
-                                                              'spkitemid',
-                                                              exclude_zeros=False,
-                                                              exclude_zero_sd=exclude_zero_sd)
+                df_excluded[feat] = pd.to_numeric(df_excluded[feat], errors="coerce").astype(float)
+                newdf, newdf_excluded = self.filter_on_column(
+                    df_filtered,
+                    feat,
+                    "spkitemid",
+                    exclude_zeros=False,
+                    exclude_zero_sd=exclude_zero_sd,
+                )
                 del df_filtered
                 df_filtered = newdf
-                with np.errstate(divide='ignore'):
+                with np.errstate(divide="ignore"):
                     df_excluded = pd.concat([df_excluded, newdf_excluded], sort=True)
 
             # make sure that the remaining data frame is not empty
             if len(df_filtered) == 0:
-                raise ValueError("No responses remaining after filtering "
-                                 "out non-numeric feature values. No further "
-                                 "analysis can be run.")
+                raise ValueError(
+                    "No responses remaining after filtering "
+                    "out non-numeric feature values. No further "
+                    "analysis can be run."
+                )
 
             # Raise warning if we excluded features that were
             # specified in the .json file because sd == 0.
             omitted_features = set(requested_feature_names).difference(df_filtered.columns)
             if omitted_features:
-                raise ValueError("The following requested features "
-                                 "were excluded because their standard "
-                                 "deviation on the training set was 0: {}.\n"
-                                 "Please edit the feature file to exclude "
-                                 "these features and re-run the "
-                                 "tool".format(', '.join(omitted_features)))
+                raise ValueError(
+                    f"The following requested features were excluded "
+                    f"because their standard deviation on the training "
+                    f"set was 0: {', '.join(omitted_features)}.\nPlease "
+                    f"edit the feature file to exclude these features "
+                    f"and re-run the tool"
+                )
             # Update the feature names
-            feature_names = [feature for feature in feature_names
-                             if feature in df_filtered]
+            feature_names = [feature for feature in feature_names if feature in df_filtered]
         else:
-            raise KeyError("DataFrame does not contain "
-                           "columns for all features specified in "
-                           "the feature file. Please check for "
-                           "capitalization and other spelling "
-                           "errors and make sure the feature "
-                           "names do not contain hyphens. "
-                           "The data does not have columns "
-                           "for the following features: "
-                           "{}".format(', '.join(missing_features)))
+            raise KeyError(
+                f"DataFrame does not contain columns for all features "
+                f"specified in the feature file. Please check for "
+                f"capitalization and other spelling errors and make "
+                f"sure the feature names do not contain hyphens. "
+                f"The data does not have columns for the following "
+                f"features: {', '.join(missing_features)}"
+            )
 
         # if ``length_column`` exists, make sure it's converted to numeric;
         # values that cannot be coerced to numeric will be set to ``np.nan``
         if length_column:
-            df_filtered['length'] = pd.to_numeric(df_filtered['length'], errors='coerce')
+            df_filtered["length"] = pd.to_numeric(df_filtered["length"], errors="coerce")
 
         # check the values for length column. We do this after filtering
         # to make sure we have removed responses that have not been
         # processed correctly. Else rename length column to
         # ##ORIGINAL_NAME##.
-        if (length_column and
-            (len(df_filtered[df_filtered['length'].isnull()]) != 0 or
-                df_filtered['length'].std() <= 0)):
-            self.logger.warning("The {} column either has missing values or a standard "
-                                "deviation <= 0. No length-based analysis will be "
-                                "provided. The column will be renamed as ##{}## and "
-                                "saved in *train_other_columns.csv.".format(length_column,
-                                                                            length_column))
-            df_filtered.rename(columns={'length': '##{}##'.format(length_column)},
-                               inplace=True)
+        if length_column and (
+            len(df_filtered[df_filtered["length"].isnull()]) != 0
+            or df_filtered["length"].std() <= 0
+        ):
+            self.logger.warning(
+                f"The {length_column} column either has missing values "
+                f"or a standard deviation <= 0. No length-based analysis "
+                f"will be provided. The column will be renamed as "
+                f"##{length_column}## and saved in *train_other_columns.csv."
+            )
+            df_filtered.rename(columns={"length": f"##{length_column}##"}, inplace=True)
 
         # if requested, exclude the candidates with less than X responses
         # left after filtering
         if min_candidate_items:
-            (df_filtered_candidates,
-             df_excluded_candidates) = self.select_candidates(df_filtered, min_candidate_items)
+            (df_filtered_candidates, df_excluded_candidates) = self.select_candidates(
+                df_filtered, min_candidate_items
+            )
             # check that there are still responses left for analysis
             if len(df_filtered_candidates) == 0:
-                raise ValueError("After filtering non-numeric scores and "
-                                 "non-numeric feature values there were "
-                                 "no candidates with {} or more responses "
-                                 "left for analysis".format(min_candidate_items))
+                raise ValueError(
+                    f"After filtering non-numeric scores and non-numeric "
+                    f"feature values there were no candidates with "
+                    f"{min_candidate_items} or more responses left "
+                    f"for analysis."
+                )
 
             # redefine df_filtered
             df_filtered = df_filtered_candidates.copy()
 
             # update df_excluded
             df_excluded = pd.concat([df_excluded, df_excluded_candidates], sort=True)
 
         # create separate data frames for features and sc1, all other
         # information, and responses excluded during filtering
         not_other_columns = set()
-        feature_columns = ['spkitemid', 'sc1'] + feature_names
+        feature_columns = ["spkitemid", "sc1"] + feature_names
         df_filtered_features = df_filtered[feature_columns]
         not_other_columns.update(feature_columns)
 
-        metadata_columns = ['spkitemid'] + subgroups
+        metadata_columns = ["spkitemid"] + subgroups
         if candidate_column:
-            metadata_columns.append('candidate')
+            metadata_columns.append("candidate")
         df_filtered_metadata = df_filtered[metadata_columns]
         not_other_columns.update(metadata_columns)
 
         df_filtered_length = pd.DataFrame()
-        length_columns = ['spkitemid', 'length']
-        if length_column and 'length' in df_filtered:
+        length_columns = ["spkitemid", "length"]
+        if length_column and "length" in df_filtered:
             df_filtered_length = df_filtered[length_columns]
             not_other_columns.update(length_columns)
 
         df_filtered_human_scores = pd.DataFrame()
-        human_score_columns = ['spkitemid', 'sc1', 'sc2']
-        if second_human_score_column and 'sc2' in df_filtered:
+        human_score_columns = ["spkitemid", "sc1", "sc2"]
+        if second_human_score_column and "sc2" in df_filtered:
             df_filtered_human_scores = df_filtered[human_score_columns].copy()
-            not_other_columns.update(['sc2'])
+            not_other_columns.update(["sc2"])
 
             # filter out any non-numeric value rows
             # as well as zeros, if we were asked to
-            df_filtered_human_scores['sc2'] = pd.to_numeric(df_filtered_human_scores['sc2'],
-                                                            errors='coerce').astype(float)
+            df_filtered_human_scores["sc2"] = pd.to_numeric(
+                df_filtered_human_scores["sc2"], errors="coerce"
+            ).astype(float)
             if exclude_zero_scores:
-                df_filtered_human_scores['sc2'] = df_filtered_human_scores['sc2'].replace(0,
-                                                                                          np.nan)
+                df_filtered_human_scores["sc2"] = df_filtered_human_scores["sc2"].replace(0, np.nan)
 
         # we need to make sure that `spkitemid` is the first column
-        df_excluded = df_excluded[['spkitemid'] + [column for column in df_excluded
-                                                   if column != 'spkitemid']]
+        df_excluded = df_excluded[
+            ["spkitemid"] + [column for column in df_excluded if column != "spkitemid"]
+        ]
 
         # now extract all other columns and add 'spkitemid'
-        other_columns = ['spkitemid'] + [column for column in df_filtered
-                                         if column not in not_other_columns]
+        other_columns = ["spkitemid"] + [
+            column for column in df_filtered if column not in not_other_columns
+        ]
         df_filtered_other_columns = df_filtered[other_columns]
 
-        return (df_filtered_features,
-                df_filtered_metadata,
-                df_filtered_other_columns,
-                df_excluded,
-                df_filtered_length,
-                df_filtered_human_scores,
-                df_responses_with_excluded_flags,
-                trim_min,
-                trim_max,
-                feature_names)
+        return (
+            df_filtered_features,
+            df_filtered_metadata,
+            df_filtered_other_columns,
+            df_excluded,
+            df_filtered_length,
+            df_filtered_human_scores,
+            df_responses_with_excluded_flags,
+            trim_min,
+            trim_max,
+            feature_names,
+        )
 
     def process_data_rsmtool(self, config_obj, data_container_obj):
         """
         Set up rsmtool experiment by loading & preprocessing train/test data.
 
         This function takes a configuration object and a container object
         as input and returns the same types of objects as output after
@@ -1617,343 +1639,393 @@
             If the second human score column is requested as a feature.
         ValueError
             If "use_truncations" was specified in the configuration,
             but no feature CSV file was found.
         """
         train = data_container_obj.train
         test = data_container_obj.test
-        feature_specs = data_container_obj.get_frame('feature_specs')
-        feature_subset = data_container_obj.get_frame('feature_subset_specs')
+        feature_specs = data_container_obj.get_frame("feature_specs")
+        feature_subset = data_container_obj.get_frame("feature_subset_specs")
 
         feature_specs_processor = FeatureSpecsProcessor()
         feature_subset_processor = FeatureSubsetProcessor()
 
         configdir = config_obj.configdir
 
-        (test_file_location,
-         train_file_location) = DataReader.locate_files([config_obj['test_file'],
-                                                         config_obj['train_file']],
-                                                        configdir)
+        (test_file_location, train_file_location) = DataReader.locate_files(
+            [config_obj["test_file"], config_obj["train_file"]], configdir
+        )
 
-        feature_subset_file = config_obj['feature_subset_file']
+        feature_subset_file = config_obj["feature_subset_file"]
 
         if feature_subset_file is not None:
             feature_subset_file = DataReader.locate_files(feature_subset_file, configdir)
 
         # get the column name for the labels for the training and testing data
-        train_label_column = config_obj['train_label_column']
-        test_label_column = config_obj['test_label_column']
+        train_label_column = config_obj["train_label_column"]
+        test_label_column = config_obj["test_label_column"]
 
         # get the column name that will hold the ID for
         # both the training and the test data
-        id_column = config_obj['id_column']
+        id_column = config_obj["id_column"]
 
         # get the specified trim min, trim max and trim tolerance values
-        (spec_trim_min,
-         spec_trim_max,
-         spec_trim_tolerance) = config_obj.get_trim_min_max_tolerance()
+        (
+            spec_trim_min,
+            spec_trim_max,
+            spec_trim_tolerance,
+        ) = config_obj.get_trim_min_max_tolerance()
 
         # get the name of the optional column that
         # contains response length.
-        length_column = config_obj['length_column']
+        length_column = config_obj["length_column"]
 
         # get the name of the optional column that
         # contains the second human score
-        second_human_score_column = config_obj['second_human_score_column']
+        second_human_score_column = config_obj["second_human_score_column"]
 
         # get the name of the optional column that
         # contains the candidate ID
-        candidate_column = config_obj['candidate_column']
+        candidate_column = config_obj["candidate_column"]
 
         # if the test label column is the same as the
         # second human score column, raise an error
         if test_label_column == second_human_score_column:
-            raise ValueError("'test_label_column' and "
-                             "'second_human_score_column' cannot have the "
-                             "same value.")
+            raise ValueError(
+                "'test_label_column' and "
+                "'second_human_score_column' cannot have the "
+                "same value."
+            )
 
         # check if we are excluding candidates based on number of responses
         exclude_listwise = config_obj.check_exclude_listwise()
-        min_items = config_obj['min_items_per_candidate']
+        min_items = config_obj["min_items_per_candidate"]
 
         # get the name of the model that we want to train and
         # check that it's valid
-        model_name = config_obj['model']
+        model_name = config_obj["model"]
         model_type = self.check_model_name(model_name)
 
         # are we excluding zero scores?
-        exclude_zero_scores = config_obj['exclude_zero_scores']
+        exclude_zero_scores = config_obj["exclude_zero_scores"]
 
         # should we standardize the features
-        standardize_features = config_obj['standardize_features']
+        standardize_features = config_obj["standardize_features"]
 
         # if we are excluding zero scores but trim_min
         # is set to 0, then we need to warn the user
         if exclude_zero_scores and spec_trim_min == 0:
-            self.logger.warning("'exclude_zero_scores' is set to True but "
-                                "'trim_min' is set to 0. This may cause "
-                                "unexpected behavior.")
+            self.logger.warning(
+                "'exclude_zero_scores' is set to True but "
+                "'trim_min' is set to 0. This may cause "
+                "unexpected behavior."
+            )
 
         # are we filtering on any other columns?
         # is `flag_column` applied to training partition only
         # or both partitions?
-        if 'flag_column_test' in config_obj:
-            flag_partition = 'train'
+        if "flag_column_test" in config_obj:
+            flag_partition = "train"
         else:
-            flag_partition = 'both'
+            flag_partition = "both"
 
         flag_column_dict = config_obj.check_flag_column(partition=flag_partition)
-        flag_column_test_dict = config_obj.check_flag_column('flag_column_test',
-                                                             partition='test')
+        flag_column_test_dict = config_obj.check_flag_column("flag_column_test", partition="test")
 
-        if (flag_column_dict and not flag_column_test_dict):
+        if flag_column_dict and not flag_column_test_dict:
             flag_column_test_dict = flag_column_dict
 
         # are we generating fake labels?
-        use_fake_train_labels = train_label_column == 'fake'
-        use_fake_test_labels = test_label_column == 'fake'
+        use_fake_train_labels = train_label_column == "fake"
+        use_fake_test_labels = test_label_column == "fake"
 
         # are we using truncations from the feature specs?
-        use_truncations = config_obj['use_truncation_thresholds']
+        use_truncations = config_obj["use_truncation_thresholds"]
 
         # get the subgroups if any
-        subgroups = config_obj.get('subgroups')
+        subgroups = config_obj.get("subgroups")
 
         # are there specific general report sections we want to include?
-        general_report_sections = config_obj['general_sections']
+        general_report_sections = config_obj["general_sections"]
 
         # what about the special or custom sections?
-        special_report_sections = config_obj['special_sections']
+        special_report_sections = config_obj["special_sections"]
 
-        custom_report_section_paths = config_obj['custom_sections']
+        custom_report_section_paths = config_obj["custom_sections"]
 
         if custom_report_section_paths and configdir is not None:
-            self.logger.info('Locating custom report sections')
-            custom_report_sections = Reporter.locate_custom_sections(custom_report_section_paths,
-                                                                     configdir)
+            self.logger.info("Locating custom report sections")
+            custom_report_sections = Reporter.locate_custom_sections(
+                custom_report_section_paths, configdir
+            )
         else:
             custom_report_sections = []
 
-        section_order = config_obj['section_order']
+        section_order = config_obj["section_order"]
 
-        chosen_notebook_files = Reporter().get_ordered_notebook_files(general_report_sections,
-                                                                      special_report_sections,
-                                                                      custom_report_sections,
-                                                                      section_order,
-                                                                      subgroups,
-                                                                      model_type=model_type,
-                                                                      context='rsmtool')
+        chosen_notebook_files = Reporter().get_ordered_notebook_files(
+            general_report_sections,
+            special_report_sections,
+            custom_report_sections,
+            section_order,
+            subgroups,
+            model_type=model_type,
+            context="rsmtool",
+        )
 
         # Location of feature file
-        feature_field = config_obj['features']
+        feature_field = config_obj["features"]
 
-        feature_subset_field = config_obj['feature_subset']
+        feature_subset_field = config_obj["feature_subset"]
 
         # if the user requested feature_subset file and feature subset,
         # read the file and check its format
         if feature_subset is not None and feature_subset_field:
             feature_subset_processor.check_feature_subset_file(feature_subset)
 
         # Do we need to automatically find the best transformations/change sign?
-        select_transformations = config_obj['select_transformations']
-        feature_sign = config_obj['sign']
+        select_transformations = config_obj["select_transformations"]
+        feature_sign = config_obj["sign"]
         requested_features = []
         generate_feature_specs_automatically = True
 
         # if the feature field is a list, then simply
         # assign it to `requested_features`
         if isinstance(feature_field, list):
             requested_features = feature_field
 
         elif feature_field is not None:
             generate_feature_specs_automatically = False
-            feature_specs = feature_specs_processor.validate_feature_specs(feature_specs,
-                                                                           use_truncations)
-            requested_features = feature_specs['feature'].tolist()
+            feature_specs = feature_specs_processor.validate_feature_specs(
+                feature_specs, use_truncations
+            )
+            requested_features = feature_specs["feature"].tolist()
 
         # if we get to this point and both ``generate_feature_specs_automatically``
         # and ``use_truncations`` are True, then we need to raise an error
         if use_truncations and generate_feature_specs_automatically:
-            raise ValueError('You have specified the ``use_truncations`` configuration '
-                             'option, but a feature file could not be found.')
+            raise ValueError(
+                "You have specified the ``use_truncations`` configuration "
+                "option, but a feature file could not be found."
+            )
 
         # check to make sure that `length_column` or `second_human_score_column`
         # are not also included in the requested features, if they are specified
-        if (length_column and
-                length_column in requested_features):
-            raise ValueError("The value of 'length_column' ('{}') cannot be "
-                             "used as a model feature.".format(length_column))
-
-        if (second_human_score_column and
-                second_human_score_column in requested_features):
-            raise ValueError("The value of 'second_human_score_column' ('{}') cannot be "
-                             "used as a model feature.".format(second_human_score_column))
+        if length_column and length_column in requested_features:
+            raise ValueError(
+                f"The value of 'length_column' ('{length_column}') "
+                f"cannot be used as a model feature."
+            )
+
+        if second_human_score_column and second_human_score_column in requested_features:
+            raise ValueError(
+                f"The value of 'second_human_score_column' "
+                f"('{second_human_score_column}') cannot be used "
+                f"as a model feature."
+            )
 
         # Specify column names that cannot be used as features
-        reserved_column_names = list(set(['spkitemid', 'spkitemlab',
-                                          'itemType', 'r1', 'r2', 'score',
-                                          'sc', 'sc1', 'adj',
-                                          train_label_column,
-                                          test_label_column,
-                                          id_column] + subgroups + list(flag_column_dict.keys())))
+        reserved_column_names = list(
+            set(
+                [
+                    "spkitemid",
+                    "spkitemlab",
+                    "itemType",
+                    "r1",
+                    "r2",
+                    "score",
+                    "sc",
+                    "sc1",
+                    "adj",
+                    train_label_column,
+                    test_label_column,
+                    id_column,
+                ]
+                + subgroups
+                + list(flag_column_dict.keys())
+            )
+        )
 
         # if `second_human_score_column` is specified, then
         # we need to add the original name as well as `sc2` to the list of reserved column
         # names. And same for 'length' and 'candidate', if `length_column`
         # and `candidate_column` are specified. We add both names to
         # simplify things downstream since neither the original name nor
         # the standardized name should be used as feature names
         if second_human_score_column:
             reserved_column_names.append(second_human_score_column)
-            reserved_column_names.append('sc2')
+            reserved_column_names.append("sc2")
         if length_column:
             reserved_column_names.append(length_column)
-            reserved_column_names.append('length')
+            reserved_column_names.append("length")
         if candidate_column:
             reserved_column_names.append(candidate_column)
-            reserved_column_names.append('candidate')
+            reserved_column_names.append("candidate")
 
         # remove duplicates (if any) from the list of reserved column names
         reserved_column_names = list(set(reserved_column_names))
 
         # Make sure that the training data as specified in the
         # config file actually exists on disk and if it does,
         # load it and filter out the bad rows and features with
         # zero standard deviation. Also double check that the requested
         # features exist in the data or obtain the feature names if
         # no feature file was given.
-        (df_train_features,
-         df_train_metadata,
-         df_train_other_columns,
-         df_train_excluded,
-         df_train_length,
-         _,
-         df_train_flagged_responses,
-         used_trim_min,
-         used_trim_max,
-         feature_names) = self.filter_data(train,
-                                           train_label_column,
-                                           id_column,
-                                           length_column,
-                                           None,
-                                           candidate_column,
-                                           requested_features,
-                                           reserved_column_names,
-                                           spec_trim_min,
-                                           spec_trim_max,
-                                           flag_column_dict,
-                                           subgroups,
-                                           exclude_zero_scores=exclude_zero_scores,
-                                           exclude_zero_sd=True,
-                                           feature_subset_specs=feature_subset,
-                                           feature_subset=feature_subset_field,
-                                           min_candidate_items=min_items,
-                                           use_fake_labels=use_fake_train_labels)
+        (
+            df_train_features,
+            df_train_metadata,
+            df_train_other_columns,
+            df_train_excluded,
+            df_train_length,
+            _,
+            df_train_flagged_responses,
+            used_trim_min,
+            used_trim_max,
+            feature_names,
+        ) = self.filter_data(
+            train,
+            train_label_column,
+            id_column,
+            length_column,
+            None,
+            candidate_column,
+            requested_features,
+            reserved_column_names,
+            spec_trim_min,
+            spec_trim_max,
+            flag_column_dict,
+            subgroups,
+            exclude_zero_scores=exclude_zero_scores,
+            exclude_zero_sd=True,
+            feature_subset_specs=feature_subset,
+            feature_subset=feature_subset_field,
+            min_candidate_items=min_items,
+            use_fake_labels=use_fake_train_labels,
+        )
 
         # Generate feature specifications now that we know what features to use
         if generate_feature_specs_automatically:
             if select_transformations:
 
-                feature_specs = feature_specs_processor.generate_specs(df_train_features,
-                                                                       feature_names,
-                                                                       'sc1',
-                                                                       feature_subset=feature_subset,
-                                                                       feature_sign=feature_sign)
+                feature_specs = feature_specs_processor.generate_specs(
+                    df_train_features,
+                    feature_names,
+                    "sc1",
+                    feature_subset=feature_subset,
+                    feature_sign=feature_sign,
+                )
             else:
                 feature_specs = feature_specs_processor.generate_default_specs(feature_names)
 
         # Do the same for the test data except we can ignore the trim min
         # and max since we already have that from the training data and
         # we have the feature_names when no feature file was specified.
         # We also allow features with 0 standard deviation in the test file.
-        if (test_file_location == train_file_location and
-                train_label_column == test_label_column):
-            self.logger.warning("The same data file and label "
-                                "column are used for both training "
-                                "and evaluating the model. No second "
-                                "score analysis will be performed, even "
-                                "if requested.")
+        if test_file_location == train_file_location and train_label_column == test_label_column:
+            self.logger.warning(
+                "The same data file and label "
+                "column are used for both training "
+                "and evaluating the model. No second "
+                "score analysis will be performed, even "
+                "if requested."
+            )
 
             df_test_features = df_train_features.copy()
             df_test_metadata = df_train_metadata.copy()
             df_test_excluded = df_train_excluded.copy()
             df_test_other_columns = df_train_other_columns.copy()
             df_test_flagged_responses = df_train_flagged_responses.copy()
             df_test_human_scores = pd.DataFrame()
         else:
 
-            (df_test_features,
-             df_test_metadata,
-             df_test_other_columns,
-             df_test_excluded,
-             _,
-             df_test_human_scores,
-             df_test_flagged_responses,
-             _, _, _) = self.filter_data(test,
-                                         test_label_column,
-                                         id_column,
-                                         None,
-                                         second_human_score_column,
-                                         candidate_column,
-                                         feature_names,
-                                         reserved_column_names,
-                                         used_trim_min,
-                                         used_trim_max,
-                                         flag_column_test_dict,
-                                         subgroups,
-                                         exclude_zero_scores=exclude_zero_scores,
-                                         exclude_zero_sd=False,
-                                         min_candidate_items=min_items,
-                                         use_fake_labels=use_fake_test_labels)
-
-        self.logger.info('Pre-processing training and test set features')
-        (df_train_preprocessed_features,
-         df_test_preprocessed_features,
-         df_feature_info) = self.preprocess_features(df_train_features,
-                                                     df_test_features,
-                                                     feature_specs,
-                                                     standardize_features,
-                                                     use_truncations)
+            (
+                df_test_features,
+                df_test_metadata,
+                df_test_other_columns,
+                df_test_excluded,
+                _,
+                df_test_human_scores,
+                df_test_flagged_responses,
+                _,
+                _,
+                _,
+            ) = self.filter_data(
+                test,
+                test_label_column,
+                id_column,
+                None,
+                second_human_score_column,
+                candidate_column,
+                feature_names,
+                reserved_column_names,
+                used_trim_min,
+                used_trim_max,
+                flag_column_test_dict,
+                subgroups,
+                exclude_zero_scores=exclude_zero_scores,
+                exclude_zero_sd=False,
+                min_candidate_items=min_items,
+                use_fake_labels=use_fake_test_labels,
+            )
+
+        self.logger.info("Pre-processing training and test set features")
+        (
+            df_train_preprocessed_features,
+            df_test_preprocessed_features,
+            df_feature_info,
+        ) = self.preprocess_features(
+            df_train_features,
+            df_test_features,
+            feature_specs,
+            standardize_features,
+            use_truncations,
+        )
 
         # configuration options that either override previous values or are
         # entirely for internal use
         new_config_obj = config_obj.copy()
-        internal_options_dict = {'chosen_notebook_files': chosen_notebook_files,
-                                 'exclude_listwise': exclude_listwise,
-                                 'feature_subset_file': feature_subset_file,
-                                 'model_name': model_name,
-                                 'model_type': model_type,
-                                 'test_file_location': test_file_location,
-                                 'train_file_location': train_file_location,
-                                 'trim_min': used_trim_min,
-                                 'trim_max': used_trim_max}
+        internal_options_dict = {
+            "chosen_notebook_files": chosen_notebook_files,
+            "exclude_listwise": exclude_listwise,
+            "feature_subset_file": feature_subset_file,
+            "model_name": model_name,
+            "model_type": model_type,
+            "test_file_location": test_file_location,
+            "train_file_location": train_file_location,
+            "trim_min": used_trim_min,
+            "trim_max": used_trim_max,
+        }
 
         for key, value in internal_options_dict.items():
             new_config_obj[key] = value
 
-        new_container = [{'name': 'train_features',
-                          'frame': df_train_features},
-                         {'name': 'test_features',
-                          'frame': df_test_features},
-                         {'name': 'train_preprocessed_features',
-                          'frame': df_train_preprocessed_features},
-                         {'name': 'test_preprocessed_features',
-                          'frame': df_test_preprocessed_features},
-                         {'name': 'train_metadata', 'frame': df_train_metadata},
-                         {'name': 'test_metadata', 'frame': df_test_metadata},
-                         {'name': 'train_other_columns', 'frame': df_train_other_columns},
-                         {'name': 'test_other_columns', 'frame': df_test_other_columns},
-                         {'name': 'train_excluded', 'frame': df_train_excluded},
-                         {'name': 'test_excluded', 'frame': df_test_excluded},
-                         {'name': 'train_length', 'frame': df_train_length},
-                         {'name': 'test_human_scores', 'frame': df_test_human_scores},
-                         {'name': 'train_flagged', 'frame': df_train_flagged_responses},
-                         {'name': 'test_flagged', 'frame': df_test_flagged_responses},
-                         {'name': 'feature_specs', 'frame': feature_specs},
-                         {'name': 'feature_info', 'frame': df_feature_info}]
+        new_container = [
+            {"name": "train_features", "frame": df_train_features},
+            {"name": "test_features", "frame": df_test_features},
+            {
+                "name": "train_preprocessed_features",
+                "frame": df_train_preprocessed_features,
+            },
+            {
+                "name": "test_preprocessed_features",
+                "frame": df_test_preprocessed_features,
+            },
+            {"name": "train_metadata", "frame": df_train_metadata},
+            {"name": "test_metadata", "frame": df_test_metadata},
+            {"name": "train_other_columns", "frame": df_train_other_columns},
+            {"name": "test_other_columns", "frame": df_test_other_columns},
+            {"name": "train_excluded", "frame": df_train_excluded},
+            {"name": "test_excluded", "frame": df_test_excluded},
+            {"name": "train_length", "frame": df_train_length},
+            {"name": "test_human_scores", "frame": df_test_human_scores},
+            {"name": "train_flagged", "frame": df_train_flagged_responses},
+            {"name": "test_flagged", "frame": df_test_flagged_responses},
+            {"name": "feature_specs", "frame": feature_specs},
+            {"name": "feature_info", "frame": df_feature_info},
+        ]
 
         new_container = DataContainer(new_container)
 
         return new_config_obj, new_container
 
     def process_data_rsmeval(self, config_obj, data_container_obj):
         """
@@ -1994,116 +2066,125 @@
             once.
         ValueError
             No responses were left after filtering out zero or non-numeric
             values for the various columns.
         """
         # get the directory where the config file lives
         configpath = config_obj.configdir
-        pred_file_location = DataReader.locate_files(config_obj['predictions_file'],
-                                                     configpath)
+        pred_file_location = DataReader.locate_files(config_obj["predictions_file"], configpath)
 
         # get the column name for the labels for the training and testing data
-        human_score_column = config_obj['human_score_column']
-        system_score_column = config_obj['system_score_column']
+        human_score_column = config_obj["human_score_column"]
+        system_score_column = config_obj["system_score_column"]
 
         # if the human score column is the same as the
         # system score column, raise an error
         if human_score_column == system_score_column:
-            raise ValueError("'human_score_column' and "
-                             "'system_score_column' "
-                             "cannot have the same value.")
+            raise ValueError(
+                "'human_score_column' and " "'system_score_column' " "cannot have the same value."
+            )
 
         # get the name of the optional column that
         # contains the second human score
-        second_human_score_column = config_obj['second_human_score_column']
+        second_human_score_column = config_obj["second_human_score_column"]
 
         # if the human score column is the same as the
         # second human score column, raise an error
         if human_score_column == second_human_score_column:
-            raise ValueError("'human_score_column' and "
-                             "'second_human_score_column' "
-                             "cannot have the same value.")
+            raise ValueError(
+                "'human_score_column' and "
+                "'second_human_score_column' "
+                "cannot have the same value."
+            )
 
         # get the column name that will hold the ID for
         # both the training and the test data
-        id_column = config_obj['id_column']
+        id_column = config_obj["id_column"]
 
         # get the specified trim min and max, if any
         # and make sure they are numeric
-        (spec_trim_min,
-         spec_trim_max,
-         spec_trim_tolerance) = config_obj.get_trim_min_max_tolerance()
+        (
+            spec_trim_min,
+            spec_trim_max,
+            spec_trim_tolerance,
+        ) = config_obj.get_trim_min_max_tolerance()
 
         # get the subgroups if any
-        subgroups = config_obj.get('subgroups')
+        subgroups = config_obj.get("subgroups")
 
         # get the candidate column if any and convert it to string
-        candidate_column = config_obj['candidate_column']
+        candidate_column = config_obj["candidate_column"]
 
         # check if we are excluding candidates based on number of responses
         exclude_listwise = config_obj.check_exclude_listwise()
-        min_items_per_candidate = config_obj['min_items_per_candidate']
+        min_items_per_candidate = config_obj["min_items_per_candidate"]
 
-        general_report_sections = config_obj['general_sections']
+        general_report_sections = config_obj["general_sections"]
 
         # get any special sections that the user might have specified
-        special_report_sections = config_obj['special_sections']
+        special_report_sections = config_obj["special_sections"]
 
         # get any custom sections and locate them to make sure
         # that they exist, otherwise raise an exception
-        custom_report_section_paths = config_obj['custom_sections']
+        custom_report_section_paths = config_obj["custom_sections"]
         if custom_report_section_paths:
-            self.logger.info('Locating custom report sections')
-            custom_report_sections = Reporter.locate_custom_sections(custom_report_section_paths,
-                                                                     configpath)
+            self.logger.info("Locating custom report sections")
+            custom_report_sections = Reporter.locate_custom_sections(
+                custom_report_section_paths, configpath
+            )
         else:
             custom_report_sections = []
 
-        section_order = config_obj['section_order']
+        section_order = config_obj["section_order"]
 
         # check all sections values and order and get the
         # ordered list of notebook files
-        chosen_notebook_files = Reporter().get_ordered_notebook_files(general_report_sections,
-                                                                      special_report_sections,
-                                                                      custom_report_sections,
-                                                                      section_order,
-                                                                      subgroups,
-                                                                      model_type=None,
-                                                                      context='rsmeval')
+        chosen_notebook_files = Reporter().get_ordered_notebook_files(
+            general_report_sections,
+            special_report_sections,
+            custom_report_sections,
+            section_order,
+            subgroups,
+            model_type=None,
+            context="rsmeval",
+        )
 
         # are we excluding zero scores?
-        exclude_zero_scores = config_obj['exclude_zero_scores']
+        exclude_zero_scores = config_obj["exclude_zero_scores"]
 
         # if we are excluding zero scores but trim_min
         # is set to 0, then we need to warn the user
         if exclude_zero_scores and spec_trim_min == 0:
-            self.logger.warning("'exclude_zero_scores' is set to True but "
-                                " 'trim_min' is set to 0. This may cause "
-                                " unexpected behavior.")
+            self.logger.warning(
+                "'exclude_zero_scores' is set to True but "
+                " 'trim_min' is set to 0. This may cause "
+                " unexpected behavior."
+            )
 
         # are we filtering on any other columns?
-        flag_column_dict = config_obj.check_flag_column(partition='test')
+        flag_column_dict = config_obj.check_flag_column(partition="test")
 
         # do we have the training set predictions and human scores CSV file
-        scale_with = config_obj.get('scale_with')
+        scale_with = config_obj.get("scale_with")
 
         # use scaled predictions for the analyses unless
         # we were told not to
-        use_scaled_predictions = (scale_with is not None)
+        use_scaled_predictions = scale_with is not None
 
         # log an appropriate message
         if scale_with is None:
-            message = ('Assuming given system predictions '
-                       'are unscaled and will be used as such.')
-        elif scale_with == 'asis':
-            message = ('Assuming given system predictions '
-                       'are already scaled and will be used as such.')
-        else:
-            message = ('Assuming given system predictions '
-                       'are unscaled and will be scaled before use.')
+            message = "Assuming given system predictions " "are unscaled and will be used as such."
+        elif scale_with == "asis":
+            message = (
+                "Assuming given system predictions " "are already scaled and will be used as such."
+            )
+        else:
+            message = (
+                "Assuming given system predictions " "are unscaled and will be scaled before use."
+            )
 
         self.logger.info(message)
 
         df_pred = data_container_obj.predictions
 
         # make sure that the columns specified in the config file actually exist
         columns_to_check = [id_column, human_score_column, system_score_column]
@@ -2112,201 +2193,237 @@
             columns_to_check.append(second_human_score_column)
 
         if candidate_column:
             columns_to_check.append(candidate_column)
 
         missing_columns = set(columns_to_check).difference(df_pred.columns)
         if missing_columns:
-            raise KeyError('Columns {} from the config file do not exist '
-                           'in the predictions file.'.format(missing_columns))
-
-        df_pred = self.rename_default_columns(df_pred,
-                                              [],
-                                              id_column,
-                                              human_score_column,
-                                              second_human_score_column,
-                                              None,
-                                              system_score_column,
-                                              candidate_column)
+            raise KeyError(
+                f"Columns {missing_columns} from the config file do not "
+                f"exist in the predictions file."
+            )
+
+        df_pred = self.rename_default_columns(
+            df_pred,
+            [],
+            id_column,
+            human_score_column,
+            second_human_score_column,
+            None,
+            system_score_column,
+            candidate_column,
+        )
 
         # check that the id_column contains unique values
-        if df_pred['spkitemid'].size != df_pred['spkitemid'].unique().size:
-            raise ValueError("The data contains duplicate response IDs "
-                             "in '{}'. Please make sure all response IDs "
-                             "are unique and re-run the tool.".format(id_column))
+        if df_pred["spkitemid"].size != df_pred["spkitemid"].unique().size:
+            raise ValueError(
+                f"The data contains duplicate response IDs in '{id_column}'. "
+                f"Please make sure all response IDs are unique and re-run the tool."
+            )
 
         df_pred = self.check_subgroups(df_pred, subgroups)
 
         # filter out the responses based on flag columns
-        (df_responses_with_requested_flags,
-         df_responses_with_excluded_flags) = self.filter_on_flag_columns(df_pred,
-                                                                         flag_column_dict)
+        (
+            df_responses_with_requested_flags,
+            df_responses_with_excluded_flags,
+        ) = self.filter_on_flag_columns(df_pred, flag_column_dict)
 
         # filter out rows that have non-numeric or zero human scores
-        df_filtered, df_excluded = self.filter_on_column(df_responses_with_requested_flags,
-                                                         'sc1',
-                                                         'spkitemid',
-                                                         exclude_zeros=exclude_zero_scores)
+        df_filtered, df_excluded = self.filter_on_column(
+            df_responses_with_requested_flags,
+            "sc1",
+            "spkitemid",
+            exclude_zeros=exclude_zero_scores,
+        )
 
         # make sure that the remaining data frame is not empty
         if len(df_filtered) == 0:
-            raise ValueError("No responses remaining after filtering out "
-                             "non-numeric human scores. No further analysis "
-                             "can be run. ")
+            raise ValueError(
+                "No responses remaining after filtering out "
+                "non-numeric human scores. No further analysis "
+                "can be run. "
+            )
 
         # Change all non-numeric machine scores in excluded
         # data to NaNs for consistency with rsmtool.
         # NOTE: This will *not* work if *all* of the values
         # in column are non-numeric. This is a known bug in
         # pandas: https://github.com/pydata/pandas/issues/9589
         # Therefore, we need add an additional check after this.
-        df_excluded['raw'] = pd.to_numeric(df_excluded['raw'], errors='coerce').astype(float)
+        df_excluded["raw"] = pd.to_numeric(df_excluded["raw"], errors="coerce").astype(float)
 
         # filter out the non-numeric machine scores from the rest of the data
-        newdf, newdf_excluded = self.filter_on_column(df_filtered,
-                                                      'raw',
-                                                      'spkitemid',
-                                                      exclude_zeros=False)
+        newdf, newdf_excluded = self.filter_on_column(
+            df_filtered, "raw", "spkitemid", exclude_zeros=False
+        )
 
         del df_filtered
         df_filtered_pred = newdf
 
         # make sure that the remaining data frame is not empty
         if len(df_filtered_pred) == 0:
-            raise ValueError("No responses remaining after filtering out "
-                             "non-numeric machine scores. No further analysis "
-                             "can be run. ")
+            raise ValueError(
+                "No responses remaining after filtering out "
+                "non-numeric machine scores. No further analysis "
+                "can be run. "
+            )
 
-        with np.errstate(divide='ignore'):
+        with np.errstate(divide="ignore"):
             df_excluded = pd.concat([df_excluded, newdf_excluded], sort=True)
 
         # if requested, exclude the candidates with less than X responses
         # left after filtering
         if exclude_listwise:
-            (df_filtered_candidates,
-             df_excluded_candidates) = self.select_candidates(df_filtered_pred,
-                                                              min_items_per_candidate)
+            (df_filtered_candidates, df_excluded_candidates) = self.select_candidates(
+                df_filtered_pred, min_items_per_candidate
+            )
 
             # check that there are still responses left for analysis
             if len(df_filtered_candidates) == 0:
-                raise ValueError("After filtering non-numeric human and system scores "
-                                 "there were "
-                                 "no candidates with {} or more responses "
-                                 "left for analysis".format(str(min_items_per_candidate)))
+                raise ValueError(
+                    f"After filtering non-numeric human and system scores "
+                    f"there were no candidates with {str(min_items_per_candidate)} "
+                    f"or more responses left for analysis."
+                )
 
             # redefine df_filtered_pred
             df_filtered_pred = df_filtered_candidates.copy()
 
             # update df_excluded
             df_excluded = pd.concat([df_excluded, df_excluded_candidates], sort=True)
-            df_excluded = df_excluded[['spkitemid'] + [column for column in df_excluded
-                                                       if column != 'spkitemid']]
+            df_excluded = df_excluded[
+                ["spkitemid"] + [column for column in df_excluded if column != "spkitemid"]
+            ]
 
         # set default values for scaling
         scale_pred_mean = 0
         scale_pred_sd = 1
         scale_human_mean = 0
         scale_human_sd = 1
 
-        if data_container_obj.get_frame('scale') is not None:
-            if ('sc1' not in data_container_obj.scale.columns and
-                    'prediction' not in data_container_obj.scale.columns):
-                raise KeyError('The CSV file specified for scaling ',
-                               'must have the "prediction" and the "sc1" '
-                               'columns.')
+        if data_container_obj.get_frame("scale") is not None:
+            if (
+                "sc1" not in data_container_obj.scale.columns
+                and "prediction" not in data_container_obj.scale.columns
+            ):
+                raise KeyError(
+                    "The CSV file specified for scaling ",
+                    'must have the "prediction" and the "sc1" ' "columns.",
+                )
             else:
-                scale_pred_mean, scale_pred_sd = (data_container_obj.scale['prediction'].mean(),
-                                                  data_container_obj.scale['prediction'].std())
-                scale_human_mean, scale_human_sd = (data_container_obj.scale['sc1'].mean(),
-                                                    data_container_obj.scale['sc1'].std())
-
-        self.logger.info('Processing predictions')
-        df_pred_processed = self.process_predictions(df_filtered_pred,
-                                                     scale_pred_mean,
-                                                     scale_pred_sd,
-                                                     scale_human_mean,
-                                                     scale_human_sd,
-                                                     spec_trim_min,
-                                                     spec_trim_max,
-                                                     spec_trim_tolerance)
+                scale_pred_mean, scale_pred_sd = (
+                    data_container_obj.scale["prediction"].mean(),
+                    data_container_obj.scale["prediction"].std(),
+                )
+                scale_human_mean, scale_human_sd = (
+                    data_container_obj.scale["sc1"].mean(),
+                    data_container_obj.scale["sc1"].std(),
+                )
+
+        self.logger.info("Processing predictions")
+        df_pred_processed = self.process_predictions(
+            df_filtered_pred,
+            scale_pred_mean,
+            scale_pred_sd,
+            scale_human_mean,
+            scale_human_sd,
+            spec_trim_min,
+            spec_trim_max,
+            spec_trim_tolerance,
+        )
         if not scale_with:
-            expected_score_types = ['raw', 'raw_trim', 'raw_trim_round']
-        elif scale_with == 'asis':
-            expected_score_types = ['scale', 'scale_trim', 'scale_trim_round']
-        else:
-            expected_score_types = ['raw', 'raw_trim', 'raw_trim_round',
-                                    'scale', 'scale_trim', 'scale_trim_round']
+            expected_score_types = ["raw", "raw_trim", "raw_trim_round"]
+        elif scale_with == "asis":
+            expected_score_types = ["scale", "scale_trim", "scale_trim_round"]
+        else:
+            expected_score_types = [
+                "raw",
+                "raw_trim",
+                "raw_trim_round",
+                "scale",
+                "scale_trim",
+                "scale_trim_round",
+            ]
 
         # extract separated data frames that we will write out
         # as separate files
         not_other_columns = set()
 
-        prediction_columns = ['spkitemid', 'sc1'] + expected_score_types
+        prediction_columns = ["spkitemid", "sc1"] + expected_score_types
         df_predictions_only = df_pred_processed[prediction_columns]
         not_other_columns.update(prediction_columns)
 
-        metadata_columns = ['spkitemid'] + subgroups
+        metadata_columns = ["spkitemid"] + subgroups
         if candidate_column:
-            metadata_columns.append('candidate')
+            metadata_columns.append("candidate")
         df_test_metadata = df_filtered_pred[metadata_columns]
         not_other_columns.update(metadata_columns)
 
         df_test_human_scores = pd.DataFrame()
-        human_score_columns = ['spkitemid', 'sc1', 'sc2']
-        if second_human_score_column and 'sc2' in df_filtered_pred:
+        human_score_columns = ["spkitemid", "sc1", "sc2"]
+        if second_human_score_column and "sc2" in df_filtered_pred:
             df_test_human_scores = df_filtered_pred[human_score_columns].copy()
-            not_other_columns.update(['sc2'])
+            not_other_columns.update(["sc2"])
             # filter out any non-numeric values nows
             # as well as zeros, if we were asked to
-            df_test_human_scores['sc2'] = pd.to_numeric(df_test_human_scores['sc2'],
-                                                        errors='coerce').astype(float)
+            df_test_human_scores["sc2"] = pd.to_numeric(
+                df_test_human_scores["sc2"], errors="coerce"
+            ).astype(float)
             if exclude_zero_scores:
-                df_test_human_scores['sc2'] = df_test_human_scores['sc2'].replace(0, np.nan)
+                df_test_human_scores["sc2"] = df_test_human_scores["sc2"].replace(0, np.nan)
 
         # remove 'spkitemid' from `not_other_columns`
         # because we want that in the other columns
         # data frame
-        not_other_columns.remove('spkitemid')
+        not_other_columns.remove("spkitemid")
 
         # extract all of the other columns in the predictions file
-        other_columns = [column for column in df_filtered_pred.columns
-                         if column not in not_other_columns]
+        other_columns = [
+            column for column in df_filtered_pred.columns if column not in not_other_columns
+        ]
 
         df_pred_other_columns = df_filtered_pred[other_columns]
 
         # add internal configuration options that we need
         new_config_obj = config_obj.copy()
-        internal_options_dict = {'pred_file_location': pred_file_location,
-                                 'exclude_listwise': exclude_listwise,
-                                 'use_scaled_predictions': use_scaled_predictions,
-                                 'chosen_notebook_files': chosen_notebook_files}
+        internal_options_dict = {
+            "pred_file_location": pred_file_location,
+            "exclude_listwise": exclude_listwise,
+            "use_scaled_predictions": use_scaled_predictions,
+            "chosen_notebook_files": chosen_notebook_files,
+        }
 
         for key, value in internal_options_dict.items():
             new_config_obj[key] = value
 
         # we need to make sure that `spkitemid` is the first column
-        df_excluded = df_excluded[['spkitemid'] + [column for column in df_excluded
-                                                   if column != 'spkitemid']]
-
-        frames = [df_predictions_only,
-                  df_test_metadata,
-                  df_pred_other_columns,
-                  df_test_human_scores,
-                  df_excluded,
-                  df_responses_with_excluded_flags]
-
-        names = ['pred_test',
-                 'test_metadata',
-                 'test_other_columns',
-                 'test_human_scores',
-                 'test_excluded',
-                 'test_responses_with_excluded_flags']
+        df_excluded = df_excluded[
+            ["spkitemid"] + [column for column in df_excluded if column != "spkitemid"]
+        ]
+
+        frames = [
+            df_predictions_only,
+            df_test_metadata,
+            df_pred_other_columns,
+            df_test_human_scores,
+            df_excluded,
+            df_responses_with_excluded_flags,
+        ]
+
+        names = [
+            "pred_test",
+            "test_metadata",
+            "test_other_columns",
+            "test_human_scores",
+            "test_excluded",
+            "test_responses_with_excluded_flags",
+        ]
 
-        new_container = [{'name': name, 'frame': frame}
-                         for frame, name in zip(frames, names)]
+        new_container = [{"name": name, "frame": frame} for frame, name in zip(frames, names)]
 
         new_container = DataContainer(new_container)
 
         return new_config_obj, new_container
 
     def process_data_rsmpredict(self, config_obj, data_container_obj):
         """
@@ -2338,153 +2455,170 @@
             If data contains duplicate response IDs.
         """
         df_input = data_container_obj.input_features
         df_feature_info = data_container_obj.feature_info
         df_postproc_params = data_container_obj.postprocessing_params
 
         # get the column name that will hold the ID
-        id_column = config_obj['id_column']
+        id_column = config_obj["id_column"]
 
         # get the column name for human score (if any)
-        human_score_column = config_obj['human_score_column']
+        human_score_column = config_obj["human_score_column"]
 
         # get the column name for second human score (if any)
-        second_human_score_column = config_obj['second_human_score_column']
+        second_human_score_column = config_obj["second_human_score_column"]
 
         # get the column name for subgroups (if any)
-        subgroups = config_obj['subgroups']
+        subgroups = config_obj["subgroups"]
 
         # get the model
-        model = config_obj['model']
+        model = config_obj["model"]
 
         # should features be standardized?
-        standardize_features = config_obj.get('standardize_features', True)
+        standardize_features = config_obj.get("standardize_features", True)
 
         # should we predict expected scores
-        predict_expected_scores = config_obj['predict_expected_scores']
+        predict_expected_scores = config_obj["predict_expected_scores"]
 
         # get the column names for flag columns (if any)
-        flag_column_dict = config_obj.check_flag_column(partition='test')
+        flag_column_dict = config_obj.check_flag_column(partition="test")
 
         # get the name for the candidate_column (if any)
-        candidate_column = config_obj['candidate_column']
+        candidate_column = config_obj["candidate_column"]
 
         # make sure that the columns specified in the config file actually exist
         columns_to_check = [id_column] + subgroups + list(flag_column_dict.keys())
 
         # add subgroups and the flag columns to the list of columns
         # that will be added to the final file
         columns_to_copy = subgroups + list(flag_column_dict.keys())
 
         # human_score_column will be set to sc1 by default
         # we only raise an error if it's set to something else.
         # However, since we cannot distinguish whether the column was set
         # to sc1 by default or specified as such in the config file
         # we append it to output anyway as long as
         # it is in the input file
-        if human_score_column != 'sc1' or 'sc1' in df_input.columns:
+        if human_score_column != "sc1" or "sc1" in df_input.columns:
             columns_to_check.append(human_score_column)
-            columns_to_copy.append('sc1')
+            columns_to_copy.append("sc1")
 
         if candidate_column:
             columns_to_check.append(candidate_column)
-            columns_to_copy.append('candidate')
+            columns_to_copy.append("candidate")
 
         if second_human_score_column:
             columns_to_check.append(second_human_score_column)
-            columns_to_copy.append('sc2')
+            columns_to_copy.append("sc2")
 
         missing_columns = set(columns_to_check).difference(df_input.columns)
         if missing_columns:
-            raise KeyError("Columns {} from the config file "
-                           "do not exist in the data.".format(missing_columns))
+            raise KeyError(
+                f"Columns {missing_columns} from the config file do not " f"exist in the data."
+            )
 
         # rename all columns
-        df_input = self.rename_default_columns(df_input,
-                                               [],
-                                               id_column,
-                                               human_score_column,
-                                               second_human_score_column,
-                                               None,
-                                               None,
-                                               candidate_column=candidate_column)
+        df_input = self.rename_default_columns(
+            df_input,
+            [],
+            id_column,
+            human_score_column,
+            second_human_score_column,
+            None,
+            None,
+            candidate_column=candidate_column,
+        )
 
         # check that the id_column contains unique values
-        if df_input['spkitemid'].size != df_input['spkitemid'].unique().size:
-            raise ValueError("The data contains repeated response IDs in {}. "
-                             "Please make sure all response IDs are unique and "
-                             "re-run the tool.".format(id_column))
-
-        (df_features_preprocessed,
-         df_excluded) = self.preprocess_new_data(df_input,
-                                                 df_feature_info,
-                                                 standardize_features)
-
-        trim_min = df_postproc_params['trim_min'].values[0]
-        trim_max = df_postproc_params['trim_max'].values[0]
-        h1_mean = df_postproc_params['h1_mean'].values[0]
-        h1_sd = df_postproc_params['h1_sd'].values[0]
+        if df_input["spkitemid"].size != df_input["spkitemid"].unique().size:
+            raise ValueError(
+                f"The data contains repeated response IDs in {id_column}. "
+                f"Please make sure all response IDs are unique and re-run the tool."
+            )
+
+        (df_features_preprocessed, df_excluded) = self.preprocess_new_data(
+            df_input, df_feature_info, standardize_features
+        )
+
+        trim_min = df_postproc_params["trim_min"].values[0]
+        trim_max = df_postproc_params["trim_max"].values[0]
+        h1_mean = df_postproc_params["h1_mean"].values[0]
+        h1_sd = df_postproc_params["h1_sd"].values[0]
 
         # if we are using a newly trained model, use trim_tolerance from the
         # df_postproc_params. If not, set it to the default value and show
         # warning
-        if 'trim_tolerance' in df_postproc_params:
-            trim_tolerance = df_postproc_params['trim_tolerance'].values[0]
+        if "trim_tolerance" in df_postproc_params:
+            trim_tolerance = df_postproc_params["trim_tolerance"].values[0]
         else:
             trim_tolerance = 0.4998
-            self.logger.warning("The tolerance for trimming scores will be assumed to be 0.4998, "
-                                "the default value in previous versions of RSMTool. "
-                                "We recommend re-training the model to ensure future "
-                                "compatibility.")
+            self.logger.warning(
+                "The tolerance for trimming scores will be assumed to be 0.4998, "
+                "the default value in previous versions of RSMTool. "
+                "We recommend re-training the model to ensure future "
+                "compatibility."
+            )
 
         # now generate the predictions for the features using this model
-        logged_str = 'Generating predictions'
-        logged_str += ' (expected scores).' if predict_expected_scores else '.'
+        logged_str = "Generating predictions"
+        logged_str += " (expected scores)." if predict_expected_scores else "."
         self.logger.info(logged_str)
 
         # compute minimum and maximum score for expected predictions
         min_score = int(np.rint(trim_min - trim_tolerance))
         max_score = int(np.rint(trim_max + trim_tolerance))
 
-        df_predictions = model.predict(df_features_preprocessed,
-                                       min_score,
-                                       max_score,
-                                       predict_expected=predict_expected_scores)
-
-        train_predictions_mean = df_postproc_params['train_predictions_mean'].values[0]
-        train_predictions_sd = df_postproc_params['train_predictions_sd'].values[0]
-
-        df_predictions = self.process_predictions(df_predictions,
-                                                  train_predictions_mean,
-                                                  train_predictions_sd,
-                                                  h1_mean,
-                                                  h1_sd,
-                                                  trim_min, trim_max,
-                                                  trim_tolerance)
+        df_predictions = model.predict(
+            df_features_preprocessed,
+            min_score,
+            max_score,
+            predict_expected=predict_expected_scores,
+        )
+
+        train_predictions_mean = df_postproc_params["train_predictions_mean"].values[0]
+        train_predictions_sd = df_postproc_params["train_predictions_sd"].values[0]
+
+        df_predictions = self.process_predictions(
+            df_predictions,
+            train_predictions_mean,
+            train_predictions_sd,
+            h1_mean,
+            h1_sd,
+            trim_min,
+            trim_max,
+            trim_tolerance,
+        )
 
         # add back the columns that we were requested to copy if any
         if len(columns_to_copy) > 0:
-            df_predictions_with_metadata = pd.merge(df_predictions,
-                                                    df_input[['spkitemid'] + columns_to_copy])
-            assert(len(df_predictions) == len(df_predictions_with_metadata))
+            df_predictions_with_metadata = pd.merge(
+                df_predictions, df_input[["spkitemid"] + columns_to_copy]
+            )
+            assert len(df_predictions) == len(df_predictions_with_metadata)
         else:
             df_predictions_with_metadata = df_predictions.copy()
 
         # we need to make sure that `spkitemid` is the first column
-        df_excluded = df_excluded[['spkitemid'] + [column for column in df_excluded
-                                                   if column != 'spkitemid']]
-
-        datasets = [{'name': 'features_processed', 'frame': df_features_preprocessed},
-                    {'name': 'excluded', 'frame': df_excluded},
-                    {'name': 'predictions_with_metadata', 'frame': df_predictions_with_metadata},
-                    {'name': 'predictions', 'frame': df_predictions}]
+        df_excluded = df_excluded[
+            ["spkitemid"] + [column for column in df_excluded if column != "spkitemid"]
+        ]
+
+        datasets = [
+            {"name": "features_processed", "frame": df_features_preprocessed},
+            {"name": "excluded", "frame": df_excluded},
+            {
+                "name": "predictions_with_metadata",
+                "frame": df_predictions_with_metadata,
+            },
+            {"name": "predictions", "frame": df_predictions},
+        ]
 
         return config_obj, DataContainer(datasets)
 
-    def process_data(self, config_obj, data_container_obj, context='rsmtool'):
+    def process_data(self, config_obj, data_container_obj, context="rsmtool"):
         """
         Process and setup the data for an experiment in the given context.
 
         Parameters
         ----------
         config_obj : configuration_parser.Configuration
             A configuration object.
@@ -2502,29 +2636,27 @@
             A new data container object.
 
         Raises
         ------
         ValueError
             If the context is not one of {"rsmtool", "rsmeval", "rsmpredict"}.
         """
-        if context == 'rsmtool':
+        if context == "rsmtool":
             return self.process_data_rsmtool(config_obj, data_container_obj)
-        elif context == 'rsmeval':
+        elif context == "rsmeval":
             return self.process_data_rsmeval(config_obj, data_container_obj)
-        elif context == 'rsmpredict':
+        elif context == "rsmpredict":
             return self.process_data_rsmpredict(config_obj, data_container_obj)
         else:
-            raise ValueError("The 'context' argument must be in the set: "
-                             "{'rsmtool', 'rsmeval', 'rsmpredict'}. "
-                             "You specified `{}`.".format(context))
-
-    def preprocess_new_data(self,
-                            df_input,
-                            df_feature_info,
-                            standardize_features=True):
+            raise ValueError(
+                f"The 'context' argument must be in the set: ['rsmtool', "
+                f"'rsmeval', 'rsmpredict']. You specified `{context}`."
+            )
+
+    def preprocess_new_data(self, df_input, df_feature_info, standardize_features=True):
         """
         Preprocess feature values using the parameters in ``df_feature_info``.
 
         For more details on what these preprocessing parameters are,
         see :ref:`documentation <preprocessing_parameters>`.
 
         Parameters
@@ -2573,120 +2705,133 @@
             responses.
         """
         # get the list of required features
         required_features = df_feature_info.index.tolist()
 
         # ensure that all the features that are needed by the model
         # are present in the input file
-        input_feature_columns = [c for c in df_input if c != 'spkitemid']
+        input_feature_columns = [c for c in df_input if c != "spkitemid"]
         missing_features = set(required_features).difference(input_feature_columns)
         if missing_features:
-            raise KeyError('The input feature file is missing the '
-                           'following features: {}'.format(missing_features))
+            raise KeyError(
+                f"The input feature file is missing the following features: {missing_features}"
+            )
 
-        extra_features = set(input_feature_columns).difference(required_features + ['spkitemid'])
+        extra_features = set(input_feature_columns).difference(required_features + ["spkitemid"])
         if extra_features:
-            self.logger.warning("The following extraneous features "
-                                "will be ignored: {}".format(extra_features))
+            self.logger.warning(
+                f"The following extraneous features will be ignored: {extra_features}"
+            )
 
         # keep the required features plus the id
-        features_to_keep = ['spkitemid'] + required_features
+        features_to_keep = ["spkitemid"] + required_features
 
         # check if actually have the human scores for this data and add
         # sc1 to preprocessed features for consistency with other tools
-        has_human_scores = 'sc1' in df_input
+        has_human_scores = "sc1" in df_input
         if has_human_scores:
-            features_to_keep.append('sc1')
+            features_to_keep.append("sc1")
 
         df_features = df_input[features_to_keep]
 
         # preprocess the feature values
-        self.logger.info('Pre-processing input features')
+        self.logger.info("Pre-processing input features")
 
         # first we need to filter out NaNs and any other
         # weird features, the same way we did for rsmtool.
         df_filtered = df_features.copy()
         df_excluded = pd.DataFrame(columns=df_filtered.columns)
 
         for feature_name in required_features:
-            newdf, newdf_excluded = self.filter_on_column(df_filtered,
-                                                          feature_name,
-                                                          'spkitemid',
-                                                          exclude_zeros=False,
-                                                          exclude_zero_sd=False)
+            newdf, newdf_excluded = self.filter_on_column(
+                df_filtered,
+                feature_name,
+                "spkitemid",
+                exclude_zeros=False,
+                exclude_zero_sd=False,
+            )
             del df_filtered
             df_filtered = newdf
-            with np.errstate(divide='ignore'):
+            with np.errstate(divide="ignore"):
                 df_excluded = pd.concat([df_excluded, newdf_excluded], sort=True)
 
         # make sure that the remaining data frame is not empty
         if len(df_filtered) == 0:
-            raise ValueError("There are no responses left after "
-                             "filtering out non-numeric feature values. No analysis "
-                             "will be run")
+            raise ValueError(
+                "There are no responses left after "
+                "filtering out non-numeric feature values. No analysis "
+                "will be run."
+            )
 
         df_features = df_filtered.copy()
         df_features_preprocess = df_features.copy()
         for feature_name in required_features:
 
             feature_values = df_features_preprocess[feature_name].values
 
-            feature_transformation = df_feature_info.loc[feature_name]['transform']
-            feature_sign = df_feature_info.loc[feature_name]['sign']
+            feature_transformation = df_feature_info.loc[feature_name]["transform"]
+            feature_sign = df_feature_info.loc[feature_name]["sign"]
 
-            train_feature_mean = df_feature_info.loc[feature_name]['train_mean']
-            train_feature_sd = df_feature_info.loc[feature_name]['train_sd']
+            train_feature_mean = df_feature_info.loc[feature_name]["train_mean"]
+            train_feature_sd = df_feature_info.loc[feature_name]["train_sd"]
 
-            train_transformed_mean = df_feature_info.loc[feature_name]['train_transformed_mean']
-            train_transformed_sd = df_feature_info.loc[feature_name]['train_transformed_sd']
+            train_transformed_mean = df_feature_info.loc[feature_name]["train_transformed_mean"]
+            train_transformed_sd = df_feature_info.loc[feature_name]["train_transformed_sd"]
 
             # transform the feature values and remove outliers
-            df_features_preprocess[feature_name] = self.preprocess_feature(feature_values,
-                                                                           feature_name,
-                                                                           feature_transformation,
-                                                                           train_feature_mean,
-                                                                           train_feature_sd,
-                                                                           exclude_zero_sd=False,
-                                                                           raise_error=False)
+            df_features_preprocess[feature_name] = self.preprocess_feature(
+                feature_values,
+                feature_name,
+                feature_transformation,
+                train_feature_mean,
+                train_feature_sd,
+                exclude_zero_sd=False,
+                raise_error=False,
+            )
 
             # filter the feature values once again to remove possible NaN and inf values that
             # might have emerged when applying transformations.
             # We do not need to do that if no transformation was applied.
-            if feature_transformation not in ['raw', 'org']:
+            if feature_transformation not in ["raw", "org"]:
                 # check that there are indeed inf or Nan values
-                if np.isnan(df_features_preprocess[feature_name]).any() or \
-                   np.isinf(df_features_preprocess[feature_name]).any():
-                    (newdf,
-                     newdf_excluded) = self.filter_on_column(df_features_preprocess,
-                                                             feature_name,
-                                                             'spkitemid',
-                                                             exclude_zeros=False,
-                                                             exclude_zero_sd=False)
+                if (
+                    np.isnan(df_features_preprocess[feature_name]).any()
+                    or np.isinf(df_features_preprocess[feature_name]).any()
+                ):
+                    (newdf, newdf_excluded) = self.filter_on_column(
+                        df_features_preprocess,
+                        feature_name,
+                        "spkitemid",
+                        exclude_zeros=False,
+                        exclude_zero_sd=False,
+                    )
                     del df_features_preprocess
                     df_features_preprocess = newdf
 
                     # add the response(s) with missing values to the excluded responses
                     # but make sure we are adding the original values, not the
                     # preprocessed ones
-                    missing_values = df_features['spkitemid'].isin(newdf_excluded['spkitemid'])
+                    missing_values = df_features["spkitemid"].isin(newdf_excluded["spkitemid"])
 
                     df_excluded_original = df_features[missing_values].copy()
-                    df_excluded = pd.merge(df_excluded, df_excluded_original, how='outer')
+                    df_excluded = pd.merge(df_excluded, df_excluded_original, how="outer")
 
             # print(standardized_features)
             if standardize_features:
 
                 # now standardize the feature values
-                df_feature_minus_mean = (df_features_preprocess[feature_name] -
-                                         train_transformed_mean)
-                df_features_preprocess[feature_name] = (df_feature_minus_mean /
-                                                        train_transformed_sd)
+                df_feature_minus_mean = (
+                    df_features_preprocess[feature_name] - train_transformed_mean
+                )
+                df_features_preprocess[feature_name] = df_feature_minus_mean / train_transformed_sd
 
             # Multiply features by sign.
-            df_features_preprocess[feature_name] = (df_features_preprocess[feature_name] *
-                                                    feature_sign)
+            df_features_preprocess[feature_name] = (
+                df_features_preprocess[feature_name] * feature_sign
+            )
 
         # we need to make sure that `spkitemid` is the first column
-        df_excluded = df_excluded[['spkitemid'] + [column for column in df_excluded
-                                                   if column != 'spkitemid']]
+        df_excluded = df_excluded[
+            ["spkitemid"] + [column for column in df_excluded if column != "spkitemid"]
+        ]
 
         return (df_features_preprocess, df_excluded)
```

### Comparing `rsmtool-9.0.1/rsmtool/reader.py` & `rsmtool-9.1.1/rsmtool/reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,38 +32,38 @@
     Parameters
     ----------
     filename: str
         Name of file to read.
     converters : dict, optional
         A dictionary specifying how the types of the columns
         in the file should be converted. Specified in the same
-        format as for `pd.read_csv() <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html>`_.
+        format as for ``pandas.read_csv()``.
         Defaults to ``None``.
 
     Returns
     -------
     df : pandas DataFrame
          Data frame containing the data in the given file.
     """
     try:
-        df = pd.read_json(filename,
-                          orient='records',
-                          lines=True,
-                          dtype=converters)
+        df = pd.read_json(filename, orient="records", lines=True, dtype=converters)
     except ValueError:
-        raise ValueError("The jsonlines file is not formatted correctly. "
-                         "Please check that each line ends with a comma, "
-                         "there is no comma at the end of the last line, "
-                         "and that all quotes match.")
+        raise ValueError(
+            "The jsonlines file is not formatted correctly. "
+            "Please check that each line ends with a comma, "
+            "there is no comma at the end of the last line, "
+            "and that all quotes match."
+        )
 
     # make sure we didn't get a plain json
     if type(df.columns) == pd.RangeIndex:
-        raise ValueError("It looks like {} is a simple json file. "
-                         "Please check documentation (for the expected "
-                         "file format".format(filename))
+        raise ValueError(
+            f"It looks like {filename} is a simple json file. Please "
+            f"check documentation (for the expected file format"
+        )
 
     dfs = []
     for column in df:
         # let's try to normalize this column
         try:
             df_column = pd.json_normalize(df[column])
 
@@ -81,33 +81,29 @@
         dfs.append(df_column)
 
     df = pd.concat(dfs, axis=1)
 
     return df
 
 
-def try_to_load_file(filename,
-                     converters=None,
-                     raise_error=False,
-                     raise_warning=False,
-                     **kwargs):
+def try_to_load_file(filename, converters=None, raise_error=False, raise_warning=False, **kwargs):
     """
     Read a single file, if it exists.
 
     Optionally raises an error or warning if the file cannot be found.
     Otherwise, returns ``None``.
 
     Parameters
     ----------
     filename : str
         Name of file to read.
     converters : dict, optional
         A dictionary specifying how the types of the columns
         in the file should be converted. Specified in the same
-        format as for `pd.read_csv() <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html>`_.
+        format as for ``pandas.read_csv()``.
         Defaults to ``None``.
     raise_error : bool, optional
         Raise an error if the file cannot be located.
         Defaults to ``False``.
     raise_warning : bool, optional
         Raise a warning if the file cannot be located.
         Defaults to ``False``.
@@ -122,29 +118,26 @@
     ------
     FileNotFoundError
         If ``raise_error`` is ``True`` and the file cannot be located.
     """
     if exists(filename):
         return DataReader.read_from_file(filename, converters, **kwargs)
 
-    message = "The file '{}' could not be located.".format(filename)
+    message = f"The file '{filename}' could not be located."
     if raise_error:
         raise FileNotFoundError(message)
 
     if raise_warning:
         warnings.warn(message)
 
 
 class DataReader:
     """Class to generate DataContainer objects."""
 
-    def __init__(self,
-                 filepaths,
-                 framenames,
-                 file_converters=None):
+    def __init__(self, filepaths, framenames, file_converters=None):
         """
         Initialize a DataReader object.
 
         Parameters
         ----------
         filepaths : list of str
             A list of paths to files that are to be read in.
@@ -172,46 +165,49 @@
         self.datasets = []
 
         # Make sure filepaths length matches frame names length
         assert len(filepaths) == len(framenames)
 
         # Make sure that there are no Nones in the filepaths
         if None in filepaths:
-            frames_with_no_path = [framenames[i] for i in range(len(framenames))
-                                   if filepaths[i] is None]
+            frames_with_no_path = [
+                framenames[i] for i in range(len(framenames)) if filepaths[i] is None
+            ]
 
-            raise ValueError("No path specified for "
-                             "{}".format(' ,'.join(frames_with_no_path)))
+            raise ValueError(f"No path specified for {' ,'.join(frames_with_no_path)}")
 
         # Assign names and paths lists
         self.dataset_names = framenames
         self.dataset_paths = filepaths
 
         # If `file_converters` exists, then
         # check to make sure it is the correct length
         # and add all elements to `file_converters` list
         if file_converters is not None:
             if not isinstance(file_converters, dict):
-                raise ValueError("The 'file_converters' argument must be a `dict`, "
-                                 "not `{}`.".format(type(file_converters)))
+                raise ValueError(
+                    f"The 'file_converters' argument must be a `dict`, "
+                    f"not `{type(file_converters)}`."
+                )
 
             for file_converter_name in file_converters:
                 # Make sure file_converter name is in `dataset_names`
                 if file_converter_name not in self.dataset_names:
-                    raise NameError('The file converter name ``{}`` '
-                                    'does not exist in the '
-                                    'dataset names that you '
-                                    'passed.'.format(file_converter_name))
+                    raise NameError(
+                        f"The file converter name ``{file_converter_name}`` "
+                        f"does not exist in the dataset names that you passed."
+                    )
 
                 # Make sure file converter is a `dict`
                 file_converter = file_converters[file_converter_name]
                 if not isinstance(file_converter, dict):
-                    raise ValueError('Value for {} must be``dict`` ',
-                                     'not {}'.format(file_converter_name,
-                                                     type(file_converter)))
+                    raise ValueError(
+                        f"Value for {file_converter_name} must be``dict`` "
+                        f"not {type(file_converter)}"
+                    )
 
         # Default file_converters dict
         self.file_converters = {} if file_converters is None else file_converters
 
     @staticmethod
     def read_from_file(filename, converters=None, **kwargs):
         """
@@ -220,15 +216,15 @@
         Parameters
         ----------
         filename : str
             Name of file to read.
         converters : dict, optional
             A dictionary specifying how the types of the columns
             in the file should be converted. Specified in the same
-            format as for `pd.read_csv() <https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html>`_.
+            format as for `pandas.read_csv()``.
             Defaults to ``None``.
 
         Returns
         -------
         df : pandas DataFrame
             Data frame containing the data in the given file.
 
@@ -242,43 +238,45 @@
         Note
         ----
         Any additional keyword arguments are passed to the underlying
         pandas IO reader function.
         """
         file_extension = splitext(filename)[1].lower()
 
-        if file_extension in ['.csv', '.tsv']:
-            sep = '\t' if file_extension == '.tsv' else ','
+        if file_extension in [".csv", ".tsv"]:
+            sep = "\t" if file_extension == ".tsv" else ","
             do_read = partial(pd.read_csv, sep=sep, converters=converters)
-        elif file_extension == '.xlsx':
+        elif file_extension == ".xlsx":
             do_read = partial(pd.read_excel, converters=converters)
-        elif file_extension == '.sas7bdat':
-            if 'encoding' not in kwargs:
-                encoding = 'latin-1'
+        elif file_extension == ".sas7bdat":
+            if "encoding" not in kwargs:
+                encoding = "latin-1"
             else:
-                encoding = kwargs.pop('encoding')
+                encoding = kwargs.pop("encoding")
             do_read = partial(pd.read_sas, encoding=encoding)
-        elif file_extension in ['.jsonlines']:
+        elif file_extension in [".jsonlines"]:
             do_read = partial(read_jsonlines, converters=converters)
         else:
-            raise ValueError("RSMTool only supports files in .csv, "
-                             ".tsv, .xlsx, and .sas7bdat formats. "
-                             "Input files should have one of these "
-                             "extensions. The file you "
-                             "passed is: {}.".format(filename))
+            raise ValueError(
+                f"RSMTool only supports files in .csv, .tsv, .xlsx, "
+                f"and .sas7bdat formats. Input files should have one "
+                f"of these extensions. The file you passed is: {filename}."
+            )
 
         # ignore warnings about mixed data types for large files
         with warnings.catch_warnings():
-            warnings.filterwarnings('ignore', category=DtypeWarning)
+            warnings.filterwarnings("ignore", category=DtypeWarning)
             try:
                 df = do_read(filename, **kwargs)
             except pd.errors.ParserError:
-                raise pd.errors.ParserError('Cannot read {}. Please check that it is '
-                                            'not corrupt or in an incompatible format. '
-                                            '(Try running dos2unix?)'.format(filename))
+                raise pd.errors.ParserError(
+                    f"Cannot read {filename}. Please check "
+                    f"that it is not corrupt or in an incompatible "
+                    f"format. (Try running dos2unix?)"
+                )
         return df
 
     @staticmethod
     def locate_files(filepaths, configdir):
         """
         Locate an experiment file, or a list of experiment files.
 
@@ -305,18 +303,18 @@
         Raises
         ------
         ValueError
             If ``filepaths`` is not a string or a list.
         """
         # the feature config file can be in the 'feature' directory
         # at the same level as the main config file
-        if not (isinstance(filepaths, str) or
-                isinstance(filepaths, list)):
-            raise ValueError("The 'filepaths' argument must be a "
-                             "string or a list, not {}.".format(type(filepaths)))
+        if not (isinstance(filepaths, str) or isinstance(filepaths, list)):
+            raise ValueError(
+                f"The 'filepaths' argument must be a string or a list, " f"not {type(filepaths)}."
+            )
 
         if isinstance(filepaths, str):
             filepaths = [filepaths]
             return_string = True
         else:
             return_string = False
 
@@ -366,22 +364,20 @@
         """
         for idx, set_path in enumerate(self.dataset_paths):
 
             name = self.dataset_names[idx]
             converter = self.file_converters.get(name, None)
 
             if not exists(set_path):
-                raise FileNotFoundError('The file {} does not exist'.format(set_path))
+                raise FileNotFoundError(f"The file {set_path} does not exist")
 
             if kwargs_dict is not None:
                 kwargs = kwargs_dict.get(name, {})
             else:
                 kwargs = {}
 
             dataframe = self.read_from_file(set_path, converter, **kwargs)
 
             # Add to list of datasets
-            self.datasets.append({'name': name.strip(),
-                                  'path': set_path,
-                                  'frame': dataframe})
+            self.datasets.append({"name": name.strip(), "path": set_path, "frame": dataframe})
 
         return DataContainer(self.datasets)
```

### Comparing `rsmtool-9.0.1/rsmtool/reporter.py` & `rsmtool-9.1.1/rsmtool/reporter.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,133 +20,167 @@
 from nbconvert.exporters.templateexporter import default_filters
 from traitlets.config import Config
 
 from . import HAS_RSMEXTRA
 from .reader import DataReader
 
 if HAS_RSMEXTRA:
-    from rsmextra.settings import (special_section_list_rsmtool, # noqa
-                                   special_section_list_rsmeval,
-                                   special_section_list_rsmcompare,
-                                   special_section_list_rsmsummarize,
-                                   ordered_section_list_with_special_sections_rsmtool,
-                                   ordered_section_list_with_special_sections_rsmeval,
-                                   ordered_section_list_with_special_sections_rsmcompare,
-                                   ordered_section_list_with_special_sections_rsmsummarize,
-                                   special_notebook_path)
+    from rsmextra.settings import (
+        ordered_section_list_with_special_sections_rsmcompare,
+        ordered_section_list_with_special_sections_rsmeval,
+        ordered_section_list_with_special_sections_rsmsummarize,
+        ordered_section_list_with_special_sections_rsmtool,
+        special_notebook_path,
+        special_section_list_rsmcompare,
+        special_section_list_rsmeval,
+        special_section_list_rsmsummarize,
+        special_section_list_rsmtool,
+    )
 
     ordered_section_list_rsmtool = ordered_section_list_with_special_sections_rsmtool
     ordered_section_list_rsmeval = ordered_section_list_with_special_sections_rsmeval
     ordered_section_list_rsmcompare = ordered_section_list_with_special_sections_rsmcompare
     ordered_section_list_rsmsummarize = ordered_section_list_with_special_sections_rsmsummarize
 
 else:
-    ordered_section_list_rsmtool = ['data_description',
-                                    'data_description_by_group',
-                                    'feature_descriptives',
-                                    'features_by_group',
-                                    'preprocessed_features',
-                                    'dff_by_group',
-                                    'consistency',
-                                    'model',
-                                    'evaluation',
-                                    'true_score_evaluation',
-                                    'evaluation_by_group',
-                                    'fairness_analyses',
-                                    'pca',
-                                    'intermediate_file_paths',
-                                    'sysinfo']
-
-    ordered_section_list_rsmeval = ['data_description',
-                                    'data_description_by_group',
-                                    'consistency',
-                                    'evaluation',
-                                    'true_score_evaluation',
-                                    'evaluation_by_group',
-                                    'fairness_analyses',
-                                    'intermediate_file_paths',
-                                    'sysinfo']
-
-    ordered_section_list_rsmcompare = ['feature_descriptives',
-                                       'features_by_group',
-                                       'preprocessed_features',
-                                       'preprocessed_features_by_group',
-                                       'consistency',
-                                       'score_distributions',
-                                       'model',
-                                       'evaluation',
-                                       'true_score_evaluation',
-                                       'pca',
-                                       'notes',
-                                       'sysinfo']
-
-    ordered_section_list_rsmsummarize = ['preprocessed_features',
-                                         'model',
-                                         'evaluation',
-                                         'true_score_evaluation',
-                                         'intermediate_file_paths',
-                                         'sysinfo']
+    ordered_section_list_rsmtool = [
+        "data_description",
+        "data_description_by_group",
+        "feature_descriptives",
+        "features_by_group",
+        "preprocessed_features",
+        "dff_by_group",
+        "consistency",
+        "model",
+        "evaluation",
+        "true_score_evaluation",
+        "evaluation_by_group",
+        "fairness_analyses",
+        "pca",
+        "intermediate_file_paths",
+        "sysinfo",
+    ]
+
+    ordered_section_list_rsmeval = [
+        "data_description",
+        "data_description_by_group",
+        "consistency",
+        "evaluation",
+        "true_score_evaluation",
+        "evaluation_by_group",
+        "fairness_analyses",
+        "intermediate_file_paths",
+        "sysinfo",
+    ]
+
+    ordered_section_list_rsmcompare = [
+        "feature_descriptives",
+        "features_by_group",
+        "preprocessed_features",
+        "preprocessed_features_by_group",
+        "consistency",
+        "score_distributions",
+        "model",
+        "evaluation",
+        "true_score_evaluation",
+        "pca",
+        "notes",
+        "sysinfo",
+    ]
+
+    ordered_section_list_rsmsummarize = [
+        "preprocessed_features",
+        "model",
+        "evaluation",
+        "true_score_evaluation",
+        "intermediate_file_paths",
+        "sysinfo",
+    ]
 
     special_section_list_rsmtool = []
     special_section_list_rsmcompare = []
     special_section_list_rsmeval = []
     special_section_list_rsmsummarize = []
     special_notebook_path = ""
 
 package_path = dirname(__file__)
-notebook_path = abspath(join(package_path, 'notebooks'))
-template_path = join(notebook_path, 'templates')
+notebook_path = abspath(join(package_path, "notebooks"))
+template_path = join(notebook_path, "templates")
 
-javascript_path = join(notebook_path, 'javascript')
-comparison_notebook_path = join(notebook_path, 'comparison')
-summary_notebook_path = join(notebook_path, 'summary')
+javascript_path = join(notebook_path, "javascript")
+comparison_notebook_path = join(notebook_path, "comparison")
+summary_notebook_path = join(notebook_path, "summary")
 
 
 # Define the general section list
 
-general_section_list_rsmtool = [section for section in ordered_section_list_rsmtool
-                                if section not in special_section_list_rsmtool]
-
-general_section_list_rsmeval = [section for section in ordered_section_list_rsmeval
-                                if section not in special_section_list_rsmeval]
-
-general_section_list_rsmcompare = [section for section in ordered_section_list_rsmcompare
-                                   if section not in special_section_list_rsmcompare]
-
-general_section_list_rsmsummarize = [section for section
-                                     in ordered_section_list_rsmsummarize
-                                     if section not in special_section_list_rsmsummarize]
+general_section_list_rsmtool = [
+    section
+    for section in ordered_section_list_rsmtool
+    if section not in special_section_list_rsmtool
+]
+
+general_section_list_rsmeval = [
+    section
+    for section in ordered_section_list_rsmeval
+    if section not in special_section_list_rsmeval
+]
+
+general_section_list_rsmcompare = [
+    section
+    for section in ordered_section_list_rsmcompare
+    if section not in special_section_list_rsmcompare
+]
+
+general_section_list_rsmsummarize = [
+    section
+    for section in ordered_section_list_rsmsummarize
+    if section not in special_section_list_rsmsummarize
+]
 
 
 # define a mapping from the tool name to the master
 # list for both general and special sections
-master_section_dict = {'general': {'rsmtool': general_section_list_rsmtool,
-                                   'rsmeval': general_section_list_rsmeval,
-                                   'rsmcompare': general_section_list_rsmcompare,
-                                   'rsmsummarize': general_section_list_rsmsummarize},
-                       'special': {'rsmtool': special_section_list_rsmtool,
-                                   'rsmeval': special_section_list_rsmeval,
-                                   'rsmcompare': special_section_list_rsmcompare,
-                                   'rsmsummarize': special_section_list_rsmsummarize}}
+master_section_dict = {
+    "general": {
+        "rsmtool": general_section_list_rsmtool,
+        "rsmeval": general_section_list_rsmeval,
+        "rsmcompare": general_section_list_rsmcompare,
+        "rsmsummarize": general_section_list_rsmsummarize,
+    },
+    "special": {
+        "rsmtool": special_section_list_rsmtool,
+        "rsmeval": special_section_list_rsmeval,
+        "rsmcompare": special_section_list_rsmcompare,
+        "rsmsummarize": special_section_list_rsmsummarize,
+    },
+}
 
 # define the mapping for section paths
-notebook_path_dict = {'general': {'rsmtool': notebook_path,
-                                  'rsmeval': notebook_path,
-                                  'rsmcompare': comparison_notebook_path,
-                                  'rsmsummarize': summary_notebook_path},
-                      'special': {'rsmtool': special_notebook_path,
-                                  'rsmeval': special_notebook_path,
-                                  'rsmcompare': special_notebook_path,
-                                  'rsmsummarize': special_notebook_path}}
+notebook_path_dict = {
+    "general": {
+        "rsmtool": notebook_path,
+        "rsmeval": notebook_path,
+        "rsmcompare": comparison_notebook_path,
+        "rsmsummarize": summary_notebook_path,
+    },
+    "special": {
+        "rsmtool": special_notebook_path,
+        "rsmeval": special_notebook_path,
+        "rsmcompare": special_notebook_path,
+        "rsmsummarize": special_notebook_path,
+    },
+}
 
 
 class Reporter:
     """Class to generate Jupyter notebook reports and convert them to HTML."""
 
     def __init__(self, logger=None):
+        """Initialize the Reporter object."""
         self.logger = logger if logger else logging.getLogger(__name__)
 
     @staticmethod
     def locate_custom_sections(custom_report_section_paths, configdir):
         """
         Locate custom report section files.
 
@@ -172,16 +206,15 @@
         FileNotFoundError
             If any of the files cannot be found.
         """
         custom_report_sections = []
         for cs_path in custom_report_section_paths:
             cs_location = DataReader.locate_files(cs_path, configdir)
             if not cs_location:
-                raise FileNotFoundError("Error: custom section not found at "
-                                        "{}.".format(cs_path))
+                raise FileNotFoundError(f"Error: custom section not found at {cs_path}.")
             else:
                 custom_report_sections.append(cs_location)
         return custom_report_sections
 
     @staticmethod
     def merge_notebooks(notebook_files, output_file):
         """
@@ -198,27 +231,25 @@
         ----
         Adapted from: https://stackoverflow.com/q/20454668.
         """
         # Merging ipython notebooks basically means that we keep the
         # metadata from the "first" notebook and then add in the cells
         # from all the other notebooks.
         first_notebook = notebook_files[0]
-        merged_notebook = json.loads(open(first_notebook, 'r', encoding='utf-8').read())
+        merged_notebook = json.loads(open(first_notebook, "r", encoding="utf-8").read())
         for notebook in notebook_files[1:]:
-            section_cells = json.loads(open(notebook, 'r', encoding='utf-8').read())["cells"]
-            merged_notebook['cells'].extend(section_cells)
+            section_cells = json.loads(open(notebook, "r", encoding="utf-8").read())["cells"]
+            merged_notebook["cells"].extend(section_cells)
 
         # output the merged cells into a report
-        with open(output_file, 'w') as outf:
+        with open(output_file, "w") as outf:
             json.dump(merged_notebook, outf, indent=1)
 
     @staticmethod
-    def check_section_names(specified_sections,
-                            section_type,
-                            context='rsmtool'):
+    def check_section_names(specified_sections, section_type, context="rsmtool"):
         """
         Validate the specified section names.
 
         This function checks whether the specified section names are valid
         and raises an exception if they are not.
 
         Parameters
@@ -237,21 +268,20 @@
         ValueError
             If any of the section names of the given type
             are not valid in the context of the given tool.
         """
         master_section_list = master_section_dict[section_type][context]
         invalid_section_names = set(specified_sections).difference(master_section_list)
         if invalid_section_names:
-            raise ValueError("The following {} report section "
-                             "names are invalid or not supported for {}: {}\n"
-                             "The following sections are currently "
-                             "available: {}".format(section_type,
-                                                    context,
-                                                    invalid_section_names,
-                                                    master_section_list))
+            raise ValueError(
+                f"The following {section_type} report section names are "
+                f"invalid or not supported for {context}: "
+                f"{invalid_section_names}\nThe following sections are "
+                f"currently available: {master_section_list}"
+            )
 
     @staticmethod
     def check_section_order(chosen_sections, section_order):
         """
         Check the order of the specified sections.
 
         Parameters
@@ -268,36 +298,37 @@
             from the list of chosen sections or vice versa.
         """
         if sorted(chosen_sections) != sorted(section_order):
 
             # check for discrepancies and create a helpful error message
             missing_sections = set(chosen_sections).difference(set(section_order))
             if missing_sections:
-                error_message_missing = ("'section_order' must list all "
-                                         "sections selected for your experiment: "
-                                         "Please edit section order to include the "
-                                         "following missing sections: "
-                                         "{}".format(', '.join(missing_sections)))
+                error_message_missing = (
+                    f"'section_order' must list all sections "
+                    f"selected for your experiment: Please edit "
+                    f"section order to include the following missing "
+                    f"sections: {', '.join(missing_sections)}"
+                )
 
             extra_sections = set(section_order).difference(set(chosen_sections))
             if extra_sections:
-                error_message_extra = ("'section order' can only include "
-                                       "sections availabe for this experiment. "
-                                       "The following sections are either unavailable "
-                                       "or were not selected for this experiment "
-                                       "{}".format(', '.join(extra_sections)))
+                error_message_extra = (
+                    f"'section order' can only include sections "
+                    f"available for this experiment. The following "
+                    f"sections are either unavailable or were not "
+                    f"selected for this experiment {', '.join(extra_sections)}"
+                )
 
             # raise an appropriate error message or a combination of messages
             if missing_sections and not extra_sections:
                 raise ValueError(error_message_missing)
             elif extra_sections and not missing_sections:
                 raise ValueError(error_message_extra)
             else:
-                raise ValueError("{}\n{}".format(error_message_missing,
-                                                 error_message_extra))
+                raise ValueError(f"{error_message_missing}\n{error_message_extra}")
 
     @staticmethod
     def convert_ipynb_to_html(notebook_file, html_file):
         """
         Convert given Jupyter notebook (``.ipynb``) to HTML file.
 
         Parameters
@@ -312,45 +343,50 @@
         This function is also exposed as the
         :ref:`render_notebook <render_notebook>` command-line utility.
         """
         # `nbconvert` uses `asyncio` which uses an entirely default
         # implemention of the event loop on Windows for Cpython 3.8
         # which breaks the report generation unless we include the
         # following workaround
-        if (sys.version_info[0] == 3 and
-                sys.version_info[1] >= 8 and
-                sys.platform.startswith('win')):
+        if sys.version_info[0] == 3 and sys.version_info[1] >= 8 and sys.platform.startswith("win"):
             asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
         # set a high timeout for datasets with a large number of features
-        report_config = Config({'ExecutePreprocessor': {'enabled': True,
-                                                        'timeout': 3600},
-                                'HTMLExporter': {"template_name": "classic",
-                                                 "template_file": join(template_path,
-                                                                       'report.tpl')}})
+        report_config = Config(
+            {
+                "ExecutePreprocessor": {"enabled": True, "timeout": 3600},
+                "HTMLExporter": {
+                    "template_name": "classic",
+                    "template_file": join(template_path, "report.tpl"),
+                },
+            }
+        )
 
         # newer versions of nbconvert use a "clean_html" filter that
         # break SVG rendering; so we override that filter here with
         # a custom function that is essentially a noop. For more
         # details, please refer to the following issue:
         # https://github.com/EducationalTestingService/rsmtool/issues/571
         def custom_clean_html(element):
             return element.decode() if isinstance(element, bytes) else str(element)
+
         default_filters["clean_html"] = custom_clean_html
 
         exportHtml = HTMLExporter(config=report_config)
         output, _ = exportHtml.from_filename(notebook_file)
-        open(html_file, mode='w', encoding='utf-8').write(output)
+        open(html_file, mode="w", encoding="utf-8").write(output)
 
-    def determine_chosen_sections(self,
-                                  general_sections,
-                                  special_sections,
-                                  custom_sections,
-                                  subgroups,
-                                  context='rsmtool'):
+    def determine_chosen_sections(
+        self,
+        general_sections,
+        special_sections,
+        custom_sections,
+        subgroups,
+        context="rsmtool",
+    ):
         """
         Compile a combined list of section names to be included in the report.
 
         Parameters
         ----------
         general_sections : list of str
             List of specified general section names.
@@ -376,70 +412,69 @@
         ------
         ValueError
             If a subgroup report section is requested but no
             subgroups were specified in the configuration file.
         """
         # 1. Include all general sections unless we are asked to include
         # a specific (and valid) subset.
-        general_section_list = master_section_dict['general'][context]
+        general_section_list = master_section_dict["general"][context]
         chosen_general_sections = general_section_list
         all_general_sections = True
 
-        if general_sections != ['all']:
-            self.check_section_names(general_sections, 'general', context)
-            chosen_general_sections = [s for s in general_sections
-                                       if s in general_section_list]
+        if general_sections != ["all"]:
+            self.check_section_names(general_sections, "general", context)
+            chosen_general_sections = [s for s in general_sections if s in general_section_list]
             all_general_sections = False
 
         # 2. Exclude the subgroup sections if we do not have subgroup information.
 
         if len(subgroups) == 0:
-            subgroup_sections = [section for section in chosen_general_sections
-                                 if section.endswith('by_group') or section == 'fairness_analyses']
+            subgroup_sections = [
+                section
+                for section in chosen_general_sections
+                if section.endswith("by_group") or section == "fairness_analyses"
+            ]
             # if we were given a list of general sections, raise an error if
             # that list included subgroup sections but no subgroups were specified
 
             if not all_general_sections and len(subgroup_sections) != 0:
-                raise ValueError("You requested sections for subgroup analysis "
-                                 "but did not specify any subgroups. "
-                                 "Please amend the config files to define "
-                                 "the subgroups or delete the following "
-                                 "sections from the list of sections: {}"
-                                 .format(', '.join(subgroup_sections)))
+                raise ValueError(
+                    f"You requested sections for subgroup analysis "
+                    f"but did not specify any subgroups. Please amend "
+                    f"the config files to define the subgroups or delete "
+                    f"the following sections from the list of sections: "
+                    f"{', '.join(subgroup_sections)}"
+                )
 
             # if we are using the default list, we simply remove the
             # subgroup sections
-            chosen_general_sections = [section for section in chosen_general_sections
-                                       if section not in subgroup_sections]
+            chosen_general_sections = [
+                section for section in chosen_general_sections if section not in subgroup_sections
+            ]
 
         # 3. Include the specified (and valid) subset of the special sections
         chosen_special_sections = []
         if special_sections:
-            special_section_list = master_section_dict['special'][context]
-            self.check_section_names(special_sections, 'special', context=context)
-            chosen_special_sections = [s for s in special_sections
-                                       if s in special_section_list]
+            special_section_list = master_section_dict["special"][context]
+            self.check_section_names(special_sections, "special", context=context)
+            chosen_special_sections = [s for s in special_sections if s in special_section_list]
 
         # 4. For the custom sections use the basename and strip off the `.ipynb` extension
         chosen_custom_sections = []
         if custom_sections:
             chosen_custom_sections = [splitext(basename(cs))[0] for cs in custom_sections]
 
         # return the final list of chosen sections
-        chosen_sections = (chosen_general_sections +
-                           chosen_special_sections +
-                           chosen_custom_sections)
+        chosen_sections = chosen_general_sections + chosen_special_sections + chosen_custom_sections
 
         return chosen_sections
 
-    def get_section_file_map(self,
-                             special_sections,
-                             custom_sections,
-                             model_type=None,
-                             context='rsmtool'):
+    def get_section_file_map(
+        self, special_sections, custom_sections, model_type=None, context="rsmtool"
+    ):
         """
         Map section names to IPython notebook filenames.
 
         Parameters
         ----------
         special_sections : list of str
             List of special sections.
@@ -458,51 +493,55 @@
         Returns
         -------
         section_file_map : dict
             Dictionary mapping each section name to the
             corresponding IPython notebook filename.
         """
         # create the original section file map for general sections
-        selected_notebook_path = notebook_path_dict['general'][context]
-        general_sections = master_section_dict['general'][context]
+        selected_notebook_path = notebook_path_dict["general"][context]
+        general_sections = master_section_dict["general"][context]
 
-        section_file_map = {s: join(selected_notebook_path, '{}.ipynb'.format(s))
-                            for s in general_sections + ['header', 'footer']}
+        section_file_map = {
+            s: join(selected_notebook_path, f"{s}.ipynb")
+            for s in general_sections + ["header", "footer"]
+        }
 
         # update the file map to point the 'model section to either the built-in
         # or the SKLL model notebook depending on the model type that
         # was passed in
-        if context == 'rsmtool' and model_type:
-            section_file_map['model'] = join(selected_notebook_path,
-                                             '{}_model.ipynb'.format(model_type.lower()))
+        if context == "rsmtool" and model_type:
+            section_file_map["model"] = join(
+                selected_notebook_path, f"{model_type.lower()}_model.ipynb"
+            )
 
         # update the file map to include the special sections
         if special_sections:
-            selected_special_notebook_path = notebook_path_dict['special'][context]
-            section_file_map.update({ss: join(selected_special_notebook_path,
-                                              "{}.ipynb".format(ss))
-                                     for ss in special_sections})
+            selected_special_notebook_path = notebook_path_dict["special"][context]
+            section_file_map.update(
+                {ss: join(selected_special_notebook_path, f"{ss}.ipynb") for ss in special_sections}
+            )
 
         # update the file map to include the custom sections with
         # the file names (without the `.ipynb` extension) as the
         # names (keys) and full paths as values
         if custom_sections:
-            section_file_map.update({splitext(basename(cs))[0]: cs
-                                     for cs in custom_sections})
+            section_file_map.update({splitext(basename(cs))[0]: cs for cs in custom_sections})
 
         return section_file_map
 
-    def get_ordered_notebook_files(self,
-                                   general_sections,
-                                   special_sections=[],
-                                   custom_sections=[],
-                                   section_order=None,
-                                   subgroups=[],
-                                   model_type=None,
-                                   context='rsmtool'):
+    def get_ordered_notebook_files(
+        self,
+        general_sections,
+        special_sections=[],
+        custom_sections=[],
+        section_order=None,
+        subgroups=[],
+        model_type=None,
+        context="rsmtool",
+    ):
         """
         Check all section names and the order of the sections.
 
         Combine all section names with the appropriate file mapping,
         and generate an ordered list of notebook files that are
         needed to generate the final report.
 
@@ -536,63 +575,60 @@
 
         Returns
         -------
         chosen_notebook_files : list of str
             List of the IPython notebook files that have
             to be rendered into the HTML report.
         """
-        chosen_sections = self.determine_chosen_sections(general_sections,
-                                                         special_sections,
-                                                         custom_sections,
-                                                         subgroups,
-                                                         context=context)
+        chosen_sections = self.determine_chosen_sections(
+            general_sections,
+            special_sections,
+            custom_sections,
+            subgroups,
+            context=context,
+        )
 
         # check to make sure that if a custom section ordering is
         # specified by the user, that it actually contains
         # *all* of the sections that have been chosen for the
         # final report.
         if section_order:
             self.check_section_order(chosen_sections, section_order)
 
         # determine which order to use by default
-        if context == 'rsmtool':
+        if context == "rsmtool":
             ordered_section_list = ordered_section_list_rsmtool
-        elif context == 'rsmeval':
+        elif context == "rsmeval":
             ordered_section_list = ordered_section_list_rsmeval
-        elif context == 'rsmcompare':
+        elif context == "rsmcompare":
             ordered_section_list = ordered_section_list_rsmcompare
-        elif context == 'rsmsummarize':
+        elif context == "rsmsummarize":
             ordered_section_list = ordered_section_list_rsmsummarize
 
         # add all custom sections to the end of the default ordered list
         ordered_section_list.extend([splitext(basename(cs))[0] for cs in custom_sections])
 
         # get the section file map
-        section_file_map = self.get_section_file_map(special_sections,
-                                                     custom_sections,
-                                                     model_type,
-                                                     context=context)
+        section_file_map = self.get_section_file_map(
+            special_sections, custom_sections, model_type, context=context
+        )
 
         # order the section list either according to the default
         # order in `ordered_section_list` or according to the custom
         # order that has been passed in via `section_order`
         order_to_use = section_order if section_order else ordered_section_list
         chosen_sections = [s for s in order_to_use if s in chosen_sections]
 
         # add the header and the footer to the chosen sections
-        chosen_sections = ['header'] + chosen_sections + ['footer']
+        chosen_sections = ["header"] + chosen_sections + ["footer"]
         chosen_notebook_files = [section_file_map[cs] for cs in chosen_sections]
 
         return chosen_notebook_files
 
-    def create_report(self,
-                      config,
-                      csvdir,
-                      figdir,
-                      context='rsmtool'):
+    def create_report(self, config, csvdir, figdir, context="rsmtool"):
         """
         Generate HTML report for an rsmtool/rsmeval experiment.
 
         Parameters
         ----------
         config : configuration_parser.Configuration
             A configuration object
@@ -607,101 +643,103 @@
 
         Raises
         ------
         KeyError
             If "test_file_location" or "pred_file_location" fields
             are not specified in the configuration.
         """
-        test_file_location = config.get('test_file_location')
+        test_file_location = config.get("test_file_location")
         if test_file_location is None:
-            test_file_location = config.get('pred_file_location')
+            test_file_location = config.get("pred_file_location")
 
         # raise error if location is still None
         if test_file_location is None:
-            raise KeyError('Could not find `test_file_location` or `pred_file_location` '
-                           'in Configuration object. Please make sure you have included '
-                           'one of these parameters in the configuration object.')
+            raise KeyError(
+                "Could not find `test_file_location` or `pred_file_location` "
+                "in Configuration object. Please make sure you have included "
+                "one of these parameters in the configuration object."
+            )
 
         # if the features subset file is None, just use empty string
-        feature_subset_file = ('' if config.get('feature_subset_file') is None
-                               else config['feature_subset_file'])
+        feature_subset_file = (
+            "" if config.get("feature_subset_file") is None else config["feature_subset_file"]
+        )
 
         # if the min items is None, just set it to zero
-        min_items = (0 if config['min_items_per_candidate'] is None
-                     else config['min_items_per_candidate'])
+        min_items = (
+            0 if config["min_items_per_candidate"] is None else config["min_items_per_candidate"]
+        )
 
         # determine minimum and maximum scores for trimming
-        (used_trim_min,
-         used_trim_max,
-         trim_tolerance) = config.get_trim_min_max_tolerance()
+        (
+            used_trim_min,
+            used_trim_max,
+            trim_tolerance,
+        ) = config.get_trim_min_max_tolerance()
         min_score = used_trim_min - trim_tolerance
         max_score = used_trim_max + trim_tolerance
 
-        environ_config = {'EXPERIMENT_ID': config['experiment_id'],
-                          'DESCRIPTION': config['description'],
-                          'MODEL_TYPE': config.get('model_type', ''),
-                          'MODEL_NAME': config.get('model_name', ''),
-                          'TRAIN_FILE_LOCATION': config.get('train_file_location', ''),
-                          'TEST_FILE_LOCATION': test_file_location,
-                          'SUBGROUPS': config.get('subgroups', []),
-                          'GROUPS_FOR_DESCRIPTIVES': config.get('subgroups', []),
-                          'GROUPS_FOR_EVALUATIONS': config.get('subgroups', []),
-                          'MIN_N_PER_GROUP': config.get('min_n_per_group', {}),
-                          'LENGTH_COLUMN': config.get('length_column', None),
-                          'H2_COLUMN': config['second_human_score_column'],
-                          'MIN_ITEMS': min_items,
-                          'FEATURE_SUBSET_FILE': feature_subset_file,
-                          'EXCLUDE_ZEROS': config.get('exclude_zero_scores', True),
-                          'SCALED': config.get('use_scaled_predictions', False),
-                          'MIN_SCORE': min_score,
-                          'MAX_SCORE': max_score,
-                          'STANDARDIZE_FEATURES': config.get('standardize_features', True),
-                          'FILE_FORMAT': config.get('file_format', 'csv'),
-                          'USE_THUMBNAILS': config.get('use_thumbnails', False),
-                          'SKLL_FIXED_PARAMETERS': config.get('skll_fixed_parameters', {}),
-                          'SKLL_OBJECTIVE': config.get('skll_objective', ''),
-                          'PREDICT_EXPECTED_SCORES': config.get('predict_expected_scores', False),
-                          'RATER_ERROR_VARIANCE': config.get('rater_error_variance', None),
-                          'CONTEXT': context,
-                          'JAVASCRIPT_PATH': javascript_path,
-                          'OUTPUT_DIR': csvdir,
-                          'FIGURE_DIR': figdir
-                          }
+        environ_config = {
+            "EXPERIMENT_ID": config["experiment_id"],
+            "DESCRIPTION": config["description"],
+            "MODEL_TYPE": config.get("model_type", ""),
+            "MODEL_NAME": config.get("model_name", ""),
+            "TRAIN_FILE_LOCATION": config.get("train_file_location", ""),
+            "TEST_FILE_LOCATION": test_file_location,
+            "SUBGROUPS": config.get("subgroups", []),
+            "GROUPS_FOR_DESCRIPTIVES": config.get("subgroups", []),
+            "GROUPS_FOR_EVALUATIONS": config.get("subgroups", []),
+            "MIN_N_PER_GROUP": config.get("min_n_per_group", {}),
+            "LENGTH_COLUMN": config.get("length_column", None),
+            "H2_COLUMN": config["second_human_score_column"],
+            "MIN_ITEMS": min_items,
+            "FEATURE_SUBSET_FILE": feature_subset_file,
+            "EXCLUDE_ZEROS": config.get("exclude_zero_scores", True),
+            "SCALED": config.get("use_scaled_predictions", False),
+            "MIN_SCORE": min_score,
+            "MAX_SCORE": max_score,
+            "STANDARDIZE_FEATURES": config.get("standardize_features", True),
+            "FILE_FORMAT": config.get("file_format", "csv"),
+            "USE_THUMBNAILS": config.get("use_thumbnails", False),
+            "SKLL_FIXED_PARAMETERS": config.get("skll_fixed_parameters", {}),
+            "SKLL_OBJECTIVE": config.get("skll_objective", ""),
+            "PREDICT_EXPECTED_SCORES": config.get("predict_expected_scores", False),
+            "RATER_ERROR_VARIANCE": config.get("rater_error_variance", None),
+            "CONTEXT": context,
+            "JAVASCRIPT_PATH": javascript_path,
+            "OUTPUT_DIR": csvdir,
+            "FIGURE_DIR": figdir,
+        }
 
         # get the report directory which is at the same level
         # as the output and the figure directory
-        reportdir = abspath(join(csvdir, '..', 'report'))
-        report_name = '{}_report'.format(config['experiment_id'])
-        merged_notebook_file = join(reportdir, '{}.ipynb'.format(report_name))
-        environ_config_file = join(reportdir, '.environ.json')
+        reportdir = abspath(join(csvdir, "..", "report"))
+        report_name = f"{config['experiment_id']}_report"
+        merged_notebook_file = join(reportdir, f"{report_name}.ipynb")
+        environ_config_file = join(reportdir, ".environ.json")
 
         # set the report directory as an environment variable
-        os.environ['RSM_REPORT_DIR'] = reportdir
+        os.environ["RSM_REPORT_DIR"] = reportdir
 
         # write out hidden environment JSON file
-        with open(environ_config_file, 'w') as out_environ_config:
+        with open(environ_config_file, "w") as out_environ_config:
             json.dump(environ_config, out_environ_config)
 
         # merge all the given sections
-        self.logger.info('Merging sections')
-        self.merge_notebooks(config['chosen_notebook_files'], merged_notebook_file)
+        self.logger.info("Merging sections")
+        self.merge_notebooks(config["chosen_notebook_files"], merged_notebook_file)
 
         # run the merged notebook and save the output as
         # an HTML file in the report directory
-        self.logger.info('Exporting HTML')
-        self.convert_ipynb_to_html(merged_notebook_file,
-                                   join(reportdir, '{}.html'.format(report_name)))
-
-    def create_comparison_report(self,
-                                 config,
-                                 csvdir_old,
-                                 figdir_old,
-                                 csvdir_new,
-                                 figdir_new,
-                                 output_dir):
+        self.logger.info("Exporting HTML")
+        self.convert_ipynb_to_html(merged_notebook_file, join(reportdir, f"{report_name}.html"))
+
+    def create_comparison_report(
+        self, config, csvdir_old, figdir_old, csvdir_new, figdir_new, output_dir
+    ):
         """
         Generate an HTML report for comparing two rsmtool experiments.
 
         Parameters
         ----------
         config : configuration_parser.Configuration
             A configuration object
@@ -713,115 +751,112 @@
             The new experiment CSV output directory.
         figdir_new : str
             The old figure output directory
         output_dir : str
             The output dir for the new report.
         """
         # whether to use scaled predictions for both new and old; default to false
-        use_scaled_predictions_old = config.get('use_scaled_predictions_old', False)
-        use_scaled_predictions_new = config.get('use_scaled_predictions_new', False)
+        use_scaled_predictions_old = config.get("use_scaled_predictions_old", False)
+        use_scaled_predictions_new = config.get("use_scaled_predictions_new", False)
 
-        environ_config = {'EXPERIMENT_ID_OLD': config['experiment_id_old'],
-                          'EXPERIMENT_ID_NEW': config['experiment_id_new'],
-                          'DESCRIPTION_OLD': config['description_old'],
-                          'DESCRIPTION_NEW': config['description_new'],
-                          'GROUPS_FOR_DESCRIPTIVES': config.get('subgroups', []),
-                          'GROUPS_FOR_EVALUATIONS': config.get('subgroups', []),
-                          'SCALED_OLD': use_scaled_predictions_old,
-                          'SCALED_NEW': use_scaled_predictions_new,
-                          'USE_THUMBNAILS': config.get('use_thumbnails', False),
-                          'JAVASCRIPT_PATH': javascript_path,
-                          'OUTPUT_DIR_NEW': csvdir_new,
-                          'FIGURE_DIR_NEW': figdir_new,
-                          'OUTPUT_DIR_OLD': csvdir_old,
-                          'FIGURE_DIR_OLD': figdir_old,
-                          }
+        environ_config = {
+            "EXPERIMENT_ID_OLD": config["experiment_id_old"],
+            "EXPERIMENT_ID_NEW": config["experiment_id_new"],
+            "DESCRIPTION_OLD": config["description_old"],
+            "DESCRIPTION_NEW": config["description_new"],
+            "GROUPS_FOR_DESCRIPTIVES": config.get("subgroups", []),
+            "GROUPS_FOR_EVALUATIONS": config.get("subgroups", []),
+            "SCALED_OLD": use_scaled_predictions_old,
+            "SCALED_NEW": use_scaled_predictions_new,
+            "USE_THUMBNAILS": config.get("use_thumbnails", False),
+            "JAVASCRIPT_PATH": javascript_path,
+            "OUTPUT_DIR_NEW": csvdir_new,
+            "FIGURE_DIR_NEW": figdir_new,
+            "OUTPUT_DIR_OLD": csvdir_old,
+            "FIGURE_DIR_OLD": figdir_old,
+        }
 
         # create the output directory
         os.makedirs(output_dir, exist_ok=True)
-        report_name = '{}_report'.format(config['comparison_id'])
-        merged_notebook_file = join(output_dir, '{}.ipynb'.format(report_name))
-        environ_config_file = join(output_dir, '.environ.json')
+        report_name = f"{config['comparison_id']}_report"
+        merged_notebook_file = join(output_dir, f"{report_name}.ipynb")
+        environ_config_file = join(output_dir, ".environ.json")
 
         # set the report directory as an environment variable
-        os.environ['RSM_REPORT_DIR'] = abspath(output_dir)
+        os.environ["RSM_REPORT_DIR"] = abspath(output_dir)
 
         # write out hidden environment JSON file
-        with open(environ_config_file, 'w') as out_environ_config:
+        with open(environ_config_file, "w") as out_environ_config:
             json.dump(environ_config, out_environ_config)
 
         # merge all the given sections
-        self.logger.info('Merging sections')
-        self.merge_notebooks(config['chosen_notebook_files'], merged_notebook_file)
+        self.logger.info("Merging sections")
+        self.merge_notebooks(config["chosen_notebook_files"], merged_notebook_file)
 
         # run the merged notebook and save the output as
         # an HTML file in the report directory
-        self.logger.info('Exporting HTML')
-        self.convert_ipynb_to_html(merged_notebook_file,
-                                   join(output_dir, '{}.html'.format(report_name)))
-
-    def create_summary_report(self,
-                              config,
-                              all_experiments,
-                              csvdir):
+        self.logger.info("Exporting HTML")
+        self.convert_ipynb_to_html(merged_notebook_file, join(output_dir, f"{report_name}.html"))
+
+    def create_summary_report(self, config, all_experiments, csvdir):
         """
         Generate an HTML report for summarizing the given rsmtool experiments.
 
         Parameters
         ----------
         config : configuration_parser.Configuration
             A configuration object
         all_experiments : list of str
             A list of experiment configuration files to summarize.
         csvdir : str
             The experiment CSV output directory.
         """
-        environ_config = {'SUMMARY_ID': config['summary_id'],
-                          'DESCRIPTION': config['description'],
-                          'GROUPS_FOR_DESCRIPTIVES': config.get('subgroups', []),
-                          'GROUPS_FOR_EVALUATIONS': config.get('subgroups', []),
-                          'USE_THUMBNAILS': config.get('use_thumbnails', False),
-                          'FILE_FORMAT': config.get('file_format', 'csv'),
-                          'JSONS': all_experiments,
-                          'JAVASCRIPT_PATH': javascript_path,
-                          'OUTPUT_DIR': csvdir
-                          }
-
-        report_name = '{}_report'.format(config['summary_id'])
-        reportdir = abspath(join(csvdir, '..', 'report'))
-        merged_notebook_file = join(reportdir, '{}.ipynb'.format(report_name))
-        environ_config_file = join(reportdir, '.environ.json')
+        environ_config = {
+            "SUMMARY_ID": config["summary_id"],
+            "DESCRIPTION": config["description"],
+            "GROUPS_FOR_DESCRIPTIVES": config.get("subgroups", []),
+            "GROUPS_FOR_EVALUATIONS": config.get("subgroups", []),
+            "USE_THUMBNAILS": config.get("use_thumbnails", False),
+            "FILE_FORMAT": config.get("file_format", "csv"),
+            "JSONS": all_experiments,
+            "JAVASCRIPT_PATH": javascript_path,
+            "OUTPUT_DIR": csvdir,
+        }
+
+        report_name = f"{config['summary_id']}_report"
+        reportdir = abspath(join(csvdir, "..", "report"))
+        merged_notebook_file = join(reportdir, f"{report_name}.ipynb")
+        environ_config_file = join(reportdir, ".environ.json")
 
         # set the report directory as an environment variable
-        os.environ['RSM_REPORT_DIR'] = reportdir
+        os.environ["RSM_REPORT_DIR"] = reportdir
 
         # write out hidden environment JSON file
-        with open(environ_config_file, 'w') as out_environ_config:
+        with open(environ_config_file, "w") as out_environ_config:
             json.dump(environ_config, out_environ_config)
 
         # merge all the given sections
-        self.logger.info('Merging sections')
-        self.merge_notebooks(config['chosen_notebook_files'], merged_notebook_file)
+        self.logger.info("Merging sections")
+        self.merge_notebooks(config["chosen_notebook_files"], merged_notebook_file)
 
         # run the merged notebook and save the output as
         # an HTML file in the report directory
-        self.logger.info('Exporting HTML')
-        self.convert_ipynb_to_html(merged_notebook_file,
-                                   join(reportdir, '{}.html'.format(report_name)))
+        self.logger.info("Exporting HTML")
+        self.convert_ipynb_to_html(merged_notebook_file, join(reportdir, f"{report_name}.html"))
 
 
 def main():  # noqa: D103
 
     # set up an argument parser
-    parser = argparse.ArgumentParser(prog='render_notebook')
-    parser.add_argument('ipynb_file', help="IPython notebook file")
-    parser.add_argument('html_file', help="output HTML file")
+    parser = argparse.ArgumentParser(prog="render_notebook")
+    parser.add_argument("ipynb_file", help="IPython notebook file")
+    parser.add_argument("html_file", help="output HTML file")
 
     # parse given command line arguments
     args = parser.parse_args()
 
     # convert notebook to HTML
     Reporter.convert_ipynb_to_html(args.ipynb_file, args.html_file)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `rsmtool-9.0.1/rsmtool/rsmcompare.py` & `rsmtool-9.1.1/rsmtool/rsmcompare.py`

 * *Files 14% similar despite different names*

```diff
@@ -35,23 +35,22 @@
 
     Raises
     ------
     FileNotFoundError
         If ``experiment_dir`` does not contain any outputs for ``experiment_id``.
     """
     # list all possible output files which start with experiment_id
-    outputs = glob.glob(join(experiment_dir,
-                             'output',
-                             '{}_*.*'.format(experiment_id)))
+    outputs = glob.glob(join(experiment_dir, "output", f"{experiment_id}_*.*"))
 
     # raise an error if none exists
     if len(outputs) == 0:
-        raise FileNotFoundError("The directory {} does not contain "
-                                "any outputs of an rsmtool experiment "
-                                "{}".format(experiment_dir, experiment_id))
+        raise FileNotFoundError(
+            f"The directory {experiment_dir} does not contain "
+            f"any outputs of an rsmtool experiment {experiment_id}"
+        )
 
 
 def run_comparison(config_file_or_obj_or_dict, output_dir):
     """
     Run an rsmcompare experiment using the given configuration.
 
     Use the given configuration file, object, or dictionary and generate
@@ -78,97 +77,103 @@
         If either of the two input directories in ``config_file_or_obj_or_dict``
         do not exist.
     FileNotFoundError
         If the directories do not contain rsmtool outputs at all.
     """
     logger = logging.getLogger(__name__)
 
-    configuration = configure('rsmcompare', config_file_or_obj_or_dict)
+    configuration = configure("rsmcompare", config_file_or_obj_or_dict)
 
-    logger.info('Saving configuration file.')
+    logger.info("Saving configuration file.")
     configuration.save(output_dir)
 
     # get the information about the "old" experiment
-    experiment_id_old = configuration['experiment_id_old']
-    experiment_dir_old = DataReader.locate_files(configuration['experiment_dir_old'],
-                                                 configuration.configdir)
+    experiment_id_old = configuration["experiment_id_old"]
+    experiment_dir_old = DataReader.locate_files(
+        configuration["experiment_dir_old"], configuration.configdir
+    )
     if not experiment_dir_old:
-        raise FileNotFoundError("The directory {} "
-                                "does not exist.".format(configuration['experiment_dir_old']))
+        raise FileNotFoundError(
+            f"The directory {configuration['experiment_dir_old']} " f"does not exist."
+        )
 
-    csvdir_old = normpath(join(experiment_dir_old, 'output'))
-    figdir_old = normpath(join(experiment_dir_old, 'figure'))
+    csvdir_old = normpath(join(experiment_dir_old, "output"))
+    figdir_old = normpath(join(experiment_dir_old, "figure"))
     if not exists(csvdir_old) or not exists(figdir_old):
-        raise FileNotFoundError("The directory {} does not contain "
-                                "the output of an rsmtool "
-                                "experiment.".format(experiment_dir_old))
+        raise FileNotFoundError(
+            f"The directory {experiment_dir_old} does not contain "
+            f"the output of an rsmtool experiment."
+        )
 
     check_experiment_id(experiment_dir_old, experiment_id_old)
 
     # get the information about the "new" experiment
-    experiment_id_new = configuration['experiment_id_new']
-    experiment_dir_new = DataReader.locate_files(configuration['experiment_dir_new'],
-                                                 configuration.configdir)
+    experiment_id_new = configuration["experiment_id_new"]
+    experiment_dir_new = DataReader.locate_files(
+        configuration["experiment_dir_new"], configuration.configdir
+    )
     if not experiment_dir_new:
-        raise FileNotFoundError("The directory {} "
-                                "does not exist.".format(configuration['experiment_dir_new']))
+        raise FileNotFoundError(
+            f"The directory {configuration['experiment_dir_new']} " f"does not exist."
+        )
 
-    csvdir_new = normpath(join(experiment_dir_new, 'output'))
-    figdir_new = normpath(join(experiment_dir_new, 'figure'))
+    csvdir_new = normpath(join(experiment_dir_new, "output"))
+    figdir_new = normpath(join(experiment_dir_new, "figure"))
     if not exists(csvdir_new) or not exists(figdir_new):
-        raise FileNotFoundError("The directory {} does not contain "
-                                "the output of an rsmtool "
-                                "experiment.".format(experiment_dir_new))
+        raise FileNotFoundError(
+            f"The directory {experiment_dir_new} does not contain the "
+            f"output of an rsmtool experiment."
+        )
 
     check_experiment_id(experiment_dir_new, experiment_id_new)
 
     # are there specific general report sections we want to include?
-    general_report_sections = configuration['general_sections']
+    general_report_sections = configuration["general_sections"]
 
     # what about the special or custom sections?
-    special_report_sections = configuration['special_sections']
+    special_report_sections = configuration["special_sections"]
 
-    custom_report_section_paths = configuration['custom_sections']
+    custom_report_section_paths = configuration["custom_sections"]
 
     # if custom report sections exist, locate sections; otherwise, create empty list
     if custom_report_section_paths:
-        logger.info('Locating custom report sections')
-        custom_report_sections = Reporter.locate_custom_sections(custom_report_section_paths,
-                                                                 configuration.configdir)
+        logger.info("Locating custom report sections")
+        custom_report_sections = Reporter.locate_custom_sections(
+            custom_report_section_paths, configuration.configdir
+        )
     else:
         custom_report_sections = []
 
     # get the section order
-    section_order = configuration['section_order']
+    section_order = configuration["section_order"]
 
     # get the subgroups if any
-    subgroups = configuration.get('subgroups')
+    subgroups = configuration.get("subgroups")
 
     # Initialize reporter
     reporter = Reporter(logger=logger)
 
-    chosen_notebook_files = reporter.get_ordered_notebook_files(general_report_sections,
-                                                                special_report_sections,
-                                                                custom_report_sections,
-                                                                section_order,
-                                                                subgroups,
-                                                                model_type=None,
-                                                                context='rsmcompare')
+    chosen_notebook_files = reporter.get_ordered_notebook_files(
+        general_report_sections,
+        special_report_sections,
+        custom_report_sections,
+        section_order,
+        subgroups,
+        model_type=None,
+        context="rsmcompare",
+    )
 
     # add chosen notebook files to configuration
-    configuration['chosen_notebook_files'] = chosen_notebook_files
+    configuration["chosen_notebook_files"] = chosen_notebook_files
 
     # now generate the comparison report
-    logger.info('Starting report generation.')
-    reporter.create_comparison_report(configuration,
-                                      csvdir_old,
-                                      figdir_old,
-                                      csvdir_new,
-                                      figdir_new,
-                                      output_dir)
+    logger.info("Starting report generation.")
+    reporter.create_comparison_report(
+        configuration, csvdir_old, figdir_old, csvdir_new, figdir_new, output_dir
+    )
 
 
 def main():  # noqa: D103
 
     # set up the basic logging configuration
     formatter = LogFormatter()
 
@@ -183,54 +188,57 @@
     stderr_handler = logging.StreamHandler(sys.stderr)
     stderr_handler.setFormatter(formatter)
 
     logging.root.setLevel(logging.INFO)
     logger = logging.getLogger(__name__)
 
     # set up an argument parser via our helper function
-    parser = setup_rsmcmd_parser('rsmcompare',
-                                 uses_output_directory=True,
-                                 uses_subgroups=True)
+    parser = setup_rsmcmd_parser("rsmcompare", uses_output_directory=True, uses_subgroups=True)
 
     # if we have no arguments at all then just show the help message
     if len(sys.argv) < 2:
         sys.argv.append("-h")
 
     # if the first argument is not one of the valid sub-commands
     # or one of the valid optional arguments, then assume that they
     # are arguments for the "run" sub-command. This allows the
     # old style command-line invocations to work without modification.
-    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + ['-h', '--help',
-                                                      '-V', '--version']:
-        args_to_pass = ['run'] + sys.argv[1:]
+    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + [
+        "-h",
+        "--help",
+        "-V",
+        "--version",
+    ]:
+        args_to_pass = ["run"] + sys.argv[1:]
     else:
         args_to_pass = sys.argv[1:]
     args = parser.parse_args(args=args_to_pass)
 
     # call the appropriate function based on which sub-command was run
-    if args.subcommand == 'run':
+    if args.subcommand == "run":
 
         # when running, log to stdout
         logging.root.addHandler(stdout_handler)
 
         # run the experiment
-        logger.info('Output directory: {}'.format(args.output_dir))
-        run_comparison(abspath(args.config_file),
-                       abspath(args.output_dir))
+        logger.info(f"Output directory: {args.output_dir}")
+        run_comparison(abspath(args.config_file), abspath(args.output_dir))
 
     else:
 
         # when generating, log to stderr
         logging.root.addHandler(stderr_handler)
 
         # auto-generate an example configuration and print it to STDOUT
-        generator = ConfigurationGenerator('rsmcompare',
-                                           as_string=True,
-                                           suppress_warnings=args.quiet,
-                                           use_subgroups=args.subgroups)
+        generator = ConfigurationGenerator(
+            "rsmcompare",
+            as_string=True,
+            suppress_warnings=args.quiet,
+            use_subgroups=args.subgroups,
+        )
         configuration = generator.interact() if args.interactive else generator.generate()
         print(configuration)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
 
     main()
```

### Comparing `rsmtool-9.0.1/rsmtool/rsmeval.py` & `rsmtool-9.1.1/rsmtool/rsmeval.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 from .reporter import Reporter
 from .utils.commandline import ConfigurationGenerator, setup_rsmcmd_parser
 from .utils.constants import VALID_PARSER_SUBCOMMANDS
 from .utils.logging import LogFormatter
 from .writer import DataWriter
 
 
-def run_evaluation(config_file_or_obj_or_dict,
-                   output_dir,
-                   overwrite_output=False,
-                   logger=None):
+def run_evaluation(config_file_or_obj_or_dict, output_dir, overwrite_output=False, logger=None):
     """
     Run an rsmeval experiment using the given configuration.
 
     All outputs are generated under ``output_dir``. If ``overwrite_output``
     is ``True``, any existing output in ``output_dir`` is overwritten.
 
     Parameters
@@ -67,156 +64,149 @@
         and ``overwrite_output`` is ``False``.
     """
     logger = logger if logger else logging.getLogger(__name__)
 
     # create the 'output' and the 'figure' sub-directories
     # where all the experiment output such as the CSV files
     # and the box plots will be saved
-    csvdir = abspath(join(output_dir, 'output'))
-    figdir = abspath(join(output_dir, 'figure'))
-    reportdir = abspath(join(output_dir, 'report'))
+    csvdir = abspath(join(output_dir, "output"))
+    figdir = abspath(join(output_dir, "figure"))
+    reportdir = abspath(join(output_dir, "report"))
     os.makedirs(csvdir, exist_ok=True)
     os.makedirs(figdir, exist_ok=True)
     os.makedirs(reportdir, exist_ok=True)
 
     # Raise an error if the specified output directory
     # already contains a non-empty `output` directory, unless
     # ``overwrite_output`` was specified, in which case we assume
     # that the user knows what she is doing and simply
     # output a warning saying that the report might
     # not be correct.
     non_empty_csvdir = exists(csvdir) and listdir(csvdir)
     if non_empty_csvdir:
         if not overwrite_output:
-            raise IOError("'{}' already contains a non-empty 'output' "
-                          "directory.".format(output_dir))
+            raise IOError(f"'{output_dir}' already contains a non-empty 'output' directory.")
         else:
-            logger.warning("{} already contains a non-empty 'output' directory. "
-                           "The generated report might contain "
-                           "unexpected information from a previous "
-                           "experiment.".format(output_dir))
+            logger.warning(
+                f"{output_dir} already contains a non-empty 'output' directory. "
+                f"The generated report might contain unexpected information "
+                f"from a previous experiment."
+            )
 
-    configuration = configure('rsmeval', config_file_or_obj_or_dict)
+    configuration = configure("rsmeval", config_file_or_obj_or_dict)
 
-    logger.info('Saving configuration file.')
+    logger.info("Saving configuration file.")
     configuration.save(output_dir)
 
     # Get output format
-    file_format = configuration.get('file_format', 'csv')
+    file_format = configuration.get("file_format", "csv")
 
     # Get DataWriter object
-    writer = DataWriter(configuration['experiment_id'])
+    writer = DataWriter(configuration["experiment_id"])
 
     # Make sure prediction file can be located
-    if not DataReader.locate_files(configuration['predictions_file'],
-                                   configuration.configdir):
-        raise FileNotFoundError('Error: Predictions file {} '
-                                'not found.\n'.format(configuration['predictions_file']))
+    if not DataReader.locate_files(configuration["predictions_file"], configuration.configdir):
+        raise FileNotFoundError(
+            f"Error: Predictions file {configuration['predictions_file']} " f"not found."
+        )
 
-    scale_with = configuration.get('scale_with')
+    scale_with = configuration.get("scale_with")
 
     # scale_with can be one of the following:
     # (a) None       : the predictions are assumed to be 'raw' and should be used as is
     #                  when computing the metrics; the names for the final columns are
     #                  'raw', 'raw_trim' and 'raw_trim_round'.
     # (b) 'asis'     : the predictions are assumed to be pre-scaled and should be used as is
     #                  when computing the metrics; the names for the final columns are
     #                  'scale', 'scale_trim' and 'scale_trim_round'.
     # (c) a CSV file : the predictions are assumed to be 'raw' and should be scaled
     #                  before computing the metrics; the names for the final columns are
     #                  'scale', 'scale_trim' and 'scale_trim_round'.
 
     # Check whether we want to do scaling
-    do_scaling = (scale_with is not None and
-                  scale_with != 'asis')
+    do_scaling = scale_with is not None and scale_with != "asis"
 
     # The paths to files and names for data container properties
-    paths = ['predictions_file']
-    names = ['predictions']
+    paths = ["predictions_file"]
+    names = ["predictions"]
 
     # If we want to do scaling, get the scale file
     if do_scaling:
 
         # Make sure scale file can be located
-        scale_file_location = DataReader.locate_files(scale_with,
-                                                      configuration.configdir)
+        scale_file_location = DataReader.locate_files(scale_with, configuration.configdir)
         if not scale_file_location:
-            raise FileNotFoundError('Could not find scaling file {}.'
-                                    ''.format(scale_file_location))
+            raise FileNotFoundError(f"Could not find scaling file {scale_file_location}.")
 
-        paths.append('scale_with')
-        names.append('scale')
+        paths.append("scale_with")
+        names.append("scale")
 
     # Get the paths, names, and converters for the DataReader
-    (file_names,
-     file_paths) = configuration.get_names_and_paths(paths, names)
+    (file_names, file_paths) = configuration.get_names_and_paths(paths, names)
 
     file_paths = DataReader.locate_files(file_paths, configuration.configdir)
 
-    converters = {'predictions': configuration.get_default_converter()}
+    converters = {"predictions": configuration.get_default_converter()}
 
-    logger.info('Reading predictions: {}.'.format(configuration['predictions_file']))
+    logger.info(f"Reading predictions: {configuration['predictions_file']}.")
 
     # Initialize the reader
     reader = DataReader(file_paths, file_names, converters)
     data_container = reader.read()
 
-    logger.info('Preprocessing predictions.')
+    logger.info("Preprocessing predictions.")
 
     # Initialize the processor
     processor = FeaturePreprocessor(logger=logger)
 
-    (processed_config,
-     processed_container) = processor.process_data(configuration,
-                                                   data_container,
-                                                   context='rsmeval')
-
-    logger.info('Saving pre-processed predictions and metadata to disk.')
-    writer.write_experiment_output(csvdir,
-                                   processed_container,
-                                   new_names_dict={'pred_test':
-                                                   'pred_processed',
-                                                   'test_excluded':
-                                                   'test_excluded_responses'},
-                                   file_format=file_format)
+    (processed_config, processed_container) = processor.process_data(
+        configuration, data_container, context="rsmeval"
+    )
+
+    logger.info("Saving pre-processed predictions and metadata to disk.")
+    writer.write_experiment_output(
+        csvdir,
+        processed_container,
+        new_names_dict={
+            "pred_test": "pred_processed",
+            "test_excluded": "test_excluded_responses",
+        },
+        file_format=file_format,
+    )
 
     # Initialize the analyzer
     analyzer = Analyzer(logger=logger)
 
     # do the data composition stats
-    (analyzed_config,
-     analyzed_container) = analyzer.run_data_composition_analyses_for_rsmeval(processed_container,
-                                                                              processed_config)
+    (
+        analyzed_config,
+        analyzed_container,
+    ) = analyzer.run_data_composition_analyses_for_rsmeval(processed_container, processed_config)
     # Write out files
-    writer.write_experiment_output(csvdir,
-                                   analyzed_container,
-                                   file_format=file_format)
+    writer.write_experiment_output(csvdir, analyzed_container, file_format=file_format)
 
     for_pred_data_container = analyzed_container + processed_container
 
     # run the analyses on the predictions of the model`
-    logger.info('Running analyses on predictions.')
-    (pred_analysis_config,
-     pred_analysis_data_container) = analyzer.run_prediction_analyses(for_pred_data_container,
-                                                                      analyzed_config)
-
-    writer.write_experiment_output(csvdir,
-                                   pred_analysis_data_container,
-                                   reset_index=True,
-                                   file_format=file_format)
+    logger.info("Running analyses on predictions.")
+    (
+        pred_analysis_config,
+        pred_analysis_data_container,
+    ) = analyzer.run_prediction_analyses(for_pred_data_container, analyzed_config)
+
+    writer.write_experiment_output(
+        csvdir, pred_analysis_data_container, reset_index=True, file_format=file_format
+    )
 
     # Initialize reporter
     reporter = Reporter(logger=logger)
 
     # generate the report
-    logger.info('Starting report generation.')
-    reporter.create_report(pred_analysis_config,
-                           csvdir,
-                           figdir,
-                           context='rsmeval')
+    logger.info("Starting report generation.")
+    reporter.create_report(pred_analysis_config, csvdir, figdir, context="rsmeval")
 
 
 def main():  # noqa: D103
 
     # set up the basic logging configuration
     formatter = LogFormatter()
 
@@ -231,55 +221,65 @@
     stderr_handler = logging.StreamHandler(sys.stderr)
     stderr_handler.setFormatter(formatter)
 
     logging.root.setLevel(logging.INFO)
     logger = logging.getLogger(__name__)
 
     # set up an argument parser via our helper function
-    parser = setup_rsmcmd_parser('rsmeval',
-                                 uses_output_directory=True,
-                                 allows_overwriting=True,
-                                 uses_subgroups=True)
+    parser = setup_rsmcmd_parser(
+        "rsmeval",
+        uses_output_directory=True,
+        allows_overwriting=True,
+        uses_subgroups=True,
+    )
 
     # if we have no arguments at all then just show the help message
     if len(sys.argv) < 2:
         sys.argv.append("-h")
 
     # if the first argument is not one of the valid sub-commands
     # or one of the valid optional arguments, then assume that they
     # are arguments for the "run" sub-command. This allows the
     # old style command-line invocations to work without modification.
-    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + ['-h', '--help',
-                                                      '-V', '--version']:
-        args_to_pass = ['run'] + sys.argv[1:]
+    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + [
+        "-h",
+        "--help",
+        "-V",
+        "--version",
+    ]:
+        args_to_pass = ["run"] + sys.argv[1:]
     else:
         args_to_pass = sys.argv[1:]
     args = parser.parse_args(args=args_to_pass)
 
     # call the appropriate function based on which sub-command was run
-    if args.subcommand == 'run':
+    if args.subcommand == "run":
 
         # when running, log to stdout
         logging.root.addHandler(stdout_handler)
 
         # run the experiment
-        logger.info('Output directory: {}'.format(args.output_dir))
-        run_evaluation(abspath(args.config_file),
-                       abspath(args.output_dir),
-                       overwrite_output=args.force_write)
+        logger.info(f"Output directory: {args.output_dir}")
+        run_evaluation(
+            abspath(args.config_file),
+            abspath(args.output_dir),
+            overwrite_output=args.force_write,
+        )
 
     else:
 
         # when generating, log to stderr
         logging.root.addHandler(stderr_handler)
 
         # auto-generate an example configuration and print it to STDOUT
-        generator = ConfigurationGenerator('rsmeval',
-                                           as_string=True,
-                                           suppress_warnings=args.quiet,
-                                           use_subgroups=args.subgroups)
+        generator = ConfigurationGenerator(
+            "rsmeval",
+            as_string=True,
+            suppress_warnings=args.quiet,
+            use_subgroups=args.subgroups,
+        )
         configuration = generator.interact() if args.interactive else generator.generate()
         print(configuration)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `rsmtool-9.0.1/rsmtool/rsmpredict.py` & `rsmtool-9.1.1/rsmtool/rsmtool.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,234 +1,325 @@
 #!/usr/bin/env python
+
 """
-Generate predictions on new data from rsmtool models.
+Run an rsmtool experiment.
 
 :author: Jeremy Biggs (jbiggs@ets.org)
 :author: Anastassia Loukina (aloukina@ets.org)
 :author: Nitin Madnani (nmadnani@ets.org)
 
 :organization: ETS
 """
 
-import glob
 import logging
-import os
 import sys
-from os.path import abspath, basename, dirname, exists, join, normpath, split, splitext
+from os import listdir, makedirs
+from os.path import abspath, exists, join
 
+from .analyzer import Analyzer
 from .configuration_parser import configure
 from .modeler import Modeler
 from .preprocessor import FeaturePreprocessor
 from .reader import DataReader
-from .utils.commandline import CmdOption, ConfigurationGenerator, setup_rsmcmd_parser
+from .reporter import Reporter
+from .utils.commandline import ConfigurationGenerator, setup_rsmcmd_parser
 from .utils.constants import VALID_PARSER_SUBCOMMANDS
 from .utils.logging import LogFormatter
 from .writer import DataWriter
 
 
-def compute_and_save_predictions(config_file_or_obj_or_dict,
-                                 output_file,
-                                 feats_file=None,
-                                 logger=None):
+def run_experiment(config_file_or_obj_or_dict, output_dir, overwrite_output=False, logger=None):
     """
-    Run rsmpredict using the given configuration.
+    Run an rsmtool experiment using the given configuration.
 
-    Generate predictions using given configuration file, object, or
-    dictionary. Predictions are saved in ``output_file``. Optionally,
-    pre-processed feature values are saved in ``feats_file``,
-    if specified.
+    Run rsmtool experiment using the given configuration file, object, or
+    dictionary. All outputs are generated under ``output_dir``. If
+    ``overwrite_output`` is ``True``, any existing output in ``output_dir``
+    is overwritten.
 
     Parameters
     ----------
     config_file_or_obj_or_dict : str or pathlib.Path or dict or Configuration
         Path to the experiment configuration file either a a string
         or as a ``pathlib.Path`` object. Users can also pass a
         ``Configuration`` object that is in memory or a Python dictionary
         with keys corresponding to fields in the configuration file. Given a
         configuration file, any relative paths in the configuration file
         will be interpreted relative to the location of the file. Given a
         ``Configuration`` object, relative paths will be interpreted
         relative to the ``configdir`` attribute, that _must_ be set. Given
         a dictionary, the reference path is set to the current directory.
-    output_file : str
-        The path to the output file.
-    feats_file : str, optional
-        Path to the output file for saving preprocessed feature values.
+    output_dir : str
+        Path to the experiment output directory.
+    overwrite_output : bool, optional
+        If ``True``, overwrite any existing output under ``output_dir``.
+        Defaults to ``False``.
     logger : logging object, optional
         A logging object. If ``None`` is passed, get logger from ``__name__``.
         Defaults to ``None``.
 
     Raises
     ------
     FileNotFoundError
-        If any of the files contained in ``config_file_or_obj_or_dict``
-        cannot be located.
-    FileNotFoundError
-        If ``experiment_dir`` does not exist.
-    FileNotFoundError
-        If ``experiment_dir`` does not contain the required output
-        needed from an rsmtool experiment.
-    RuntimeError
-        If the name of the output file does not end in
-        ".csv", ".tsv", or ".xlsx".
+        If any of the files contained in ``config_file_or_obj_or_dict`` cannot
+        be located.
+    IOError
+        If ``output_dir`` already contains the output of a previous experiment
+        and ``overwrite_output`` is ``False``.
+    ValueError
+        If the current configuration specifies a non-linear model but
+        ``output_dir`` already contains the output of a previous
+        experiment that used a linear model with the same experiment ID.
     """
     logger = logger if logger else logging.getLogger(__name__)
 
-    configuration = configure('rsmpredict', config_file_or_obj_or_dict)
+    # create the 'output' and the 'figure' sub-directories
+    # where all the experiment output such as the CSV files
+    # and the box plots will be saved
+
+    # Get absolute paths to output directories
+    csvdir = abspath(join(output_dir, "output"))
+    figdir = abspath(join(output_dir, "figure"))
+    reportdir = abspath(join(output_dir, "report"))
+    featuredir = abspath(join(output_dir, "feature"))
+
+    # Make directories, if necessary
+    makedirs(csvdir, exist_ok=True)
+    makedirs(figdir, exist_ok=True)
+    makedirs(reportdir, exist_ok=True)
+
+    # Raise an error if the specified output directory
+    # already contains a non-empty `output` directory, unless
+    # `overwrite_output` was specified, in which case we assume
+    # that the user knows what she is doing and simply
+    # output a warning saying that the report might
+    # not be correct.
+    non_empty_csvdir = exists(csvdir) and listdir(csvdir)
+    if non_empty_csvdir:
+        if not overwrite_output:
+            raise IOError(f"'{output_dir}' already contains a non-empty 'output' directory.")
+        else:
+            logger.warning(
+                f"{output_dir} already contains a non-empty 'output' directory. "
+                f"The generated report might contain unexpected information from "
+                f"a previous experiment."
+            )
 
-    # get the experiment ID
-    experiment_id = configuration['experiment_id']
+    configuration = configure("rsmtool", config_file_or_obj_or_dict)
+
+    logger.info("Saving configuration file.")
+    configuration.save(output_dir)
 
     # Get output format
-    file_format = configuration.get('file_format', 'csv')
+    file_format = configuration.get("file_format", "csv")
 
     # Get DataWriter object
-    writer = DataWriter(experiment_id)
+    writer = DataWriter(configuration["experiment_id"])
 
-    # get the input file containing the feature values
-    # for which we want to generate the predictions
-    input_features_file = DataReader.locate_files(configuration['input_features_file'],
-                                                  configuration.configdir)
-    if not input_features_file:
-        raise FileNotFoundError('Input file {} does not exist'
-                                ''.format(configuration['input_features_file']))
-
-    experiment_dir = DataReader.locate_files(configuration['experiment_dir'],
-                                             configuration.configdir)
-    if not experiment_dir:
-        raise FileNotFoundError('The directory {} does not exist.'
-                                ''.format(configuration['experiment_dir']))
-    else:
-        experiment_output_dir = normpath(join(experiment_dir, 'output'))
-        if not exists(experiment_output_dir):
-            raise FileNotFoundError('The directory {} does not contain '
-                                    'the output of an rsmtool experiment.'.format(experiment_dir))
-
-    # find all the .model files in the experiment output directory
-    model_files = glob.glob(join(experiment_output_dir, '*.model'))
-    if not model_files:
-        raise FileNotFoundError('The directory {} does not contain any rsmtool models.'
-                                ''.format(experiment_output_dir))
-
-    experiment_ids = [splitext(basename(mf))[0] for mf in model_files]
-    if experiment_id not in experiment_ids:
-        raise FileNotFoundError('{} does not contain a model for the experiment "{}". '
-                                'The following experiments are contained in this '
-                                'directory: {}'.format(experiment_output_dir,
-                                                       experiment_id,
-                                                       experiment_ids))
-
-    # check that the directory contains outher required files
-    required_file_types = ['feature', 'postprocessing_params']
-    for file_type in required_file_types:
-        expected_file_name = "{}_{}.csv".format(experiment_id, file_type)
-        if not exists(join(experiment_output_dir, expected_file_name)):
-            raise FileNotFoundError('{} does not contain the required file '
-                                    '{} that was generated during the '
-                                    'original model training'.format(experiment_output_dir,
-                                                                     expected_file_name))
-
-    logger.info('Reading input files.')
-
-    feature_info = join(experiment_output_dir,
-                        '{}_feature.csv'.format(experiment_id))
-
-    post_processing = join(experiment_output_dir,
-                           '{}_postprocessing_params.csv'.format(experiment_id))
-
-    file_paths = [input_features_file, feature_info, post_processing]
-    file_names = ['input_features',
-                  'feature_info',
-                  'postprocessing_params']
+    # Get the paths and names for the DataReader
+
+    (file_names, file_paths_org) = configuration.get_names_and_paths(
+        ["train_file", "test_file", "features", "feature_subset_file"],
+        ["train", "test", "feature_specs", "feature_subset_specs"],
+    )
+
+    file_paths = DataReader.locate_files(file_paths_org, configuration.configdir)
+
+    # if there are any missing files after trying to locate
+    # all expected files, raise an error
+    if None in file_paths:
+        missing_file_paths = [
+            file_paths_org[idx] for idx, path in enumerate(file_paths) if path is None
+        ]
+        raise FileNotFoundError(f"The following files were not found: {repr(missing_file_paths)}")
+
+    # Use the default converter for both train and test
+    converters = {
+        "train": configuration.get_default_converter(),
+        "test": configuration.get_default_converter(),
+    }
 
-    converters = {'input_features': configuration.get_default_converter()}
+    logger.info("Reading in all data from files.")
 
     # Initialize the reader
     reader = DataReader(file_paths, file_names, converters)
-    data_container = reader.read(kwargs_dict={'feature_info': {'index_col': 0}})
+    data_container = reader.read()
 
-    # load the Modeler to generate the predictions
-    model = Modeler.load_from_file(join(experiment_output_dir,
-                                        '{}.model'.format(experiment_id)))
-
-    # Add the model to the configuration object
-    configuration['model'] = model
+    logger.info("Preprocessing all features.")
 
     # Initialize the processor
     processor = FeaturePreprocessor(logger=logger)
 
-    (processed_config,
-     processed_container) = processor.process_data(configuration,
-                                                   data_container,
-                                                   context='rsmpredict')
-
-    # save the pre-processed features to disk if we were asked to
-    if feats_file is not None:
-        logger.info('Saving pre-processed feature values to {}'.format(feats_file))
-
-        feats_dir = dirname(feats_file)
-
-        # create any directories needed for the output file
-        os.makedirs(feats_dir, exist_ok=True)
-
-        _, feats_filename = split(feats_file)
-        feats_filename, _ = splitext(feats_filename)
-
-        # Write out files
-        writer.write_experiment_output(feats_dir,
-                                       processed_container,
-                                       include_experiment_id=False,
-                                       dataframe_names=['features_processed'],
-                                       new_names_dict={'features_processed':
-                                                       feats_filename},
-                                       file_format=file_format)
-
-    if (output_file.lower().endswith('.csv') or
-            output_file.lower().endswith('.xlsx')):
-
-        output_dir = dirname(output_file)
-        _, filename = split(output_file)
-        filename, _ = splitext(filename)
+    (processed_config, processed_container) = processor.process_data(configuration, data_container)
 
-    else:
-        output_dir = output_file
-        filename = 'predictions_with_metadata'
+    # Rename certain frames with more descriptive names
+    # for writing out experiment files
+    rename_dict = {
+        "train_excluded": "train_excluded_responses",
+        "test_excluded": "test_excluded_responses",
+        "train_length": "train_response_lengths",
+        "train_flagged": "train_responses_with_excluded_flags",
+        "test_flagged": "test_responses_with_excluded_flags",
+    }
 
-    # create any directories needed for the output file
-    os.makedirs(output_dir, exist_ok=True)
+    logger.info("Saving training and test set data to disk.")
 
-    # save the predictions to disk
-    logger.info('Saving predictions.')
+    # Write out files
+    writer.write_experiment_output(
+        csvdir,
+        processed_container,
+        [
+            "train_features",
+            "test_features",
+            "train_metadata",
+            "test_metadata",
+            "train_other_columns",
+            "test_other_columns",
+            "train_preprocessed_features",
+            "test_preprocessed_features",
+            "train_excluded",
+            "test_excluded",
+            "train_length",
+            "test_human_scores",
+            "train_flagged",
+            "test_flagged",
+        ],
+        rename_dict,
+        file_format=file_format,
+    )
+
+    # Initialize the analyzer
+    analyzer = Analyzer(logger=logger)
+
+    (_, analyzed_container) = analyzer.run_data_composition_analyses_for_rsmtool(
+        processed_container, processed_config
+    )
 
     # Write out files
-    writer.write_experiment_output(output_dir,
-                                   processed_container,
-                                   include_experiment_id=False,
-                                   dataframe_names=['predictions_with_metadata'],
-                                   new_names_dict={'predictions_with_metadata':
-                                                   filename},
-                                   file_format=file_format)
-
-    # save excluded responses to disk
-    if not processed_container.excluded.empty:
-
-        # save the predictions to disk
-        logger.info('Saving excluded responses to {}'.format(join(output_dir,
-                                                                  '{}_excluded_responses.csv'
-                                                                  ''.format(filename))))
-
-        # Write out files
-        writer.write_experiment_output(output_dir,
-                                       processed_container,
-                                       include_experiment_id=False,
-                                       dataframe_names=['excluded'],
-                                       new_names_dict={'excluded':
-                                                       '{}_excluded_responses'
-                                                       ''.format(filename)},
-                                       file_format=file_format)
+    writer.write_experiment_output(csvdir, analyzed_container, file_format=file_format)
+
+    logger.info(f"Training {processed_config['model_name']} model.")
+
+    # Initialize modeler
+    modeler = Modeler(logger=logger)
+
+    modeler.train(processed_config, processed_container, csvdir, figdir, file_format)
+
+    # Identify the features used by the model
+    selected_features = modeler.get_feature_names()
+
+    # Add selected features to processed configuration
+    processed_config["selected_features"] = selected_features
+
+    # Write out files
+    writer.write_feature_csv(
+        featuredir, processed_container, selected_features, file_format=file_format
+    )
+
+    features_data_container = processed_container.copy()
+
+    # Get selected feature info, and write out to file
+    df_feature_info = features_data_container.feature_info.copy()
+    df_selected_feature_info = df_feature_info[df_feature_info["feature"].isin(selected_features)]
+    selected_feature_dataset_dict = {
+        "name": "selected_feature_info",
+        "frame": df_selected_feature_info,
+    }
+
+    features_data_container.add_dataset(selected_feature_dataset_dict, update=True)
+
+    writer.write_experiment_output(
+        csvdir,
+        features_data_container,
+        dataframe_names=["selected_feature_info"],
+        new_names_dict={"selected_feature_info": "feature"},
+        file_format=file_format,
+    )
+
+    logger.info("Running analyses on training set.")
+
+    (_, train_analyzed_container) = analyzer.run_training_analyses(
+        processed_container, processed_config
+    )
+
+    # Write out files
+    writer.write_experiment_output(
+        csvdir, train_analyzed_container, reset_index=True, file_format=file_format
+    )
+
+    # Use only selected features for predictions
+    columns_for_prediction = ["spkitemid", "sc1"] + selected_features
+    train_for_prediction = processed_container.train_preprocessed_features[columns_for_prediction]
+    test_for_prediction = processed_container.test_preprocessed_features[columns_for_prediction]
+
+    logged_str = "Generating training and test set predictions"
+    logged_str += " (expected scores)." if configuration["predict_expected_scores"] else "."
+    logger.info(logged_str)
+    (pred_config, pred_data_container) = modeler.predict_train_and_test(
+        train_for_prediction, test_for_prediction, processed_config
+    )
+
+    # Write out files
+    writer.write_experiment_output(
+        csvdir,
+        pred_data_container,
+        new_names_dict={"pred_test": "pred_processed"},
+        file_format=file_format,
+    )
+
+    original_coef_file = join(csvdir, f"{pred_config['experiment_id']}_coefficients.{file_format}")
+
+    # If coefficients file exists, then try to generate the scaled
+    # coefficients and save them to a file
+    if exists(original_coef_file):
+        logger.info("Scaling the coefficients and saving them to disk")
+        try:
+
+            # scale coefficients, and return DataContainer w/ scaled coefficients
+            scaled_data_container = modeler.scale_coefficients(pred_config)
+
+        # raise an error if the coefficient file exists but the
+        # coefficients are not available for the current model
+        # which can happen if the user is re-running the same experiment
+        # with the same ID but with a non-linear model whereas the previous
+        # run of the same ID was with a linear model and the user has not
+        # cleared the directory
+        except RuntimeError:
+            raise ValueError(
+                "It appears you previously ran an experiment with the "
+                "same ID using a linear model and saved its output to "
+                "the same directory. That output is interfering with "
+                "the current experiment. Either clear the contents "
+                "of the output directory or re-run the current "
+                "experiment using a different experiment ID."
+            )
+        else:
+
+            # Write out scaled coefficients to disk
+            writer.write_experiment_output(csvdir, scaled_data_container, file_format=file_format)
+
+    # Add processed data_container frames to pred_data_container
+    new_pred_data_container = pred_data_container + processed_container
+
+    logger.info("Running prediction analyses.")
+    (
+        pred_analysis_config,
+        pred_analysis_data_container,
+    ) = analyzer.run_prediction_analyses(new_pred_data_container, pred_config)
+
+    # Write out files
+    writer.write_experiment_output(
+        csvdir, pred_analysis_data_container, reset_index=True, file_format=file_format
+    )
+    # Initialize reporter
+    reporter = Reporter(logger=logger)
+
+    # generate the report
+    logger.info("Starting report generation.")
+    reporter.create_report(pred_analysis_config, csvdir, figdir)
 
 
 def main():  # noqa: D103
 
     # set up the basic logging configuration
     formatter = LogFormatter()
 
@@ -239,66 +330,69 @@
     # generated configuration file
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setFormatter(formatter)
 
     stderr_handler = logging.StreamHandler(sys.stderr)
     stderr_handler.setFormatter(formatter)
 
-    # to set up the argument parser, we first need to instantiate options
-    # specific to rsmpredict so we use the `CmdOption` namedtuples
-    non_standard_options = [CmdOption(dest='output_file',
-                                      help="output file where predictions will be saved."),
-                            CmdOption(dest='preproc_feats_file',
-                                      help="if specified, the preprocessed features "
-                                           "will be saved in this file",
-                                      longname='features',
-                                      required=False)]
-
-    # now call the helper function to instantiate the parser for us
-    parser = setup_rsmcmd_parser('rsmpredict',
-                                 uses_output_directory=False,
-                                 extra_run_options=non_standard_options)
+    logging.root.setLevel(logging.INFO)
+    logger = logging.getLogger(__name__)
+
+    # set up an argument parser via our helper function
+    parser = setup_rsmcmd_parser(
+        "rsmtool",
+        uses_output_directory=True,
+        allows_overwriting=True,
+        uses_subgroups=True,
+    )
 
     # if we have no arguments at all then just show the help message
     if len(sys.argv) < 2:
         sys.argv.append("-h")
 
     # if the first argument is not one of the valid sub-commands
     # or one of the valid optional arguments, then assume that they
     # are arguments for the "run" sub-command. This allows the
     # old style command-line invocations to work without modification.
-    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + ['-h', '--help',
-                                                      '-V', '--version']:
-        args_to_pass = ['run'] + sys.argv[1:]
+    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + [
+        "-h",
+        "--help",
+        "-V",
+        "--version",
+    ]:
+        args_to_pass = ["run"] + sys.argv[1:]
     else:
         args_to_pass = sys.argv[1:]
     args = parser.parse_args(args=args_to_pass)
 
     # call the appropriate function based on which sub-command was run
-    if args.subcommand == 'run':
+    if args.subcommand == "run":
 
         # when running, log to stdout
         logging.root.addHandler(stdout_handler)
 
         # run the experiment
-        preproc_feats_file = None
-        if args.preproc_feats_file:
-            preproc_feats_file = abspath(args.preproc_feats_file)
-        compute_and_save_predictions(abspath(args.config_file),
-                                     abspath(args.output_file),
-                                     feats_file=preproc_feats_file)
+        logger.info(f"Output directory: {args.output_dir}")
+        run_experiment(
+            abspath(args.config_file),
+            abspath(args.output_dir),
+            overwrite_output=args.force_write,
+        )
 
     else:
 
         # when generating, log to stderr
         logging.root.addHandler(stderr_handler)
 
         # auto-generate an example configuration and print it to STDOUT
-        generator = ConfigurationGenerator('rsmpredict',
-                                           as_string=True,
-                                           suppress_warnings=args.quiet)
+        generator = ConfigurationGenerator(
+            "rsmtool",
+            as_string=True,
+            suppress_warnings=args.quiet,
+            use_subgroups=args.subgroups,
+        )
         configuration = generator.interact() if args.interactive else generator.generate()
         print(configuration)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `rsmtool-9.0.1/rsmtool/rsmsummarize.py` & `rsmtool-9.1.1/rsmtool/rsmsummarize.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,17 +20,15 @@
 from .reader import DataReader
 from .reporter import Reporter
 from .utils.commandline import ConfigurationGenerator, setup_rsmcmd_parser
 from .utils.constants import VALID_PARSER_SUBCOMMANDS
 from .utils.logging import LogFormatter
 
 
-def check_experiment_dir(experiment_dir,
-                         experiment_name,
-                         configpath):
+def check_experiment_dir(experiment_dir, experiment_name, configpath):
     """
     Check that ``experiment_dir`` exists & contains output for ``experiment_name``.
 
     Parameters
     ----------
     experiment_dir : str
         Supplied path to the experiment directory.
@@ -51,53 +49,52 @@
         If ``experiment_dir`` does not exist.
     FileNotFoundError
         If ``experiment_dir`` does not contain the output of the experiment.
     ValueError
         If ``experiment_dir`` contains several JSON configuration
         files instead of just one.
     """
-    full_path_experiment_dir = DataReader.locate_files(experiment_dir,
-                                                       configpath)
+    full_path_experiment_dir = DataReader.locate_files(experiment_dir, configpath)
     if not full_path_experiment_dir:
-        raise FileNotFoundError("The directory {} "
-                                "does not exist.".format(experiment_dir))
+        raise FileNotFoundError(f"The directory {experiment_dir} does not exist.")
     else:
         # check that there is an output directory
-        csvdir = normpath(join(full_path_experiment_dir, 'output'))
+        csvdir = normpath(join(full_path_experiment_dir, "output"))
         if not exists(csvdir):
-            raise FileNotFoundError("The directory {} does not contain "
-                                    "the output of an rsmtool "
-                                    "experiment.".format(full_path_experiment_dir))
+            raise FileNotFoundError(
+                f"The directory {full_path_experiment_dir} does "
+                f"not contain the output of an rsmtool experiment."
+            )
 
         # find the json configuration files for all experiments stored in this directory
-        jsons = glob.glob(join(csvdir, '*.json'))
+        jsons = glob.glob(join(csvdir, "*.json"))
         if len(jsons) == 0:
-            raise FileNotFoundError("The directory {} does not contain "
-                                    "the .json configuration files for rsmtool "
-                                    "experiments.".format(full_path_experiment_dir))
+            raise FileNotFoundError(
+                f"The directory {full_path_experiment_dir} does "
+                f"not contain the .json configuration files for "
+                f"rsmtool experiments."
+            )
 
         # Raise an error if the user specified a list of experiment names
         # but we found several .jsons in the same directory
         if experiment_name and len(jsons) > 1:
-            raise ValueError("{} seems to contain the output of multiple experiments. "
-                             "In order to use custom experiment names, you must have "
-                             "a separate directory "
-                             "for each experiment".format(full_path_experiment_dir))
+            raise ValueError(
+                f"{full_path_experiment_dir} seems to contain the output "
+                f"of multiple experiments. In order to use custom experiment "
+                f"names, you must have a separate directory for each experiment"
+            )
 
         # return [(json, experiment_name)] when we have experiment name or
         # [(json, None)] if no experiment name has been specified.
         # If the folder contains the output of multiple experiments, return
         # [(json1, None), (json2, None) .... ]
         return list(zip(jsons, [experiment_name] * len(jsons)))
 
 
-def run_summary(config_file_or_obj_or_dict,
-                output_dir,
-                overwrite_output=False,
-                logger=None):
+def run_summary(config_file_or_obj_or_dict, output_dir, overwrite_output=False, logger=None):
     """
     Run rsmsummarize experiment using the given configuration.
 
     Summarize several rsmtool experiments using the given configuration
     file, object, or dictionary. All outputs are generated under ``output_dir``.
     If ``overwrite_output`` is ``True``, any existing output in ``output_dir``
     is overwritten.
@@ -130,104 +127,103 @@
         and ``overwrite_output`` is ``False``.
     """
     logger = logger if logger else logging.getLogger(__name__)
 
     # create the 'output' and the 'figure' sub-directories
     # where all the experiment output such as the CSV files
     # and the box plots will be saved
-    csvdir = abspath(join(output_dir, 'output'))
-    figdir = abspath(join(output_dir, 'figure'))
-    reportdir = abspath(join(output_dir, 'report'))
+    csvdir = abspath(join(output_dir, "output"))
+    figdir = abspath(join(output_dir, "figure"))
+    reportdir = abspath(join(output_dir, "report"))
 
     os.makedirs(csvdir, exist_ok=True)
     os.makedirs(figdir, exist_ok=True)
     os.makedirs(reportdir, exist_ok=True)
 
     # Raise an error if the specified output directory
     # already contains a non-empty `output` directory, unless
     # `overwrite_output` was specified, in which case we assume
     # that the user knows what she is doing and simply
     # output a warning saying that the report might
     # not be correct.
     non_empty_csvdir = exists(csvdir) and listdir(csvdir)
     if non_empty_csvdir:
         if not overwrite_output:
-            raise IOError("'{}' already contains a non-empty 'output' "
-                          "directory.".format(output_dir))
+            raise IOError(f"'{output_dir}' already contains a non-empty 'output' directory.")
         else:
-            logger.warning("{} already contains a non-empty 'output' directory. "
-                           "The generated report might contain "
-                           "unexpected information from a previous "
-                           "experiment.".format(output_dir))
+            logger.warning(
+                f"{output_dir} already contains a non-empty 'output' directory. "
+                f"The generated report might contain unexpected information from "
+                f"a previous experiment."
+            )
 
-    configuration = configure('rsmsummarize', config_file_or_obj_or_dict)
+    configuration = configure("rsmsummarize", config_file_or_obj_or_dict)
 
-    logger.info('Saving configuration file.')
+    logger.info("Saving configuration file.")
     configuration.save(output_dir)
 
     # get the list of the experiment dirs
-    experiment_dirs = configuration['experiment_dirs']
+    experiment_dirs = configuration["experiment_dirs"]
 
     # Get experiment names if any
-    experiment_names = configuration.get('experiment_names')
+    experiment_names = configuration.get("experiment_names")
     experiment_names = experiment_names if experiment_names else [None] * len(experiment_dirs)
     dirs_with_names = zip(experiment_dirs, experiment_names)
 
     # check the experiment dirs and assemble the list of csvdir and jsons
     all_experiments = []
     for (experiment_dir, experiment_name) in dirs_with_names:
-        experiments = check_experiment_dir(experiment_dir,
-                                           experiment_name,
-                                           configuration.configdir)
+        experiments = check_experiment_dir(experiment_dir, experiment_name, configuration.configdir)
         all_experiments.extend(experiments)
 
     # get the subgroups if any
     # Note: at the moment no comparison are reported for subgroups.
     # this option is added to the code to make it easier to add
     # subgroup comparisons in future versions
-    subgroups = configuration.get('subgroups')
+    subgroups = configuration.get("subgroups")
 
-    general_report_sections = configuration['general_sections']
+    general_report_sections = configuration["general_sections"]
 
     # get any special sections that the user might have specified
-    special_report_sections = configuration['special_sections']
+    special_report_sections = configuration["special_sections"]
 
     # get any custom sections and locate them to make sure
     # that they exist, otherwise raise an exception
-    custom_report_section_paths = configuration['custom_sections']
+    custom_report_section_paths = configuration["custom_sections"]
     if custom_report_section_paths:
-        logger.info('Locating custom report sections')
-        custom_report_sections = Reporter.locate_custom_sections(custom_report_section_paths,
-                                                                 configuration.configdir)
+        logger.info("Locating custom report sections")
+        custom_report_sections = Reporter.locate_custom_sections(
+            custom_report_section_paths, configuration.configdir
+        )
     else:
         custom_report_sections = []
 
-    section_order = configuration['section_order']
+    section_order = configuration["section_order"]
 
     # Initialize reporter
     reporter = Reporter(logger=logger)
 
     # check all sections values and order and get the
     # ordered list of notebook files
-    chosen_notebook_files = reporter.get_ordered_notebook_files(general_report_sections,
-                                                                special_report_sections,
-                                                                custom_report_sections,
-                                                                section_order,
-                                                                subgroups,
-                                                                model_type=None,
-                                                                context='rsmsummarize')
+    chosen_notebook_files = reporter.get_ordered_notebook_files(
+        general_report_sections,
+        special_report_sections,
+        custom_report_sections,
+        section_order,
+        subgroups,
+        model_type=None,
+        context="rsmsummarize",
+    )
 
     # add chosen notebook files to configuration
-    configuration['chosen_notebook_files'] = chosen_notebook_files
+    configuration["chosen_notebook_files"] = chosen_notebook_files
 
     # now generate the comparison report
-    logger.info('Starting report generation')
-    reporter.create_summary_report(configuration,
-                                   all_experiments,
-                                   csvdir)
+    logger.info("Starting report generation")
+    reporter.create_summary_report(configuration, all_experiments, csvdir)
 
 
 def main():  # noqa: D103
 
     # set up the basic logging configuration
     formatter = LogFormatter()
 
@@ -242,53 +238,59 @@
     stderr_handler = logging.StreamHandler(sys.stderr)
     stderr_handler.setFormatter(formatter)
 
     logging.root.setLevel(logging.INFO)
     logger = logging.getLogger(__name__)
 
     # set up an argument parser via our helper function
-    parser = setup_rsmcmd_parser('rsmsummarize',
-                                 uses_output_directory=True,
-                                 allows_overwriting=True)
+    parser = setup_rsmcmd_parser(
+        "rsmsummarize", uses_output_directory=True, allows_overwriting=True
+    )
 
     # if we have no arguments at all then just show the help message
     if len(sys.argv) < 2:
         sys.argv.append("-h")
 
     # if the first argument is not one of the valid sub-commands
     # or one of the valid optional arguments, then assume that they
     # are arguments for the "run" sub-command. This allows the
     # old style command-line invocations to work without modification.
-    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + ['-h', '--help',
-                                                      '-V', '--version']:
-        args_to_pass = ['run'] + sys.argv[1:]
+    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + [
+        "-h",
+        "--help",
+        "-V",
+        "--version",
+    ]:
+        args_to_pass = ["run"] + sys.argv[1:]
     else:
         args_to_pass = sys.argv[1:]
     args = parser.parse_args(args=args_to_pass)
 
     # call the appropriate function based on which sub-command was run
-    if args.subcommand == 'run':
+    if args.subcommand == "run":
 
         # when running, log to stdout
         logging.root.addHandler(stdout_handler)
 
         # run the experiment
-        logger.info('Output directory: {}'.format(args.output_dir))
-        run_summary(abspath(args.config_file),
-                    abspath(args.output_dir),
-                    overwrite_output=args.force_write)
+        logger.info(f"Output directory: {args.output_dir}")
+        run_summary(
+            abspath(args.config_file),
+            abspath(args.output_dir),
+            overwrite_output=args.force_write,
+        )
 
     else:
 
         # when generating, log to stderr
         logging.root.addHandler(stderr_handler)
 
         # auto-generate an example configuration and print it to STDOUT
-        generator = ConfigurationGenerator('rsmsummarize',
-                                           as_string=True,
-                                           suppress_warnings=args.quiet)
+        generator = ConfigurationGenerator(
+            "rsmsummarize", as_string=True, suppress_warnings=args.quiet
+        )
         configuration = generator.interact() if args.interactive else generator.generate()
         print(configuration)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `rsmtool-9.0.1/rsmtool/rsmtool.py` & `rsmtool-9.1.1/rsmtool/rsmpredict.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,332 +1,394 @@
 #!/usr/bin/env python
-
 """
-Run an rsmtool experiment.
+Generate predictions on new data from rsmtool models.
 
 :author: Jeremy Biggs (jbiggs@ets.org)
 :author: Anastassia Loukina (aloukina@ets.org)
 :author: Nitin Madnani (nmadnani@ets.org)
 
 :organization: ETS
 """
 
+import glob
 import logging
+import os
 import sys
-from os import listdir, makedirs
-from os.path import abspath, exists, join
+from os.path import abspath, basename, dirname, exists, join, normpath, split, splitext
+
+import numpy as np
+import pandas as pd
 
-from .analyzer import Analyzer
 from .configuration_parser import configure
 from .modeler import Modeler
 from .preprocessor import FeaturePreprocessor
 from .reader import DataReader
-from .reporter import Reporter
-from .utils.commandline import ConfigurationGenerator, setup_rsmcmd_parser
+from .utils.commandline import CmdOption, ConfigurationGenerator, setup_rsmcmd_parser
 from .utils.constants import VALID_PARSER_SUBCOMMANDS
 from .utils.logging import LogFormatter
 from .writer import DataWriter
 
 
-def run_experiment(config_file_or_obj_or_dict,
-                   output_dir,
-                   overwrite_output=False,
-                   logger=None):
+def fast_predict(
+    input_features,
+    modeler,
+    df_feature_info,
+    trim_min=None,
+    trim_max=None,
+    trim_tolerance=0.4998,
+    train_predictions_mean=None,
+    train_predictions_sd=None,
+    h1_mean=None,
+    h1_sd=None,
+    logger=None,
+):
+    """
+    Compute predictions for a single instance against given model.
+
+    The main difference between this function and the ``compute_and_save_predictions()``
+    function is that the former is meant for batch prediction and reads
+    all its inputs from disk and writes its outputs to disk. This function,
+    however, is meant for real-time inference rather than batch. To this end,
+    it operates *entirely* in memory. Note that there is still a bit of overlap
+    between the two computation paths since we want to use the RSMTool API
+    as much as possible.
+
+    This function should only be used when the goal is to generate predictions
+    using RSMTool models in production. The user should read everything from disk
+    in a separate thread/function and pass the inputs to this function.
+
+    Note that this function only computes regular predictions, not expected
+    scores.
+
+    Parameters
+    ----------
+    input_features : dict[str, float]
+        A dictionary containing the features for the instance for which to
+        generate the model predictions. The keys should be names of the
+        features on which the model was trained and the values should
+        be the *raw* feature values.
+    modeler : rsmtool.modeler.Modeler object
+        The RSMTool modeler object using which the predictions
+        are to be generated. This object should be created from the already
+        existing model file in the "output" directory of the previously run
+        RSMTool experiment.
+    df_feature_info : pandas DataFrame
+        A DataFrame containing the information regarding the model features.
+        The index of the dataframe should be the names of the features and
+        the columns should be:
+
+        - "sign" : 1 or -1.  Indicates whether the feature value needs to
+          be multiplied by -1.
+        - "transform" : :ref:`transformation <select_transformations_rsmtool>`
+          that needs to be applied to this feature.
+        - "train_mean", "train_sd" : mean and standard deviation for outlier
+          truncation.
+        - "train_transformed_mean", "train_transformed_sd" : mean and standard
+          deviation for computing z-scores.
+
+        This dataframe should be read from the "feature.csv" file under the
+        "output" directory of the previously run RSMTool experiment.
+    trim_min : int, optional
+        The lowest possible integer score that the machine should predict.
+        If ``None``, raw predictions will not be trimmed.
+        Defaults to ``None``.
+    trim_max : int, optional
+        The highest possible integer score that the machine should predict.
+        If ``None``, raw predictions will not be trimmed.
+        Defaults to ``None``.
+    trim_tolerance : float, optional
+       The single numeric value that will be used to pad the trimming range
+       specified in ``trim_min`` and ``trim_max``.
+       Defaults to 0.4998.
+    train_predictions_mean : float, optional
+       The mean of the predictions on the training set used to re-scale the
+       predictions. May be read from the "postprocessing_params.csv" file
+       under the "output" directory of the RSMTool experiment used to train
+       the model. If ``None``, predictions will not be scaled.
+       Defaults to ``None``.
+    train_predictions_sd : float, optional
+       The standard deviation of the predictions on the training set used to
+       re-scale the predictions. May be read from the "postprocessing_params.csv"
+       file under the "output" directory of the RSMTool experiment used to train
+       the model.If ``None``, predictions will not be scaled.
+       Defaults to ``None``.
+    h1_mean : float, optional
+       The mean of the human scores in the training set also used to re-scale
+       the predictions. May be read from the "postprocessing_params.csv" file
+       under the "output" directory of the RSMTool experiment used to train
+       the model. If ``None``, predictions will not be scaled.
+       Defaults to ``None``.
+    h1_sd : float, optional
+       The standard deviation of the human scores in the training set used to
+       re-scale the predictions. May be read from the "postprocessing_params.csv"
+       file under the "output" directory of the RSMTool experiment used to train
+       the model. If ``None``, predictions will not be scaled.
+       Defaults to ``None``.
+    logger : logging object, optional
+        A logging object. If ``None`` is passed, get logger from ``__name__``.
+        Defaults to ``None``.
+
+    Returns
+    -------
+    dict[str, float]
+        A dictionary containing the raw, scaled, trimmed, and rounded
+        predictions for the input features. It always contains the
+        "raw" key and may contain the following additional keys depending
+        on the availability of the various optional arguments:
+        "raw_trim", "raw_trim_round", "scale", "scale_trim",
+        and "scale_trim_round".
+
+    Raises
+    ------
+    ValueError
+        If ``input_features`` contains any non-numeric features.
+    """
+    # initialize a logger if none provided
+    logger = logger if logger else logging.getLogger(__name__)
+
+    # instantiate a feature preprocessor
+    preprocessor = FeaturePreprocessor(logger=logger)
+
+    # convert the given features to a data frame and add the "spkitemid" column
+    df_input_features = pd.DataFrame([input_features])
+    df_input_features["spkitemid"] = "RESPONSE"
+
+    # preprocess the input features so that they match what the model expects
+    try:
+        df_processed_features, _ = preprocessor.preprocess_new_data(
+            df_input_features, df_feature_info
+        )
+    except ValueError:
+        raise ValueError("Input features must not contain non-numeric values.") from None
+
+    # now compute the raw prediction for the given features
+    df_predictions = modeler.predict(df_processed_features)
+
+    # compute scaled prediction if the scaling parameters are available
+    if train_predictions_mean and train_predictions_sd and h1_mean and h1_sd:
+        df_predictions["scale"] = (
+            (df_predictions["raw"] - train_predictions_mean) / train_predictions_sd
+        ) * h1_sd + h1_mean
+
+    # drop the spkitemid column since it's not needed from this point onwards
+    df_predictions.drop("spkitemid", axis="columns", inplace=True)
+
+    # trim both raw and scale predictions if ``trim_min`` and ``trim_max`` were specified
+    if trim_min and trim_max:
+        for column in df_predictions.columns:
+            df_predictions[f"{column}_trim"] = preprocessor.trim(
+                df_predictions[column], trim_min, trim_max, trim_tolerance
+            )
+            df_predictions[f"{column}_trim_round"] = np.rint(
+                df_predictions[f"{column}_trim"]
+            ).astype("int64")
+
+    # return the predictions as a dictionary
+    return df_predictions.to_dict(orient="records")[0]
+
+
+def compute_and_save_predictions(
+    config_file_or_obj_or_dict, output_file, feats_file=None, logger=None
+):
     """
-    Run an rsmtool experiment using the given configuration.
+    Run rsmpredict using the given configuration.
 
-    Run rsmtool experiment using the given configuration file, object, or
-    dictionary. All outputs are generated under ``output_dir``. If
-    ``overwrite_output`` is ``True``, any existing output in ``output_dir``
-    is overwritten.
+    Generate predictions using given configuration file, object, or
+    dictionary. Predictions are saved in ``output_file``. Optionally,
+    pre-processed feature values are saved in ``feats_file``,
+    if specified.
 
     Parameters
     ----------
     config_file_or_obj_or_dict : str or pathlib.Path or dict or Configuration
         Path to the experiment configuration file either a a string
         or as a ``pathlib.Path`` object. Users can also pass a
         ``Configuration`` object that is in memory or a Python dictionary
         with keys corresponding to fields in the configuration file. Given a
         configuration file, any relative paths in the configuration file
         will be interpreted relative to the location of the file. Given a
         ``Configuration`` object, relative paths will be interpreted
         relative to the ``configdir`` attribute, that _must_ be set. Given
         a dictionary, the reference path is set to the current directory.
-    output_dir : str
-        Path to the experiment output directory.
-    overwrite_output : bool, optional
-        If ``True``, overwrite any existing output under ``output_dir``.
-        Defaults to ``False``.
+    output_file : str
+        The path to the output file.
+    feats_file : str, optional
+        Path to the output file for saving preprocessed feature values.
     logger : logging object, optional
         A logging object. If ``None`` is passed, get logger from ``__name__``.
         Defaults to ``None``.
 
     Raises
     ------
     FileNotFoundError
-        If any of the files contained in ``config_file_or_obj_or_dict`` cannot
-        be located.
-    IOError
-        If ``output_dir`` already contains the output of a previous experiment
-        and ``overwrite_output`` is ``False``.
-    ValueError
-        If the current configuration specifies a non-linear model but
-        ``output_dir`` already contains the output of a previous
-        experiment that used a linear model with the same experiment ID.
+        If any of the files contained in ``config_file_or_obj_or_dict``
+        cannot be located.
+    FileNotFoundError
+        If ``experiment_dir`` does not exist.
+    FileNotFoundError
+        If ``experiment_dir`` does not contain the required output
+        needed from an rsmtool experiment.
+    RuntimeError
+        If the name of the output file does not end in
+        ".csv", ".tsv", or ".xlsx".
     """
     logger = logger if logger else logging.getLogger(__name__)
 
-    # create the 'output' and the 'figure' sub-directories
-    # where all the experiment output such as the CSV files
-    # and the box plots will be saved
-
-    # Get absolute paths to output directories
-    csvdir = abspath(join(output_dir, 'output'))
-    figdir = abspath(join(output_dir, 'figure'))
-    reportdir = abspath(join(output_dir, 'report'))
-    featuredir = abspath(join(output_dir, 'feature'))
-
-    # Make directories, if necessary
-    makedirs(csvdir, exist_ok=True)
-    makedirs(figdir, exist_ok=True)
-    makedirs(reportdir, exist_ok=True)
-
-    # Raise an error if the specified output directory
-    # already contains a non-empty `output` directory, unless
-    # `overwrite_output` was specified, in which case we assume
-    # that the user knows what she is doing and simply
-    # output a warning saying that the report might
-    # not be correct.
-    non_empty_csvdir = exists(csvdir) and listdir(csvdir)
-    if non_empty_csvdir:
-        if not overwrite_output:
-            raise IOError("'{}' already contains a non-empty 'output' "
-                          "directory.".format(output_dir))
-        else:
-            logger.warning("{} already contains a non-empty 'output' directory. "
-                           "The generated report might contain "
-                           "unexpected information from a previous "
-                           "experiment.".format(output_dir))
-
-    configuration = configure('rsmtool', config_file_or_obj_or_dict)
+    configuration = configure("rsmpredict", config_file_or_obj_or_dict)
 
-    logger.info('Saving configuration file.')
-    configuration.save(output_dir)
+    # get the experiment ID
+    experiment_id = configuration["experiment_id"]
 
     # Get output format
-    file_format = configuration.get('file_format', 'csv')
+    file_format = configuration.get("file_format", "csv")
 
     # Get DataWriter object
-    writer = DataWriter(configuration['experiment_id'])
+    writer = DataWriter(experiment_id)
 
-    # Get the paths and names for the DataReader
+    # get the input file containing the feature values
+    # for which we want to generate the predictions
+    input_features_file = DataReader.locate_files(
+        configuration["input_features_file"], configuration.configdir
+    )
+    if not input_features_file:
+        raise FileNotFoundError(f"Input file {configuration['input_features_file']} does not exist")
+
+    experiment_dir = DataReader.locate_files(
+        configuration["experiment_dir"], configuration.configdir
+    )
+    if not experiment_dir:
+        raise FileNotFoundError(f"The directory {configuration['experiment_dir']} does not exist.")
+    else:
+        experiment_output_dir = normpath(join(experiment_dir, "output"))
+        if not exists(experiment_output_dir):
+            raise FileNotFoundError(
+                f"The directory {experiment_dir} does not contain "
+                f"the output of an rsmtool experiment."
+            )
+
+    # find all the .model files in the experiment output directory
+    model_files = glob.glob(join(experiment_output_dir, "*.model"))
+    if not model_files:
+        raise FileNotFoundError(
+            f"The directory {experiment_output_dir} does not " f"contain any rsmtool models."
+        )
+
+    experiment_ids = [splitext(basename(mf))[0] for mf in model_files]
+    if experiment_id not in experiment_ids:
+        raise FileNotFoundError(
+            f"{experiment_output_dir} does not contain a model "
+            f'for the experiment "{experiment_id}". The following '
+            f"experiments are contained in this directory: {experiment_ids}"
+        )
+
+    # check that the directory contains outher required files
+    required_file_types = ["feature", "postprocessing_params"]
+    for file_type in required_file_types:
+        expected_file_name = f"{experiment_id}_{file_type}.csv"
+        if not exists(join(experiment_output_dir, expected_file_name)):
+            raise FileNotFoundError(
+                f"{experiment_output_dir} does not contain the "
+                f"required file {expected_file_name} that was "
+                f"generated during the original model training."
+            )
+
+    logger.info("Reading input files.")
 
-    (file_names,
-     file_paths_org) = configuration.get_names_and_paths(['train_file', 'test_file',
-                                                          'features',
-                                                          'feature_subset_file'],
-                                                         ['train', 'test',
-                                                          'feature_specs',
-                                                          'feature_subset_specs'])
-
-    file_paths = DataReader.locate_files(file_paths_org, configuration.configdir)
-
-    # if there are any missing files after trying to locate
-    # all expected files, raise an error
-    if None in file_paths:
-        missing_file_paths = [file_paths_org[idx] for idx, path in enumerate(file_paths)
-                              if path is None]
-        raise FileNotFoundError('The following files were not found: '
-                                '{}'.format(repr(missing_file_paths)))
-
-    # Use the default converter for both train and test
-    converters = {'train': configuration.get_default_converter(),
-                  'test': configuration.get_default_converter()}
+    feature_info = join(experiment_output_dir, f"{experiment_id}_feature.csv")
 
-    logger.info('Reading in all data from files.')
+    post_processing = join(experiment_output_dir, f"{experiment_id}_postprocessing_params.csv")
+
+    file_paths = [input_features_file, feature_info, post_processing]
+    file_names = ["input_features", "feature_info", "postprocessing_params"]
+
+    converters = {"input_features": configuration.get_default_converter()}
 
     # Initialize the reader
     reader = DataReader(file_paths, file_names, converters)
-    data_container = reader.read()
+    data_container = reader.read(kwargs_dict={"feature_info": {"index_col": 0}})
+
+    # load the Modeler to generate the predictions
+    model = Modeler.load_from_file(join(experiment_output_dir, f"{experiment_id}.model"))
 
-    logger.info('Preprocessing all features.')
+    # Add the model to the configuration object
+    configuration["model"] = model
 
     # Initialize the processor
     processor = FeaturePreprocessor(logger=logger)
 
-    (processed_config,
-     processed_container) = processor.process_data(configuration,
-                                                   data_container)
-
-    # Rename certain frames with more descriptive names
-    # for writing out experiment files
-    rename_dict = {'train_excluded': 'train_excluded_responses',
-                   'test_excluded': 'test_excluded_responses',
-                   'train_length': 'train_response_lengths',
-                   'train_flagged': 'train_responses_with_excluded_flags',
-                   'test_flagged': 'test_responses_with_excluded_flags'}
+    (processed_config, processed_container) = processor.process_data(
+        configuration, data_container, context="rsmpredict"
+    )
+
+    # save the pre-processed features to disk if we were asked to
+    if feats_file is not None:
+        logger.info(f"Saving pre-processed feature values to {feats_file}")
+
+        feats_dir = dirname(feats_file)
+
+        # create any directories needed for the output file
+        os.makedirs(feats_dir, exist_ok=True)
+
+        _, feats_filename = split(feats_file)
+        feats_filename, _ = splitext(feats_filename)
+
+        # Write out files
+        writer.write_experiment_output(
+            feats_dir,
+            processed_container,
+            include_experiment_id=False,
+            dataframe_names=["features_processed"],
+            new_names_dict={"features_processed": feats_filename},
+            file_format=file_format,
+        )
+
+    if output_file.lower().endswith(".csv") or output_file.lower().endswith(".xlsx"):
+
+        output_dir = dirname(output_file)
+        _, filename = split(output_file)
+        filename, _ = splitext(filename)
 
-    logger.info('Saving training and test set data to disk.')
-
-    # Write out files
-    writer.write_experiment_output(csvdir,
-                                   processed_container,
-                                   ['train_features',
-                                    'test_features',
-                                    'train_metadata',
-                                    'test_metadata',
-                                    'train_other_columns',
-                                    'test_other_columns',
-                                    'train_preprocessed_features',
-                                    'test_preprocessed_features',
-                                    'train_excluded',
-                                    'test_excluded',
-                                    'train_length',
-                                    'test_human_scores',
-                                    'train_flagged',
-                                    'test_flagged'],
-                                   rename_dict,
-                                   file_format=file_format)
-
-    # Initialize the analyzer
-    analyzer = Analyzer(logger=logger)
-
-    (_,
-     analyzed_container) = analyzer.run_data_composition_analyses_for_rsmtool(processed_container,
-                                                                              processed_config)
-
-    # Write out files
-    writer.write_experiment_output(csvdir,
-                                   analyzed_container,
-                                   file_format=file_format)
-
-    logger.info('Training {} model.'.format(processed_config['model_name']))
-
-    # Initialize modeler
-    modeler = Modeler(logger=logger)
-
-    modeler.train(processed_config,
-                  processed_container,
-                  csvdir,
-                  figdir,
-                  file_format)
-
-    # Identify the features used by the model
-    selected_features = modeler.get_feature_names()
-
-    # Add selected features to processed configuration
-    processed_config['selected_features'] = selected_features
-
-    # Write out files
-    writer.write_feature_csv(featuredir,
-                             processed_container,
-                             selected_features,
-                             file_format=file_format)
-
-    features_data_container = processed_container.copy()
-
-    # Get selected feature info, and write out to file
-    df_feature_info = features_data_container.feature_info.copy()
-    df_selected_feature_info = df_feature_info[df_feature_info['feature'].isin(selected_features)]
-    selected_feature_dataset_dict = {'name': 'selected_feature_info',
-                                     'frame': df_selected_feature_info}
-
-    features_data_container.add_dataset(selected_feature_dataset_dict,
-                                        update=True)
-
-    writer.write_experiment_output(csvdir,
-                                   features_data_container,
-                                   dataframe_names=['selected_feature_info'],
-                                   new_names_dict={'selected_feature_info': 'feature'},
-                                   file_format=file_format)
-
-    logger.info('Running analyses on training set.')
-
-    (_,
-     train_analyzed_container) = analyzer.run_training_analyses(processed_container,
-                                                                processed_config)
+    else:
+        output_dir = output_file
+        filename = "predictions_with_metadata"
 
-    # Write out files
-    writer.write_experiment_output(csvdir,
-                                   train_analyzed_container,
-                                   reset_index=True,
-                                   file_format=file_format)
-
-    # Use only selected features for predictions
-    columns_for_prediction = ['spkitemid', 'sc1'] + selected_features
-    train_for_prediction = processed_container.train_preprocessed_features[columns_for_prediction]
-    test_for_prediction = processed_container.test_preprocessed_features[columns_for_prediction]
-
-    logged_str = 'Generating training and test set predictions'
-    logged_str += ' (expected scores).' if configuration['predict_expected_scores'] else '.'
-    logger.info(logged_str)
-    (pred_config,
-     pred_data_container) = modeler.predict_train_and_test(train_for_prediction,
-                                                           test_for_prediction,
-                                                           processed_config)
+    # create any directories needed for the output file
+    os.makedirs(output_dir, exist_ok=True)
 
-    # Write out files
-    writer.write_experiment_output(csvdir,
-                                   pred_data_container,
-                                   new_names_dict={'pred_test': 'pred_processed'},
-                                   file_format=file_format)
-
-    original_coef_file = join(csvdir, '{}_coefficients.{}'.format(pred_config['experiment_id'],
-                                                                  file_format))
-
-    # If coefficients file exists, then try to generate the scaled
-    # coefficients and save them to a file
-    if exists(original_coef_file):
-        logger.info('Scaling the coefficients and saving them to disk')
-        try:
-
-            # scale coefficients, and return DataContainer w/ scaled coefficients
-            scaled_data_container = modeler.scale_coefficients(pred_config)
-
-        # raise an error if the coefficient file exists but the
-        # coefficients are not available for the current model
-        # which can happen if the user is re-running the same experiment
-        # with the same ID but with a non-linear model whereas the previous
-        # run of the same ID was with a linear model and the user has not
-        # cleared the directory
-        except RuntimeError:
-            raise ValueError("It appears you previously ran an experiment with the "
-                             "same ID using a linear model and saved its output to "
-                             "the same directory. That output is interfering with "
-                             "the current experiment. Either clear the contents "
-                             "of the output directory or re-run the current "
-                             "experiment using a different experiment ID.")
-        else:
-
-            # Write out scaled coefficients to disk
-            writer.write_experiment_output(csvdir,
-                                           scaled_data_container,
-                                           file_format=file_format)
-
-    # Add processed data_container frames to pred_data_container
-    new_pred_data_container = pred_data_container + processed_container
-
-    logger.info('Running prediction analyses.')
-    (pred_analysis_config,
-     pred_analysis_data_container) = analyzer.run_prediction_analyses(new_pred_data_container,
-                                                                      pred_config)
+    # save the predictions to disk
+    logger.info("Saving predictions.")
 
     # Write out files
-    writer.write_experiment_output(csvdir,
-                                   pred_analysis_data_container,
-                                   reset_index=True,
-                                   file_format=file_format)
-    # Initialize reporter
-    reporter = Reporter(logger=logger)
-
-    # generate the report
-    logger.info('Starting report generation.')
-    reporter.create_report(pred_analysis_config,
-                           csvdir,
-                           figdir)
+    writer.write_experiment_output(
+        output_dir,
+        processed_container,
+        include_experiment_id=False,
+        dataframe_names=["predictions_with_metadata"],
+        new_names_dict={"predictions_with_metadata": filename},
+        file_format=file_format,
+    )
+
+    # save excluded responses to disk
+    if not processed_container.excluded.empty:
+
+        # save the predictions to disk
+        logger.info(
+            f"Saving excluded responses to "
+            f"{join(output_dir, '{}_excluded_responses.csv'.format(filename))}"
+        )
+
+        # Write out files
+        writer.write_experiment_output(
+            output_dir,
+            processed_container,
+            include_experiment_id=False,
+            dataframe_names=["excluded"],
+            new_names_dict={"excluded": f"{filename}_excluded_responses"},
+            file_format=file_format,
+        )
 
 
 def main():  # noqa: D103
 
     # set up the basic logging configuration
     formatter = LogFormatter()
 
@@ -337,59 +399,76 @@
     # generated configuration file
     stdout_handler = logging.StreamHandler(sys.stdout)
     stdout_handler.setFormatter(formatter)
 
     stderr_handler = logging.StreamHandler(sys.stderr)
     stderr_handler.setFormatter(formatter)
 
-    logging.root.setLevel(logging.INFO)
-    logger = logging.getLogger(__name__)
-
-    # set up an argument parser via our helper function
-    parser = setup_rsmcmd_parser('rsmtool',
-                                 uses_output_directory=True,
-                                 allows_overwriting=True,
-                                 uses_subgroups=True)
+    # to set up the argument parser, we first need to instantiate options
+    # specific to rsmpredict so we use the `CmdOption` namedtuples
+    non_standard_options = [
+        CmdOption(dest="output_file", help="output file where predictions will be saved."),
+        CmdOption(
+            dest="preproc_feats_file",
+            help="if specified, the preprocessed features " "will be saved in this file",
+            longname="features",
+            required=False,
+        ),
+    ]
+
+    # now call the helper function to instantiate the parser for us
+    parser = setup_rsmcmd_parser(
+        "rsmpredict",
+        uses_output_directory=False,
+        extra_run_options=non_standard_options,
+    )
 
     # if we have no arguments at all then just show the help message
     if len(sys.argv) < 2:
         sys.argv.append("-h")
 
     # if the first argument is not one of the valid sub-commands
     # or one of the valid optional arguments, then assume that they
     # are arguments for the "run" sub-command. This allows the
     # old style command-line invocations to work without modification.
-    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + ['-h', '--help',
-                                                      '-V', '--version']:
-        args_to_pass = ['run'] + sys.argv[1:]
+    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + [
+        "-h",
+        "--help",
+        "-V",
+        "--version",
+    ]:
+        args_to_pass = ["run"] + sys.argv[1:]
     else:
         args_to_pass = sys.argv[1:]
     args = parser.parse_args(args=args_to_pass)
 
     # call the appropriate function based on which sub-command was run
-    if args.subcommand == 'run':
+    if args.subcommand == "run":
 
         # when running, log to stdout
         logging.root.addHandler(stdout_handler)
 
         # run the experiment
-        logger.info('Output directory: {}'.format(args.output_dir))
-        run_experiment(abspath(args.config_file),
-                       abspath(args.output_dir),
-                       overwrite_output=args.force_write)
+        preproc_feats_file = None
+        if args.preproc_feats_file:
+            preproc_feats_file = abspath(args.preproc_feats_file)
+        compute_and_save_predictions(
+            abspath(args.config_file),
+            abspath(args.output_file),
+            feats_file=preproc_feats_file,
+        )
 
     else:
 
         # when generating, log to stderr
         logging.root.addHandler(stderr_handler)
 
         # auto-generate an example configuration and print it to STDOUT
-        generator = ConfigurationGenerator('rsmtool',
-                                           as_string=True,
-                                           suppress_warnings=args.quiet,
-                                           use_subgroups=args.subgroups)
+        generator = ConfigurationGenerator(
+            "rsmpredict", as_string=True, suppress_warnings=args.quiet
+        )
         configuration = generator.interact() if args.interactive else generator.generate()
         print(configuration)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `rsmtool-9.0.1/rsmtool/rsmxval.py` & `rsmtool-9.1.1/rsmtool/rsmxval.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,41 +24,47 @@
   `<outdir>/final-model`.
 
 :author: Nitin Madnani (nmadnani@ets.org)
 :organization: ETS
 """
 
 import logging
-from os import listdir, makedirs
 import sys
+from os import listdir, makedirs
 from os.path import abspath, exists, join
 from pathlib import Path
 
 from joblib.parallel import Parallel, delayed
 from tqdm import tqdm
 
 from .configuration_parser import Configuration, configure
 from .rsmeval import run_evaluation
-from .rsmtool import run_experiment
 from .rsmsummarize import run_summary
+from .rsmtool import run_experiment
 from .utils.commandline import ConfigurationGenerator, setup_rsmcmd_parser
 from .utils.constants import VALID_PARSER_SUBCOMMANDS
-from .utils.cross_validation import combine_fold_prediction_files, create_xval_files, process_fold
-from .utils.logging import LogFormatter, tqdm_joblib, get_file_logger
+from .utils.cross_validation import (
+    combine_fold_prediction_files,
+    create_xval_files,
+    process_fold,
+)
+from .utils.logging import LogFormatter, get_file_logger, tqdm_joblib
 from .writer import DataWriter
 
 # a constant defining all of the sections we can use when
 # generating the final model report in the last stage
-FINAL_MODEL_SECTION_LIST = ['feature_descriptives',
-                            'features_by_group',
-                            'preprocessed_features',
-                            'dff_by_group',
-                            'model',
-                            'intermediate_file_paths',
-                            'sysinfo']
+FINAL_MODEL_SECTION_LIST = [
+    "feature_descriptives",
+    "features_by_group",
+    "preprocessed_features",
+    "dff_by_group",
+    "model",
+    "intermediate_file_paths",
+    "sysinfo",
+]
 
 
 def run_cross_validation(config_file_or_obj_or_dict, output_dir, silence_tqdm=False):
     """
     Run cross-validation experiment.
 
     Parameters
@@ -86,70 +92,68 @@
     IOError
         If ``output_dir`` already contains the output of a previous experiment.
 
     """
     logger = logging.getLogger(__name__)
 
     # Get absolute paths to output directories
-    foldsdir = abspath(join(output_dir, 'folds'))
-    summarydir = abspath(join(output_dir, 'fold-summary'))
-    evaldir = abspath(join(output_dir, 'evaluation'))
-    modeldir = abspath(join(output_dir, 'final-model'))
+    foldsdir = abspath(join(output_dir, "folds"))
+    summarydir = abspath(join(output_dir, "fold-summary"))
+    evaldir = abspath(join(output_dir, "evaluation"))
+    modeldir = abspath(join(output_dir, "final-model"))
 
     # Make directories, if necessary
     makedirs(foldsdir, exist_ok=True)
     makedirs(summarydir, exist_ok=True)
     makedirs(evaldir, exist_ok=True)
     makedirs(modeldir, exist_ok=True)
 
     # Raise an error if the specified output directory
     # already contains a non-empty `folds` directory;
     # we do not allow overwriting the output directory
     # for cross-validation experiments because of the
     # multitude of moving parts
     non_empty_foldsdir = exists(foldsdir) and listdir(foldsdir)
     if non_empty_foldsdir:
-        raise IOError("'{}' already contains a non-empty 'folds' "
-                      "directory.".format(output_dir))
+        raise IOError(f"'{output_dir}' already contains a non-empty 'folds' directory.")
 
-    configuration = configure('rsmxval', config_file_or_obj_or_dict)
+    configuration = configure("rsmxval", config_file_or_obj_or_dict)
 
     logger.info("Saving configuration file.")
     with open(Path(output_dir) / "rsmxval.json", "w") as outfh:
         outfh.write(str(configuration))
 
     # create any cross-validation related files that are needed and
     # get a data frame containing the training set and the final
     # number of folds that are to be used in the experiment
     df_train, folds = create_xval_files(configuration, output_dir, logger=logger)
 
     # run RSMTool in parallel on each fold using joblib
     logger.info("Running RSMTool on each fold in parallel")
     with tqdm_joblib(tqdm(desc="Progress", total=folds, disable=silence_tqdm)):
-        Parallel(n_jobs=folds)(delayed(process_fold)(fold_num, foldsdir)
-                               for fold_num in range(1, folds + 1))
+        Parallel(n_jobs=folds)(
+            delayed(process_fold)(fold_num, foldsdir) for fold_num in range(1, folds + 1)
+        )
 
     # generate an rsmsummarize configuration file
     logger.info("Creating fold summary")
     given_file_format = configuration.get("file_format")
     fold_summary_configdict = {
         "summary_id": f"{configuration['experiment_id']}_fold_summary",
-        "experiment_dirs": [f"{foldsdir}/{fold_num:02}"
-                            for fold_num in range(1, folds + 1)],
+        "experiment_dirs": [f"{foldsdir}/{fold_num:02}" for fold_num in range(1, folds + 1)],
         "description": f"{configuration['description']} (Fold Summary)",
         "file_format": given_file_format,
-        "use_thumbnails": f"{configuration['use_thumbnails']}"
+        "use_thumbnails": f"{configuration['use_thumbnails']}",
     }
-    fold_summary_configuration = Configuration(fold_summary_configdict,
-                                               configdir=summarydir,
-                                               context="rsmsummarize")
+    fold_summary_configuration = Configuration(
+        fold_summary_configdict, configdir=summarydir, context="rsmsummarize"
+    )
 
     # run rsmsummarize on all of the fold directories
-    summary_logger = get_file_logger("fold-summary",
-                                     Path(summarydir) / "rsmsummarize.log")
+    summary_logger = get_file_logger("fold-summary", Path(summarydir) / "rsmsummarize.log")
     run_summary(fold_summary_configuration, summarydir, False, logger=summary_logger)
 
     # combine all of the fold prediction files for evaluation
     df_predictions = combine_fold_prediction_files(foldsdir, given_file_format)
 
     # if there were subgroups and a second human score column specified, then
     # we need to add those to the combined predictions file as well
@@ -157,59 +161,61 @@
     columns_to_use = [id_column]
     if subgroups := configuration["subgroups"]:
         columns_to_use.extend(subgroups)
     if second_human_score_column := configuration["second_human_score_column"]:
         columns_to_use.append(second_human_score_column)
     if len(columns_to_use) > 1:
         df_to_add = df_train[columns_to_use]
-        df_predictions = df_predictions.merge(df_to_add,
-                                              left_on="spkitemid",
-                                              right_on=id_column)
+        df_predictions = df_predictions.merge(df_to_add, left_on="spkitemid", right_on=id_column)
         # drop any extra ID column if we have added one
         if id_column != "spkitemid":
             df_predictions.drop(id_column, axis=1, inplace=True)
 
     # write out the predictions file to disk
     predictions_file_prefix = str(Path(evaldir) / "xval_predictions")
-    DataWriter.write_frame_to_file(df_predictions,
-                                   predictions_file_prefix,
-                                   file_format=given_file_format,
-                                   index=False)
+    DataWriter.write_frame_to_file(
+        df_predictions,
+        predictions_file_prefix,
+        file_format=given_file_format,
+        index=False,
+    )
 
     # create a new rsmeval configuration dictionary;
     # note that we do not want to set "id_column" and "human_score_column"
     # here since those columns already have default names given that the
     # predictions are generated from RSMTool
     evaluation_configdict = {
         "experiment_id": f"{configuration['experiment_id']}_evaluation",
         "description": f"{configuration['description']} (Evaluating Fold Predictions)",
         "predictions_file": f"{predictions_file_prefix}.{given_file_format}",
         "system_score_column": "scale" if configuration["use_scaled_predictions"] else "raw",
         "scale_with": "asis" if configuration["use_scaled_predictions"] else "raw",
         "trim_min": int(f"{configuration['trim_min']}"),
         "trim_max": int(f"{configuration['trim_max']}"),
-        "file_format": given_file_format
+        "file_format": given_file_format,
     }
 
     # copy over the relevant configuration fields from the main configuration
-    for field_name in ["second_human_score_column",
-                       "candidate_column",
-                       "flag_column",
-                       "exclude_zero_scores",
-                       "min_items_per_candidate",
-                       "rater_error_variance",
-                       "subgroups",
-                       "trim_tolerance",
-                       "use_thumbnails"]:
+    for field_name in [
+        "second_human_score_column",
+        "candidate_column",
+        "flag_column",
+        "exclude_zero_scores",
+        "min_items_per_candidate",
+        "rater_error_variance",
+        "subgroups",
+        "trim_tolerance",
+        "use_thumbnails",
+    ]:
         evaluation_configdict[field_name] = configuration[field_name]
 
     # create an rsmeval configuration object with this dictionary
-    evaluation_configuration = Configuration(evaluation_configdict,
-                                             configdir=evaldir,
-                                             context="rsmeval")
+    evaluation_configuration = Configuration(
+        evaluation_configdict, configdir=evaldir, context="rsmeval"
+    )
 
     # run rsmeval on the combined predictions file
     logger.info("Evaluating combined fold predictions")
     eval_logger = get_file_logger("evaluation", Path(evaldir) / "rsmeval.log")
     run_evaluation(evaluation_configuration, evaldir, False, logger=eval_logger)
 
     # run rsmtool on the full dataset and generate only model/feature
@@ -225,17 +231,17 @@
     # remove by-group sections if we don't have the info
     sections_to_use = []
     for section in FINAL_MODEL_SECTION_LIST:
         if section.endswith("_by_group") and not subgroups:
             continue
         sections_to_use.append(section)
     final_rsmtool_configdict["general_sections"] = sections_to_use
-    final_rsmtool_configuration = Configuration(final_rsmtool_configdict,
-                                                configdir=configuration.configdir,
-                                                context="rsmtool")
+    final_rsmtool_configuration = Configuration(
+        final_rsmtool_configdict, configdir=configuration.configdir, context="rsmtool"
+    )
     run_experiment(final_rsmtool_configuration, modeldir, False, logger=model_logger)
 
 
 def main():  # noqa: D103
 
     # set up the basic logging configuration
     formatter = LogFormatter()
@@ -251,54 +257,61 @@
     stderr_handler = logging.StreamHandler(sys.stderr)
     stderr_handler.setFormatter(formatter)
 
     logging.root.setLevel(logging.INFO)
     logger = logging.getLogger(__name__)
 
     # set up an argument parser via our helper function
-    parser = setup_rsmcmd_parser('rsmxval',
-                                 uses_output_directory=True,
-                                 allows_overwriting=False,
-                                 uses_subgroups=True)
+    parser = setup_rsmcmd_parser(
+        "rsmxval",
+        uses_output_directory=True,
+        allows_overwriting=False,
+        uses_subgroups=True,
+    )
 
     # if we have no arguments at all then just show the help message
     if len(sys.argv) < 2:
         sys.argv.append("-h")
 
     # if the first argument is not one of the valid sub-commands
     # or one of the valid optional arguments, then assume that they
     # are arguments for the "run" sub-command. This allows the
     # old style command-line invocations to work without modification.
-    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + ['-h', '--help',
-                                                      '-V', '--version']:
-        args_to_pass = ['run'] + sys.argv[1:]
+    if sys.argv[1] not in VALID_PARSER_SUBCOMMANDS + [
+        "-h",
+        "--help",
+        "-V",
+        "--version",
+    ]:
+        args_to_pass = ["run"] + sys.argv[1:]
     else:
         args_to_pass = sys.argv[1:]
     args = parser.parse_args(args=args_to_pass)
 
     # call the appropriate function based on which sub-command was run
-    if args.subcommand == 'run':
+    if args.subcommand == "run":
 
         # when running, log to stdout
         logging.root.addHandler(stdout_handler)
 
         # run the experiment
-        logger.info('Output directory: {}'.format(args.output_dir))
-        run_cross_validation(abspath(args.config_file),
-                             abspath(args.output_dir))
+        logger.info(f"Output directory: {args.output_dir}")
+        run_cross_validation(abspath(args.config_file), abspath(args.output_dir))
 
     else:
 
         # when generating, log to stderr
         logging.root.addHandler(stderr_handler)
 
         # auto-generate an example configuration and print it to STDOUT
-        generator = ConfigurationGenerator('rsmxval',
-                                           as_string=True,
-                                           suppress_warnings=args.quiet,
-                                           use_subgroups=args.subgroups)
+        generator = ConfigurationGenerator(
+            "rsmxval",
+            as_string=True,
+            suppress_warnings=args.quiet,
+            use_subgroups=args.subgroups,
+        )
         configuration = generator.interact() if args.interactive else generator.generate()
         print(configuration)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `rsmtool-9.0.1/rsmtool/test_utils.py` & `rsmtool-9.1.1/rsmtool/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,41 +22,42 @@
 from .rsmcompare import run_comparison
 from .rsmeval import run_evaluation
 from .rsmpredict import compute_and_save_predictions
 from .rsmsummarize import run_summary
 from .rsmtool import run_experiment
 from .rsmxval import run_cross_validation
 
-html_error_regexp = re.compile(r'Traceback \(most recent call last\)')
+html_error_regexp = re.compile(r"Traceback \(most recent call last\)")
 html_warning_regexp = re.compile(r'<div class=".*?output_stderr.*?>([^<]+)')
-section_regexp = re.compile(r'<h2>(.*?)</h2>')
+section_regexp = re.compile(r"<h2>(.*?)</h2>")
 
 # get the directory containing the tests
-rsmtool_test_dir = Path(__file__).absolute().parent.parent.joinpath('tests')
+rsmtool_test_dir = Path(__file__).absolute().parent.parent.joinpath("tests")
 
-tools_with_input_data = ['rsmsummarize', 'rsmcompare']
-tools_with_output = ['rsmtool', 'rsmeval',
-                     'rsmsummarize', 'rsmpredict']
+tools_with_input_data = ["rsmsummarize", "rsmcompare"]
+tools_with_output = ["rsmtool", "rsmeval", "rsmsummarize", "rsmpredict"]
 
 # check if tests are being run in strict mode
 # if so, any warnings found in HTML
 # reports should not be ignored
-STRICT_MODE = os.environ.get('STRICT', None)
+STRICT_MODE = os.environ.get("STRICT", None)
 IGNORE_WARNINGS = False if STRICT_MODE else True
 
 
-def check_run_experiment(source,
-                         experiment_id,
-                         subgroups=None,
-                         consistency=False,
-                         skll=False,
-                         file_format='csv',
-                         given_test_dir=None,
-                         config_obj_or_dict=None,
-                         suppress_warnings_for=[]):
+def check_run_experiment(
+    source,
+    experiment_id,
+    subgroups=None,
+    consistency=False,
+    skll=False,
+    file_format="csv",
+    given_test_dir=None,
+    config_obj_or_dict=None,
+    suppress_warnings_for=[],
+):
     """
     Run a parameterized rsmtool experiment test.
 
     Parameters
     ----------
     source : str
         The name of the source directory containing the experiment
@@ -95,34 +96,29 @@
         experiments.
         Defaults to ``[]``.
     """
     # use the test directory from this file unless it's been overridden
     test_dir = given_test_dir if given_test_dir else rsmtool_test_dir
 
     if config_obj_or_dict is None:
-        config_input = join(test_dir,
-                            'data',
-                            'experiments',
-                            source,
-                            '{}.json'.format(experiment_id))
+        config_input = join(test_dir, "data", "experiments", source, f"{experiment_id}.json")
     else:
         config_input = config_obj_or_dict
 
-    model_type = 'skll' if skll else 'rsmtool'
+    model_type = "skll" if skll else "rsmtool"
 
-    do_run_experiment(source,
-                      experiment_id,
-                      config_input,
-                      suppress_warnings_for=suppress_warnings_for)
-
-    output_dir = join('test_outputs', source, 'output')
-    expected_output_dir = join(test_dir, 'data', 'experiments', source, 'output')
-    html_report = join('test_outputs', source, 'report', '{}_report.html'.format(experiment_id))
+    do_run_experiment(
+        source, experiment_id, config_input, suppress_warnings_for=suppress_warnings_for
+    )
 
-    output_files = glob(join(output_dir, '*.{}'.format(file_format)))
+    output_dir = join("test_outputs", source, "output")
+    expected_output_dir = join(test_dir, "data", "experiments", source, "output")
+    html_report = join("test_outputs", source, "report", f"{experiment_id}_report.html")
+
+    output_files = glob(join(output_dir, f"*.{file_format}"))
     for output_file in output_files:
         output_filename = basename(output_file)
         expected_output_file = join(expected_output_dir, output_filename)
 
         if exists(expected_output_file):
             check_file_output(output_file, expected_output_file, file_format=file_format)
 
@@ -144,22 +140,24 @@
     # make sure that there are no warnings in the report
     # but ignore warnings if appropriate
     if not IGNORE_WARNINGS:
         warning_msgs = collect_warning_messages_from_report(html_report)
         assert_equal(len(warning_msgs), 0)
 
 
-def check_run_evaluation(source,
-                         experiment_id,
-                         subgroups=None,
-                         consistency=False,
-                         file_format='csv',
-                         given_test_dir=None,
-                         config_obj_or_dict=None,
-                         suppress_warnings_for=[]):
+def check_run_evaluation(
+    source,
+    experiment_id,
+    subgroups=None,
+    consistency=False,
+    file_format="csv",
+    given_test_dir=None,
+    config_obj_or_dict=None,
+    suppress_warnings_for=[],
+):
     """
     Run a parameterized rsmeval experiment test.
 
     Parameters
     ----------
     source : str
         The name of the source directory containing the experiment
@@ -194,32 +192,27 @@
         experiments.
         Defaults to ``[]``.
     """
     # use the test directory from this file unless it's been overridden
     test_dir = given_test_dir if given_test_dir else rsmtool_test_dir
 
     if config_obj_or_dict is None:
-        config_input = join(test_dir,
-                            'data',
-                            'experiments',
-                            source,
-                            '{}.json'.format(experiment_id))
+        config_input = join(test_dir, "data", "experiments", source, f"{experiment_id}.json")
     else:
         config_input = config_obj_or_dict
 
-    do_run_evaluation(source,
-                      experiment_id,
-                      config_input,
-                      suppress_warnings_for=suppress_warnings_for)
-
-    output_dir = join('test_outputs', source, 'output')
-    expected_output_dir = join(test_dir, 'data', 'experiments', source, 'output')
-    html_report = join('test_outputs', source, 'report', '{}_report.html'.format(experiment_id))
+    do_run_evaluation(
+        source, experiment_id, config_input, suppress_warnings_for=suppress_warnings_for
+    )
+
+    output_dir = join("test_outputs", source, "output")
+    expected_output_dir = join(test_dir, "data", "experiments", source, "output")
+    html_report = join("test_outputs", source, "report", f"{experiment_id}_report.html")
 
-    output_files = glob(join(output_dir, '*.{}'.format(file_format)))
+    output_files = glob(join(output_dir, f"*.{file_format}"))
     for output_file in output_files:
         output_filename = basename(output_file)
         expected_output_file = join(expected_output_dir, output_filename)
 
         if exists(expected_output_file):
             check_file_output(output_file, expected_output_file, file_format=file_format)
 
@@ -233,19 +226,21 @@
     # make sure that there are no warnings in the report
     # but ignore warnings if appropriate
     if not IGNORE_WARNINGS:
         warning_msgs = collect_warning_messages_from_report(html_report)
         assert_equal(len(warning_msgs), 0)
 
 
-def check_run_comparison(source,
-                         experiment_id,
-                         given_test_dir=None,
-                         config_obj_or_dict=None,
-                         suppress_warnings_for=[]):
+def check_run_comparison(
+    source,
+    experiment_id,
+    given_test_dir=None,
+    config_obj_or_dict=None,
+    suppress_warnings_for=[],
+):
     """
     Run a parameterized rsmcompare experiment test.
 
     Parameters
     ----------
     source : str
         The name of the source directory containing the experiment
@@ -267,45 +262,41 @@
         experiments.
         Defaults to ```[]``.
     """
     # use the test directory from this file unless it's been overridden
     test_dir = given_test_dir if given_test_dir else rsmtool_test_dir
 
     if config_obj_or_dict is None:
-        config_input = join(test_dir,
-                            'data',
-                            'experiments',
-                            source,
-                            'rsmcompare.json')
+        config_input = join(test_dir, "data", "experiments", source, "rsmcompare.json")
     else:
         config_input = config_obj_or_dict
 
-    do_run_comparison(source,
-                      config_input,
-                      suppress_warnings_for=suppress_warnings_for)
+    do_run_comparison(source, config_input, suppress_warnings_for=suppress_warnings_for)
 
-    html_report = join('test_outputs', source, '{}_report.html'.format(experiment_id))
+    html_report = join("test_outputs", source, f"{experiment_id}_report.html")
 
     # check report for any errors but ignore warnings
     # which we check below separately
     check_report(html_report, raise_warnings=False)
 
     # make sure that there are no warnings in the report
     # but ignore warnings if appropriate
     if not IGNORE_WARNINGS:
         warning_msgs = collect_warning_messages_from_report(html_report)
         assert_equal(len(warning_msgs), 0)
 
 
-def check_run_prediction(source,
-                         excluded=False,
-                         file_format='csv',
-                         given_test_dir=None,
-                         config_obj_or_dict=None,
-                         suppress_warnings_for=[]):
+def check_run_prediction(
+    source,
+    excluded=False,
+    file_format="csv",
+    given_test_dir=None,
+    config_obj_or_dict=None,
+    suppress_warnings_for=[],
+):
     """
     Run a parameterized rsmpredict experiment test.
 
     Parameters
     ----------
     source : str
         The name of the source directory containing the experiment
@@ -331,45 +322,43 @@
         experiments.
         Defaults to ``[]``.
     """
     # use the test directory from this file unless it's been overridden
     test_dir = given_test_dir if given_test_dir else rsmtool_test_dir
 
     if config_obj_or_dict is None:
-        config_input = join(test_dir,
-                            'data',
-                            'experiments',
-                            source,
-                            'rsmpredict.json')
+        config_input = join(test_dir, "data", "experiments", source, "rsmpredict.json")
     else:
         config_input = config_obj_or_dict
 
-    do_run_prediction(source,
-                      config_input,
-                      suppress_warnings_for=suppress_warnings_for)
+    do_run_prediction(source, config_input, suppress_warnings_for=suppress_warnings_for)
 
-    output_dir = join('test_outputs', source, 'output')
-    expected_output_dir = join(test_dir, 'data', 'experiments', source, 'output')
+    output_dir = join("test_outputs", source, "output")
+    expected_output_dir = join(test_dir, "data", "experiments", source, "output")
 
-    output_files = ['predictions.{}'.format(file_format),
-                    'preprocessed_features.{}'.format(file_format)]
+    output_files = [
+        f"predictions.{file_format}",
+        f"preprocessed_features.{file_format}",
+    ]
     if excluded:
-        output_files.append('predictions_excluded_responses.{}'.format(file_format))
+        output_files.append(f"predictions_excluded_responses.{file_format}")
     for output_file in output_files:
         generated_output_file = join(output_dir, output_file)
         expected_output_file = join(expected_output_dir, output_file)
 
         check_file_output(generated_output_file, expected_output_file)
 
 
-def check_run_summary(source,
-                      file_format='csv',
-                      given_test_dir=None,
-                      config_obj_or_dict=None,
-                      suppress_warnings_for=[]):
+def check_run_summary(
+    source,
+    file_format="csv",
+    given_test_dir=None,
+    config_obj_or_dict=None,
+    suppress_warnings_for=[],
+):
     """
     Run a parameterized rsmsummarize experiment test.
 
     Parameters
     ----------
     source : str
         The name of the source directory containing the experiment
@@ -392,32 +381,26 @@
         experiments.
         Defaults to ``[]``.
     """
     # use the test directory from this file unless it's been overridden
     test_dir = given_test_dir if given_test_dir else rsmtool_test_dir
 
     if config_obj_or_dict is None:
-        config_input = join(test_dir,
-                            'data',
-                            'experiments',
-                            source,
-                            'rsmsummarize.json')
+        config_input = join(test_dir, "data", "experiments", source, "rsmsummarize.json")
     else:
         config_input = config_obj_or_dict
 
-    do_run_summary(source,
-                   config_input,
-                   suppress_warnings_for=suppress_warnings_for)
+    do_run_summary(source, config_input, suppress_warnings_for=suppress_warnings_for)
 
-    html_report = join('test_outputs', source, 'report', 'model_comparison_report.html')
+    html_report = join("test_outputs", source, "report", "model_comparison_report.html")
 
-    output_dir = join('test_outputs', source, 'output')
-    expected_output_dir = join(test_dir, 'data', 'experiments', source, 'output')
+    output_dir = join("test_outputs", source, "output")
+    expected_output_dir = join(test_dir, "data", "experiments", source, "output")
 
-    output_files = glob(join(output_dir, '*.{}'.format(file_format)))
+    output_files = glob(join(output_dir, f"*.{file_format}"))
     for output_file in output_files:
         output_filename = basename(output_file)
         expected_output_file = join(expected_output_dir, output_filename)
 
         if exists(expected_output_file):
             check_file_output(output_file, expected_output_file)
 
@@ -428,24 +411,26 @@
     # make sure that there are no warnings in the report
     # but ignore warnings if appropriate
     if not IGNORE_WARNINGS:
         warning_msgs = collect_warning_messages_from_report(html_report)
         assert_equal(len(warning_msgs), 0)
 
 
-def check_run_cross_validation(source,
-                               experiment_id,
-                               folds=5,
-                               subgroups=None,
-                               consistency=False,
-                               skll=False,
-                               file_format='csv',
-                               given_test_dir=None,
-                               config_obj_or_dict=None,
-                               suppress_warnings_for=[]):
+def check_run_cross_validation(
+    source,
+    experiment_id,
+    folds=5,
+    subgroups=None,
+    consistency=False,
+    skll=False,
+    file_format="csv",
+    given_test_dir=None,
+    config_obj_or_dict=None,
+    suppress_warnings_for=[],
+):
     """
     Run a parameterized rsmxval experiment test.
 
     Parameters
     ----------
     source : str
         The name of the source directory containing the experiment
@@ -487,167 +472,149 @@
         experiments.
         Defaults to ``[]``.
     """
     # use the test directory from this file unless it's been overridden
     test_dir = given_test_dir if given_test_dir else rsmtool_test_dir
 
     if config_obj_or_dict is None:
-        config_input = join(test_dir,
-                            'data',
-                            'experiments',
-                            source,
-                            '{}.json'.format(experiment_id))
+        config_input = join(test_dir, "data", "experiments", source, f"{experiment_id}.json")
     else:
         config_input = config_obj_or_dict
 
-    model_type = 'skll' if skll else 'rsmtool'
+    model_type = "skll" if skll else "rsmtool"
 
-    do_run_cross_validation(source,
-                            experiment_id,
-                            config_input,
-                            suppress_warnings_for=suppress_warnings_for)
+    do_run_cross_validation(
+        source, experiment_id, config_input, suppress_warnings_for=suppress_warnings_for
+    )
 
-    output_prefix = join('test_outputs', source)
-    expected_output_prefix = join(test_dir, 'data', 'experiments', source, 'output')
+    output_prefix = join("test_outputs", source)
+    expected_output_prefix = join(test_dir, "data", "experiments", source, "output")
 
     # first check that each fold's rsmtool output is as expected
-    actual_folds_dir = join(output_prefix, 'folds')
-    expected_folds_dir = join(expected_output_prefix, 'folds')
+    actual_folds_dir = join(output_prefix, "folds")
+    expected_folds_dir = join(expected_output_prefix, "folds")
     for fold_num in range(1, folds + 1):
         fold_experiment_id = f"{experiment_id}_fold{fold_num:02}"
-        fold_output_dir = join(actual_folds_dir, f'{fold_num:02}', 'output')
-        fold_output_files = glob(join(fold_output_dir, f'*.{file_format}'))
+        fold_output_dir = join(actual_folds_dir, f"{fold_num:02}", "output")
+        fold_output_files = glob(join(fold_output_dir, f"*.{file_format}"))
         for fold_output_file in fold_output_files:
             output_filename = basename(fold_output_file)
-            expected_output_file = join(expected_folds_dir,
-                                        f'{fold_num:02}',
-                                        'output',
-                                        output_filename)
+            expected_output_file = join(
+                expected_folds_dir, f"{fold_num:02}", "output", output_filename
+            )
 
             if exists(expected_output_file):
-                check_file_output(fold_output_file,
-                                  expected_output_file,
-                                  file_format=file_format)
-
-        check_generated_output(fold_output_files,
-                               fold_experiment_id,
-                               model_type,
-                               file_format=file_format)
+                check_file_output(fold_output_file, expected_output_file, file_format=file_format)
+
+        check_generated_output(
+            fold_output_files, fold_experiment_id, model_type, file_format=file_format
+        )
 
         if not skll:
-            check_scaled_coefficients(fold_output_dir,
-                                      fold_experiment_id,
-                                      file_format=file_format)
+            check_scaled_coefficients(fold_output_dir, fold_experiment_id, file_format=file_format)
 
         if subgroups:
-            check_subgroup_outputs(fold_output_dir,
-                                   fold_experiment_id,
-                                   subgroups,
-                                   file_format=file_format)
+            check_subgroup_outputs(
+                fold_output_dir, fold_experiment_id, subgroups, file_format=file_format
+            )
 
         if consistency:
-            check_consistency_files_exist(fold_output_files,
-                                          fold_experiment_id,
-                                          file_format=file_format)
+            check_consistency_files_exist(
+                fold_output_files, fold_experiment_id, file_format=file_format
+            )
 
     # next check that the evaluation output is as expected
-    actual_eval_output_dir = join(output_prefix, 'evaluation', 'output')
-    expected_eval_output_dir = join(expected_output_prefix, 'evaluation', 'output')
+    actual_eval_output_dir = join(output_prefix, "evaluation", "output")
+    expected_eval_output_dir = join(expected_output_prefix, "evaluation", "output")
 
-    output_files = glob(join(actual_eval_output_dir, '*.{}'.format(file_format)))
+    output_files = glob(join(actual_eval_output_dir, f"*.{file_format}"))
     for output_file in output_files:
         output_filename = basename(output_file)
         expected_output_file = join(expected_eval_output_dir, output_filename)
 
         if exists(expected_output_file):
             check_file_output(output_file, expected_output_file, file_format=file_format)
 
     if consistency:
         check_consistency_files_exist(output_files, f"{experiment_id}_evaluation")
 
     # next check that the summary output is as expected
-    actual_summary_output_dir = join(output_prefix, 'fold-summary', 'output')
-    expected_summary_output_dir = join(expected_output_prefix, 'fold-summary', 'output')
+    actual_summary_output_dir = join(output_prefix, "fold-summary", "output")
+    expected_summary_output_dir = join(expected_output_prefix, "fold-summary", "output")
 
-    output_files = glob(join(actual_summary_output_dir, '*.{}'.format(file_format)))
+    output_files = glob(join(actual_summary_output_dir, f"*.{file_format}"))
     for output_file in output_files:
         output_filename = basename(output_file)
         expected_output_file = join(expected_summary_output_dir, output_filename)
 
         if exists(expected_output_file):
             check_file_output(output_file, expected_output_file)
 
     # next check that the final model rsmtool output is as expected
-    actual_final_model_output_dir = join(output_prefix, 'final-model', 'output')
-    expected_final_model_output_dir = join(expected_output_prefix, 'final-model', 'output')
+    actual_final_model_output_dir = join(output_prefix, "final-model", "output")
+    expected_final_model_output_dir = join(expected_output_prefix, "final-model", "output")
     model_experiment_id = f"{experiment_id}_model"
 
-    output_files = glob(join(actual_final_model_output_dir, '*.{}'.format(file_format)))
+    output_files = glob(join(actual_final_model_output_dir, f"*.{file_format}"))
     for output_file in output_files:
         output_filename = basename(output_file)
         expected_output_file = join(expected_final_model_output_dir, output_filename)
 
         if exists(expected_output_file):
             check_file_output(output_file, expected_output_file, file_format=file_format)
 
-    check_generated_output(output_files,
-                           model_experiment_id,
-                           model_type,
-                           file_format=file_format)
+    check_generated_output(output_files, model_experiment_id, model_type, file_format=file_format)
 
     if not skll:
-        check_scaled_coefficients(actual_final_model_output_dir,
-                                  model_experiment_id,
-                                  file_format=file_format)
+        check_scaled_coefficients(
+            actual_final_model_output_dir, model_experiment_id, file_format=file_format
+        )
 
     if subgroups:
-        check_subgroup_outputs(actual_final_model_output_dir,
-                               model_experiment_id,
-                               subgroups,
-                               file_format=file_format)
+        check_subgroup_outputs(
+            actual_final_model_output_dir,
+            model_experiment_id,
+            subgroups,
+            file_format=file_format,
+        )
 
     # finally check all the HTML reports for any errors but ignore warnings
     # which we check below separately
-    per_fold_html_reports = glob(join(output_prefix,
-                                      'folds',
-                                      '*',
-                                      'report',
-                                      '*.html'))
-
-    evaluation_report = join(output_prefix,
-                             'evaluation',
-                             'report',
-                             f'{experiment_id}_evaluation_report.html')
-
-    summary_report = join(output_prefix,
-                          'fold-summary',
-                          'report',
-                          f'{experiment_id}_fold_summary_report.html')
-
-    final_model_report = join(output_prefix,
-                              'final-model',
-                              'report',
-                              f'{experiment_id}_model_report.html')
-
-    for html_report in per_fold_html_reports + [evaluation_report,
-                                                summary_report,
-                                                final_model_report]:
+    per_fold_html_reports = glob(join(output_prefix, "folds", "*", "report", "*.html"))
+
+    evaluation_report = join(
+        output_prefix, "evaluation", "report", f"{experiment_id}_evaluation_report.html"
+    )
+
+    summary_report = join(
+        output_prefix,
+        "fold-summary",
+        "report",
+        f"{experiment_id}_fold_summary_report.html",
+    )
+
+    final_model_report = join(
+        output_prefix, "final-model", "report", f"{experiment_id}_model_report.html"
+    )
+
+    for html_report in per_fold_html_reports + [
+        evaluation_report,
+        summary_report,
+        final_model_report,
+    ]:
         check_report(html_report, raise_warnings=False)
 
         # make sure that there are no warnings in the report
         # but ignore warnings if appropriate
         if not IGNORE_WARNINGS:
             warning_msgs = collect_warning_messages_from_report(html_report)
             assert_equal(len(warning_msgs), 0)
 
 
-def do_run_experiment(source,
-                      experiment_id,
-                      config_input,
-                      suppress_warnings_for=[]):
+def do_run_experiment(source, experiment_id, config_input, suppress_warnings_for=[]):
     """
     Run rsmtool experiment automatically.
 
     Use the given experiment configuration file located in the
     given source directory and use the given experiment ID.
 
     Parameters
@@ -663,39 +630,36 @@
         configuration file.
     suppress_warnings_for : list, optional
         Categories for which warnings should be suppressed
         when running the experiments. Note that ``RuntimeWarning``s
         are always suppressed.
         Defaults to ``[]``.
     """
-    source_output_dir = 'test_outputs'
+    source_output_dir = "test_outputs"
     experiment_dir = join(source_output_dir, source)
 
     # remove all previously created files
-    for output_subdir in ['output', 'figure', 'report']:
-        files = glob(join(source_output_dir, source, output_subdir, '*'))
+    for output_subdir in ["output", "figure", "report"]:
+        files = glob(join(source_output_dir, source, output_subdir, "*"))
         for f in files:
             remove(f)
 
     with warnings.catch_warnings():
 
         # always suppress runtime warnings
-        warnings.filterwarnings('ignore', category=RuntimeWarning)
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
 
         # suppress additional warning types if specified
         for warning_type in suppress_warnings_for:
-            warnings.filterwarnings('ignore', category=warning_type)
+            warnings.filterwarnings("ignore", category=warning_type)
 
         run_experiment(config_input, experiment_dir)
 
 
-def do_run_evaluation(source,
-                      experiment_id,
-                      config_input,
-                      suppress_warnings_for=[]):
+def do_run_evaluation(source, experiment_id, config_input, suppress_warnings_for=[]):
     """
     Run rsmeval experiment automatically.
 
     Use the given experiment configuration file located in the given
     source directory and use the given experiment ID.
 
     Parameters
@@ -711,38 +675,36 @@
         configuration file.
     suppress_warnings_for : list, optional
         Categories for which warnings should be suppressed
         when running the experiments. Note that ``RuntimeWarning``s
         are always suppressed.
         Defaults to ``[]``.
     """
-    source_output_dir = 'test_outputs'
+    source_output_dir = "test_outputs"
     experiment_dir = join(source_output_dir, source)
 
     # remove all previously created files
-    for output_subdir in ['output', 'figure', 'report']:
-        files = glob(join(source_output_dir, source, output_subdir, '*'))
+    for output_subdir in ["output", "figure", "report"]:
+        files = glob(join(source_output_dir, source, output_subdir, "*"))
         for f in files:
             remove(f)
 
     with warnings.catch_warnings():
 
         # always suppress runtime warnings
-        warnings.filterwarnings('ignore', category=RuntimeWarning)
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
 
         # suppress additional warning types if specified
         for warning_type in suppress_warnings_for:
-            warnings.filterwarnings('ignore', category=warning_type)
+            warnings.filterwarnings("ignore", category=warning_type)
 
         run_evaluation(config_input, experiment_dir)
 
 
-def do_run_prediction(source,
-                      config_input,
-                      suppress_warnings_for=[]):
+def do_run_prediction(source, config_input, suppress_warnings_for=[]):
     """
     Run rsmpredict experiment automatically.
 
     Use the given experiment configuration file located in the given
     source directory.
 
     Parameters
@@ -755,41 +717,39 @@
         or a dictionary with keys corresponding to fields in the
         configuration file
     suppress_warnings_for : list, optional
         Categories for which warnings should be suppressed when running the
         experiments.
         Defaults to ``[]``.
     """
-    source_output_dir = 'test_outputs'
+    source_output_dir = "test_outputs"
 
     # The `csv` file extension is ultimately dropped by the `rsmpredict.py`
     # script, so these arguments can be used for CSV, TSV, or XLSX output
-    output_file = join(source_output_dir, source, 'output', 'predictions.csv')
-    feats_file = join(source_output_dir, source, 'output', 'preprocessed_features.csv')
+    output_file = join(source_output_dir, source, "output", "predictions.csv")
+    feats_file = join(source_output_dir, source, "output", "preprocessed_features.csv")
 
     # remove all previously created files
-    files = glob(join(source_output_dir, 'output', '*'))
+    files = glob(join(source_output_dir, "output", "*"))
     for f in files:
         remove(f)
 
     with warnings.catch_warnings():
 
         # always suppress runtime warnings
-        warnings.filterwarnings('ignore', category=RuntimeWarning)
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
 
         # suppress additional warning types if specified
         for warning_type in suppress_warnings_for:
-            warnings.filterwarnings('ignore', category=warning_type)
+            warnings.filterwarnings("ignore", category=warning_type)
 
         compute_and_save_predictions(config_input, output_file, feats_file)
 
 
-def do_run_comparison(source,
-                      config_input,
-                      suppress_warnings_for=[]):
+def do_run_comparison(source, config_input, suppress_warnings_for=[]):
     """
     Run rsmcompre experiment automatically.
 
     Use the given experiment configuration file located in the given
     source directory.
 
     Parameters
@@ -803,32 +763,30 @@
         configuration file
     suppress_warnings_for : list, optional
         Categories for which warnings should be suppressed
         when running the experiments. Note that ``RuntimeWarning``s
         are always suppressed.
         Defaults to ``[]``.
     """
-    source_output_dir = 'test_outputs'
+    source_output_dir = "test_outputs"
     experiment_dir = join(source_output_dir, source)
 
     with warnings.catch_warnings():
 
         # always suppress runtime warnings
-        warnings.filterwarnings('ignore', category=RuntimeWarning)
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
 
         # suppress additional warning types if specified
         for warning_type in suppress_warnings_for:
-            warnings.filterwarnings('ignore', category=warning_type)
+            warnings.filterwarnings("ignore", category=warning_type)
 
         run_comparison(config_input, experiment_dir)
 
 
-def do_run_summary(source,
-                   config_input,
-                   suppress_warnings_for=[]):
+def do_run_summary(source, config_input, suppress_warnings_for=[]):
     """
     Run rsmsummarize experiment automatically.
 
     Use the given experiment configuration file located in the given
     source directory.
 
     Parameters
@@ -841,39 +799,36 @@
         or a dictionary with keys corresponding to fields in the
         configuration file
     suppress_warnings_for : list, optional
         Categories for which warnings should be suppressed when running the
         experiments.
         Defaults to ``[]``.
     """
-    source_output_dir = 'test_outputs'
+    source_output_dir = "test_outputs"
     experiment_dir = join(source_output_dir, source)
 
     # remove all previously created files
-    for output_subdir in ['output', 'figure', 'report']:
-        files = glob(join(source_output_dir, source, output_subdir, '*'))
+    for output_subdir in ["output", "figure", "report"]:
+        files = glob(join(source_output_dir, source, output_subdir, "*"))
         for f in files:
             remove(f)
 
     with warnings.catch_warnings():
 
         # always suppress runtime warnings
-        warnings.filterwarnings('ignore', category=RuntimeWarning)
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
 
         # suppress additional warning types if specified
         for warning_type in suppress_warnings_for:
-            warnings.filterwarnings('ignore', category=warning_type)
+            warnings.filterwarnings("ignore", category=warning_type)
 
         run_summary(config_input, experiment_dir)
 
 
-def do_run_cross_validation(source,
-                            experiment_id,
-                            config_input,
-                            suppress_warnings_for=[]):
+def do_run_cross_validation(source, experiment_id, config_input, suppress_warnings_for=[]):
     """
     Run rsmxval experiment automatically.
 
     Use the given experiment configuration file located in the
     given source directory and use the given experiment ID.
 
     Parameters
@@ -889,15 +844,15 @@
         configuration file.
     suppress_warnings_for : list, optional
         Categories for which warnings should be suppressed
         when running the experiments. Note that ``RuntimeWarning``s
         are always suppressed.
         Defaults to ``[]``.
     """
-    source_output_dir = 'test_outputs'
+    source_output_dir = "test_outputs"
     experiment_dir = join(source_output_dir, source)
 
     # remove all previously created files
     for output_subdir in ["folds", "fold-summary", "evaluation", "final-model"]:
         try:
             rmtree(join(source_output_dir, source, output_subdir))
         except FileNotFoundError:
@@ -906,26 +861,26 @@
         remove(join(source_output_dir, source, "rsmxval.json"))
     except FileNotFoundError:
         pass
 
     with warnings.catch_warnings():
 
         # always suppress runtime warnings
-        warnings.filterwarnings('ignore', category=RuntimeWarning)
+        warnings.filterwarnings("ignore", category=RuntimeWarning)
 
         # suppress additional warning types if specified
         for warning_type in suppress_warnings_for:
-            warnings.filterwarnings('ignore', category=warning_type)
+            warnings.filterwarnings("ignore", category=warning_type)
 
         # call rsmxval but make sure to silence the progress bar
         # that is displayed for the parallel rsmtool runs
         run_cross_validation(config_input, experiment_dir, silence_tqdm=True)
 
 
-def check_file_output(file1, file2, file_format='csv'):
+def check_file_output(file1, file2, file_format="csv"):
     """
     Check if the two given tabular files contain matching values.
 
     This function checks if two experiment files have values that are
     the same to within 3 decimal places. It raises an AssertionError if
     they are not.
 
@@ -937,15 +892,15 @@
         Path to the second files.
     file_format : str, optional
         The format of the output files.
         Defaults to "csv".
     """
     # make sure that the main id columns are read as strings since
     # this may affect merging in custom notebooks
-    string_columns = ['spkitemid', 'candidate']
+    string_columns = ["spkitemid", "candidate"]
 
     converter_dict = {column: str for column in string_columns}
 
     df1 = DataReader.read_from_file(file1, converters=converter_dict)
     df2 = DataReader.read_from_file(file2, converters=converter_dict)
 
     # convert all column names to strings
@@ -976,29 +931,25 @@
     for df in [df1, df2]:
         for c in df.columns:
             if df[c].dtype == np.int64:
                 df[c] = df[c].astype(np.float64)
 
     # for pca and factor correlations convert all values to absolutes
     # because the sign may not always be the same
-    if (file1.endswith('pca.{}'.format(file_format)) or
-            file1.endswith('factor_correlations.{}'.format(file_format))):
+    if file1.endswith(f"pca.{file_format}") or file1.endswith(f"factor_correlations.{file_format}"):
         for df in [df1, df2]:
             msk = df.dtypes == np.float64
             df.loc[:, msk] = df.loc[:, msk].abs()
 
     try:
-        assert_frame_equal(df1,
-                           df2,
-                           check_exact=False,
-                           rtol=1e-03)
+        assert_frame_equal(df1, df2, check_exact=False, rtol=1e-03)
     except AssertionError as e:
         message = e.args[0]
-        new_message = 'File {} - {}'.format(basename(file1), message)
-        e.args = (new_message, )
+        new_message = f"File {basename(file1)} - {message}"
+        e.args = (new_message,)
         raise
 
 
 def collect_warning_messages_from_report(html_file):
     """
     Collect all warning messages from the given HTML report.
 
@@ -1008,33 +959,31 @@
         Path to the HTML report file on disk.
 
     Returns
     -------
     warnings_text : list of str
         The list of collected warnings.
     """
-    with open(html_file, 'r') as htmlf:
-        soup = BeautifulSoup(htmlf.read(), 'html.parser')
+    with open(html_file, "r") as htmlf:
+        soup = BeautifulSoup(htmlf.read(), "html.parser")
 
     warnings_text = []
     for div in soup.findAll("div", {"class": "output_stderr"}):
 
         # we collect the text in the <pre> tags after the standard error,
         # and split the lines; we only keep the lines that contain 'Warning:'
         for pre in div.findAll("pre"):
             warnings_msgs = pre.text.splitlines()
-            warnings_msgs = [msg for msg in warnings_msgs if 'Warning:' in msg]
+            warnings_msgs = [msg for msg in warnings_msgs if "Warning:" in msg]
             warnings_text.extend(warnings_msgs)
 
     return warnings_text
 
 
-def check_report(html_file,
-                 raise_errors=True,
-                 raise_warnings=True):
+def check_report(html_file, raise_errors=True, raise_warnings=True):
     """
     Raise ``AssertionError`` if given HTML report contains errors or warnings.
 
     Parameters
     ----------
     html_file : str
         Path to the HTML report file on disk.
@@ -1050,15 +999,15 @@
     report_errors = 0
     report_warnings = 0
 
     # Setting raise_warnings to false if not in STRICT mode
     if IGNORE_WARNINGS:
         raise_warnings = False
 
-    with open(html_file, 'r') as htmlf:
+    with open(html_file, "r") as htmlf:
         for line in htmlf:
             m_error = html_error_regexp.search(line)
             if m_error:
                 report_errors += 1
             m_warning = html_warning_regexp.search(line)
             if m_warning:
                 # actual text of warning is in the next line of HTML file
@@ -1067,76 +1016,69 @@
                 # NOTE: there is a separate function
                 # ``collect_warning_messages_from_the_report`` that once again
                 # checks for warnings. The warnings filtered here might still
                 # be flagged by that function.
                 # See https://github.com/EducationalTestingService/rsmtool/issues/539
 
                 # we do not want to flag matlplotlib font cache warning
-                if not re.search(r'font\s*cache', warning_text, flags=re.IGNORECASE):
+                if not re.search(r"font\s*cache", warning_text, flags=re.IGNORECASE):
                     report_warnings += 1
 
     if raise_errors:
         assert_equal(report_errors, 0)
 
     if raise_warnings:
         assert_equal(report_warnings, 0)
 
 
-def check_scaled_coefficients(output_dir, experiment_id, file_format='csv'):
+def check_scaled_coefficients(output_dir, experiment_id, file_format="csv"):
     """
     Check that predictions using scaled coefficients match scaled scores.
 
     Parameters
     ----------
     output_dir : str
          Path to the experiment output directory for a test.
     experiment_id : str
         The experiment ID.
     file_format : str, optional
         The format of the output files.
         Defaults to "csv".
-        """
-    preprocessed_test_file = join(output_dir,
-                                  '{}_test_preprocessed_features.{}'.format(experiment_id,
-                                                                            file_format))
-    scaled_coefficients_file = join(output_dir,
-                                    '{}_coefficients_scaled.{}'.format(experiment_id,
-                                                                       file_format))
-    predictions_file = join(output_dir,
-                            '{}_pred_processed.{}'.format(experiment_id,
-                                                          file_format))
-
-    postprocessing_params_file = join(output_dir,
-                                      '{}_postprocessing_params.{}'.format(experiment_id,
-                                                                           file_format))
+    """
+    preprocessed_test_file = join(
+        output_dir, f"{experiment_id}_test_preprocessed_features.{file_format}"
+    )
+    scaled_coefficients_file = join(
+        output_dir, f"{experiment_id}_coefficients_scaled.{file_format}"
+    )
+    predictions_file = join(output_dir, f"{experiment_id}_pred_processed.{file_format}")
 
-    postproc_params = DataReader.read_from_file(postprocessing_params_file).loc[0]
     df_preprocessed_test_data = DataReader.read_from_file(preprocessed_test_file)
     df_old_predictions = DataReader.read_from_file(predictions_file)
-    df_old_predictions = df_old_predictions[['spkitemid', 'sc1', 'scale']]
+    df_old_predictions = df_old_predictions[["spkitemid", "sc1", "scale"]]
 
     # create fake skll objects with new coefficients
     df_coef = DataReader.read_from_file(scaled_coefficients_file)
     learner = Modeler().create_fake_skll_learner(df_coef)
     modeler = Modeler.load_from_learner(learner)
 
     # generate new predictions and rename the prediction column to 'scale'
-    df_new_predictions = modeler.predict(df_preprocessed_test_data,
-                                         postproc_params['trim_min'],
-                                         postproc_params['trim_max'])
-    df_new_predictions.rename(columns={'raw': 'scale'}, inplace=True)
+    df_new_predictions = modeler.predict(df_preprocessed_test_data)
+    df_new_predictions.rename(columns={"raw": "scale"}, inplace=True)
 
     # check that new predictions match the scaled old predictions
-    assert_frame_equal(df_new_predictions.sort_index(axis=1),
-                       df_old_predictions.sort_index(axis=1),
-                       check_exact=False,
-                       rtol=1e-03)
+    assert_frame_equal(
+        df_new_predictions.sort_index(axis=1),
+        df_old_predictions.sort_index(axis=1),
+        check_exact=False,
+        rtol=1e-03,
+    )
 
 
-def check_generated_output(generated_files, experiment_id, model_source, file_format='csv'):
+def check_generated_output(generated_files, experiment_id, model_source, file_format="csv"):
     """
     Check that all necessary output files have been generated.
 
     Parameters
     ----------
     generated_files : list of str
         List of files generated by a test.
@@ -1144,74 +1086,76 @@
         The experiment ID.
     model_source : str
         One of "rsmtool" or "skll".
     file_format : str, optional
         The format of the output files.
         Defaults to "csv".
     """
-    file_must_have_both = ["_confMatrix.{}".format(file_format),
-                           "_cors_orig.{}".format(file_format),
-                           "_cors_processed.{}".format(file_format),
-                           "_eval.{}".format(file_format),
-                           "_eval_short.{}".format(file_format),
-                           "_feature.{}".format(file_format),
-                           "_feature_descriptives.{}".format(file_format),
-                           "_feature_descriptivesExtra.{}".format(file_format),
-                           "_feature_outliers.{}".format(file_format),
-                           "_margcor_score_all_data.{}".format(file_format),
-                           "_pca.{}".format(file_format),
-                           "_pcavar.{}".format(file_format),
-                           "_pcor_score_all_data.{}".format(file_format),
-                           "_pred_processed.{}".format(file_format),
-                           "_pred_train.{}".format(file_format),
-                           "_score_dist.{}".format(file_format),
-                           "_train_preprocessed_features.{}".format(file_format),
-                           "_test_preprocessed_features.{}".format(file_format),
-                           "_postprocessing_params.{}".format(file_format)
-                           ]
-
-    file_must_have_rsmtool = ["_betas.{}".format(file_format),
-                              "_coefficients.{}".format(file_format)]
-    if model_source == 'rsmtool':
+    file_must_have_both = [
+        f"_confMatrix.{file_format}",
+        f"_cors_orig.{file_format}",
+        f"_cors_processed.{file_format}",
+        f"_eval.{file_format}",
+        f"_eval_short.{file_format}",
+        f"_feature.{file_format}",
+        f"_feature_descriptives.{file_format}",
+        f"_feature_descriptivesExtra.{file_format}",
+        f"_feature_outliers.{file_format}",
+        f"_margcor_score_all_data.{file_format}",
+        f"_pca.{file_format}",
+        f"_pcavar.{file_format}",
+        f"_pcor_score_all_data.{file_format}",
+        f"_pred_processed.{file_format}",
+        f"_pred_train.{file_format}",
+        f"_score_dist.{file_format}",
+        f"_train_preprocessed_features.{file_format}",
+        f"_test_preprocessed_features.{file_format}",
+        f"_postprocessing_params.{file_format}",
+    ]
+
+    file_must_have_rsmtool = [f"_betas.{file_format}", f"_coefficients.{file_format}"]
+    if model_source == "rsmtool":
         file_must_have = file_must_have_both + file_must_have_rsmtool
     else:
         file_must_have = file_must_have_both
 
     file_must_with_id = [experiment_id + file_name for file_name in file_must_have]
     file_exist = [basename(file_name) for file_name in generated_files]
     missing_file = set(file_must_with_id).difference(set(file_exist))
-    assert_equal(len(missing_file), 0, "Missing files: {}".format(','.join(missing_file)))
+    assert_equal(len(missing_file), 0, f"Missing files: {','.join(missing_file)}")
 
 
-def check_consistency_files_exist(generated_files, experiment_id, file_format='csv'):
+def check_consistency_files_exist(generated_files, experiment_id, file_format="csv"):
     """
     Check that the consistency files were generated.
 
     Parameters
     ----------
     generated_files : list of str
         List of files generated by a test.
     experiment_id : str
         The experiment ID.
     file_format : str, optional
         The format of the output files.
         Defaults to "csv".
     """
-    file_must_have = ["_consistency.{}".format(file_format),
-                      "_degradation.{}".format(file_format),
-                      "_disattenuated_correlations.{}".format(file_format),
-                      "_true_score_eval.{}".format(file_format)]
+    file_must_have = [
+        f"_consistency.{file_format}",
+        f"_degradation.{file_format}",
+        f"_disattenuated_correlations.{file_format}",
+        f"_true_score_eval.{file_format}",
+    ]
 
     file_must_with_id = [experiment_id + file_name for file_name in file_must_have]
     file_exist = [basename(file_name) for file_name in generated_files]
     missing_file = set(file_must_with_id).difference(set(file_exist))
-    assert_equal(len(missing_file), 0, "Missing files: {}".format(','.join(missing_file)))
+    assert_equal(len(missing_file), 0, f"Missing files: {','.join(missing_file)}")
 
 
-def check_subgroup_outputs(output_dir, experiment_id, subgroups, file_format='csv'):
+def check_subgroup_outputs(output_dir, experiment_id, subgroups, file_format="csv"):
     """
     Check that the subgroup-related outputs are accurate.
 
     Parameters
     ----------
     output_dir : str
         Path to the `output` experiment output directory for a test.
@@ -1220,57 +1164,46 @@
     subgroups : list of str
         List of column names that contain grouping
         information.
     file_format : str, optional
         The format of the output files.
         Defaults to "csv".
     """
-    train_preprocessed_file = join(output_dir,
-                                   '{}_train_metadata.{}'.format(experiment_id,
-                                                                 file_format))
+    train_preprocessed_file = join(output_dir, f"{experiment_id}_train_metadata.{file_format}")
     train_preprocessed = DataReader.read_from_file(train_preprocessed_file, index_col=0)
 
-    test_preprocessed_file = join(output_dir,
-                                  '{}_test_metadata.{}'.format(experiment_id,
-                                                               file_format))
-    test_preprocessed = DataReader.read_from_file(test_preprocessed_file,
-                                                  index_col=0)
+    test_preprocessed_file = join(output_dir, f"{experiment_id}_test_metadata.{file_format}")
+    test_preprocessed = DataReader.read_from_file(test_preprocessed_file, index_col=0)
     for group in subgroups:
         ok_(group in train_preprocessed.columns)
         ok_(group in test_preprocessed.columns)
 
     # check that the total sum of N per category matches the total N
     # in data composition and the total N categories matches what is
     # in overall data composition
-    file_data_composition_all = join(output_dir,
-                                     '{}_data_composition.{}'.format(experiment_id,
-                                                                     file_format))
+    file_data_composition_all = join(output_dir, f"{experiment_id}_data_composition.{file_format}")
     df_data_composition_all = DataReader.read_from_file(file_data_composition_all)
     for group in subgroups:
-        file_composition_by_group = join(output_dir,
-                                         '{}_data_composition_by_{}.{}'.format(experiment_id,
-                                                                               group,
-                                                                               file_format))
+        file_composition_by_group = join(
+            output_dir, f"{experiment_id}_data_composition_by_{group}.{file_format}"
+        )
         composition_by_group = DataReader.read_from_file(file_composition_by_group)
-        for partition in ['Training', 'Evaluation']:
-            partition_info = df_data_composition_all.loc[df_data_composition_all['partition'] ==
-                                                         partition]
-
-            summation = sum(composition_by_group['{} set'
-                                                 ''.format(partition)])
-            ok_(summation == partition_info.iloc[0]['responses'])
+        for partition in ["Training", "Evaluation"]:
+            partition_info = df_data_composition_all.loc[
+                df_data_composition_all["partition"] == partition
+            ]
 
-            length = len(composition_by_group.loc[composition_by_group['{} set'
-                                                                       ''.format(partition)] != 0])
+            summation = sum(composition_by_group[f"{partition} set"])
+            ok_(summation == partition_info.iloc[0]["responses"])
+
+            length = len(composition_by_group.loc[composition_by_group[f"{partition} set"] != 0])
             ok_(length == partition_info.iloc[0][group])
 
 
-def copy_data_files(temp_dir_name,
-                    input_file_dict,
-                    given_test_dir):
+def copy_data_files(temp_dir_name, input_file_dict, given_test_dir):
     """
     Copy files from given test directory to a temporary directory.
 
     Useful for tests where the current directory is to be used as the
     reference for resolving paths in the configuration.
 
     Parameters
@@ -1339,18 +1272,15 @@
         or been added in those outputs.
     missing_or_empty_sources : list
         List of source names whose corresponding directories are either
         missing under ``updated_outputs_directory` or do exist but are
         empty.
     """
 
-    def __init__(self,
-                 test_suffixes,
-                 tests_directory,
-                 updated_outputs_directory):
+    def __init__(self, test_suffixes, tests_directory, updated_outputs_directory):
         """Instantiate a FileUpdater object."""
         self.test_suffixes = test_suffixes
         self.tests_directory = Path(tests_directory)
         self.updated_outputs_directory = Path(updated_outputs_directory)
         self.missing_or_empty_sources = []
         self.deleted_files = []
         self.updated_files = []
@@ -1369,29 +1299,32 @@
 
         Returns
         -------
         exclude : bool
             ``True`` if the file should be excluded.
             ``False`` otherwise.
         """
-        possible_suffixes = ['.model', '.npy']
-        possible_stems = ['_postprocessing_params', '_eval', '_eval_short',
-                          '_confMatrix', '_pred_train', '_pred_processed',
-                          '_score_dist']
+        possible_suffixes = [".model", ".npy"]
+        possible_stems = [
+            "_postprocessing_params",
+            "_eval",
+            "_eval_short",
+            "_confMatrix",
+            "_pred_train",
+            "_pred_processed",
+            "_score_dist",
+        ]
 
         file_stem = Path(filename).stem
         file_suffix = Path(filename).suffix
-        return any(file_suffix == suffix for suffix in possible_suffixes) or \
-            any(file_stem.endswith(stem) for stem in possible_stems)
+        return any(file_suffix == suffix for suffix in possible_suffixes) or any(
+            file_stem.endswith(stem) for stem in possible_stems
+        )
 
-    def update_source(self,
-                      source,
-                      skll=False,
-                      file_type='output',
-                      input_source=None):
+    def update_source(self, source, skll=False, file_type="output", input_source=None):
         """
         Update test output or input data for test named ``source``.
 
         This method updates the test output or input data for experiment test
         with ``source`` as the given name. It deletes files that are only in
         the tests directory, adds files that are only in the updated test
         outputs directory, and updates the files that have changed in the
@@ -1413,38 +1346,38 @@
         input_source: str, optional
             The name of the source directory for input files
             Defaults to ``None``.
         """
         # locate the updated outputs for the experiment under the given
         # outputs directory, locate the existing experiment outputs
         # and define how we will refer to the test
-        if file_type == 'output':
+        if file_type == "output":
             updated_output_path = self.updated_outputs_directory / source / "output"
             existing_output_path = self.tests_directory / "data" / "experiments" / source / "output"
             test_name = source
         else:
             updated_output_path = self.updated_outputs_directory / input_source / "output"
-            existing_output_path = (self.tests_directory / "data" / "experiments" / source /
-                                    input_source / "output")
-            test_name = f'{source}/{input_source}'
+            existing_output_path = (
+                self.tests_directory / "data" / "experiments" / source / input_source / "output"
+            )
+            test_name = f"{source}/{input_source}"
 
         # if the directory for this source does not exist on the updated output
         # side, then that's a problem and something we should report on later
         try:
             assert updated_output_path.exists()
         except AssertionError:
             self.missing_or_empty_sources.append(test_name)
             return
 
         # if the existing output path does not exist, then create it
         try:
             assert existing_output_path.exists()
         except AssertionError:
-            sys.stderr.write("\nNo existing output for \"{}\". "
-                             "Creating directory ...\n".format(test_name))
+            sys.stderr.write(f'\nNo existing output for "{test_name}". Creating directory ...\n')
             existing_output_path.mkdir(parents=True)
 
         # get a comparison betwen the two directories
         dir_comparison = dircmp(updated_output_path, existing_output_path)
 
         # if no output was found in the updated outputs directory, that's
         # likely to be a problem so save that source
@@ -1459,25 +1392,32 @@
             remove(existing_output_path / file)
 
         # Next find all the NEW files in the updated outputs.
         new_files = dir_comparison.left_only
 
         # We also define several types of files we exclude.
         # 1. we exclude OLS summary files
-        excluded_suffixes = ['_ols_summary.txt',
-                             '.ols', '.model', '.npy']
+        excluded_suffixes = ["_ols_summary.txt", ".ols", ".model", ".npy"]
 
         # 2. for output files we exclude all json files.
         # We keep these files if we are dealing with input files.
-        if file_type == 'output':
-            excluded_suffixes.extend(['_rsmtool.json', '_rsmeval.json',
-                                      '_rsmsummarize.json', '_rsmcompare.json',
-                                      '_rsmxval.json'])
-
-        new_files = [f for f in new_files if not any(f.endswith(suffix) for suffix in excluded_suffixes)]
+        if file_type == "output":
+            excluded_suffixes.extend(
+                [
+                    "_rsmtool.json",
+                    "_rsmeval.json",
+                    "_rsmsummarize.json",
+                    "_rsmcompare.json",
+                    "_rsmxval.json",
+                ]
+            )
+
+        new_files = [
+            f for f in new_files if not any(f.endswith(suffix) for suffix in excluded_suffixes)
+        ]
 
         # 3. We also exclude files related to model evaluations for SKLL models.
         if skll:
             new_files = [f for f in new_files if not self.is_skll_excluded_file(f)]
 
         # next we get the files that have changed and try to figure out if they
         # have actually changed beyond a tolerance level that we care about for
@@ -1486,20 +1426,22 @@
         # assume that they have really changed since we have no easy way to compare.
         changed_files = dir_comparison.diff_files
         really_changed_files = []
         for changed_file in changed_files:
             include_file = True
             updated_output_filepath = updated_output_path / changed_file
             existing_output_filepath = existing_output_path / changed_file
-            file_format = updated_output_filepath.suffix.lstrip('.')
-            if file_format in ['csv', 'tsv', 'xlsx']:
+            file_format = updated_output_filepath.suffix.lstrip(".")
+            if file_format in ["csv", "tsv", "xlsx"]:
                 try:
-                    check_file_output(str(updated_output_filepath),
-                                      str(existing_output_filepath),
-                                      file_format=file_format)
+                    check_file_output(
+                        str(updated_output_filepath),
+                        str(existing_output_filepath),
+                        file_format=file_format,
+                    )
                 except AssertionError:
                     pass
                 else:
                     include_file = False
 
             if include_file:
                 really_changed_files.append(changed_file)
@@ -1509,18 +1451,15 @@
         for file in new_or_changed_files:
             copyfile(updated_output_path / file, existing_output_path / file)
 
         # Update the lists with files that were changed for this source
         self.deleted_files.extend([(test_name, file) for file in existing_output_only_files])
         self.updated_files.extend([(test_name, file) for file in new_or_changed_files])
 
-    def update_test_data(self,
-                         source,
-                         test_tool,
-                         skll=False):
+    def update_test_data(self, source, test_tool, skll=False):
         """
         Determine whether to update input or output data and run ``update_source()``.
 
         Parameters
         ----------
         source : str
             Name of source directory.
@@ -1536,99 +1475,99 @@
         if test_tool in tools_with_output:
             self.update_source(source, skll=skll)
         # if we have a tool with input data we also update inputs
         if test_tool in tools_with_input_data:
             for input_dir in existing_output_path.parent.iterdir():
                 if not input_dir.is_dir():
                     continue
-                if input_dir.name in ['output', 'figure', 'report']:
+                if input_dir.name in ["output", "figure", "report"]:
                     continue
                 else:
                     input_source = input_dir.name
-                    self.update_source(source,
-                                       skll=skll,
-                                       file_type='input',
-                                       input_source=input_source)
+                    self.update_source(
+                        source, skll=skll, file_type="input", input_source=input_source
+                    )
 
     def run(self):
         """Update test data in files given by the ``test_suffixes`` attribute."""
         # import all the test_suffix experiment files using SourceFileLoader
-        # adapted from: http://stackoverflow.com/questions/67631/how-to-import-a-module-given-the-full-path
+        # adapted from: https://stackoverflow.com/a/67692
         for test_suffix in self.test_suffixes:
-            test_module_path = join(self.tests_directory, 'test_experiment_{}.py'.format(test_suffix))
-            test_module = SourceFileLoader('loaded_{}'.format(test_suffix), test_module_path).load_module()
-            test_tool = test_suffix.split('_')[0]
+            test_module_path = join(self.tests_directory, f"test_experiment_{test_suffix}.py")
+            test_module = SourceFileLoader(f"loaded_{test_suffix}", test_module_path).load_module()
+            test_tool = test_suffix.split("_")[0]
 
             # skip the module if it tells us that it doesn't want the data for its tests updated
-            if hasattr(test_module, '_AUTO_UPDATE'):
+            if hasattr(test_module, "_AUTO_UPDATE"):
                 if not test_module._AUTO_UPDATE:
                     continue
 
             # iterate over all the members and focus on only the experiment functions.
             # For rsmtool/rsmeval we skip over the functions that are decorated with
             # '@raises' since those functions do not need any test data to be updated.
             # For rsmsummarize and rsmcompare we only update the input files for these functions.
             # For the rest, try to get the source since that's what we need to update
             # the test files.
             for member_name, member_object in getmembers(test_module):
-                if isfunction(member_object) and member_name.startswith('test_run_experiment'):
+                if isfunction(member_object) and member_name.startswith("test_run_experiment"):
                     function = member_object
 
                     # get the qualified name of the member function
                     member_qualified_name = member_object.__qualname__
 
                     # check if it has 'raises' in the qualified name
                     # and skip it
-                    if 'raises' in member_qualified_name:
+                    if "raises" in member_qualified_name:
                         continue
 
                     # otherwise first we check if it's the parameterized function and if so
                     # we can easily get the source from the parameter list
-                    if member_name.endswith('parameterized'):
+                    if member_name.endswith("parameterized"):
                         for param in function.parameterized_input:
                             source_name = param.args[0]
-                            skll = param.kwargs.get('skll', False)
-                            self.update_test_data(source_name,
-                                                  test_tool,
-                                                  skll=skll)
+                            skll = param.kwargs.get("skll", False)
+                            self.update_test_data(source_name, test_tool, skll=skll)
 
                     # if it's another function, then we actually inspect the code
                     # to get the source. Note that this should never be a SKLL experiment
                     # since those should always be run parameterized
                     else:
                         function_code_lines = getsourcelines(function)
-                        source_line = [line for line in function_code_lines[0]
-                                       if re.search(r'source = ', line)]
-                        source_name = eval(source_line[0].strip().split(' = ')[1])
+                        source_line = [
+                            line for line in function_code_lines[0] if re.search(r"source = ", line)
+                        ]
+                        source_name = eval(source_line[0].strip().split(" = ")[1])
                         self.update_test_data(source_name, test_tool)
 
     def print_report(self):
         """Print a report of all changes made when the updater was run."""
         # print out the number and list of overall deleted files
-        print('{} deleted:'.format(len(self.deleted_files)))
+        print(f"{len(self.deleted_files)} deleted:")
         for source, deleted_file in self.deleted_files:
-            print('{} {}'.format(source, deleted_file))
+            print(f"{source} {deleted_file}")
         print()
 
         # find added/updated input files: in this case the source # will consist of
         # the test name and the input test name separated by '/'.
-        updated_input_files = [(source, updated_file) for (source, updated_file)
-                               in self.updated_files if '/' in source]
+        updated_input_files = [
+            (source, updated_file) for (source, updated_file) in self.updated_files if "/" in source
+        ]
 
         # print out the number and list of overall added/updated non-model files
-        print('{} added/updated:'.format(len(self.updated_files)))
+        print(f"{len(self.updated_files)} added/updated:")
         for source, updated_file in self.updated_files:
-            print('{} {}'.format(source, updated_file))
+            print(f"{source} {updated_file}")
         print()
 
         # now print out missing and/or empty updated output directories
-        print('{} missing/empty sources in updated outputs:'.format(len(self.missing_or_empty_sources)))
+        print(f"{len(self.missing_or_empty_sources)} missing/empty sources in updated outputs:")
         for source in self.missing_or_empty_sources:
-            print('{}'.format(source))
+            print(f"{source}")
         print()
 
         # if we updated any input files, let the user know that they need to
         # re-run the tests and update test outputs
         if len(updated_input_files) > 0:
-            print("WARNING: {} input files for rsmcompare/rsmsummarize "
-                  "tests have been updated. You need to re-run these "
-                  "tests and update test outputs".format(len(updated_input_files)))
+            print(
+                f"WARNING: {len(updated_input_files)} input files for rsmcompare/rsmsummarize "
+                f"tests have been updated. You need to re-run these tests and update test outputs"
+            )
```

### Comparing `rsmtool-9.0.1/rsmtool/transformer.py` & `rsmtool-9.1.1/rsmtool/transformer.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,18 @@
 from scipy.stats.stats import pearsonr
 
 
 class FeatureTransformer:
     """Encapsulate feature transformation methods."""
 
     def __init__(self, logger=None):
+        """Initialize the FeatureTransformer object."""
         self.logger = logger if logger else logging.getLogger(__name__)
 
-    def apply_sqrt_transform(self,
-                             name,
-                             values,
-                             raise_error=True):
+    def apply_sqrt_transform(self, name, values, raise_error=True):
         """
         Apply the "sqrt" transform to ``values``.
 
         Parameters
         ----------
         name : str
             Name of the feature to transform.
@@ -48,32 +46,30 @@
         ValueError
             If the transform is applied to a feature that has negative
             values and ``raise_error`` is ``True``.
         """
         # check if the feature has any negative values
         if np.any(values < 0):
             if raise_error:
-                raise ValueError("The sqrt transformation should not be "
-                                 "applied to feature {} which can have "
-                                 "negative values".format(name))
+                raise ValueError(
+                    f"The sqrt transformation should not be applied to "
+                    f"feature {name} which can have negative values."
+                )
             else:
-                self.logger.warning("The sqrt transformation was "
-                                    "applied to feature {} which has "
-                                    "negative values for some responses. "
-                                    "No system score will be generated "
-                                    "for such responses".format(name))
+                self.logger.warning(
+                    f"The sqrt transformation was applied to feature "
+                    f"{name} which has negative values for some responses. "
+                    f"No system score will be generated for such responses"
+                )
 
-        with np.errstate(invalid='ignore'):
+        with np.errstate(invalid="ignore"):
             new_data = np.sqrt(values)
         return new_data
 
-    def apply_log_transform(self,
-                            name,
-                            values,
-                            raise_error=True):
+    def apply_log_transform(self, name, values, raise_error=True):
         """
         Apply the "log" transform to ``values``.
 
         Parameters
         ----------
         name : str
             Name of the feature to transform.
@@ -95,45 +91,43 @@
         ValueError
             If the transform is applied to a feature that has
             zero or negative values and ``raise_error`` is ``True``.
         """
         # check if the feature has any zeros
         if np.any(values == 0):
             if raise_error:
-                raise ValueError("The log transformation should not be "
-                                 "applied to feature {} which can have a "
-                                 "value of 0".format(name))
+                raise ValueError(
+                    f"The log transformation should not be applied to "
+                    f"feature {name} which can have a value of 0."
+                )
             else:
-                self.logger.warning("The log transformation was "
-                                    "applied to feature {} which has a "
-                                    "value of 0 for some responses. No system "
-                                    "score will "
-                                    "be generated for such responses".format(name))
+                self.logger.warning(
+                    f"The log transformation was applied to feature "
+                    f"{name} which has a value of 0 for some responses. "
+                    f"No system score will be generated for such responses."
+                )
 
         # check if the feature has any negative values
         if np.any(values < 0):
             if raise_error:
-                raise ValueError("The log transformation should not be "
-                                 "applied to feature {} which can have "
-                                 "negative values".format(name))
+                raise ValueError(
+                    f"The log transformation should not be applied to "
+                    f"feature {name} which can have negative values."
+                )
             else:
-                self.logger.warning("The log transformation was "
-                                    "applied to feature {} which has "
-                                    "negative values for some responses. No system "
-                                    "score will "
-                                    "be generated for such responses".format(name))
+                self.logger.warning(
+                    f"The log transformation was applied to feature "
+                    f"{name} which has negative values for some responses. "
+                    f"No system score will be generated for such responses"
+                )
 
         new_data = np.log(values)
         return new_data
 
-    def apply_inverse_transform(self,
-                                name,
-                                values,
-                                raise_error=True,
-                                sd_multiplier=4):
+    def apply_inverse_transform(self, name, values, raise_error=True, sd_multiplier=4):
         """
         Apply the "inv" (inverse) transform to ``values``.
 
         Parameters
         ----------
         name : str
             Name of the feature to transform.
@@ -161,56 +155,58 @@
         ValueError
             If the transform is applied to a feature that is
             zero or to a feature that can have different
             signs, and ``raise_error`` is ``True``.
         """
         if np.any(values == 0):
             if raise_error:
-                raise ValueError("The inverse transformation should not be "
-                                 "applied to feature {} which can have a "
-                                 "value of 0".format(name))
+                raise ValueError(
+                    f"The inverse transformation should not be applied "
+                    f"to feature {name} which can have a value of 0."
+                )
             else:
-                self.logger.warning("The inverse transformation was applied to "
-                                    "feature {} which has a value of 0 for "
-                                    "some responses. No system score will be "
-                                    "generated for such responses".format(name))
+                self.logger.warning(
+                    f"The inverse transformation was applied to feature "
+                    f"{name} which has a value of 0 for some responses. "
+                    f"No system score will be generated for such responses."
+                )
 
         # check if the floor or ceiling are zero
         data_mean = np.mean(values)
         data_sd = np.std(values, ddof=1)
         floor = data_mean - sd_multiplier * data_sd
         ceiling = data_mean + sd_multiplier * data_sd
         if floor == 0 or ceiling == 0:
-            self.logger.warning("The floor/ceiling for feature {} "
-                                "is zero after applying the inverse "
-                                "transformation".format(name))
+            self.logger.warning(
+                f"The floor/ceiling for feature {name} is zero after "
+                f"applying the inverse transformation."
+            )
 
         # check if the feature can be both positive and negative
         all_positive = np.all(np.abs(values) == values)
         all_negative = np.all(np.abs(values) == -values)
         if not (all_positive or all_negative):
             if raise_error:
-                raise ValueError("The inverse transformation should not be "
-                                 "applied to feature {} where the values can "
-                                 "have different signs".format(name))
+                raise ValueError(
+                    f"The inverse transformation should not be applied "
+                    f"to feature {name} where the values can have different signs"
+                )
             else:
-                self.logger.warning("The inverse transformation was "
-                                    "applied to feature {} where the values can"
-                                    "have different signs. This can change "
-                                    "the ranking of the responses".format(name))
+                self.logger.warning(
+                    f"The inverse transformation was applied to feature "
+                    f"{name} where the values can have different signs. "
+                    f"This can change the ranking of the responses."
+                )
 
-        with np.errstate(divide='ignore'):
+        with np.errstate(divide="ignore"):
             new_data = 1 / values
 
         return new_data
 
-    def apply_add_one_inverse_transform(self,
-                                        name,
-                                        values,
-                                        raise_error=True):
+    def apply_add_one_inverse_transform(self, name, values, raise_error=True):
         """
         Apply the "addOneInv" (add one and invert) transform to ``values``.
 
         Parameters
         ----------
         name : str
             Name of the feature to transform.
@@ -231,31 +227,30 @@
         ValueError
             If the transform is applied to a feature that
             has negative values and ``raise_error`` is ``True``.
         """
         # check if the feature has any negative values
         if np.any(values < 0):
             if raise_error:
-                raise ValueError("The addOneInv transformation should not "
-                                 "be applied to feature {} which can have "
-                                 "negative values".format(name))
+                raise ValueError(
+                    f"The addOneInv transformation should not be applied "
+                    f"to feature {name} which can have negative values."
+                )
             else:
-                self.logger.warning("The addOneInv transformation was "
-                                    "applied to feature {} which has "
-                                    "negative values for some responses. "
-                                    "This can change the ranking of the "
-                                    "responses".format(name))
+                self.logger.warning(
+                    f"The addOneInv transformation was applied to "
+                    f"feature {name} which has negative values for "
+                    f"some responses. This can change the ranking of "
+                    f"the responses."
+                )
 
         new_data = 1 / (values + 1)
         return new_data
 
-    def apply_add_one_log_transform(self,
-                                    name,
-                                    values,
-                                    raise_error=True):
+    def apply_add_one_log_transform(self, name, values, raise_error=True):
         """
         Apply the "addOneLn" (add one and log) transform to ``values``.
 
         Parameters
         ----------
         name : str
             Name of the feature to transform.
@@ -276,33 +271,30 @@
         ValueError
             If the transform is applied to a feature that
             has negative values and ``raise_error`` is ``True``.
         """
         # check if the feature has any negative values
         if np.any(values < 0):
             if raise_error:
-                raise ValueError("The addOneLn transformation should not "
-                                 "be applied to feature {} which can have "
-                                 "negative values".format(name))
+                raise ValueError(
+                    f"The addOneLn transformation should not be applied "
+                    f"to feature {name} which can have negative values."
+                )
             else:
-                self.logger.warning("The log transformation was "
-                                    "applied to feature {} which has "
-                                    "negative values for some responses. "
-                                    "If the feature value remains negative "
-                                    "after adding one, no score will "
-                                    "be generated for such responses".format(name))
+                self.logger.warning(
+                    f"The log transformation was applied to feature "
+                    f"{name} which has negative values for some responses. "
+                    f"If the feature value remains negative after adding one, "
+                    f"no score will be generated for such responses."
+                )
 
         new_data = np.log(values + 1)
         return new_data
 
-    def transform_feature(self,
-                          values,
-                          column_name,
-                          transform,
-                          raise_error=True):
+    def transform_feature(self, values, column_name, transform, raise_error=True):
         """
         Apply given transform to all values in the given numpy array.
 
         The values are assumed to be for the feature with the given name.
 
         Parameters
         ----------
@@ -330,35 +322,33 @@
 
         Note
         ----
         Many of these transformations may be meaningless for features which
         span both negative and positive values. Some transformations may
         throw errors for negative feature values.
         """
-        transforms = {'inv': self.apply_inverse_transform,
-                      'sqrt': self.apply_sqrt_transform,
-                      'log': self.apply_log_transform,
-                      'addOneInv': self.apply_add_one_inverse_transform,
-                      'addOneLn': self.apply_add_one_log_transform,
-                      'raw': lambda column_name, data, raise_error: data,
-                      'org': lambda column_name, data, raise_error: data}
+        transforms = {
+            "inv": self.apply_inverse_transform,
+            "sqrt": self.apply_sqrt_transform,
+            "log": self.apply_log_transform,
+            "addOneInv": self.apply_add_one_inverse_transform,
+            "addOneLn": self.apply_add_one_log_transform,
+            "raw": lambda column_name, data, raise_error: data,
+            "org": lambda column_name, data, raise_error: data,
+        }
 
         # make sure we have a valid transform function
         if transform is None or transform not in transforms:
-            raise ValueError('Unrecognized feature transformation: '
-                             ' {}'.format(transform))
+            raise ValueError(f"Unrecognized feature transformation:  {transform}")
 
         transformer = transforms.get(transform)
         new_data = transformer(column_name, values, raise_error)
         return new_data
 
-    def find_feature_transform(self,
-                               feature_name,
-                               feature_value,
-                               scores):
+    def find_feature_transform(self, feature_name, feature_value, scores):
         """
         Identify best transformation for feature given correlation with score.
 
         The best transformation is chosen based on the absolute Pearson
         correlation with human score.
 
         Parameters
@@ -377,27 +367,22 @@
             between the feature values and the human scores. See
             :ref:`documentation <select_transformations_rsmtool>` for the
             full list of transformations.
         """
         # Do not use sqrt and ln for potential negative features.
         # Do not use inv for positive features.
         if any(feature_value < 0):
-            applicable_transformations = ['org', 'inv']
+            applicable_transformations = ["org", "inv"]
         else:
-            applicable_transformations = ['org',
-                                          'sqrt',
-                                          'addOneInv',
-                                          'addOneLn']
+            applicable_transformations = ["org", "sqrt", "addOneInv", "addOneLn"]
 
         correlations = []
         for trans in applicable_transformations:
             try:
-                transformed_value = self.transform_feature(feature_value,
-                                                           feature_name,
-                                                           trans)
+                transformed_value = self.transform_feature(feature_value, feature_name, trans)
 
                 correlations.append(abs(pearsonr(transformed_value, scores)[0]))
             except ValueError:
                 # If the transformation returns an error, append 0.
                 correlations.append(0)
         best = np.argmax(correlations)
         best_transformation = applicable_transformations[best]
```

### Comparing `rsmtool-9.0.1/rsmtool/utils/commandline.py` & `rsmtool-9.1.1/rsmtool/utils/commandline.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,42 +17,48 @@
 from itertools import chain, product
 from pathlib import Path
 
 from prompt_toolkit.completion import FuzzyWordCompleter, PathCompleter, WordCompleter
 from prompt_toolkit.formatted_text import HTML
 from prompt_toolkit.shortcuts import CompleteStyle, clear, print_formatted_text, prompt
 from prompt_toolkit.validation import Validator
+
 from rsmtool import VERSION_STRING
 from rsmtool.configuration_parser import Configuration
 from rsmtool.reporter import Reporter
 
-from .constants import (CHECK_FIELDS,
-                        CONFIGURATION_DOCUMENTATION_SLUGS,
-                        DEFAULTS,
-                        INTERACTIVE_MODE_METADATA,
-                        POSSIBLE_EXTENSIONS)
+from .constants import (
+    CHECK_FIELDS,
+    CONFIGURATION_DOCUMENTATION_SLUGS,
+    DEFAULTS,
+    INTERACTIVE_MODE_METADATA,
+    POSSIBLE_EXTENSIONS,
+)
 
 # a named tuple for use with the `setup_rsmcmd_parser` function below
 # to specify additional options for either of the subcommand parsers.
 # An example can be found in `rsmpredict.py`. All of the attributes
 # are directly named for the arguments that are used with
 # the `ArgParser.add_argument()` method. The `dest` and `help`
 # options are required but the rest can be left unspecified and
 # will default to `None`.
-CmdOption = namedtuple('CmdOption',
-                       ['dest', 'help', 'shortname', 'longname', 'action',
-                        'default', 'required', 'nargs'],
-                       defaults=(None,) * 6)
+CmdOption = namedtuple(
+    "CmdOption",
+    ["dest", "help", "shortname", "longname", "action", "default", "required", "nargs"],
+    defaults=(None,) * 6,
+)
 
 
-def setup_rsmcmd_parser(name,
-                        uses_output_directory=True,
-                        allows_overwriting=False,
-                        extra_run_options=[],
-                        uses_subgroups=False):
+def setup_rsmcmd_parser(
+    name,
+    uses_output_directory=True,
+    allows_overwriting=False,
+    extra_run_options=[],
+    uses_subgroups=False,
+):
     """
     Create argument parsers for RSM command-line utilities.
 
     Since the various RSM command-line utilities (``rsmtool``, ``rsmeval``,
     ``rsmcompare``, etc.) have very similar argument parsers, refactoring that
     shared code out into this helper function makes it easier to extend
     and modify the command-line interface to all utilities at the same time.
@@ -119,111 +125,124 @@
     # a special callable to test whether configuration files exist
     # or not; this is nested because it is only used within this function
     # and should never be used externally
     def existing_configuration_file(string):
         if Path(string).exists():
             return string
         else:
-            msg = 'The configuration file %r does not exist.' % string
+            msg = f"The configuration file {string!r} does not exist."
             raise argparse.ArgumentTypeError(msg)
 
     # initialize an argument parser
     parser = argparse.ArgumentParser(prog=f"{name}")
 
     # we always want to have a version flag for the main parser
-    parser.add_argument('-V',
-                        '--version',
-                        action='version',
-                        version=VERSION_STRING,
-                        help=f"show the {name} version number and exit")
+    parser.add_argument(
+        "-V",
+        "--version",
+        action="version",
+        version=VERSION_STRING,
+        help=f"show the {name} version number and exit",
+    )
 
     # each RSM command-line utility has two subcommands
     # - generate : used to auto-generate configuration files
     # - run : used to run experiments
 
     # let's set up the sub-parsers corresponding to these subcommands
-    subparsers = parser.add_subparsers(dest='subcommand', title='subcommands')
-    parser_generate = subparsers.add_parser('generate',
-                                            help=f"automatically generate an "
-                                                 f"{name} configuration file")
-    parser_run = subparsers.add_parser('run',
-                                       help=f"run an {name} experiment")
+    subparsers = parser.add_subparsers(dest="subcommand", title="subcommands")
+    parser_generate = subparsers.add_parser(
+        "generate", help=f"automatically generate an " f"{name} configuration file"
+    )
+    parser_run = subparsers.add_parser("run", help=f"run an {name} experiment")
 
     ###################################################
     # Setting up options for the "generate" subparser #
     ###################################################
     if uses_subgroups:
         # we need to display a special help message for ``rsmxval``
         # since its config does not actually contain a sections list
         if name == "rsmxval":
-            parser_generate.add_argument('-g',
-                                         '--subgroups',
-                                         dest='subgroups',
-                                         action='store_true',
-                                         default=False,
-                                         help=f"if specified, {name} will ensure that "
-                                              f"subgroup sections are included in "
-                                              f"the various reports")
+            parser_generate.add_argument(
+                "-g",
+                "--subgroups",
+                dest="subgroups",
+                action="store_true",
+                default=False,
+                help=f"if specified, {name} will ensure that "
+                f"subgroup sections are included in "
+                f"the various reports",
+            )
         else:
-            parser_generate.add_argument('-g',
-                                         '--subgroups',
-                                         dest='subgroups',
-                                         action='store_true',
-                                         default=False,
-                                         help=f"if specified, the generated {name} "
-                                              f"configuration file will include the "
-                                              f"subgroup sections in the general "
-                                              f"sections list")
-
-    parser_generate.add_argument('-q',
-                                 '--quiet',
-                                 dest='quiet',
-                                 action='store_true',
-                                 default=False,
-                                 help="if specified, the warning about not "
-                                      "using the generated configuration "
-                                      "as-is will be suppressed.")
-
-    parser_generate.add_argument('-i',
-                                 '--interactive',
-                                 dest='interactive',
-                                 action='store_true',
-                                 default=False,
-                                 help=f"if specified, generate the {name} "
-                                      f"configuration file interactively")
+            parser_generate.add_argument(
+                "-g",
+                "--subgroups",
+                dest="subgroups",
+                action="store_true",
+                default=False,
+                help=f"if specified, the generated {name} "
+                f"configuration file will include the "
+                f"subgroup sections in the general "
+                f"sections list",
+            )
+
+    parser_generate.add_argument(
+        "-q",
+        "--quiet",
+        dest="quiet",
+        action="store_true",
+        default=False,
+        help="if specified, the warning about not "
+        "using the generated configuration "
+        "as-is will be suppressed.",
+    )
+
+    parser_generate.add_argument(
+        "-i",
+        "--interactive",
+        dest="interactive",
+        action="store_true",
+        default=False,
+        help=f"if specified, generate the {name} " f"configuration file interactively",
+    )
 
     ##############################################
     # Setting up options for the "run" subparser #
     ##############################################
 
     # since this is an RSMTool command-line utility, we will
     # always need a configuration file
-    parser_run.add_argument('config_file',
-                            type=existing_configuration_file,
-                            help=f"the {name} JSON configuration file to run")
+    parser_run.add_argument(
+        "config_file",
+        type=existing_configuration_file,
+        help=f"the {name} JSON configuration file to run",
+    )
 
     # if it uses an output directory, let's add that
     if uses_output_directory:
-        parser_run.add_argument('output_dir',
-                                nargs='?',
-                                default=os.getcwd(),
-                                help="the output directory where all the files "
-                                     "for this run will be stored")
+        parser_run.add_argument(
+            "output_dir",
+            nargs="?",
+            default=os.getcwd(),
+            help="the output directory where all the files " "for this run will be stored",
+        )
 
     # if it allows overwrting the output directory, let's add that
     if allows_overwriting:
-        parser_run.add_argument('-f',
-                                '--force',
-                                dest='force_write',
-                                action='store_true',
-                                default=False,
-                                help=f"if specified, {name} will overwrite the "
-                                     f"contents of the output file or directory "
-                                     f"even if it contains the output of a "
-                                     f"previous run ")
+        parser_run.add_argument(
+            "-f",
+            "--force",
+            dest="force_write",
+            action="store_true",
+            default=False,
+            help=f"if specified, {name} will overwrite the "
+            f"contents of the output file or directory "
+            f"even if it contains the output of a "
+            f"previous run ",
+        )
 
     # add any extra options passed in for the rub subcommand;
     for parser_option in extra_run_options:
 
         # construct the arguments and keyword arguments needed for the
         # `add_argument()` call to the parser
         argparse_option_args = []
@@ -235,27 +254,29 @@
 
         # now add any optional information
         if parser_option.shortname is not None:
             argparse_option_args.append(f"-{parser_option.shortname}")
         if parser_option.longname is not None:
             argparse_option_args.append(f"--{parser_option.longname}")
         if parser_option.action is not None:
-            argparse_option_kwargs['action'] = f"{parser_option.action}"
+            argparse_option_kwargs["action"] = f"{parser_option.action}"
         if parser_option.default is not None:
             argparse_option_kwargs["default"] = f"{parser_option.default}"
         if parser_option.required is not None:
             try:
                 assert type(parser_option.required) == bool
             except AssertionError:
-                raise TypeError(f"the 'required' field for CmdOption must be "
-                                f"boolean, you specified '{parser_option.required}'")
+                raise TypeError(
+                    f"the 'required' field for CmdOption must be "
+                    f"boolean, you specified '{parser_option.required}'"
+                )
             else:
                 argparse_option_kwargs["required"] = parser_option.required
         if parser_option.nargs is not None:
-            argparse_option_kwargs['nargs'] = f"{parser_option.nargs}"
+            argparse_option_kwargs["nargs"] = f"{parser_option.nargs}"
 
         # add this argument to the parser
         parser_run.add_argument(*argparse_option_args, **argparse_option_kwargs)
 
     return parser
 
 
@@ -335,52 +356,52 @@
         ValueError
             If the list of choices is not available for a field
             of type "choice".
         """
         # assign metadata attributes to class attributes
         self.field_name = field_name
         self.field_type = field_type
-        self.label = field_metadata['label']
-        self.choices = field_metadata.get('choices', [])
-        self.count = field_metadata.get('count', 'single')
-        self.data_type = field_metadata.get('type', 'text')
+        self.label = field_metadata["label"]
+        self.choices = field_metadata.get("choices", [])
+        self.count = field_metadata.get("count", "single")
+        self.data_type = field_metadata.get("type", "text")
 
         # instantiate the interaction-related attributes to their default values
         self.completer = None
         self.complete_style = None
         self.validator = None
 
         # now override these attributes as necessary depending on field data types
-        if self.data_type == 'boolean':
-            allow_empty = field_type == 'optional'
-            self.completer = WordCompleter(['true', 'false'])
+        if self.data_type == "boolean":
+            allow_empty = field_type == "optional"
+            self.completer = WordCompleter(["true", "false"])
             self.validator = self._make_boolean_validator(allow_empty=allow_empty)
-        elif self.data_type == 'choice':
+        elif self.data_type == "choice":
             if not self.choices:
                 raise ValueError(f"invalid list of choices for field '{field_name}'")
             else:
                 self.completer = FuzzyWordCompleter(self.choices)
                 self.validator = self._make_choice_validator(self.choices)
                 self.complete_style = CompleteStyle.MULTI_COLUMN
-        elif self.data_type == 'dir':
+        elif self.data_type == "dir":
             self.completer = self._make_directory_completer()
             self.validator = self._make_directory_validator()
-        elif self.data_type == 'file':
-            allow_empty = field_type == 'optional'
+        elif self.data_type == "file":
+            allow_empty = field_type == "optional"
             self.completer = self._make_file_completer()
             self.validator = self._make_file_validator(allow_empty=allow_empty)
-        elif self.data_type == 'format':
+        elif self.data_type == "format":
             self.completer = WordCompleter(POSSIBLE_EXTENSIONS)
             self.validator = self._make_file_format_validator()
-        elif self.data_type == 'id':
+        elif self.data_type == "id":
             self.completer = None
             self.validator = self._make_id_validator()
-        elif self.data_type == 'integer':
+        elif self.data_type == "integer":
             self.completer = None
-            allow_empty = field_type == 'optional'
+            allow_empty = field_type == "optional"
             self.validator = self._make_integer_validator(allow_empty=allow_empty)
 
     def _make_boolean_validator(self, allow_empty=False):
         """
         Create a validator for boolean fields.
 
         This private method creates a validator for a field with
@@ -400,16 +421,17 @@
             A ``Validator`` instance that ensures that the user
             input for the field is "true" / "false", or possibly
             the empty string, if ``allow_empty`` is ``True``.
         """
         correct_choices = ["true", "false"]
         if allow_empty:
             correct_choices.append("")
-        validator = Validator.from_callable(lambda answer: answer in correct_choices,
-                                            error_message="invalid answer")
+        validator = Validator.from_callable(
+            lambda answer: answer in correct_choices, error_message="invalid answer"
+        )
         return validator
 
     def _make_choice_validator(self, choices):
         """
         Create a validator for choice fields.
 
         This private method creates a validator for a field
@@ -422,16 +444,17 @@
 
         Returns
         -------
         validator : prompt_toolkit.validation.Validator
             A ``Validator`` instance that ensures that the user
             input for the field is one of the possible choices.
         """
-        validator = Validator.from_callable(lambda choice: choice in choices,
-                                            error_message="invalid choice")
+        validator = Validator.from_callable(
+            lambda choice: choice in choices, error_message="invalid choice"
+        )
         return validator
 
     def _make_directory_completer(self):
         """
         Create a completer for directory fields.
 
         This private method creates a completer for a field
@@ -454,16 +477,17 @@
 
         Returns
         -------
         validator : prompt_toolkit.validation.Validator
             A ``Validator`` instance that makes sure that only
             directory names are chosen as the final user input.
         """
-        validator = Validator.from_callable(lambda filepath: Path(filepath).is_dir(),
-                                            error_message="invalid directory")
+        validator = Validator.from_callable(
+            lambda filepath: Path(filepath).is_dir(), error_message="invalid directory"
+        )
         return validator
 
     def _make_file_completer(self):
         """
         Create a completer for file fields.
 
         This private method creates a completer for a field
@@ -475,21 +499,24 @@
             A ``Completer`` instance that suggests directory names
             and files with valid input file extensions as potential
             completions for user input. Valid input file
             extensions are "csv", "jsonlines", "sas7bdat", "tsv",
             and "xlsx". We need directory names so that
             users can look into sub-directories etc.
         """
+
         def valid_file(filename):
-            return (Path(filename).is_dir() or
-                    Path(filename).suffix.lower().lstrip('.') in ['csv',
-                                                                  'jsonlines',
-                                                                  'sas7bdat',
-                                                                  'tsv',
-                                                                  'xlsx'])
+            return Path(filename).is_dir() or Path(filename).suffix.lower().lstrip(".") in [
+                "csv",
+                "jsonlines",
+                "sas7bdat",
+                "tsv",
+                "xlsx",
+            ]
+
         return PathCompleter(expanduser=False, file_filter=valid_file)
 
     def _make_file_validator(self, allow_empty=False):
         """
         Create a validator for file fields.
 
         This private method creates a validator for a field
@@ -507,28 +534,31 @@
         validator : prompt_toolkit.validation.Validator
             A ``Validator`` instance that makes sure that only
             actually existing files with valid input file extensions
             are chosen as the final user input. Valid input file
             extensions are "csv", "jsonlines", "sas7bdat", "tsv",
             and "xlsx".
         """
+
         def is_valid(path):
-            return (Path(path).is_file() and
-                    Path(path).suffix.lower().lstrip('.') in ['csv',
-                                                              'jsonlines',
-                                                              'sas7bdat',
-                                                              'tsv',
-                                                              'xlsx'])
+            return Path(path).is_file() and Path(path).suffix.lower().lstrip(".") in [
+                "csv",
+                "jsonlines",
+                "sas7bdat",
+                "tsv",
+                "xlsx",
+            ]
 
         def is_empty(path):
-            return path == ''
+            return path == ""
 
-        validator = Validator.from_callable(lambda path: is_valid(path)
-                                            or (allow_empty and is_empty(path)),
-                                            error_message="invalid file")
+        validator = Validator.from_callable(
+            lambda path: is_valid(path) or (allow_empty and is_empty(path)),
+            error_message="invalid file",
+        )
         return validator
 
     def _make_file_format_validator(self):
         """
         Create a validator for file format fields.
 
         This private method creates a validator for a field
@@ -539,15 +569,18 @@
         validator : prompt_toolkit.validation.Validator
             A ``Validator`` instance that makes sure that only
             valid intermediate file extensions ("csv", "tsv",
             and "xlsx") and empty string are allowed as final
             user input. We want to allow empty string because
             intermediate file formats are optional to specify.
         """
-        validator = Validator.from_callable(lambda ext: ext in POSSIBLE_EXTENSIONS or ext == '', error_message="invalid format")
+        validator = Validator.from_callable(
+            lambda ext: ext in POSSIBLE_EXTENSIONS or ext == "",
+            error_message="invalid format",
+        )
         return validator
 
     def _make_id_validator(self):
         """
         Create a validator for id fields.
 
         This private method creates a validator for a field
@@ -557,16 +590,18 @@
         -------
         validator : prompt_toolkit.validation.Validator
             A ``Validator`` instance that makes sure that IDs
             specified by the user are not blank and do not
             contain spaces. We do not allow blanks since IDs
             are always required.
         """
-        validator = Validator.from_callable(lambda text: len(text) > 0 and ' ' not in text,
-                                            error_message="blanks/spaces not allowed")
+        validator = Validator.from_callable(
+            lambda text: len(text) > 0 and " " not in text,
+            error_message="blanks/spaces not allowed",
+        )
         return validator
 
     def _make_integer_validator(self, allow_empty=False):
         """
         Create a validator for integer fields.
 
         This private method creates a validator for a field
@@ -583,19 +618,21 @@
         -------
         validator : prompt_toolkit.validation.Validator
             A ``Validator`` instance that makes sure that the
             final user input is a string representation of a
             fixed-point number or integer. Blank strings may
             also be allowed if ``allow_empty`` is ``True``.
         """
-        integer_regex = r'^[0-9]+$'
+        integer_regex = r"^[0-9]+$"
         if allow_empty:
-            integer_regex += r'|^$'
-        validator = Validator.from_callable(lambda answer: re.match(integer_regex, answer),
-                                            error_message="invalid integer")
+            integer_regex += r"|^$"
+        validator = Validator.from_callable(
+            lambda answer: re.match(integer_regex, answer),
+            error_message="invalid integer",
+        )
         return validator
 
     def _get_user_input(self):
         """
         Display appropriate label and collect user input.
 
         This private method displays the appropriate prompt label
@@ -606,51 +643,57 @@
         -------
         user_input : list or str
             A string for fields that accepts a single input
             or a list of strings for fields that accept multiple
             inputs, e.g., subgroups.
         """
         # if we are dealing with a field that accepts multiple inputs
-        if self.count == 'multiple':
+        if self.count == "multiple":
 
             # instantiate a blank list to hold the multiple values
             values = []
 
             # show the name of the field as a heading but do not
             # ask for input yet
             print_formatted_text(HTML(f" <b>{self.label}</b>"))
 
             # ask the user how many of the multiple inputs they
             # intend to provide; this must be non-zero
-            num_entries = prompt("  How many do you want to specify: ",
-                                 validator=self._make_integer_validator())
+            num_entries = prompt(
+                "  How many do you want to specify: ",
+                validator=self._make_integer_validator(),
+            )
             num_entries = int(num_entries)
 
             # display secondary prompts, one for each of the inputs
             # with the appropriate completer, validator, and style
             for i in range(num_entries):
-                value = prompt(f"   Enter #{i+1}: ",
-                               completer=self.completer,
-                               validator=self.validator,
-                               complete_style=self.complete_style)
+                value = prompt(
+                    f"   Enter #{i+1}: ",
+                    completer=self.completer,
+                    validator=self.validator,
+                    complete_style=self.complete_style,
+                )
                 # save the value in the list
                 values.append(value)
 
             # this is what we will return
             user_input = values
 
         # if we are dealing with a simple single-input field
         else:
             # nothing fancy, just display the label, attach
             # the appropriate completer, validator, and style,
             # and get the user input
-            user_input = prompt(HTML(f" <b>{self.label}</b>: "),
-                                completer=self.completer,
-                                validator=self.validator,
-                                complete_style=self.complete_style)
+            user_input = prompt(
+                HTML(f" <b>{self.label}</b>: "),
+                completer=self.completer,
+                validator=self.validator,
+                complete_style=self.complete_style,
+            )
 
         return user_input
 
     def _finalize(self, user_input):
         """
         Convert given input to appropriate type.
 
@@ -663,22 +706,22 @@
             Description
 
         Returns
         -------
         final value
             The converted value.
         """
-        if (user_input == '' or user_input == []) and self.field_type == 'optional':
+        if (user_input == "" or user_input == []) and self.field_type == "optional":
             final_value = DEFAULTS.get(self.field_name)
         else:
             # boolean fields need to be converted to actual booleans
-            if self.data_type == 'boolean':
-                final_value = False if user_input == 'false' else True
+            if self.data_type == "boolean":
+                final_value = False if user_input == "false" else True
             # and integer fields to integers/None
-            elif self.data_type == 'integer':
+            elif self.data_type == "integer":
                 final_value = int(user_input)
             else:
                 final_value = user_input
 
         return final_value
 
     def get_value(self):
@@ -728,77 +771,85 @@
         Defaults to ``False``.
     use_subgroups : bool, optional
         If ``True``, include subgroup-related sections in the list of general sections
         in the configuration file.
         Defaults to ``False``.
     """
 
-    def __init__(self,
-                 context,
-                 as_string=False,
-                 suppress_warnings=False,
-                 use_subgroups=False):  # noqa
+    def __init__(
+        self, context, as_string=False, suppress_warnings=False, use_subgroups=False
+    ):  # noqa
         self.context = context
         self.use_subgroups = use_subgroups
         self.suppress_warnings = suppress_warnings
         self.as_string = as_string
         self.logger = logging.getLogger(__name__)
 
         # we need to save the first required and first optional field we will
         # insert since we will use them as sign posts to insert comments later
-        self._required_fields = CHECK_FIELDS[self.context]['required']
-        self._optional_fields = sorted(CHECK_FIELDS[self.context]['optional'])
+        self._required_fields = CHECK_FIELDS[self.context]["required"]
+        self._optional_fields = sorted(CHECK_FIELDS[self.context]["optional"])
         self._first_required_field = self._required_fields[0]
         self._first_optional_field = self._optional_fields[0]
 
-    def _convert_to_string(self,
-                           config_object,
-                           insert_url_comment=True,
-                           insert_required_comment=True,
-                           insert_optional_comment=True):
+    def _convert_to_string(
+        self,
+        config_object,
+        insert_url_comment=True,
+        insert_required_comment=True,
+        insert_optional_comment=True,
+    ):
         configuration = str(config_object)
 
         # insert the URL comment first, right above the first required field
         if insert_url_comment:
-            base_url = 'https://rsmtool.readthedocs.io/en/stable'
+            base_url = "https://rsmtool.readthedocs.io/en/stable"
             doc_slug = CONFIGURATION_DOCUMENTATION_SLUGS[self.context]
             doc_url = f"{base_url}/{doc_slug}"
-            configuration = re.sub(fr'([ ]+)("{self._first_required_field}": [^,]+,\n)',
-                                   fr'\1// Reference: {doc_url}\n\1\2',
-                                   configuration)
+            configuration = re.sub(
+                rf'([ ]+)("{self._first_required_field}": [^,]+,\n)',
+                rf"\1// Reference: {doc_url}\n\1\2",
+                configuration,
+            )
 
         # insert first comment right above the first required field
         if insert_required_comment:
-            configuration = re.sub(fr'([ ]+)("{self._first_required_field}": [^,]+,\n)',
-                                   fr'\1// REQUIRED: replace "ENTER_VALUE_HERE" with the appropriate value!\n\1\2',
-                                   configuration)
+            configuration = re.sub(
+                rf'([ ]+)("{self._first_required_field}": [^,]+,\n)',
+                rf'\1// REQUIRED: replace "ENTER_VALUE_HERE" with the appropriate value!\n\1\2',  # noqa
+                configuration,
+            )
 
         # insert second comment right above the first optional field
         if insert_optional_comment:
-            configuration = re.sub(fr'([ ]+)("{self._first_optional_field}": [^,]+,\n)',
-                                   r'\1// OPTIONAL: replace default values below based on your data.\n\1\2',
-                                   configuration)
+            configuration = re.sub(
+                rf'([ ]+)("{self._first_optional_field}": [^,]+,\n)',
+                r"\1// OPTIONAL: replace default values below based on your data.\n\1\2",
+                configuration,
+            )
 
         return configuration
 
     def _get_all_general_section_names(self):
 
-        default_general_sections_value = DEFAULTS.get('general_sections', '')
-        default_special_sections_value = DEFAULTS.get('special_sections', '')
-        default_custom_sections_value = DEFAULTS.get('custom_sections', '')
+        default_general_sections_value = DEFAULTS.get("general_sections", "")
+        default_special_sections_value = DEFAULTS.get("special_sections", "")
+        default_custom_sections_value = DEFAULTS.get("custom_sections", "")
 
         # if we are told ot use subgroups then just make up a dummy subgroup
         # value so that the subgroup-based sections will be included in the
         # section list. This value is not actually used in configuration file.
-        subgroups_value = ['GROUP'] if self.use_subgroups else DEFAULTS.get('subgroups', '')
-        return Reporter().determine_chosen_sections(default_general_sections_value,
-                                                    default_special_sections_value,
-                                                    default_custom_sections_value,
-                                                    subgroups_value,
-                                                    context=self.context)
+        subgroups_value = ["GROUP"] if self.use_subgroups else DEFAULTS.get("subgroups", "")
+        return Reporter().determine_chosen_sections(
+            default_general_sections_value,
+            default_special_sections_value,
+            default_custom_sections_value,
+            subgroups_value,
+            context=self.context,
+        )
 
     def interact(self):
         """
         Automatically generate an example configuration in interactive mode.
 
         Returns
         -------
@@ -821,60 +872,62 @@
         sys.stderr.write(" - press tab or start typing when choosing files/directories/models\n")
         sys.stderr.write(" - press enter to accept the default value for a field (underlined)\n")
         sys.stderr.write(" - press ctrl-c to cancel current entry for a field and enter again\n")
         sys.stderr.write(" - you may still need to edit the generated configuration\n")
         sys.stderr.write("\n")
 
         if not self.use_subgroups:
-            sys.stderr.write("IMPORTANT: If you have subgroups and didn't specify the '-g' "
-                             "option, exit now (ctrl-d) and re-run!\n")
+            sys.stderr.write(
+                "IMPORTANT: If you have subgroups and didn't specify the '-g' "
+                "option, exit now (ctrl-d) and re-run!\n"
+            )
             sys.stderr.write("\n")
 
         # instantiate a blank dictionary
         configdict = OrderedDict()
 
         # iterate over the required fields first, and then the (sorted) optional fields
         # keep track of which field type we are currently dealing with
-        for field_type, field_name in chain(product(['required'], self._required_fields),
-                                            product(['optional'], self._optional_fields)):
+        for field_type, field_name in chain(
+            product(["required"], self._required_fields),
+            product(["optional"], self._optional_fields),
+        ):
 
             # skip the subgroups field unless we were told to use subgroups
-            if field_name == 'subgroups' and not self.use_subgroups:
-                configdict['subgroups'] = DEFAULTS.get('subgroups')
+            if field_name == "subgroups" and not self.use_subgroups:
+                configdict["subgroups"] = DEFAULTS.get("subgroups")
                 continue
 
             # if the field is not one that is meant to be filled interactively,
             # then just use its default value; for "general_sections", expand it
             # so that it is easy for the user to remove sections
             if field_name not in INTERACTIVE_MODE_METADATA:
-                non_interactive_field_value = DEFAULTS.get(field_name, '')
-                if field_name == 'general_sections':
+                non_interactive_field_value = DEFAULTS.get(field_name, "")
+                if field_name == "general_sections":
                     non_interactive_field_value = self._get_all_general_section_names()
                 configdict[field_name] = non_interactive_field_value
             else:
                 # instantiate the interactive field first
                 try:
-                    interactive_field = InteractiveField(field_name,
-                                                         field_type,
-                                                         INTERACTIVE_MODE_METADATA[field_name])
+                    interactive_field = InteractiveField(
+                        field_name, field_type, INTERACTIVE_MODE_METADATA[field_name]
+                    )
                     configdict[field_name] = interactive_field.get_value()
                 # if the user pressed Ctrl-D, then exit out of interactive mode
                 # without generating anything and return an empty string
                 except EOFError:
                     sys.stderr.write("\n")
                     sys.stderr.write("You exited interactive mode without a configuration.")
                     sys.stderr.write("\n")
-                    return ''
+                    return ""
                 # otherwise get the field value and save it
 
         # create a Configuration instance from the dictionary we just generated
         sys.stderr.write("\n")
-        config_object = Configuration(configdict,
-                                      configdir=os.getcwd(),
-                                      context=self.context)
+        config_object = Configuration(configdict, configdir=os.getcwd(), context=self.context)
         # convert the Configuration object to a string - we are using
         # a special wrapper method since we also want to insert comments
         return self._convert_to_string(config_object, insert_required_comment=False)
 
     def generate(self):
         """
         Automatically generate an example configuration in batch mode.
@@ -886,42 +939,42 @@
             a formatted string, depending on the value of ``as_string``.
         """
         # instantiate a dictionary that remembers key insertion order
         configdict = OrderedDict()
 
         # insert the required fields first and give them a dummy value
         for required_field in self._required_fields:
-            configdict[required_field] = 'ENTER_VALUE_HERE'
+            configdict[required_field] = "ENTER_VALUE_HERE"
 
         # insert the optional fields in alphabetical order
         for optional_field in self._optional_fields:
 
             # to make it easy for users to add/remove sections, we should
             # populate the `general_sections` field with an explicit list
             # instead of the default value which is simply ``['all']``. To
             # do this, we can use the reporter class.
-            if optional_field == 'general_sections':
-                configdict['general_sections'] = self._get_all_general_section_names()
+            if optional_field == "general_sections":
+                configdict["general_sections"] = self._get_all_general_section_names()
             else:
-                configdict[optional_field] = DEFAULTS.get(optional_field, '')
+                configdict[optional_field] = DEFAULTS.get(optional_field, "")
 
         # create a Configuration object
-        config_object = Configuration(configdict,
-                                      configdir=os.getcwd(),
-                                      context=self.context)
+        config_object = Configuration(configdict, configdir=os.getcwd(), context=self.context)
 
         # if we were asked for string output, then convert this dictionary to
         # a string that will also insert some useful comments
         if self.as_string:
             configuration = self._convert_to_string(config_object)
         # otherwise we just return the dictionary underlying the Configuration object
         else:
             configuration = config_object._config
 
         # print out a warning to make it clear that it cannot be used as is
         if not self.suppress_warnings:
-            self.logger.warning("Automatically generated configuration files MUST "
-                                "be edited to add values for required fields and "
-                                "even for optional ones depending on your data.")
+            self.logger.warning(
+                "Automatically generated configuration files MUST "
+                "be edited to add values for required fields and "
+                "even for optional ones depending on your data."
+            )
 
         # return either the Configuration object or the string
         return configuration
```

### Comparing `rsmtool-9.0.1/rsmtool/utils/conversion.py` & `rsmtool-9.1.1/rsmtool/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `rsmtool-9.0.1/rsmtool/utils/cross_validation.py` & `rsmtool-9.1.1/rsmtool/utils/cross_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Various utility functions used for cross-validation.
 
 :author: Nitin Madnani (nmadnani@ets.org)
 
 :organization: ETS
 """
 import logging
-from shutil import copyfile
 from pathlib import Path
+from shutil import copyfile
 
 from pandas import concat
-from skll.config.utils import load_cv_folds
 from sklearn.model_selection import KFold, LeaveOneGroupOut
+from skll.config.utils import load_cv_folds
 
 from rsmtool.reader import DataReader
 from rsmtool.rsmtool import run_experiment
 from rsmtool.utils.logging import get_file_logger
 from rsmtool.writer import DataWriter
 
 
@@ -55,61 +55,66 @@
     modeldir = Path(output_dir) / "final-model"
 
     # get the file format specified by the user
     given_file_format = configuration["file_format"]
 
     # locate the training data file, the folds file, and feature file(s)
     located_filepaths = {}
-    located_filepaths["train"] = DataReader.locate_files(configuration.get("train_file"),
-                                                         configuration.configdir)
+    located_filepaths["train"] = DataReader.locate_files(
+        configuration.get("train_file"), configuration.configdir
+    )
     if not located_filepaths["train"]:
-        raise FileNotFoundError('The training data file was not found: '
-                                '{}'.format(repr(configuration.get("train_file"))))
+        raise FileNotFoundError(
+            f"The training data file was not found: " f"{repr(configuration.get('train_file'))}"
+        )
 
     # "features" could be a list of features so check for that
     additional_filenames = ["folds_file", "feature_subset_file"]
     if isinstance(configuration.get("features"), str):
         additional_filenames.append("features")
 
     for additional_filename in additional_filenames:
         if additional_file := configuration.get(additional_filename):
-            located_filepaths[additional_filename] = DataReader.locate_files(additional_file,
-                                                                             configuration.configdir)
+            located_filepaths[additional_filename] = DataReader.locate_files(
+                additional_file, configuration.configdir
+            )
 
     # read the training file into a dataframe making sure that the specified
     # ID column is read as a string
-    df_train = DataReader.read_from_file(located_filepaths["train"],
-                                         converters={configuration["id_column"]: str})
+    df_train = DataReader.read_from_file(
+        located_filepaths["train"], converters={configuration["id_column"]: str}
+    )
 
     # we need to sub-sample the full training data file to create a dummy
     # test file that we need to use when running RSMTool on the full
     # training dataset to get the model/feature descriptives; we use 10%
     # of the training data to create this dummy test set
-    df_sampled_test = df_train.sample(frac=0.1,
-                                      replace=False,
-                                      random_state=1234567890,
-                                      axis=0)
-    DataWriter.write_frame_to_file(df_sampled_test,
-                                   str(modeldir / "dummy_test"),
-                                   file_format=given_file_format,
-                                   index=False)
+    df_sampled_test = df_train.sample(frac=0.1, replace=False, random_state=1234567890, axis=0)
+    DataWriter.write_frame_to_file(
+        df_sampled_test,
+        str(modeldir / "dummy_test"),
+        file_format=given_file_format,
+        index=False,
+    )
 
     # read the folds file if it exists, otherwise use specified number of folds
     folds_file = located_filepaths.get("folds_file")
     if folds_file and Path(folds_file).exists():
         cv_folds = load_cv_folds(located_filepaths["folds_file"])
         folds = len(set(cv_folds.values()))
         logger.info(f"Using {folds} folds specified in {located_filepaths['folds_file']}")
         logo = LeaveOneGroupOut()
         id_column = configuration.get("id_column")
         try:
             train_ids = df_train[id_column]
         except KeyError:
-            logger.error("Column f{id_column} not found! Check the value of "
-                         "'id_column' in the configuration file.")
+            logger.error(
+                "Column f{id_column} not found! Check the value of "
+                "'id_column' in the configuration file."
+            )
         else:
             fold_groups = [cv_folds[train_id] for train_id in train_ids.values]
             fold_generator = logo.split(range(len(df_train)), y=None, groups=fold_groups)
     else:
         # if we are in this code path but the configuration did
         # specify "folds_file", then we must not have found the file
         # so raise a warning to that effect
@@ -118,33 +123,36 @@
         folds = configuration.get("folds")
         logger.info(f"Generating {folds} folds after shuffling")
         kfold = KFold(n_splits=folds, random_state=1234567890, shuffle=True)
         fold_generator = kfold.split(range(len(df_train)))
 
     # iterate over each of the folds and generate an rsmtool configuration file
     # which is then saved to disk in a directory specific to each fold
-    for fold_num, (fold_train_indices,
-                   fold_test_indices) in enumerate(fold_generator, start=1):
+    for fold_num, (fold_train_indices, fold_test_indices) in enumerate(fold_generator, start=1):
 
         # get the train and test files for this fold and
         # write them out to disk
         df_fold_train = df_train.loc[fold_train_indices]
         df_fold_test = df_train.loc[fold_test_indices]
         this_fold_dir = Path(foldsdir) / f"{fold_num:02}"
         this_fold_dir.mkdir()
         fold_train_file_prefix = str(this_fold_dir / "train")
-        DataWriter.write_frame_to_file(df_fold_train,
-                                       fold_train_file_prefix,
-                                       file_format=given_file_format,
-                                       index=False)
+        DataWriter.write_frame_to_file(
+            df_fold_train,
+            fold_train_file_prefix,
+            file_format=given_file_format,
+            index=False,
+        )
         fold_test_file_prefix = str(this_fold_dir / "test")
-        DataWriter.write_frame_to_file(df_fold_test,
-                                       fold_test_file_prefix,
-                                       file_format=given_file_format,
-                                       index=False)
+        DataWriter.write_frame_to_file(
+            df_fold_test,
+            fold_test_file_prefix,
+            file_format=given_file_format,
+            index=False,
+        )
 
         # update the value of "train_file" and add "test_file"
         # & "test_label_column" in the configuration file
         fold_configuration = configuration.copy(deep=True)
         fold_configuration["train_file"] = f"{fold_train_file_prefix}.{given_file_format}"
         fold_configuration["test_file"] = f"{fold_test_file_prefix}.{given_file_format}"
         fold_configuration["test_label_column"] = configuration["train_label_column"]
@@ -220,15 +228,17 @@
         Data frame containing the combined predictions for all folds.
     """
     # initialize empty list to hold each prediction data frame
     prediction_dfs = []
 
     # iterate over each fold in the given directory & read and save predictions
     for prediction_file in Path(foldsdir).glob(f"**/*pred_processed*.{file_format}"):
-        df_fold_predictions = DataReader.read_from_file(prediction_file, converters={'spkitemid': str})
+        df_fold_predictions = DataReader.read_from_file(
+            prediction_file, converters={"spkitemid": str}
+        )
         prediction_dfs.append(df_fold_predictions)
 
     # concatenate all of the predictions into a single frame using
     # "spkitemid" column which must exist since this is the output of RSMTool
     df_all_predictions = concat(prediction_dfs, keys="spkitemid").reset_index(drop=True)
 
     return df_all_predictions
```

### Comparing `rsmtool-9.0.1/rsmtool/utils/files.py` & `rsmtool-9.1.1/rsmtool/utils/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,30 +38,32 @@
 
     Note
     ----
     This code was adapted from:
     https://web.archive.org/web/20150520154859/http://www.lifl.fr/~riquetd/parse-a-json-file-with-comments.html
     """
     # Regular expression to identify comments
-    comment_re = re.compile(r'(^)?[^\S\n]*(?:/\*(.*?)\*/[^\S\n]*|(?<!https:)(?<!http:)//[^\n]*)($)?',
-                            re.DOTALL | re.MULTILINE)
+    comment_re = re.compile(
+        r"(^)?[^\S\n]*(?:/\*(.*?)\*/[^\S\n]*|(?<!https:)(?<!http:)//[^\n]*)($)?",
+        re.DOTALL | re.MULTILINE,
+    )
 
     # if we passed in a string, convert it to a Path
     if isinstance(pathlike, str):
         pathlike = Path(pathlike)
 
-    with open(pathlike, 'r') as file_buff:
-        content = ''.join(file_buff.readlines())
+    with open(pathlike, "r") as file_buff:
+        content = "".join(file_buff.readlines())
 
         # Looking for comments
         match = comment_re.search(content)
         while match:
 
             # single line comment
-            content = content[:match.start()] + content[match.end():]
+            content = content[: match.start()] + content[match.end() :]  # noqa
             match = comment_re.search(content)
 
         # Return JSON object
         config = json.loads(content)
         return config
 
 
@@ -78,15 +80,15 @@
 
     Returns
     -------
     ans : bool
         ``True`` if directory contains files with given extension,
         else ``False``.
     """
-    files_with_extension = glob(join(directory, '*.{}'.format(ext)))
+    files_with_extension = glob(join(directory, f"*.{ext}"))
     return len(files_with_extension) > 0
 
 
 def get_output_directory_extension(directory, experiment_id):
     """
     Check output directory to determine what file extensions exist.
 
@@ -113,23 +115,24 @@
 
     Raises
     ------
     ValueError
         If any files in the directory have extensions
         other than "csv", "tsv", or "xlsx".
     """
-    extension = 'csv'
-    extensions_identified = {ext for ext in POSSIBLE_EXTENSIONS
-                             if has_files_with_extension(directory, ext)}
+    extension = "csv"
+    extensions_identified = {
+        ext for ext in POSSIBLE_EXTENSIONS if has_files_with_extension(directory, ext)
+    }
 
     if len(extensions_identified) > 1:
-        raise ValueError('Some of the files in the experiment output directory (`{}`) '
-                         'for `{}` have different extensions. All files in this directory '
-                         'must have the same extension. The following extensions were '
-                         'identified : {}'.format(directory,
-                                                  experiment_id,
-                                                  ', '.join(extensions_identified)))
+        raise ValueError(
+            f"Some of the files in the experiment output directory (`{directory}`) "
+            f"for `{experiment_id}` have different extensions. All files in this "
+            f"directory must have the same extension. The following extensions "
+            f"were identified : {', '.join(extensions_identified)}"
+        )
 
     elif len(extensions_identified) == 1:
         extension = list(extensions_identified)[0]
 
     return extension
```

### Comparing `rsmtool-9.0.1/rsmtool/utils/logging.py` & `rsmtool-9.1.1/rsmtool/utils/logging.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     Returns
     -------
     logger
         A logging.Logger object attached to a file handler.
     """
     logger = logging.getLogger(logger_name)
     logger.propagate = False
-    formatter = logging.Formatter('%(message)s')
+    formatter = logging.Formatter("%(message)s")
     file_handler = logging.FileHandler(log_file_path, mode="w")
     file_handler.setFormatter(formatter)
     file_handler.setLevel(logging.INFO)
     logger.addHandler(file_handler)
     logger.setLevel(logging.INFO)
     return logger
 
@@ -113,14 +113,15 @@
     Adapted from: https://stackoverflow.com/a/58936697
 
     Parameters
     ----------
     tqdm_object : tqdm progress bar
         The given tqdm progress bar into which joblib should report
     """
+
     class TqdmBatchCompletionCallback(joblib.parallel.BatchCompletionCallBack):
         def __call__(self, *args, **kwargs):
             tqdm_object.update(n=self.batch_size)
             return super().__call__(*args, **kwargs)
 
     old_batch_callback = joblib.parallel.BatchCompletionCallBack
     joblib.parallel.BatchCompletionCallBack = TqdmBatchCompletionCallback
```

### Comparing `rsmtool-9.0.1/rsmtool/utils/metrics.py` & `rsmtool-9.1.1/rsmtool/utils/metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,26 +51,30 @@
         model.probability = True
         probability_distributions = model.predict(featureset, class_labels=False)
         # check to make sure that the number of labels in the probability
         # distributions matches the number of score points we have
         num_score_points_specified = max_score - min_score + 1
         num_score_points_in_learner = probability_distributions.shape[1]
         if num_score_points_specified != num_score_points_in_learner:
-            raise ValueError('The specified number of score points ({}) '
-                             'does not match that from the the learner '
-                             '({}).'.format(num_score_points_specified,
-                                            num_score_points_in_learner))
+            raise ValueError(
+                f"The specified number of score points ({num_score_points_specified}) "
+                f"does not match that from the learner ({num_score_points_in_learner})."
+            )
         expected_scores = probability_distributions.dot(range(min_score, max_score + 1))
     else:
-        if model.model_type.__name__ == 'SVC':
-            raise ValueError("Expected scores cannot be computed since the SVC model was "
-                             "not originally trained to predict probabilities.")
+        if model.model_type.__name__ == "SVC":
+            raise ValueError(
+                "Expected scores cannot be computed since the SVC model was "
+                "not originally trained to predict probabilities."
+            )
         else:
-            raise ValueError("Expected scores cannot be computed since {} is not a "
-                             "probabilistic classifier.".format(model.model_type.__name__))
+            raise ValueError(
+                f"Expected scores cannot be computed since "
+                f"{model.model_type.__name__} is not a probabilistic classifier."
+            )
 
     return expected_scores
 
 
 def covariance_to_correlation(m):
     """
     Implement the R ``cov2cor`` function in Python.
@@ -89,15 +93,15 @@
     ------
     ValueError
         If the input matrix is not square.
     """
     # make sure the matrix is square
     numrows, numcols = m.shape
     if not numrows == numcols:
-        raise ValueError('Input matrix must be square')
+        raise ValueError("Input matrix must be square")
 
     Is = np.sqrt(1 / np.diag(m))
     retval = Is * m * np.repeat(Is, numrows).reshape(numrows, numrows)
     np.fill_diagonal(retval, 1.0)
     return retval
 
 
@@ -141,19 +145,21 @@
         # otherwise, use the inverse; if a linear algebra error
         # occurs, then we just set the matrix to empty
         try:
             assert np.linalg.det(df_cov) > np.finfo(np.float32).eps
             icvx = np.linalg.inv(df_cov)
         except AssertionError:
             icvx = np.linalg.pinv(df_cov)
-            warnings.warn('When computing partial correlations '
-                          'the inverse of the variance-covariance matrix '
-                          'was calculated using the Moore-Penrose generalized '
-                          'matrix inversion, due to its determinant being at '
-                          'or very close to zero.')
+            warnings.warn(
+                "When computing partial correlations "
+                "the inverse of the variance-covariance matrix "
+                "was calculated using the Moore-Penrose generalized "
+                "matrix inversion, due to its determinant being at "
+                "or very close to zero."
+            )
         except np.linalg.LinAlgError:
             icvx = empty_array
 
     pcor = -1 * covariance_to_correlation(icvx)
     np.fill_diagonal(pcor, 1.0)
     df_pcor = pd.DataFrame(pcor, columns=columns, index=columns)
     return df_pcor
@@ -178,27 +184,28 @@
     agreement_value : float
         The percentage agreement between the two scores.
     """
     # make sure the two sets of scores
     # are for the same number of items
     assert len(score1) == len(score2)
 
-    num_agreements = sum([int(abs(s1 - s2) <= tolerance)
-                          for s1, s2 in zip(score1, score2)])
+    num_agreements = sum([int(abs(s1 - s2) <= tolerance) for s1, s2 in zip(score1, score2)])
 
     agreement_value = (float(num_agreements) / len(score1)) * 100
     return agreement_value
 
 
-def standardized_mean_difference(y_true_observed,
-                                 y_pred,
-                                 population_y_true_observed_sd=None,
-                                 population_y_pred_sd=None,
-                                 method='unpooled',
-                                 ddof=1):
+def standardized_mean_difference(
+    y_true_observed,
+    y_pred,
+    population_y_true_observed_sd=None,
+    population_y_pred_sd=None,
+    method="unpooled",
+    ddof=1,
+):
     """
     Compute the standardized mean difference between system and human scores.
 
     The numerator is calculated as mean(y_pred) - mean(y_true_observed)
     for all of the available methods.
 
     Parameters
@@ -260,47 +267,53 @@
       et al. (2012).
     - The metric is only applicable when both sets of scores are on
       the same scale.
     """
     numerator = np.mean(y_pred) - np.mean(y_true_observed)
 
     method = method.lower()
-    if method == 'unpooled':
+    if method == "unpooled":
         denominator = np.std(y_true_observed, ddof=ddof)
-    elif method == 'pooled':
-        denominator = np.sqrt((np.std(y_true_observed, ddof=ddof)**2 +
-                               np.std(y_pred, ddof=ddof)**2) / 2)
-    elif method == 'johnson':
+    elif method == "pooled":
+        denominator = np.sqrt(
+            (np.std(y_true_observed, ddof=ddof) ** 2 + np.std(y_pred, ddof=ddof) ** 2) / 2
+        )
+    elif method == "johnson":
         if population_y_true_observed_sd is None:
-            raise ValueError("If `method='johnson'`, then `population_y_true_observed_sd` "
-                             "must be provided.")
+            raise ValueError(
+                "If `method='johnson'`, then `population_y_true_observed_sd` " "must be provided."
+            )
         denominator = population_y_true_observed_sd
-    elif method == 'williamson':
+    elif method == "williamson":
         if population_y_true_observed_sd is None or population_y_pred_sd is None:
-            raise ValueError("If `method='williamson'`, both `population_y_true_observed_sd` "
-                             "and `population_y_pred_sd` must be provided.")
-        denominator = np.sqrt((population_y_true_observed_sd**2 +
-                               population_y_pred_sd**2) / 2)
+            raise ValueError(
+                "If `method='williamson'`, both `population_y_true_observed_sd` "
+                "and `population_y_pred_sd` must be provided."
+            )
+        denominator = np.sqrt((population_y_true_observed_sd**2 + population_y_pred_sd**2) / 2)
     else:
         possible_methods = {"'unpooled'", "'pooled'", "'johnson'", "'williamson'"}
-        raise ValueError("The available methods are {{{}}}; you selected {}."
-                         "".format(', '.join(possible_methods), method))
+        raise ValueError(
+            f"The available methods are {{{', '.join(possible_methods)}}}; you selected {method}."
+        )
 
     # if the denominator is zero, then return NaN as the SMD
     smd = np.nan if denominator == 0 else numerator / denominator
     return smd
 
 
-def difference_of_standardized_means(y_true_observed,
-                                     y_pred,
-                                     population_y_true_observed_mn=None,
-                                     population_y_pred_mn=None,
-                                     population_y_true_observed_sd=None,
-                                     population_y_pred_sd=None,
-                                     ddof=1):
+def difference_of_standardized_means(
+    y_true_observed,
+    y_pred,
+    population_y_true_observed_mn=None,
+    population_y_pred_mn=None,
+    population_y_true_observed_sd=None,
+    population_y_pred_sd=None,
+    ddof=1,
+):
     """
     Calculate the difference between standardized means.
 
     First, standardize both observed and predicted scores to z-scores using
     mean and standard deviation for the whole population. Then
     calculate differences between standardized means for each subgroup.
 
@@ -355,66 +368,75 @@
         If only one of ``population_y_pred_mn`` and ``population_y_pred_sd``
         is not ``None``.
     """
     assert len(y_true_observed) == len(y_pred)
 
     # all of this is just to make sure users aren't passing the population
     # standard deviation and not population mean for either true or predicted
-    y_true_observed_population_params = [population_y_true_observed_mn,
-                                         population_y_true_observed_sd]
-    y_pred_population_params = [population_y_pred_mn,
-                                population_y_pred_sd]
-
-    if len([param for param in y_true_observed_population_params
-            if param is None]) == 1:
-        raise ValueError('You must pass both `population_y_true_observed_mn` and '
-                         '`population_y_true_observed_sd` or neither.')
-
-    if len([param for param in y_pred_population_params
-            if param is None]) == 1:
-        raise ValueError('You must pass both `population_y_pred_mn` and '
-                         '`population_y_pred_sd` or neither.')
-
-    warning_msg = ('You did not pass population mean and std. for `{}`; '
-                   'thus, the calculated z-scores will be zero.')
+    y_true_observed_population_params = [
+        population_y_true_observed_mn,
+        population_y_true_observed_sd,
+    ]
+    y_pred_population_params = [population_y_pred_mn, population_y_pred_sd]
+
+    if len([param for param in y_true_observed_population_params if param is None]) == 1:
+        raise ValueError(
+            "You must pass both `population_y_true_observed_mn` and "
+            "`population_y_true_observed_sd` or neither."
+        )
+
+    if len([param for param in y_pred_population_params if param is None]) == 1:
+        raise ValueError(
+            "You must pass both `population_y_pred_mn` and " "`population_y_pred_sd` or neither."
+        )
+
+    warning_msg = (
+        "You did not pass population mean and std. for `{}`; "
+        "thus, the calculated z-scores will be zero."
+    )
 
     # if the population means and standard deviations were not provided, calculate from the data
     # We only check for mean since the function requires
     # both of these to be set or both to be None
     if population_y_true_observed_mn is None:
 
-        warnings.warn(warning_msg.format('y_true_observed'))
-        (population_y_true_observed_sd,
-         population_y_true_observed_mn) = (np.std(y_true_observed, ddof=ddof),
-                                           np.mean(y_true_observed))
+        warnings.warn(warning_msg.format("y_true_observed"))
+        (population_y_true_observed_sd, population_y_true_observed_mn) = (
+            np.std(y_true_observed, ddof=ddof),
+            np.mean(y_true_observed),
+        )
 
     if population_y_pred_mn is None:
 
-        warnings.warn(warning_msg.format('y_pred'))
-        (population_y_pred_sd,
-         population_y_pred_mn) = (np.std(y_pred, ddof=ddof),
-                                  np.mean(y_pred))
+        warnings.warn(warning_msg.format("y_pred"))
+        (population_y_pred_sd, population_y_pred_mn) = (
+            np.std(y_pred, ddof=ddof),
+            np.mean(y_pred),
+        )
 
     # if any of the standard deviations equal zero
     # raise a warning and return None.
     # We use np.isclose since sometimes sd for float
     # values is a value very close to 0.
     # We use the same tolerance as used for identifying
     # features with zero standard deviation
-    if (np.isclose(population_y_pred_sd, 0, atol=1e-07) or
-            np.isclose(population_y_true_observed_sd, 0, atol=1e-07)):
-        warnings.warn("Population standard deviations for the computation of "
-                      "DSM is zero. No value will be computed.")
+    if np.isclose(population_y_pred_sd, 0, atol=1e-07) or np.isclose(
+        population_y_true_observed_sd, 0, atol=1e-07
+    ):
+        warnings.warn(
+            "Population standard deviations for the computation of "
+            "DSM is zero. No value will be computed."
+        )
         return None
 
     # calculate the z-scores for observed and predicted
-    y_true_observed_subgroup_z = ((y_true_observed - population_y_true_observed_mn) /
-                                  population_y_true_observed_sd)
-    y_pred_subgroup_z = ((y_pred - population_y_pred_mn) /
-                         population_y_pred_sd)
+    y_true_observed_subgroup_z = (
+        y_true_observed - population_y_true_observed_mn
+    ) / population_y_true_observed_sd
+    y_pred_subgroup_z = (y_pred - population_y_pred_mn) / population_y_pred_sd
 
     # calculate the DSM, given the z-scores for observed and predicted
     difference_of_std_means = np.mean(y_pred_subgroup_z - y_true_observed_subgroup_z)
 
     return difference_of_std_means
 
 
@@ -428,15 +450,15 @@
     for the full derivation. The discrete case is simply treated as a
     special case of the continuous one.
 
     The formula is as follows:
 
     :math:`QWK=\\displaystyle\\frac{2*Cov(M,H)}{Var(H)+Var(M)+(\\bar{M}-\\bar{H})^2}`, where
 
-        - :math:`Cov` - covariance with normalization by :math:`N` (the total number of observations given)
+        - :math:`Cov` - covariance with normalization by :math:`N` (total number of observations)
         - :math:`H` - the human score
         - :math:`M` - the system score
         - :math:`\\bar{H}` - mean of :math:`H`
         - :math:`\\bar{M}` - mean of :math:`M`
         - :math:`Var(X)` - variance of X
 
     Parameters
@@ -460,16 +482,17 @@
     Raises
     ------
     AssertionError
         If the number of elements in ``y_true_observed`` is not equal
         to the number of elements in ``y_pred``.
     """
     assert len(y_true_observed) == len(y_pred)
-    y_true_observed_var, y_true_observed_avg = (np.var(y_true_observed, ddof=ddof),
-                                                np.mean(y_true_observed))
-    y_pred_var, y_pred_avg = (np.var(y_pred, ddof=ddof),
-                              np.mean(y_pred))
+    y_true_observed_var, y_true_observed_avg = (
+        np.var(y_true_observed, ddof=ddof),
+        np.mean(y_true_observed),
+    )
+    y_pred_var, y_pred_avg = (np.var(y_pred, ddof=ddof), np.mean(y_pred))
 
     numerator = 2 * np.cov(y_true_observed, y_pred, ddof=ddof)[0][1]
-    denominator = y_true_observed_var + y_pred_var + (y_true_observed_avg - y_pred_avg)**2
+    denominator = y_true_observed_var + y_pred_var + (y_true_observed_avg - y_pred_avg) ** 2
     kappa = numerator / denominator
     return kappa
```

### Comparing `rsmtool-9.0.1/rsmtool/utils/models.py` & `rsmtool-9.1.1/rsmtool/utils/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,49 @@
+"""
+Utility functions for SKLL and built-in models.
+
+:author: Jeremy Biggs (jbiggs@ets.org)
+:author: Anastassia Loukina (aloukina@ets.org)
+:author: Nitin Madnani (nmadnani@ets.org)
+
+:organization: ETS
+"""
+
 from importlib import import_module
 from inspect import getmembers, isclass
 
-_skll_module = import_module('skll.learner')
+_skll_module = import_module("skll.learner")
 
-BUILTIN_MODELS = ['LinearRegression',
-                  'EqualWeightsLR',
-                  'ScoreWeightedLR',
-                  'RebalancedLR',
-                  'NNLR',
-                  'NNLRIterative',
-                  'LassoFixedLambdaThenNNLR',
-                  'LassoFixedLambdaThenLR',
-                  'PositiveLassoCVThenLR',
-                  'LassoFixedLambda',
-                  'PositiveLassoCV']
+BUILTIN_MODELS = [
+    "LinearRegression",
+    "EqualWeightsLR",
+    "ScoreWeightedLR",
+    "RebalancedLR",
+    "NNLR",
+    "NNLRIterative",
+    "LassoFixedLambdaThenNNLR",
+    "LassoFixedLambdaThenLR",
+    "PositiveLassoCVThenLR",
+    "LassoFixedLambda",
+    "PositiveLassoCV",
+]
 
 # compute all the classes from sklearn imported into SKLL that have
 # an `_estimator_type` attribute - this should give us a list of
 # all the SKLL learners that we can support but we need to exclude
 # `GridSearchCV` and `Pipeline` which we know are false positives
-VALID_SKLL_MODELS = [name for name, member in getmembers(_skll_module)
-                     if (isclass(member) and
-                         hasattr(member, '_estimator_type') and
-                         name not in ['GridSearchCV', 'Pipeline'])]
+VALID_SKLL_MODELS = [
+    name
+    for name, member in getmembers(_skll_module)
+    if (
+        isclass(member)
+        and hasattr(member, "_estimator_type")
+        and name not in ["GridSearchCV", "Pipeline"]
+    )
+]
 
 
 def is_skll_model(model_name):
     """
     Check whether the given model is a valid learner name in SKLL.
 
     Note that the "LinearRegression" model is also available in
@@ -39,15 +56,15 @@
 
     Returns
     -------
     valid: bool
         ``True`` if the given model name is a valid SKLL learner,
         ``False`` otherwise.
     """
-    return hasattr(_skll_module, model_name) and model_name != 'LinearRegression'
+    return hasattr(_skll_module, model_name) and model_name != "LinearRegression"
 
 
 def is_built_in_model(model_name):
     """
     Check whether the given model is a valid built-in model.
 
     Parameters
```

### Comparing `rsmtool-9.0.1/rsmtool/utils/notebook.py` & `rsmtool-9.1.1/rsmtool/utils/notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from os.path import exists, isabs, relpath
 from pathlib import Path
 from string import Template
 from textwrap import wrap
 
 from IPython.display import HTML, display
 
-HTML_STRING = ("""<li><b>{}</b>: <a href="{}" download>{}</a></li>""")
+HTML_STRING = """<li><b>{}</b>: <a href="{}" download>{}</a></li>"""
 
 
 def float_format_func(num, prec=3):
     """
     Format given float to the specified precision as a string.
 
     Parameters:
@@ -32,15 +32,15 @@
         Defaults to 3.
 
     Returns:
     -------
     ans : str
         The formatted string representing the given number.
     """
-    formatter_string = Template('{:.${prec}f}').substitute(prec=prec)
+    formatter_string = Template("{:.${prec}f}").substitute(prec=prec)
     ans = formatter_string.format(num)
     return ans
 
 
 def int_or_float_format_func(num, prec=3):
     """
     Identify whether the number is float or integer.
@@ -58,26 +58,21 @@
 
     Returns:
     -------
     ans : str
         The formatted string representing the given number.
     """
     if float.is_integer(num):
-        ans = '{}'.format(int(num))
+        ans = f"{int(num)}"
     else:
         ans = float_format_func(num, prec=prec)
     return ans
 
 
-def custom_highlighter(num,
-                       low=0,
-                       high=1,
-                       prec=3,
-                       absolute=False,
-                       span_class='bold'):
+def custom_highlighter(num, low=0, high=1, prec=3, absolute=False, span_class="bold"):
     """
     Convert float to an HTML <span> element with given class.
 
     The conversion only happens if the given float is below ``low``
     or above ``high``. If it does not meet those constraints, then
     a plain string is returned with specified number of decimal places.
 
@@ -103,16 +98,19 @@
     Returns:
     --------
     ans : str
         The plain or HTML string representing the given number.
     """
     abs_num = abs(num) if absolute else num
     val = float_format_func(num, prec=prec)
-    ans = ('<span class="highlight_{}">{}</span>'.format(span_class, val)
-           if abs_num < low or abs_num > high else val)
+    ans = (
+        f'<span class="highlight_{span_class}">{val}</span>'
+        if abs_num < low or abs_num > high
+        else val
+    )
     return ans
 
 
 def bold_highlighter(num, low=0, high=1, prec=3, absolute=False):
     """
     Instantiate a ``custom_highlighter()`` with "bold" as default class.
 
@@ -134,15 +132,15 @@
         Defaults to ``False``.
 
     Returns:
     --------
     ans : str
         The formatted highlighter with bold class as default.
     """
-    ans = custom_highlighter(num, low, high, prec, absolute, 'bold')
+    ans = custom_highlighter(num, low, high, prec, absolute, "bold")
     return ans
 
 
 def color_highlighter(num, low=0, high=1, prec=3, absolute=False):
     """
     Instantiate a ``custom_highlighter()`` with "color" as the default class.
 
@@ -164,15 +162,15 @@
         Defaults to ``False``.
 
     Returns:
     --------
     ans : str
         The formatted highlighter with color class as default.
     """
-    ans = custom_highlighter(num, low, high, prec, absolute, 'color')
+    ans = custom_highlighter(num, low, high, prec, absolute, "color")
     return ans
 
 
 def compute_subgroup_plot_params(group_names, num_plots):
     """
     Compute subgroup plot and figure parameters.
 
@@ -195,15 +193,15 @@
     num_rows : int
         The number of rows for the plots.
     num_columns : int
         The number of columns for the plots.
     wrapped_group_names : list of str
         A list of group names for plots.
     """
-    wrapped_group_names = ['\n'.join(wrap(str(gn), 20)) for gn in group_names]
+    wrapped_group_names = ["\n".join(wrap(str(gn), 20)) for gn in group_names]
     plot_height = 4 if wrapped_group_names == group_names else 6
     num_groups = len(group_names)
     if num_groups <= 6:
         num_columns = 2
         num_rows = ceil(num_plots / num_columns)
         figure_width = num_columns * num_groups
         figure_height = plot_height * num_rows
@@ -245,15 +243,15 @@
         The HTML string generated for the image.
 
     Raises
     ------
     FileNotFoundError
         If the image file cannot be located.
     """
-    error_message = 'The file `{}` could not be located.'
+    error_message = "The file `{}` could not be located."
     if not exists(path_to_image):
         raise FileNotFoundError(error_message.format(path_to_image))
 
     # check if the path is relative or absolute
     if isabs(path_to_image):
         rel_image_path = relpath(path_to_image)
     else:
@@ -280,25 +278,25 @@
     }
     </style>
     """
 
     # on click, open larger image in new window
     script = """
     <script>
-    function getPicture(picpath) {{
+    function getPicture(picpath) {
         window.open(picpath, 'Image', resizable=1);
-    }};
-    </script>""".format(image_id)
+    };
+    </script>"""
 
     # generate image tags
-    image = ("""<img id='{}' src='{}' onclick='getPicture("{}")' """
-             """title="Click to enlarge">"""
-             """</img>""").format(image_id,
-                                  rel_image_path,
-                                  rel_thumbnail_path)
+    image = (
+        f"""<img id='{image_id}' src='{rel_image_path}' """
+        f"""onclick='getPicture("{rel_thumbnail_path}")' """
+        f"""title="Click to enlarge"></img>"""
+    )
 
     # create the image HTML
     image += style
     image += script
     return image
 
 
@@ -324,17 +322,15 @@
         Defaults to ``None``.
 
     Displays
     --------
     display : IPython.core.display.HTML
         The HTML for the thumbnail image.
     """
-    display(HTML(get_thumbnail_as_html(path_to_image,
-                                       image_id,
-                                       path_to_thumbnail)))
+    display(HTML(get_thumbnail_as_html(path_to_image, image_id, path_to_thumbnail)))
 
 
 def get_files_as_html(output_dir, experiment_id, file_format, replace_dict={}):
     """
     Generate an HTML list for each output file in given directory.
 
     Optionally pass a replacement dictionary to use more descriptive
@@ -355,33 +351,31 @@
     Returns
     ------
     html_string : str
         HTML string with file descriptions and links.
     """
     output_dir = Path(output_dir)
     parent_dir = output_dir.parent
-    files = output_dir.glob('*.{}'.format(file_format))
-    html_string = ''
+    files = output_dir.glob(f"*.{file_format}")
+    html_string = ""
     for file in sorted(files):
         relative_file = ".." / file.relative_to(parent_dir)
-        relative_name = relative_file.stem.replace('{}_'.format(experiment_id), '')
+        relative_name = relative_file.stem.replace(f"{experiment_id}_", "")
 
         # check if relative name is in the replacement dictionary and,
         # if it is, use the more descriptive name in the replacement
         # dictionary. Otherwise, normalize the file name and use that
         # as the description instead.
         if relative_name in replace_dict:
             descriptive_name = replace_dict[relative_name]
         else:
-            descriptive_name_components = relative_name.split('_')
-            descriptive_name = ' '.join(descriptive_name_components).title()
+            descriptive_name_components = relative_name.split("_")
+            descriptive_name = " ".join(descriptive_name_components).title()
 
-        html_string += HTML_STRING.format(descriptive_name,
-                                          relative_file,
-                                          file_format)
+        html_string += HTML_STRING.format(descriptive_name, relative_file, file_format)
 
     return """<ul><html>""" + html_string + """</ul></html>"""
 
 
 def show_files(output_dir, experiment_id, file_format, replace_dict={}):
     """
     Show files in a given directory as an HTML list in a Jupyter notebook.
@@ -399,12 +393,9 @@
         Defaults to ``{}``.
 
     Displays
     --------
     display : IPython.core.display.HTML
         The HTML file descriptions and links.
     """
-    html_string = get_files_as_html(output_dir,
-                                    experiment_id,
-                                    file_format,
-                                    replace_dict)
+    html_string = get_files_as_html(output_dir, experiment_id, file_format, replace_dict)
     display(HTML(html_string))
```

### Comparing `rsmtool-9.0.1/rsmtool/utils/prmse.py` & `rsmtool-9.1.1/rsmtool/utils/prmse.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,20 @@
     # we will only be using responses with more
     # than one score
     multiple_mask = n_scores > 1
 
     # show a warning and return None
     # if we don't have valid human scores
     if multiple_mask.sum() == 0:
-        warnings.warn("True score evaluations cannot be "
-                      "computed because none of the responses in the "
-                      "evaluation set has valid "
-                      "system scores and 2 human scores.")
+        warnings.warn(
+            "True score evaluations cannot be "
+            "computed because none of the responses in the "
+            "evaluation set has valid "
+            "system scores and 2 human scores."
+        )
         return None
 
     else:
         # only select the responses with multiple scores
         multiple_scores = human_scores[multiple_mask]
 
         n_scores = n_scores[multiple_mask]
@@ -82,16 +84,15 @@
         # of response variances
 
         variance_of_errors = np.average(response_variances, weights=n_scores - 1)
 
         return variance_of_errors
 
 
-def true_score_variance(human_scores,
-                        variance_errors_human=None):
+def true_score_variance(human_scores, variance_errors_human=None):
     """
     Compute variance of true scores for multiple raters.
 
     Parameters
     ----------
     human_scores : array-like of shape (n_samples, n_ratings)
         Human ratings for each response.
@@ -131,15 +132,15 @@
         # let N be total number of responses
         N = len(human_scores)
 
         # let M be total number of human ratings
         M = n_scores.sum()
 
         # compute squared deviations
-        squared_devs = (mean_scores - mean_human_score)**2
+        squared_devs = (mean_scores - mean_human_score) ** 2
 
         # adjust them by the number of human scores available
         # for each responses: deviations with higher number of
         # human scores are assigned a greater weight
         adjusted_squared_devs = n_scores * squared_devs
 
         # compute sum of squares
@@ -154,17 +155,15 @@
 
         # finally compute variance of true scores
         variance_true_scores = numerator / denominator
 
         return variance_true_scores
 
 
-def mse_true(system,
-             human_scores,
-             variance_errors_human=None):
+def mse_true(system, human_scores, variance_errors_human=None):
     """
     Compute mean squared error (MSE) when predicting true score from system score.
 
     Parameters
     ----------
     system : array-like of shape (n_samples,)
         System scores for each response.
@@ -196,24 +195,22 @@
 
         # get total number of scores for each response
         n_scores = get_n_human_scores(human_scores)
         mean_scores = np.nanmean(human_scores, axis=1)
 
         N = len(system)
 
-        se = ((mean_scores - system)**2) * n_scores
+        se = ((mean_scores - system) ** 2) * n_scores
 
         # Compute mean squared error when predicting true score
         mse = (se.sum() - N * variance_errors_human) / n_scores.sum()
     return mse
 
 
-def prmse_true(system,
-               human_scores,
-               variance_errors_human=None):
+def prmse_true(system, human_scores, variance_errors_human=None):
     """
     Compute PRMSE when predicting true score from system scores.
 
     PRMSE = Proportional Reduction in Mean Squared Error.
     The formula to compute PRMSE implemented in RSMTool
     was derived at ETS by Matthew S. Johnson. See
     `Loukina et al. (2020) <https://www.aclweb.org/anthology/2020.bea-1.2.pdf>`_
@@ -262,18 +259,17 @@
         mse = mse_true(system, human_scores, variance_errors_human)
 
         prmse = 1 - (mse / variance_true)
 
         return prmse
 
 
-def get_true_score_evaluations(df,
-                               system_score_columns,
-                               human_score_columns,
-                               variance_errors_human=None):
+def get_true_score_evaluations(
+    df, system_score_columns, human_score_columns, variance_errors_human=None
+):
     """
     Generate true score evaluations for HTML reports.
 
     Parameters
     ----------
     df: pandas DataFrame
         Input data frame. Must contain columns listed in
@@ -312,44 +308,49 @@
         - "prmse": proportional reduction in mean squared error when
           predicting true score
     """
     # check that if we only have one human column, we were also given
     # variance of errors
     if isinstance(human_score_columns, str):
         if variance_errors_human is None:
-            raise(ValueError("True score evaluations require estimating "
-                             "variance of human errors, "
-                             "which can only be computed when a subset "
-                             "of responses has two or more human ratings. "
-                             "If a single human_score_column "
-                             "is supplied, one must also specify variance_errors_human"))
+            raise (
+                ValueError(
+                    "True score evaluations require estimating "
+                    "variance of human errors, "
+                    "which can only be computed when a subset "
+                    "of responses has two or more human ratings. "
+                    "If a single human_score_column "
+                    "is supplied, one must also specify variance_errors_human"
+                )
+            )
 
     if isinstance(system_score_columns, str):
         system_score_columns = [system_score_columns]
 
     # compute variance of errors if it wasn't specified
     if variance_errors_human is None:
         variance_errors_human = variance_of_errors(df[human_score_columns])
 
     # compute prmse
     prmse_all = []
     for system in system_score_columns:
         mse = mse_true(df[system], df[human_score_columns], variance_errors_human)
         prmse = prmse_true(df[system], df[human_score_columns], variance_errors_human)
-        prmse_metrics = pd.Series({'MSE true': mse,
-                                   'PRMSE true': prmse}, name=system)
+        prmse_metrics = pd.Series({"MSE true": mse, "PRMSE true": prmse}, name=system)
         prmse_all.append(prmse_metrics)
 
     df_prmse = pd.concat(prmse_all, axis=1, sort=True).transpose()
 
     score_counts = get_n_human_scores(df[human_score_columns])
 
     # compute values that are the same for all scores
-    df_prmse.insert(0, 'N', len(df))
-    df_prmse.insert(1, 'N raters', score_counts.max())
-    df_prmse.insert(2, 'N single', (score_counts == 1).sum()),
-    df_prmse.insert(3, 'N multiple', (score_counts > 1).sum()),
-    df_prmse.insert(4, 'Variance of errors', variance_errors_human)
-    df_prmse.insert(5, 'True score var',
-                    true_score_variance(df[human_score_columns],
-                                        variance_errors_human))
+    df_prmse.insert(0, "N", len(df))
+    df_prmse.insert(1, "N raters", score_counts.max())
+    df_prmse.insert(2, "N single", (score_counts == 1).sum()),
+    df_prmse.insert(3, "N multiple", (score_counts > 1).sum()),
+    df_prmse.insert(4, "Variance of errors", variance_errors_human)
+    df_prmse.insert(
+        5,
+        "True score var",
+        true_score_variance(df[human_score_columns], variance_errors_human),
+    )
     return df_prmse
```

### Comparing `rsmtool-9.0.1/rsmtool/writer.py` & `rsmtool-9.1.1/rsmtool/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,47 +41,51 @@
         Raises
         ------
         KeyError
             If ``file_format`` is not valid.
         """
         file_format = file_format.lower()
 
-        if file_format == 'csv':
-            name_prefix += '.csv'
+        if file_format == "csv":
+            name_prefix += ".csv"
             df.to_csv(name_prefix, index=index, **kwargs)
 
-        elif file_format == 'tsv':
-            name_prefix += '.tsv'
-            df.to_csv(name_prefix, index=index, sep='\t', **kwargs)
+        elif file_format == "tsv":
+            name_prefix += ".tsv"
+            df.to_csv(name_prefix, index=index, sep="\t", **kwargs)
 
         # Added jsonlines for experimental purposes, but leaving
         # this out of the documentation at this stage
-        elif file_format == 'jsonlines':
-            name_prefix += '.jsonlines'
-            df.to_json(name_prefix, orient='records', lines=True, **kwargs)
+        elif file_format == "jsonlines":
+            name_prefix += ".jsonlines"
+            df.to_json(name_prefix, orient="records", lines=True, **kwargs)
 
-        elif file_format == 'xlsx':
-            name_prefix += '.xlsx'
+        elif file_format == "xlsx":
+            name_prefix += ".xlsx"
             df.to_excel(name_prefix, index=index, **kwargs)
 
         else:
-            raise KeyError("Please make sure that the `file_format` specified "
-                           "is one of the following:\n{`csv`, `tsv`, `xlsx`}.\n"
-                           f"You specified {file_format}.")
-
-    def write_experiment_output(self,
-                                csvdir,
-                                container_or_dict,
-                                dataframe_names=None,
-                                new_names_dict=None,
-                                include_experiment_id=True,
-                                reset_index=False,
-                                file_format='csv',
-                                index=False,
-                                **kwargs):
+            raise KeyError(
+                "Please make sure that the `file_format` specified "
+                "is one of the following:\n{`csv`, `tsv`, `xlsx`}.\n"
+                f"You specified {file_format}."
+            )
+
+    def write_experiment_output(
+        self,
+        csvdir,
+        container_or_dict,
+        dataframe_names=None,
+        new_names_dict=None,
+        include_experiment_id=True,
+        reset_index=False,
+        file_format="csv",
+        index=False,
+        **kwargs,
+    ):
         """
         Write out each of the named frames to disk.
 
         This function writes out each of the given list of data frames as a
         ".csv", ".tsv", or ``.xlsx`` file in the given directory. Each data
         frame was generated as part of running an RSMTool experiment. All files
         are prefixed with the given experiment ID and suffixed with either the
@@ -131,60 +135,57 @@
             dataframe_names = container_or_dict.keys()
 
         # Otherwise, check to make sure all specified names
         # are actually in the DataContainer
         else:
             for name in dataframe_names:
                 if name not in container_or_dict:
-                    raise KeyError("The name `{}` is not in the container "
-                                   "or dictionary.".format(name))
+                    raise KeyError(f"The name `{name}` is not in the container or dictionary.")
 
         # Loop through DataFrames, and save
         # output in specified format
         for dataframe_name in dataframe_names:
 
             df = container_or_dict[dataframe_name]
             if df is None:
-                raise KeyError('The DataFrame `{}` does not exist.'.format(dataframe_name))
+                raise KeyError(f"The DataFrame `{dataframe_name}` does not exist.")
 
             # If the DataFrame is empty, skip it
             if df.empty:
                 continue
 
             # If there is a desire to rename the DataFrame,
             # get the new name
             if new_names_dict is not None:
                 if dataframe_name in new_names_dict:
                     dataframe_name = new_names_dict[dataframe_name]
 
             # Reset the index, if desired
             if reset_index:
-                df.index.name = ''
+                df.index.name = ""
                 df.reset_index(inplace=True)
 
             # If include_experiment_id is True, and the experiment_id exists
             # include it in the file name; otherwise, do not include it.
             if include_experiment_id and self._id is not None:
-                outfile = join(csvdir, '{}_{}'.format(self._id, dataframe_name))
+                outfile = join(csvdir, f"{self._id}_{dataframe_name}")
             else:
                 outfile = join(csvdir, dataframe_name)
 
             # write out the frame to disk in the given file
-            self.write_frame_to_file(df,
-                                     outfile,
-                                     file_format=file_format,
-                                     index=index,
-                                     **kwargs)
-
-    def write_feature_csv(self,
-                          featuredir,
-                          data_container,
-                          selected_features,
-                          include_experiment_id=True,
-                          file_format='csv'):
+            self.write_frame_to_file(df, outfile, file_format=file_format, index=index, **kwargs)
+
+    def write_feature_csv(
+        self,
+        featuredir,
+        data_container,
+        selected_features,
+        include_experiment_id=True,
+        file_format="csv",
+    ):
         """
         Write out the selected features to disk.
 
         Parameters
         ----------
         featuredir : str
             Path to the experiment output directory where the
@@ -197,23 +198,24 @@
             Whether to include the experiment ID in the file name.
             Defaults to ``True``.
         file_format : str, optional
             The file format in which to output the data.
             One of {"csv", "tsv", "xlsx"}.
             Defaults to "csv".
         """
-        df_feature_specs = data_container['feature_specs']
+        df_feature_specs = data_container["feature_specs"]
 
         # Select specific features used in training
-        df_selected = df_feature_specs[df_feature_specs['feature'].isin(selected_features)]
+        df_selected = df_feature_specs[df_feature_specs["feature"].isin(selected_features)]
 
         # Replace existing `feature_specs` with selected features specs
-        data_container.add_dataset({'frame': df_selected,
-                                    'name': 'feature_specs'}, update=True)
+        data_container.add_dataset({"frame": df_selected, "name": "feature_specs"}, update=True)
 
         makedirs(featuredir, exist_ok=True)
-        self.write_experiment_output(featuredir,
-                                     data_container,
-                                     ['feature_specs'],
-                                     {'feature_specs': 'selected'},
-                                     include_experiment_id=include_experiment_id,
-                                     file_format=file_format)
+        self.write_experiment_output(
+            featuredir,
+            data_container,
+            ["feature_specs"],
+            {"feature_specs": "selected"},
+            include_experiment_id=include_experiment_id,
+            file_format=file_format,
+        )
```

### Comparing `rsmtool-9.0.1/rsmtool.egg-info/PKG-INFO` & `rsmtool-9.1.1/rsmtool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsmtool
-Version: 9.0.1
+Version: 9.1.1
 Summary: Rater scoring modeling tool
 Home-page: http://github.com/EducationalTestingService/rsmtool
 Maintainer: Nitin Madnani
 Maintainer-email: nmadnani@ets.org
 License: Apache 2
 Keywords: scoring modeling
 Classifier: Intended Audience :: Science/Research
@@ -36,15 +36,15 @@
    :target: https://codecov.io/gh/EducationalTestingService/rsmtool
    :alt: Coverage status
 
 .. image:: https://img.shields.io/conda/v/ets/rsmtool.svg
    :target: https://anaconda.org/ets/rsmtool
    :alt: Conda package for SKLL
 
-.. image:: https://img.shields.io/readthedocs/rsmtool/v9.0.1.svg
+.. image:: https://img.shields.io/readthedocs/rsmtool/v9.1.0.svg
    :target: https://rsmtool.readthedocs.io
    :alt: Docs
 
 .. image:: https://img.shields.io/badge/DOI-10.21105%2Fjoss.00033-blue.svg
    :target: http://joss.theoj.org/papers/10.21105/joss.00033
    :alt: DOI for citing RSMTool
```

### Comparing `rsmtool-9.0.1/setup.py` & `rsmtool-9.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 #!/usr/bin/env python
 from setuptools import find_packages, setup
 
 # Get version without importing, which avoids dependency issues
-exec(compile(open('rsmtool/version.py').read(), 'rsmtool/version.py', 'exec'))
+exec(compile(open("rsmtool/version.py").read(), "rsmtool/version.py", "exec"))
 # (we use the above instead of execfile for Python 3.x compatibility)
 
 
 def readme():
-    with open('README.rst') as f:
+    with open("README.rst") as f:
         return f.read()
 
 
 def requirements():
-    req_path = 'requirements.txt'
+    req_path = "requirements.txt"
     with open(req_path) as f:
         reqs = f.read().splitlines()
     return reqs
 
 
-setup(name='rsmtool',
-      version=__version__,
-      description='Rater scoring modeling tool',
-      long_description=readme(),
-      keywords='scoring modeling',
-      url='http://github.com/EducationalTestingService/rsmtool',
-      maintainer='Nitin Madnani',
-      maintainer_email='nmadnani@ets.org',
-      license='Apache 2',
-      packages=find_packages(),
-      include_package_data=True,
-      entry_points={'console_scripts':
-                    ['rsmtool = rsmtool.rsmtool:main',
-                     'rsmeval = rsmtool.rsmeval:main',
-                     'rsmpredict = rsmtool.rsmpredict:main',
-                     'rsmcompare = rsmtool.rsmcompare:main',
-                     'rsmsummarize = rsmtool.rsmsummarize:main',
-                     'rsmxval = rsmtool.rsmxval:main',
-                     'render_notebook = rsmtool.reporter:main',
-                     'convert_feature_json = rsmtool.convert_feature_json:main']
-                    },
-      install_requires=requirements(),
-      classifiers=['Intended Audience :: Science/Research',
-                   'Intended Audience :: Developers',
-                   'Programming Language :: Python',
-                   'Topic :: Scientific/Engineering',
-                   'Operating System :: Microsoft :: Windows',
-                   'Operating System :: POSIX',
-                   'Operating System :: Unix',
-                   'Operating System :: MacOS',
-                   'Programming Language :: Python :: 3',
-                   'Programming Language :: Python :: 3.8',
-                   'Programming Language :: Python :: 3.9',
-                   'Programming Language :: Python :: 3.10',
-                   ],
-      zip_safe=False)
+setup(
+    name="rsmtool",
+    version=__version__,  # noqa
+    description="Rater scoring modeling tool",
+    long_description=readme(),
+    keywords="scoring modeling",
+    url="http://github.com/EducationalTestingService/rsmtool",
+    maintainer="Nitin Madnani",
+    maintainer_email="nmadnani@ets.org",
+    license="Apache 2",
+    packages=find_packages(),
+    include_package_data=True,
+    entry_points={
+        "console_scripts": [
+            "rsmtool = rsmtool.rsmtool:main",
+            "rsmeval = rsmtool.rsmeval:main",
+            "rsmpredict = rsmtool.rsmpredict:main",
+            "rsmcompare = rsmtool.rsmcompare:main",
+            "rsmsummarize = rsmtool.rsmsummarize:main",
+            "rsmxval = rsmtool.rsmxval:main",
+            "render_notebook = rsmtool.reporter:main",
+            "convert_feature_json = rsmtool.convert_feature_json:main",
+        ]
+    },
+    install_requires=requirements(),
+    classifiers=[
+        "Intended Audience :: Science/Research",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python",
+        "Topic :: Scientific/Engineering",
+        "Operating System :: Microsoft :: Windows",
+        "Operating System :: POSIX",
+        "Operating System :: Unix",
+        "Operating System :: MacOS",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+    ],
+    zip_safe=False,
+)
```

