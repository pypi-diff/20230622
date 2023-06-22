# Comparing `tmp/alphastats-0.6.1.tar.gz` & `tmp/alphastats-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphastats-0.6.1.tar", last modified: Mon Jun 12 17:39:16 2023, max compression
+gzip compressed data, was "alphastats-0.6.2.tar", last modified: Thu Jun 22 13:02:10 2023, max compression
```

## Comparing `alphastats-0.6.1.tar` & `alphastats-0.6.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.418555 alphastats-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-12 17:38:35.000000 alphastats-0.6.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-12 17:38:35.000000 alphastats-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-12 17:39:16.418555 alphastats-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-12 17:38:35.000000 alphastats-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.398555 alphastats-0.6.1/alphastats/
--rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet_Plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet_Preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/DataSet_Statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/data/
--rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/data/contaminations.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/gui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/gui/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/AlphaPeptStats.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/alphapeptstats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/alphastats_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/alphastats_logo_2.png
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/gui/pages/
--rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/02_Import Data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/03_Data Overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/03_Preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/04_Analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/pages/06_Results.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.402555 alphastats-0.6.1/alphastats/gui/sample_data/
--rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-06-12 17:38:35.000000 alphastats-0.6.1/alphastats/gui/sample_data/metadata.xlsx
--rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/sample_data/proteinGroups.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/gui/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/utils/analysis_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/utils/software_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/gui/utils/ui_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/load_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/loader/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/AlphaPeptLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/BaseLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/DIANNLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/FragPipeLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/MaxQuantLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/SpectronautLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/loader/mzTabLoader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/multicova/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/multicova/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/multicova/multicova.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/ClusterMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/DimensionalityReduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/IntensityPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/PlotUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/SampleHistogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/VolcanoPlot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/plots/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.414555 alphastats-0.6.1/alphastats/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/statistics/Anova.py
--rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/statistics/DifferentialExpressionAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/statistics/MultiCovaAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/statistics/StatisticUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-12 17:38:36.000000 alphastats-0.6.1/alphastats/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.398555 alphastats-0.6.1/alphastats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6004 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-12 17:39:16.000000 alphastats-0.6.1/alphastats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 17:39:16.418555 alphastats-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-06-12 17:38:36.000000 alphastats-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:39:16.418555 alphastats-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    35022 2023-06-12 17:38:36.000000 alphastats-0.6.1/tests/test_DataSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-12 17:38:36.000000 alphastats-0.6.1/tests/test_DataSet_Pathway.py
--rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-12 17:38:36.000000 alphastats-0.6.1/tests/test_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-06-22 13:01:29.000000 alphastats-0.6.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-22 13:01:29.000000 alphastats-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-22 13:02:10.215180 alphastats-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-06-22 13:01:29.000000 alphastats-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19551 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet_Plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11609 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet_Preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/DataSet_Statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    70534 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/data/contaminations.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/gui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/gui/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/AlphaPeptStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31042 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/alphapeptstats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    30529 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/alphastats_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20433 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/alphastats_logo_2.png
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/gui/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)    12385 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/02_Import Data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/03_Data Overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/03_Preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/04_Analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/pages/06_Results.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats/gui/sample_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    26661 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/sample_data/metadata.xlsx
+-rw-r--r--   0 runner    (1001) docker     (123)  9509624 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/sample_data/proteinGroups.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.211180 alphastats-0.6.2/alphastats/gui/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/utils/analysis_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/utils/software_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/gui/utils/ui_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/load_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/alphastats/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/AlphaPeptLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/BaseLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/DIANNLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/FragPipeLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/MaxQuantLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/SpectronautLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/loader/mzTabLoader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/alphastats/multicova/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/multicova/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29756 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/multicova/multicova.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/alphastats/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/ClusterMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5132 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/DimensionalityReduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/IntensityPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/PlotUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/SampleHistogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/VolcanoPlot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/plots/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/alphastats/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/statistics/Anova.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8319 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/statistics/DifferentialExpressionAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/statistics/MultiCovaAnalysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/statistics/StatisticUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-22 13:01:29.000000 alphastats-0.6.2/alphastats/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.203180 alphastats-0.6.2/alphastats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 13:02:10.000000 alphastats-0.6.2/alphastats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 13:02:10.215180 alphastats-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-22 13:01:30.000000 alphastats-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:02:10.215180 alphastats-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    35024 2023-06-22 13:01:30.000000 alphastats-0.6.2/tests/test_DataSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-06-22 13:01:30.000000 alphastats-0.6.2/tests/test_DataSet_Pathway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9477 2023-06-22 13:01:30.000000 alphastats-0.6.2/tests/test_loaders.py
```

### Comparing `alphastats-0.6.1/LICENSE.txt` & `alphastats-0.6.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/PKG-INFO` & `alphastats-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.1
-Summary: An open-source Python package for Mass Spectrometry Analysis
+Version: 0.6.2
+Summary: An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
-Author-email: elena.krismer@hotmail.com
+Author-email: elena.krismer@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
 Project-URL: ReadTheDocs, https://mannlabs.github.io/alphapeptstats/
 Project-URL: PyPi, https://pypi.org/project/alphastats/
 Keywords: bioinformatics,software,mass spectometry
 Classifier: Development Status :: 1 - Planning
```

### Comparing `alphastats-0.6.1/README.md` & `alphastats-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/DataSet.py` & `alphastats-0.6.2/alphastats/DataSet.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
         df = df.set_index(self.index_column)
         df = df.filter(regex=(regex_find_intensity_columns), axis=1)
         # remove Intensity so only sample names remain
         substring_to_remove = regex_find_intensity_columns.replace(".*", "")
         df.columns = df.columns.str.replace(substring_to_remove, "")
         # transpose dataframe
         mat = df.transpose()
+        mat.replace([np.inf, -np.inf], np.nan, inplace=True)
         # remove proteins with only zero
         self.mat = mat.loc[:, (mat != 0).any(axis=0)]
         self.mat = self.mat.astype(float)
         # reset preproccessing info
         self.preprocessing_info = self._save_dataset_info()
         self.preprocessed = False
         self.rawmat = mat
@@ -202,11 +203,11 @@
         return preprocessing_dict
 
     def overview(self):
         """Print overview of the DataSet"""
         dataset_overview = (
             "Attributes of the DataSet can be accessed using: \n"
             + "DataSet.rawinput:\t Raw Protein data.\n"
-            + "DataSet.mat:\tProcessed data matrix with ProteinIDs/ProteinGroups as columns and samples as rows. All computations are performed on this matrix.\n"
+            + "DataSet.mat:\t\tProcessed data matrix with ProteinIDs/ProteinGroups as columns and samples as rows. All computations are performed on this matrix.\n"
             + "DataSet.metadata:\tMetadata for the samples in the matrix. Metadata will be matched with DataSet.mat when needed (for instance Volcano Plot)."
         )
         print(dataset_overview)
```

### Comparing `alphastats-0.6.1/alphastats/DataSet_Pathway.py` & `alphastats-0.6.2/alphastats/DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/DataSet_Plot.py` & `alphastats-0.6.2/alphastats/DataSet_Plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,14 +111,16 @@
             plotly.graph_objects._figure.Figure: UMAP plot
         """
         dimensionality_reduction = DimensionalityReduction(
             dataset=self, group=group, method="umap", circle=circle
         )
         return dimensionality_reduction.plot
 
+    
+    @ignore_warning(RuntimeWarning)
     def plot_volcano(
         self,
         group1,
         group2,
         column:str=None,
         method:str="ttest",
         labels:bool=False,
```

### Comparing `alphastats-0.6.1/alphastats/DataSet_Preprocess.py` & `alphastats-0.6.2/alphastats/DataSet_Preprocess.py`

 * *Files 14% similar despite different names*

```diff
@@ -77,19 +77,19 @@
             logging.info(
                 f" {len(protein_group_na)} Protein Groups were removed due to missing values."
             )
 
         logging.info("Imputing data...")
 
         if method == "mean":
-            imp = sklearn.impute.SimpleImputer(missing_values=np.nan, strategy="mean")
+            imp = sklearn.impute.SimpleImputer(missing_values=np.nan, strategy="mean", keep_empty_features=True)
             imputation_array = imp.fit_transform(self.mat.values)
 
         elif method == "median":
-            imp = sklearn.impute.SimpleImputer(missing_values=np.nan, strategy="median")
+            imp = sklearn.impute.SimpleImputer(missing_values=np.nan, strategy="median", keep_empty_features=True)
             imputation_array = imp.fit_transform(self.mat.values)
 
         elif method == "knn":
             # change for text
             method = "k-Nearest Neighbor"
             imp = sklearn.impute.KNNImputer(n_neighbors=2, weights="uniform")
             imputation_array = imp.fit_transform(self.mat.values)
@@ -141,15 +141,15 @@
 
         elif method == "linear":
             normalized_array = sklearn.preprocessing.normalize(
                 self.mat.values, norm="l2"
             )
 
         elif method == "vst":
-            scaler = sklearn.preprocessing.PowerTransformer()
+            scaler = sklearn.preprocessing.PowerTransformer(standardize=False)
             normalized_array = scaler.fit_transform(self.mat.values)
 
         else:
             raise ValueError(
                 "Normalization method: {method} is invalid"
                 "Choose from 'zscore', 'quantile', 'linear' normalization. or 'vst' for variance stabilization transformation"
             )
@@ -163,39 +163,48 @@
     def reset_preprocessing(self):
         """ Reset all preprocessing steps
         """
         # reset all preprocessing steps
         self.create_matrix()
         print("All preprocessing steps are reset.")
     
+    @ignore_warning(RuntimeWarning)
     def _compare_preprocessing_modes(self, func, params_for_func) -> list:
         dataset = self
-        imputation_methods = ["mean", "median", "knn"]
-        normalization_methods = ["zscore", "quantile", "vst"]
+
+        #    normalization_methods = methods["normalization"]
+       # if isinstance(methods, dict):
+        #    imputation_methods = methods["imputation"]
+        
+        imputation_methods = ["mean", "median", "knn", "randomforest"]
+        normalization_methods = ["vst","zscore", "quantile" ]
+        
         preprocessing_modes = list(itertools.product(normalization_methods, imputation_methods))
 
         results_list = []
 
         del params_for_func["compare_preprocessing_modes"]
         params_for_func["dataset"] = params_for_func.pop("self")
 
         for preprocessing_mode in preprocessing_modes:
             # reset preprocessing
             dataset.reset_preprocessing()
             print(f"Normalization {preprocessing_mode[0]}, Imputation {str(preprocessing_mode[1])}")
-            
+            dataset.mat.replace([np.inf, -np.inf], np.nan, inplace=True)
             dataset.preprocess(
                 subset=True,
                 normalization = preprocessing_mode[0],
                 imputation = preprocessing_mode[1]
             )
             
             res = func(**params_for_func)
             results_list.append(res)
         
+            print("\t")
+
         return results_list
 
     def _log2_transform(self):
         self.mat = np.log2(self.mat + 0.1)
         self.preprocessing_info.update({"Log2-transformed": True})
         print("Data has been log2-transformed.")
     
@@ -268,18 +277,20 @@
         
         if remove_samples is not None:
             self._remove_sampels(sample_list=remove_samples)
 
         if subset:
             self.mat = self._subset()
         
-        if log2_transform:
+        if log2_transform and self.preprocessing_info.get("Log2-transformed") is False:
             self._log2_transform()
 
         if normalization is not None:
             self._normalization(method=normalization)
+            self.mat = self.mat.replace([np.inf, -np.inf], np.nan)
+            #self.mat[:] = np.nan_to_num(self.mat)
 
         if imputation is not None:
             self._imputation(method=imputation)
 
         self.mat = self.mat.loc[:, (self.mat != 0).any(axis=0)]
         self.preprocessed = True
```

### Comparing `alphastats-0.6.1/alphastats/DataSet_Statistics.py` & `alphastats-0.6.2/alphastats/DataSet_Statistics.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/__init__.py` & `alphastats-0.6.2/alphastats/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 __project__ = "alphastats"
-__version__ = "0.6.1"
+__version__ = "0.6.2"
 __license__ = "Apache"
 __description__ = "An open-source Python package for Mass Spectrometry Analysis"
 __author__ = "Mann Labs"
 __author_email__ = "elena.krismer@hotmail.com"
 __github__ = "https://github.com/MannLabs/alphapeptstats"
 __keywords__ = [
     "bioinformatics",
```

### Comparing `alphastats-0.6.1/alphastats/data/contaminations.txt` & `alphastats-0.6.2/alphastats/data/contaminations.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/AlphaPeptStats.py` & `alphastats-0.6.2/alphastats/gui/AlphaPeptStats.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/alphapeptstats_logo.png` & `alphastats-0.6.2/alphastats/gui/alphapeptstats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/alphastats_logo.png` & `alphastats-0.6.2/alphastats/gui/alphastats_logo.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/alphastats_logo_2.png` & `alphastats-0.6.2/alphastats/gui/alphastats_logo_2.png`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/gui.py` & `alphastats-0.6.2/alphastats/gui/gui.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/pages/02_Import Data.py` & `alphastats-0.6.2/alphastats/gui/pages/02_Import Data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/pages/03_Data Overview.py` & `alphastats-0.6.2/alphastats/gui/pages/03_Data Overview.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/pages/03_Preprocessing.py` & `alphastats-0.6.2/alphastats/gui/pages/03_Preprocessing.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/pages/04_Analysis.py` & `alphastats-0.6.2/alphastats/gui/pages/04_Analysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/pages/06_Results.py` & `alphastats-0.6.2/alphastats/gui/pages/06_Results.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/sample_data/metadata.xlsx` & `alphastats-0.6.2/alphastats/gui/sample_data/metadata.xlsx`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/sample_data/proteinGroups.txt` & `alphastats-0.6.2/alphastats/gui/sample_data/proteinGroups.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/utils/analysis_helper.py` & `alphastats-0.6.2/alphastats/gui/utils/analysis_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/utils/options.py` & `alphastats-0.6.2/alphastats/gui/utils/options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/utils/software_options.py` & `alphastats-0.6.2/alphastats/gui/utils/software_options.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/gui/utils/ui_helper.py` & `alphastats-0.6.2/alphastats/gui/utils/ui_helper.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/load_data.py` & `alphastats-0.6.2/alphastats/load_data.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/loader/AlphaPeptLoader.py` & `alphastats-0.6.2/alphastats/loader/AlphaPeptLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/loader/BaseLoader.py` & `alphastats-0.6.2/alphastats/loader/BaseLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/loader/DIANNLoader.py` & `alphastats-0.6.2/alphastats/loader/DIANNLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/loader/FragPipeLoader.py` & `alphastats-0.6.2/alphastats/loader/FragPipeLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/loader/MaxQuantLoader.py` & `alphastats-0.6.2/alphastats/loader/MaxQuantLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/loader/SpectronautLoader.py` & `alphastats-0.6.2/alphastats/loader/SpectronautLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/loader/mzTabLoader.py` & `alphastats-0.6.2/alphastats/loader/mzTabLoader.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/multicova/multicova.py` & `alphastats-0.6.2/alphastats/multicova/multicova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/plots/ClusterMap.py` & `alphastats-0.6.2/alphastats/plots/ClusterMap.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/plots/DimensionalityReduction.py` & `alphastats-0.6.2/alphastats/plots/DimensionalityReduction.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,14 +130,15 @@
         fig = px.scatter(
             components,
             x=0,
             y=1,
             labels=self.labels,
             color=group_color,
             hover_data=[components[self.dataset.sample]],
+            template="simple_white+alphastats_colors"
         )
 
         # rename hover_data_0 to sample
         fig_dict = fig.to_plotly_json()
         data = fig_dict.get("data")
 
         for count, d in enumerate(data):
```

### Comparing `alphastats-0.6.1/alphastats/plots/IntensityPlot.py` & `alphastats-0.6.2/alphastats/plots/IntensityPlot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,37 @@
 
 import logging
 import scipy
 import numpy as np
 import plotly.graph_objects as go
 import plotly.express as px
+import plotly
 
 from alphastats.plots.PlotUtils import plotly_object, PlotUtils
 
+plotly.io.templates["alphastats_colors"] = plotly.graph_objects.layout.Template(
+    layout=plotly.graph_objects.Layout(
+        paper_bgcolor="rgba(0,0,0,0)",
+        plot_bgcolor="rgba(0,0,0,0)",
+        colorway=[
+            "#009599",
+            "#005358",
+            "#772173",
+            "#B65EAF",  # pink
+            "#A73A00",
+            "#6490C1",
+            "#FF894F",
+            "#2B5E8B",
+            "#A87F32",
+        ],
+    )
+)
+
+plotly.io.templates.default = "simple_white+alphastats_colors"
+
 
 class IntensityPlot(PlotUtils):
     def __init__(self,
         dataset,
         protein_id,
         group,
         subgroups,
@@ -111,31 +132,34 @@
 
         self.y_label = self.protein_id + " - " + self.dataset.intensity_column.replace("[sample]", "")
         self.prepared_df = df
 
     def _plot(self):
         if self.method == "violin":
             fig = px.violin(
-                self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label}
+                self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label},
+                template="simple_white+alphastats_colors"
             )
 
         elif self.method == "box":
             fig = px.box(
-                self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label}
+                self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label},
+                template="simple_white+alphastats_colors"
             )
 
         elif self.method == "scatter":
             fig = px.scatter(
-                 self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label}
+                 self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label},
+                 template="simple_white+alphastats_colors"
             )
 
         elif self.method == "all":
             fig = px.violin(
                  self.prepared_df, y=self.protein_id, x=self.group, color=self.group, labels={self.protein_id: self.y_label},
-                 box=True, points="all"
+                 box=True, points="all", template= "simple_white+alphastats_colors"
             )
 
         else:
             raise ValueError(
                 f"{self.method} is not available."
                 + "Please select from 'violin' for Violinplot, 'box' for Boxplot and 'scatter' for Scatterplot."
             )
```

### Comparing `alphastats-0.6.1/alphastats/plots/PlotUtils.py` & `alphastats-0.6.2/alphastats/plots/PlotUtils.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,31 @@
 import plotly
 import seaborn as sns
 import plotly.graph_objects as go
 
+plotly.io.templates["alphastats_colors"] = plotly.graph_objects.layout.Template(
+    layout=plotly.graph_objects.Layout(
+        paper_bgcolor="rgba(0,0,0,0)",
+        plot_bgcolor="rgba(0,0,0,0)",
+        colorway=[
+            "#009599",
+            "#005358",
+            "#772173",
+            "#B65EAF",  # pink
+            "#A73A00",
+            "#6490C1",
+            "#FF894F",
+            "#2B5E8B",
+            "#A87F32",
+        ],
+    )
+)
+
+plotly.io.templates.default = "simple_white+alphastats_colors"
+
 class PlotUtils:
     def __init__(self) -> None:
         pass
 
     @staticmethod
     def _update_colors_plotly(fig, color_dict):
         # plotly doesnt allow to assign color to certain group
```

### Comparing `alphastats-0.6.1/alphastats/plots/SampleHistogram.py` & `alphastats-0.6.2/alphastats/plots/SampleHistogram.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/plots/VolcanoPlot.py` & `alphastats-0.6.2/alphastats/plots/VolcanoPlot.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 from alphastats.plots.PlotUtils import PlotUtils, plotly_object
 from alphastats.utils import ignore_warning, check_for_missing_values
 
 import numpy as np
 import pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
-
+import plotly
 from functools import lru_cache
 
+plotly.io.templates["alphastats_colors"] = plotly.graph_objects.layout.Template(
+    layout=plotly.graph_objects.Layout(
+        paper_bgcolor="rgba(0,0,0,0)",
+        plot_bgcolor="rgba(0,0,0,0)",
+        colorway=[
+            "#009599",
+            "#005358",
+            "#772173",
+            "#B65EAF",  # pink
+            "#A73A00",
+            "#6490C1",
+            "#FF894F",
+            "#2B5E8B",
+            "#A87F32",
+        ],
+    )
+)
+
+plotly.io.templates.default = "simple_white+alphastats_colors"
 
 class VolcanoPlot(PlotUtils):
     def __init__(
         self, dataset, group1, group2, 
         column=None, method=None, 
         labels=None, min_fc=None, 
         alpha=None, draw_line=None, 
@@ -241,15 +260,15 @@
 
 
     def _annotate_result_df(self):
         """
         convert pvalue to log10
         add color labels for up and down regulates
         """
-        self.res = self.res[(self.res["log2fc"] < 10) & (self.res["log2fc"] > -10)]
+        self.res = self.res[(self.res["log2fc"] < 20) & (self.res["log2fc"] > -20)]
         self.res["-log10(p-value)"] = -np.log10(self.res[self.pvalue_column])
         
         self.alpha = -np.log10(self.alpha)
         # add color variable to plot
 
         if self.method != "sam":
         
@@ -349,14 +368,15 @@
     def _plot(self):
         self.plot = px.scatter(
             self.res,
             x="log2fc",
             y="-log10(p-value)",
             color="color",
             hover_data=self.hover_data,
+            template= "simple_white+alphastats_colors"
         )
         
         # update coloring
         self._color_data_points()
 
         if self.labels:
             self._add_labels_plot()
```

### Comparing `alphastats-0.6.1/alphastats/statistics/Anova.py` & `alphastats-0.6.2/alphastats/statistics/Anova.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/statistics/DifferentialExpressionAnalysis.py` & `alphastats-0.6.2/alphastats/statistics/DifferentialExpressionAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/statistics/MultiCovaAnalysis.py` & `alphastats-0.6.2/alphastats/statistics/MultiCovaAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/statistics/StatisticUtils.py` & `alphastats-0.6.2/alphastats/statistics/StatisticUtils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats/utils.py` & `alphastats-0.6.2/alphastats/utils.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/alphastats.egg-info/PKG-INFO` & `alphastats-0.6.2/alphastats.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: alphastats
-Version: 0.6.1
-Summary: An open-source Python package for Mass Spectrometry Analysis
+Version: 0.6.2
+Summary: An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics
 Home-page: https://github.com/MannLabs/alphastats
 Author: Mann Labs
-Author-email: elena.krismer@hotmail.com
+Author-email: elena.krismer@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: GitHub, https://github.com/MannLabs/alphapeptstats
 Project-URL: ReadTheDocs, https://mannlabs.github.io/alphapeptstats/
 Project-URL: PyPi, https://pypi.org/project/alphastats/
 Keywords: bioinformatics,software,mass spectometry
 Classifier: Development Status :: 1 - Planning
```

### Comparing `alphastats-0.6.1/alphastats.egg-info/SOURCES.txt` & `alphastats-0.6.2/alphastats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/setup.py` & `alphastats-0.6.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,21 +21,21 @@
     return required
     
 
 def create_pip_wheel():
     requirements = get_requirements()
     setuptools.setup(
         name="alphastats",
-        version="0.6.1",
+        version="0.6.2",
         license="Apache",
-        description="An open-source Python package for Mass Spectrometry Analysis",
+        description="An open-source Python package for automated and scalable statistical analysis of mass spectrometry-based proteomics",
         long_description=get_long_description(),
         long_description_content_type="text/markdown",
         author="Mann Labs",
-        author_email="elena.krismer@hotmail.com",
+        author_email="elena.krismer@gmail.com",
         url="https://github.com/MannLabs/alphastats",
         project_urls={
             "Mann Labs at MPIB": "https://www.biochem.mpg.de/mann",
             "GitHub": "https://github.com/MannLabs/alphapeptstats",
             "ReadTheDocs": "https://mannlabs.github.io/alphapeptstats/",
             "PyPi": "https://pypi.org/project/alphastats/"
             # "Scientific paper": None,
```

### Comparing `alphastats-0.6.1/tests/test_DataSet.py` & `alphastats-0.6.2/tests/test_DataSet.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,20 +291,20 @@
 
     def test_preprocess_normalize_vst(self):
         self.obj.mat = pd.DataFrame({"a": [2, 5, 4], "b": [5, 4, 4], "c": [0, 10, 8]})
         # Linear Normalization
         self.obj.preprocess(log2_transform=False,normalization="vst")
         expected_mat = pd.DataFrame(
             {
-                "a": [-1.30773413, 1.12010046, 0.18763367],
-                "b": [1.41421361, -0.70710674, -0.70710674],
-                "c": [-1.39384919, 0.90401955, 0.48982964],
+                "a": [ 3.19059101,  11.591763, 8.365096],
+                "b": [0.084829, 0.084829, 0.084829],
+                "c": [0.000000, 7.850074, 6.435102],
             }
         )
-        pd._testing.assert_frame_equal(self.obj.mat, expected_mat)
+        pd._testing.assert_frame_equal(self.obj.mat.round(2), expected_mat.round(2))
 
     def test_preprocess_imputation_mean_values(self):
         self.obj.mat = pd.DataFrame(
             {"a": [2, np.nan, 4], "b": [5, 4, 4], "c": [np.nan, 10, np.nan]}
         )
         self.obj.preprocess(log2_transform=False,imputation="mean")
         expected_mat = pd.DataFrame(
@@ -452,15 +452,15 @@
     def test_plot_volcano_compare_preprocessing_modes(self):
         result_list = self.obj.plot_volcano(
             method="ttest",
             group1=["1_31_C6", "1_32_C7", "1_57_E8"],
             group2=["1_71_F10", "1_73_F12"],
             compare_preprocessing_modes=True
         )
-        self.assertEqual(len(result_list), 9)               
+        self.assertEqual(len(result_list), 12)               
 
     def test_preprocess_subset(self):
         self.obj.preprocess(subset=True, log2_transform=False)
         self.assertEqual(self.obj.mat.shape, (48, 1364))
 
     @patch.object(Statistics, "tukey_test")
     def test_anova_without_tukey(self, mock):
```

### Comparing `alphastats-0.6.1/tests/test_DataSet_Pathway.py` & `alphastats-0.6.2/tests/test_DataSet_Pathway.py`

 * *Files identical despite different names*

### Comparing `alphastats-0.6.1/tests/test_loaders.py` & `alphastats-0.6.2/tests/test_loaders.py`

 * *Files identical despite different names*

