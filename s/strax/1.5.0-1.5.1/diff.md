# Comparing `tmp/strax-1.5.0.tar.gz` & `tmp/strax-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strax-1.5.0.tar", last modified: Tue May  2 19:36:47 2023, max compression
+gzip compressed data, was "strax-1.5.1.tar", last modified: Thu Jun 22 19:15:15 2023, max compression
```

## Comparing `strax-1.5.0.tar` & `strax-1.5.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.352210 strax-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-02 19:36:44.000000 strax-1.5.0/CODE-OF-CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-02 19:36:44.000000 strax-1.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    18803 2023-05-02 19:36:44.000000 strax-1.5.0/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-02 19:36:44.000000 strax-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-02 19:36:44.000000 strax-1.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    26592 2023-05-02 19:36:47.352210 strax-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-02 19:36:44.000000 strax-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.332210 strax-1.5.0/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-05-02 19:36:44.000000 strax-1.5.0/bin/rechunker
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.332210 strax-1.5.0/extra_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-02 19:36:44.000000 strax-1.5.0/extra_requirements/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-02 19:36:44.000000 strax-1.5.0/extra_requirements/requirements-tests.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-05-02 19:36:44.000000 strax-1.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-02 19:36:47.352210 strax-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-02 19:36:44.000000 strax-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.336210 strax-1.5.0/strax/
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-02 19:36:44.000000 strax-1.5.0/strax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-02 19:36:44.000000 strax-1.5.0/strax/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-05-02 19:36:44.000000 strax-1.5.0/strax/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-05-02 19:36:44.000000 strax-1.5.0/strax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    93514 2023-05-02 19:36:44.000000 strax-1.5.0/strax/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-05-02 19:36:44.000000 strax-1.5.0/strax/corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-02 19:36:44.000000 strax-1.5.0/strax/dtypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-02 19:36:44.000000 strax-1.5.0/strax/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20577 2023-05-02 19:36:44.000000 strax-1.5.0/strax/mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.340210 strax-1.5.0/strax/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/loop_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/merge_only_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/overlap_window_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/parrallel_source_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    27174 2023-05-02 19:36:44.000000 strax-1.5.0/strax/plugins/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.344210 strax-1.5.0/strax/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)    11787 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/general.py
--rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/hitlets.py
--rw-r--r--   0 runner    (1001) docker     (123)    19284 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/peak_building.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processing/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-05-02 19:36:44.000000 strax-1.5.0/strax/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19611 2023-05-02 19:36:44.000000 strax-1.5.0/strax/run_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.344210 strax-1.5.0/strax/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28547 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/file_rechunker.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-05-02 19:36:44.000000 strax-1.5.0/strax/storage/zipfiles.py
--rw-r--r--   0 runner    (1001) docker     (123)    11197 2023-05-02 19:36:44.000000 strax-1.5.0/strax/testutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23951 2023-05-02 19:36:44.000000 strax-1.5.0/strax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.340210 strax-1.5.0/strax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26592 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-02 19:36:47.000000 strax-1.5.0/strax.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:47.352210 strax-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 19:36:44.000000 strax-1.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_child_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    16586 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_corrections.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_cut_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_data_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_fixed_plugin_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    12413 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_general_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_get_zarr.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_hitlet.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_inline_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_lone_hit_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_loop_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_mailbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_mongo_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_multi_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_overlap_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_peak_merging.py
--rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_peak_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_peak_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_peak_splitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_pulse_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_saving.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_superruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-02 19:36:44.000000 strax-1.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.967150 strax-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-06-22 19:15:12.000000 strax-1.5.1/CODE-OF-CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-22 19:15:12.000000 strax-1.5.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    20356 2023-06-22 19:15:12.000000 strax-1.5.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-22 19:15:12.000000 strax-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 19:15:12.000000 strax-1.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    28313 2023-06-22 19:15:15.967150 strax-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-06-22 19:15:12.000000 strax-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.959150 strax-1.5.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-06-22 19:15:12.000000 strax-1.5.1/bin/rechunker
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.959150 strax-1.5.1/extra_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 19:15:12.000000 strax-1.5.1/extra_requirements/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 19:15:12.000000 strax-1.5.1/extra_requirements/requirements-tests.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 19:15:12.000000 strax-1.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-22 19:15:15.967150 strax-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-22 19:15:12.000000 strax-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.959150 strax-1.5.1/strax/
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-22 19:15:12.000000 strax-1.5.1/strax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-22 19:15:12.000000 strax-1.5.1/strax/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14225 2023-06-22 19:15:12.000000 strax-1.5.1/strax/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11166 2023-06-22 19:15:12.000000 strax-1.5.1/strax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96667 2023-06-22 19:15:12.000000 strax-1.5.1/strax/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-06-22 19:15:12.000000 strax-1.5.1/strax/corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-06-22 19:15:12.000000 strax-1.5.1/strax/dtypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-06-22 19:15:12.000000 strax-1.5.1/strax/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20577 2023-06-22 19:15:12.000000 strax-1.5.1/strax/mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.963150 strax-1.5.1/strax/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/loop_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/merge_only_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/overlap_window_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7265 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/parrallel_source_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27242 2023-06-22 19:15:12.000000 strax-1.5.1/strax/plugins/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.963150 strax-1.5.1/strax/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18534 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23837 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/hitlets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19279 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/peak_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6938 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13818 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14551 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processing/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-22 19:15:12.000000 strax-1.5.1/strax/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20957 2023-06-22 19:15:12.000000 strax-1.5.1/strax/run_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.963150 strax-1.5.1/strax/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28547 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7709 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/file_rechunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-06-22 19:15:12.000000 strax-1.5.1/strax/storage/zipfiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11713 2023-06-22 19:15:12.000000 strax-1.5.1/strax/testutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-06-22 19:15:12.000000 strax-1.5.1/strax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.959150 strax-1.5.1/strax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28313 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 19:15:15.000000 strax-1.5.1/strax.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:15.967150 strax-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:15:12.000000 strax-1.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11542 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_child_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17852 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3948 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_corrections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_cut_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_data_reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_fixed_plugin_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16513 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_general_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_get_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20240 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_hitlet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_inline_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_lone_hit_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_loop_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5212 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_mailbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_mongo_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_multi_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_overlap_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_peak_merging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_peak_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_peak_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6045 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_peak_splitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_pulse_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_saving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_superruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-06-22 19:15:12.000000 strax-1.5.1/tests/test_utils.py
```

### Comparing `strax-1.5.0/CODE-OF-CONDUCT.md` & `strax-1.5.1/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/CONTRIBUTING.md` & `strax-1.5.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/HISTORY.md` & `strax-1.5.1/HISTORY.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+1.5.1 / 2023-06-22
+---------------------
+* Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/AxFoundation/strax/pull/721
+* Fix urllib3 version to 1.26.15 by @dachengx in https://github.com/AxFoundation/strax/pull/723
+* Save other fields in the merged peaks to their default value by @dachengx in https://github.com/AxFoundation/strax/pull/722
+* add a metadata comparison method by @KaraMelih in https://github.com/AxFoundation/strax/pull/706
+* Accelerate select_runs by @shenyangshi in https://github.com/AxFoundation/strax/pull/727
+* Stop assigning dependabot to Joran by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/732
+* Bump urllib3 from 1.26.15 to 2.0.2 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/729
+* Add new general fucntion which computes dt to some interval by @WenzDaniel in https://github.com/AxFoundation/strax/pull/726
+* Check whether `things` and `containers` are sorted by @dachengx in https://github.com/AxFoundation/strax/pull/725
+* Set start of further chunk to be the smallest start of dependencies by @dachengx in https://github.com/AxFoundation/strax/pull/715
+* Fix touching window by @dachengx in https://github.com/AxFoundation/strax/pull/736
+
+New Contributors
+* @KaraMelih made their first contribution in https://github.com/AxFoundation/strax/pull/706
+* @shenyangshi made their first contribution in https://github.com/AxFoundation/strax/pull/727
+
+**Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.5.0...v1.5.1
+
+
 1.5.0 / 2023-05-02
 ---------------------
 * Fix ipython version by @dachengx in https://github.com/AxFoundation/strax/pull/719
 * Do not change channel when sort_by_time by @dachengx in https://github.com/AxFoundation/strax/pull/718
 * Save hits level information(hits time difference) in peaks by @dachengx in https://github.com/AxFoundation/strax/pull/716
 
 **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.3...v1.5.0
```

### Comparing `strax-1.5.0/LICENSE` & `strax-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/PKG-INFO` & `strax-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.5.0
+Version: 1.5.1
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: Jelle Aalbers
 License: UNKNOWN
 Description: # strax
         Streaming analysis for xenon experiments
         
@@ -22,14 +22,35 @@
         
         Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
         
         Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
         
         
         
+        1.5.1 / 2023-06-22
+        ---------------------
+        * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/AxFoundation/strax/pull/721
+        * Fix urllib3 version to 1.26.15 by @dachengx in https://github.com/AxFoundation/strax/pull/723
+        * Save other fields in the merged peaks to their default value by @dachengx in https://github.com/AxFoundation/strax/pull/722
+        * add a metadata comparison method by @KaraMelih in https://github.com/AxFoundation/strax/pull/706
+        * Accelerate select_runs by @shenyangshi in https://github.com/AxFoundation/strax/pull/727
+        * Stop assigning dependabot to Joran by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/732
+        * Bump urllib3 from 1.26.15 to 2.0.2 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/729
+        * Add new general fucntion which computes dt to some interval by @WenzDaniel in https://github.com/AxFoundation/strax/pull/726
+        * Check whether `things` and `containers` are sorted by @dachengx in https://github.com/AxFoundation/strax/pull/725
+        * Set start of further chunk to be the smallest start of dependencies by @dachengx in https://github.com/AxFoundation/strax/pull/715
+        * Fix touching window by @dachengx in https://github.com/AxFoundation/strax/pull/736
+        
+        New Contributors
+        * @KaraMelih made their first contribution in https://github.com/AxFoundation/strax/pull/706
+        * @shenyangshi made their first contribution in https://github.com/AxFoundation/strax/pull/727
+        
+        **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.5.0...v1.5.1
+        
+        
         1.5.0 / 2023-05-02
         ---------------------
         * Fix ipython version by @dachengx in https://github.com/AxFoundation/strax/pull/719
         * Do not change channel when sort_by_time by @dachengx in https://github.com/AxFoundation/strax/pull/718
         * Save hits level information(hits time difference) in peaks by @dachengx in https://github.com/AxFoundation/strax/pull/716
         
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.3...v1.5.0
```

### Comparing `strax-1.5.0/README.md` & `strax-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/bin/rechunker` & `strax-1.5.1/bin/rechunker`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/setup.py` & `strax-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 with open('README.md') as file:
     readme = file.read()
 
 with open('HISTORY.md') as file:
     history = file.read()
 
 setuptools.setup(name='strax',
-                 version='1.5.0',
+                 version='1.5.1',
                  description='Streaming analysis for xenon TPCs',
                  author='Jelle Aalbers',
                  url='https://github.com/AxFoundation/strax',
                  setup_requires=['pytest-runner'],
                  install_requires=requires,
                  tests_require=requires + tests_requires,
                  long_description=readme + '\n\n' + history,
```

### Comparing `strax-1.5.0/strax/__init__.py` & `strax-1.5.1/strax/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flake8: noqa
-__version__ = '1.5.0'
+__version__ = '1.5.1'
 
 # Glue the package together
 # See https://www.youtube.com/watch?v=0oTh1CXRaQ0 if this confuses you
 # The order of subpackes is not invariant, since we use strax.xxx inside strax
 from .utils import *
 from .chunk import *
 from .dtypes import *
```

### Comparing `strax-1.5.0/strax/chunk.py` & `strax-1.5.1/strax/chunk.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/config.py` & `strax-1.5.1/strax/config.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/context.py` & `strax-1.5.1/strax/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import datetime
 import logging
 import warnings
 import fnmatch
 from functools import partial
 import typing as ty
 import time
+import json
 import numpy as np
 import pandas as pd
+import click
+import deepdiff
 import strax
 import inspect
 import types
 from collections import defaultdict
 from immutabledict import immutabledict
 from enum import IntEnum
 
@@ -1660,14 +1663,74 @@
             except strax.DataNotAvailable:
                 self.log.debug(f"Frontend {sf} does not have {key}")
         raise strax.DataNotAvailable(f"Can't load metadata, "
                                      f"data for {key} not available")
 
     get_metadata = get_meta
 
+    def compare_metadata(self, run_id, target, old_metadata):
+        """
+        Compare the metadata between two strax data
+
+        :param run_id: run id to get
+        :param target: data type to get
+        :param old_metadata: path to metadata to compare, or a dictionary, or a tuple with
+            another run_id, target to compare against the metadata of the first id-target pair
+        """
+        color_values = lambda oldval, newval: (
+            click.style(oldval, fg='red', bold=True), click.style(newval, fg='green', bold=True))
+        underline = lambda text, bold=True: click.style(text, bold=bold, underline=True)
+
+        # new metadata for the given runid + target; fetch from context
+        new_metadata = self.get_metadata(run_id, target)
+        # old metadata to compare
+        if isinstance(old_metadata, str):
+            with open(old_metadata) as json_file:
+                old_metadata = json.load(json_file)
+        elif isinstance(old_metadata, dict):
+            old_metadata = old_metadata
+        elif isinstance(old_metadata, (tuple, list)):
+            old_metadata = self.get_metadata(old_metadata[0], old_metadata[1])
+        else:
+            raise ValueError(f"Expected old_metadata as `str` or `dict` got {type(old_metadata)}")
+
+        differences = deepdiff.DeepDiff(old_metadata, new_metadata)
+        for key, value in differences.items():
+            if key in ['values_changed', 'iterable_item_added', 'iterable_item_removed']:
+                print(underline(f"\n> {key}"))
+                for kk, vv in value.items():
+                    if key == "values_changed":
+                        old_values = vv['old_value']
+                        new_values = vv['new_value']
+                    elif key == "iterable_item_added":
+                        old_values = "-"
+                        new_values = vv
+                    else:  # if key == "iterable_item_removed":
+                        old_values = vv
+                        new_values = "-"
+                    old, new = color_values(old_values, new_values)
+                    click.secho(f"\t in {kk[4:]}", bold=False)
+                    print(f"\t\t{old} -> {new}")
+            elif key in ['dictionary_item_added', 'dictionary_item_removed']:
+                color = "red" if "removed" in key else "green"
+                print(underline(f"\n> {key:25s}"), end="->")
+                click.secho(f"\t{', '.join(value)}", fg=color)
+            elif key in ['type_changes']:
+                print(underline(f"\n> {key}"))
+                for kk, vv in value.items():
+                    click.secho(f"\t{kk}")
+                    oldtype = vv['old_type']
+                    newtype = vv['new_type']
+                    keyold, keynew = color_values('old_type', 'new_type')
+                    valueold, valuenew = color_values(vv['old_value'], vv['new_value'])
+                    print(f"\t\t{keyold:10s} : {oldtype} ({valueold})")
+                    print(f"\t\t{keynew:10s} : {newtype} ({valuenew})")
+            else:
+                raise KeyError(f"Unkown key in comparison {key}")
+
     def run_metadata(self, run_id, projection=None) -> dict:
         """
         Return run-level metadata for run_id, or raise DataNotAvailable
         if this is not available
 
         :param run_id: run id to get
         :param projection: Selection of fields to get, following MongoDB
```

### Comparing `strax-1.5.0/strax/corrections.py` & `strax-1.5.1/strax/corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/dtypes.py` & `strax-1.5.1/strax/dtypes.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/io.py` & `strax-1.5.1/strax/io.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/mailbox.py` & `strax-1.5.1/strax/mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/plugins/cut_plugin.py` & `strax-1.5.1/strax/plugins/cut_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/plugins/loop_plugin.py` & `strax-1.5.1/strax/plugins/loop_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/plugins/merge_only_plugin.py` & `strax-1.5.1/strax/plugins/merge_only_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/plugins/overlap_window_plugin.py` & `strax-1.5.1/strax/plugins/overlap_window_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/plugins/parrallel_source_plugin.py` & `strax-1.5.1/strax/plugins/parrallel_source_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/plugins/plugin.py` & `strax-1.5.1/strax/plugins/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,14 +576,15 @@
             if hasattr(self.save_when, 'values'):
                 save_when = max([int(save_when) for save_when in self.save_when.values()])
             else:
                 save_when = self.save_when
             if save_when <= strax.SaveWhen.EXPLICIT:
                 # </start>This warning/check will be deleted, see UserWarning
                 if len(set(tranges.values())) != 1:
+                    start = min([v.start for v in kwargs.values()])
                     end = max([v.end for v in kwargs.values()])  # Don't delete
                     message = (
                         f"New feature, we are ignoring inconsistent the "
                         f"possible ValueError in time ranges for "
                         f"{self.__class__.__name__} of inputs: {tranges}"
                         f"because this occurred in a save_when.NEVER "
                         f"plugin. Report any findings in "
```

### Comparing `strax-1.5.0/strax/processing/data_reduction.py` & `strax-1.5.1/strax/processing/data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/processing/hitlets.py` & `strax-1.5.1/strax/processing/hitlets.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/processing/peak_building.py` & `strax-1.5.1/strax/processing/peak_building.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         p = buffer[offset]
         t0 = hit['time']
         dt = hit['dt']
         t1 = hit['time'] + dt * hit['length']
 
         if in_peak:
             # This hit continues an existing peak
-            p['max_gap'] = max(p['max_gap'], abs(t0 - peak_endtime))
+            p['max_gap'] = max(p['max_gap'], t0 - peak_endtime)
 
         else:
             # This hit starts a new peak candidate
             area_per_channel *= 0
             peak_endtime = t1
             p['time'] = t0 - left_extension
             p['channel'] = DIGITAL_SUM_WAVEFORM_CHANNEL
```

### Comparing `strax-1.5.0/strax/processing/peak_merging.py` & `strax-1.5.1/strax/processing/peak_merging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import strax
 import numba
 import numpy as np
 
+import strax
+from strax.processing.general import _fully_contained_in, _fully_contained_in_sanity
+
 export, __all__ = strax.exporter()
 
 
 @export
 def merge_peaks(peaks, start_merge_at, end_merge_at,
                 max_buffer=int(1e5)):
     """Merge specified peaks with their neighbors, return merged peaks
@@ -40,27 +42,23 @@
         new_p['length'] = \
             (strax.endtime(last_peak) - new_p['time']) // common_dt
 
         # re-zero relevant part of buffers (overkill? not sure if
         # this saves much time)
         buffer[:min(
             int(
-                (
-                        last_peak['time']
-                        + (last_peak['length'] * old_peaks['dt'].max())
-                        - first_peak['time']) / common_dt
+                (last_peak['time']- first_peak['time']
+                 + (last_peak['length'] * old_peaks['dt'].max())) / common_dt
             ),
             len(buffer)
         )] = 0
         buffer_top[:min(
             int(
-                (
-                        last_peak['time']
-                        + (last_peak['length'] * old_peaks['dt'].max())
-                        - first_peak['time']) / common_dt
+                (last_peak['time'] - first_peak['time']
+                 + (last_peak['length'] * old_peaks['dt'].max())) / common_dt
             ),
             len(buffer_top)
         )] = 0
 
         for p in old_peaks:
             # Upsample the sum and top/bottom array waveforms into their buffers
             upsample = p['dt'] // common_dt
@@ -79,19 +77,24 @@
 
         # Downsample the buffers into new_p['data'], new_p['data_top'],
         # and new_p['data_bot']
         strax.store_downsampled_waveform(new_p, buffer, True, buffer_top)
 
         new_p['n_saturated_channels'] = new_p['saturated_channel'].sum()
 
-        # Use the tight coincidence of the peak with the highest amplitude
+        # Use tight_coincidence of the peak with the highest amplitude
         i_max_subpeak = old_peaks['data'].max(axis=1).argmax()
         new_p['tight_coincidence'] = old_peaks['tight_coincidence'][i_max_subpeak]
-        
-        # If the endtime was in the peaks we have to recompute it here 
+
+        # Too lazy to compute these
+        for p in 'max_gap max_diff min_diff'.split():
+            new_p[p] = -1
+        new_p['max_goodness_of_split'] = np.nan
+
+        # If the endtime was in the peaks we have to recompute it here
         # because otherwise it will stay set to zero due to the buffer
         if 'endtime' in new_p.dtype.names:
             new_p['endtime'] = strax.endtime(last_peak)
     return new_peaks
 
 
 @export
@@ -146,29 +149,35 @@
         result[result_i] = merge[window_i]
         result_i += 1
         window_i += 1
 
     assert result_i == len(result)
     assert window_i == len(skip_windows)
 
-    
+
 @export
-@numba.njit(cache=True, nogil=True)
 def add_lone_hits(peaks, lone_hits, to_pe, n_top_channels=0):
     """
     Function which adds information from lone hits to peaks if lone hit
     is inside a peak (e.g. after merging.). Modifies peak area and data
     inplace.
 
     :param peaks: Numpy array of peaks
     :param lone_hits: Numpy array of lone_hits
     :param to_pe: Gain values to convert lone hit area into PE.
     :param n_top_channels: Number of top array channels.
     """
-    fully_contained_index = strax.fully_contained_in(lone_hits, peaks)
+    _fully_contained_in_sanity(lone_hits, peaks)
+    _add_lone_hits(peaks, lone_hits, to_pe, n_top_channels=0)
+
+
+@numba.njit(cache=True, nogil=True)
+def _add_lone_hits(peaks, lone_hits, to_pe, n_top_channels=0):
+    """The core function of add_lone_hits"""
+    fully_contained_index = _fully_contained_in(lone_hits, peaks)
 
     for fc_i, lh_i in zip(fully_contained_index, lone_hits):
         if fc_i == -1:
             continue
         p = peaks[fc_i]
         lh_area = lh_i['area'] * to_pe[lh_i['channel']]
         p['area'] += lh_area
```

### Comparing `strax-1.5.0/strax/processing/peak_properties.py` & `strax-1.5.1/strax/processing/peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/processing/peak_splitting.py` & `strax-1.5.1/strax/processing/peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/processing/pulse_processing.py` & `strax-1.5.1/strax/processing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/processing/statistics.py` & `strax-1.5.1/strax/processing/statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     area_tot = np.sum(data)
     if area_tot <= 0:
         raise ValueError('Highest density regions are not defined for distributions '
                          'with a total probability of less-equal 0.')
 
     # Need an index which sorted by amplitude
-    max_to_min = np.argsort(data)[::-1]
+    max_to_min = np.argsort(data, kind='mergesort')[::-1]
 
     lowest_sample_seen = np.inf
     for j in range(1, len(data)):
         # Loop over indices compute fractions from max to min
         if lowest_sample_seen == data[max_to_min[j]]:
             # We saw this sample height already, so no need to repeat
             continue
```

### Comparing `strax-1.5.0/strax/processor.py` & `strax-1.5.1/strax/processor.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/run_selection.py` & `strax-1.5.1/strax/run_selection.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,26 +12,35 @@
 # use tqdm as loaded in utils (from tqdm.notebook when in a juypyter env)
 tqdm = strax.utils.tqdm
 
 export, __all__ = strax.exporter()
 
 
 @strax.Context.add_method
-def list_available(self, target, **kwargs) -> list:
-    """Return sorted list of run_id's for which target is available"""
+def list_available(self, target,
+                   runs=None,
+                   **kwargs) -> list:
+    """Return sorted list of run_id's for which target is available
+    :param target: Data type to check
+    :param runs: Runs to check. If None, check all runs.
+    """
+
     if len(kwargs):
         # noinspection PyMethodFirstArgAssignment
         self = self.new_context(**kwargs)
 
     if self.runs is None:
         self.scan_runs()
 
-    keys = set(self.keys_for_runs(
-        target,
-        self.runs['name'].values))
+    if runs is None:
+        runs = self.runs['name'].values
+    else:
+        runs = strax.to_str_tuple(runs)
+
+    keys = set(self.keys_for_runs(target, runs))
 
     found = set()
     for sf in self.storage:
         remaining = keys - found
         is_found = sf.find_several(list(remaining), **self._find_options)
         found |= set([k for i, k in enumerate(remaining)
                       if is_found[i]])
@@ -64,37 +73,45 @@
     else:
         return []
 
 
 @strax.Context.add_method
 def scan_runs(self: strax.Context,
               check_available=tuple(),
+              if_check_available='raise',
               store_fields=tuple(),
              ) -> pd.DataFrame:
     """
     Update and return self.runs with runs currently available
     in all storage frontends.
 
     :param check_available: Check whether these data types are available
         Availability of xxx is stored as a boolean in the xxx_available
         column.
+    :param if_check_available: 'raise' (default) or 'skip', whether to do the check
     :param store_fields: Additional fields from run doc to include
         as rows in the dataframe.
 
     The context options scan_availability and store_run_fields list
     data types and run fields, respectively, that will always be scanned.
     """
     store_fields = tuple(set(
         list(strax.to_str_tuple(store_fields))
         + ['name', 'number', 'tags', 'mode',
            strax.RUN_DEFAULTS_KEY]
         + list(self.context_config['store_run_fields'])))
-    check_available = tuple(set(
-        list(strax.to_str_tuple(check_available))
-        + list(self.context_config['check_available'])))
+    if if_check_available == 'raise':
+        check_available = tuple(set(
+            list(strax.to_str_tuple(check_available))
+            + list(self.context_config['check_available'])))
+    elif if_check_available == 'skip':
+        check_available = tuple()
+    else:
+        raise ValueError(
+            f"Invalid value for if_check_available: {if_check_available}")
 
     for target in check_available:
         save_when = self.get_save_when(target)
         if save_when < strax.SaveWhen.ALWAYS:
             p = self._plugin_class_registry[target]
             self.log.warning(f'{p.__name__}-plugin is {str(save_when)}. '
                              f'Therefore {target} is most likely not stored!')
@@ -133,30 +150,30 @@
                     and 'end' in store_fields
                     and 'livetime' in store_fields
                     and doc.get('start') is not None
                     and doc.get('end') is not None):
                 doc.setdefault('livetime', doc['end'] - doc['start'])
 
             if _is_superrun:
-                # In contrast to regular run-docs, 
-                # superruns are timezone aware. So strip off timezone 
+                # In contrast to regular run-docs,
+                # superruns are timezone aware. So strip off timezone
                 # again:
                 start = doc.get('start')
                 if start:
                     doc['start'] = start.replace(tzinfo=None)
-                    
+
                 start = doc.get('end')
                 if start:
                     doc['end'] = start.replace(tzinfo=None)
-                    
+
                 if type(doc.get('livetime')) == float:
                     # If we have a superrun livetime is stored as intger seconds
-                    # as timedelta is not json serializable 
+                    # as timedelta is not json serializable
                     doc['livetime'] = datetime.timedelta(seconds=doc['livetime'])
-            
+
             # Put the strax defaults stuff into a different cache
             if strax.RUN_DEFAULTS_KEY in doc:
                 self._run_defaults_cache[doc['name']] = \
                     doc[strax.RUN_DEFAULTS_KEY]
                 del doc[strax.RUN_DEFAULTS_KEY]
 
             doc = flatten_run_metadata(doc)
@@ -183,32 +200,35 @@
     if (not self.context_config['use_per_run_defaults']
         and strax.RUN_DEFAULTS_KEY in docs.columns):
         del docs[strax.RUN_DEFAULTS_KEY]
     docs = docs[['name'] + [x for x in docs.columns.tolist()
                             if x != 'name']]
     self.runs = docs
 
+    # Add available data types,
+    # this is kept for the case users directly call list_available
     for d in tqdm(check_available,
                   desc='Checking data availability'):
         self.runs[d + '_available'] = np.in1d(
             self.runs.name.values,
             self.list_available(d))
 
     return self.runs
 
 
 @strax.Context.add_method
 def select_runs(self, run_mode=None, run_id=None,
                 include_tags=None, exclude_tags=None,
                 available=tuple(),
-                pattern_type='fnmatch', ignore_underscore=True):
+                pattern_type='fnmatch', ignore_underscore=True,
+                force_reload=False):
     """
     Return pandas.DataFrame with basic info from runs
         that match selection criteria.
-   
+
     :param run_mode: Pattern to match run modes (reader.ini.name)
     :param run_id: Pattern to match a run_id or run_ids
     :param available: str or tuple of strs of data types for which data
         must be available according to the runs DB.
     :param include_tags: String or list of strings of patterns
         for required tags
     :param exclude_tags: String / list of strings of patterns
@@ -217,69 +237,85 @@
     :param pattern_type: Type of pattern matching to use.
         Defaults to 'fnmatch', which means you can use
         unix shell-style wildcards (`?`, `*`).
         The alternative is 're', which means you can use
         full python regular expressions.
     :param ignore_underscore: Ignore the underscore at the start of tags
         (indicating some degree of officialness or automation).
+    :param force_reload: Force reloading of runs from storage.
+        Otherwise, runs are cached after the first time they are loaded in self.runs.
 
     Examples:
      - `run_selection(include_tags='blinded')`
         select all datasets with a blinded or _blinded tag.
      - `run_selection(include_tags='*blinded')`
         ... with blinded or _blinded, unblinded, blablinded, etc.
      - `run_selection(include_tags=['blinded', 'unblinded'])`
         ... with blinded OR unblinded, but not blablinded.
      - `run_selection(include_tags='blinded',
                       exclude_tags=['bad', 'messy'])`
         ... select blinded dsatasets that aren't bad or messy
     """
-    if self.runs is None:
-        self.scan_runs(check_available=strax.to_str_tuple(available))
+    if self.runs is None or force_reload:
+        self.scan_runs(if_check_available='skip')
     dsets = self.runs.copy()
 
     if pattern_type not in ('re', 'fnmatch'):
         raise ValueError("Pattern type must be 're' or 'fnmatch'")
 
-    # Filter datasets by run mode and/or name
+    # Filter datasets by run mode and/or name first
     for field_name, requested_value in (
             ('name', run_id),
             ('mode', run_mode)):
 
         if requested_value is None:
             continue
-            
+
         requested_value = strax.to_str_tuple(requested_value)
 
         values = dsets[field_name].values
         mask = np.zeros(len(values), dtype=np.bool_)
 
         if pattern_type == 'fnmatch':
             for i, x in enumerate(values):
-                mask[i] = np.any([fnmatch.fnmatch(x, rv) for rv in requested_value]) 
+                mask[i] = np.any([fnmatch.fnmatch(x, rv) for rv in requested_value])
         elif pattern_type == 're':
             for i, x in enumerate(values):
                 mask[i] = np.any([re.match(rv, x) for rv in requested_value])
 
         dsets = dsets[mask]
 
     dsets = _include_exclude_tags(dsets, include_tags, exclude_tags, pattern_type,
                                   ignore_underscore,
                                   )
 
+    # Check data availability only for selected datasets
+    check_available = tuple(set(
+        list(strax.to_str_tuple(available))
+        + list(self.context_config['check_available'])))
+
+    for d in tqdm(check_available,
+                  desc='Checking data availability'):
+        dsets[d + '_available'] = np.in1d(
+            dsets.name.values,
+            self.list_available(target=d, runs=dsets.name.values))
+
+    # This will help users call select_runs multiple times
+    # with same run mode and/or name, but different available
     have_available = strax.to_str_tuple(available)
     for d in have_available:
         if not d + '_available' in dsets.columns:
             # Get extra availability info from the run db
-            d_available = np.in1d(self.runs.name.values,
-                                  self.list_available(d))
+            d_available = np.in1d(dsets.name.values,
+                                  self.list_available(target=d, runs=dsets.name.values))
             # Save both in the context and for this selection using
             # available = ('data_type',)
-            self.runs[d + '_available'] = d_available
             dsets[d + '_available'] = d_available
+
+    # Only return dsets available
     for d in have_available:
         dsets = dsets[dsets[d + '_available']]
 
     return dsets
 
 
 @strax.Context.add_method
@@ -302,15 +338,15 @@
         numpy.array/pandas.DataFrame containing some data.
     :param from_run: List of run_ids which were used to create the
         numpy.array/pandas.DataFrame passed in data.
     """
     if isinstance(data, (pd.DataFrame, np.ndarray)):
         if isinstance(data, np.ndarray):
             data = pd.DataFrame.from_records(data)
-      
+
         # strax.endtime does not work with DataFrames due to numba
         if 'endtime' in data.columns:
             end = data['endtime']
         else:
             end = data['time'] + data['length'] * data['dt']
             
         # Array of events / regions of interest
```

### Comparing `strax-1.5.0/strax/storage/common.py` & `strax-1.5.1/strax/storage/common.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/storage/file_rechunker.py` & `strax-1.5.1/strax/storage/file_rechunker.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/storage/files.py` & `strax-1.5.1/strax/storage/files.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/storage/mongo.py` & `strax-1.5.1/strax/storage/mongo.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/storage/zipfiles.py` & `strax-1.5.1/strax/storage/zipfiles.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/strax/testutils.py` & `strax-1.5.1/strax/testutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,41 +15,55 @@
 
 
 # Since we use np.cumsum to get disjoint intervals, we don't want stuff
 # wrapping around to the integer boundary. Hence max_value is limited.
 def sorted_bounds(disjoint=False,
                   max_value=50,
                   max_len=10,
+                  min_size=0,
+                  max_size=20,
                   remove_duplicates=False):
     if disjoint:
         # Since we accumulate later:
         max_value /= max_len
 
     s = strategies.lists(strategies.integers(min_value=0,
                                              max_value=max_value),
-                         min_size=0, max_size=20)
+                         min_size=min_size, max_size=max_size)
     if disjoint:
         s = s.map(accumulate).map(list)
 
     # Select only cases with even-length lists
     s = s.filter(lambda x: len(x) % 2 == 0)
 
     # Convert to list of 2-tuples
-    s = s.map(lambda x: [tuple(q)
-                         for q in iterutils.chunked(sorted(x), size=2)])
+    if disjoint:
+        s = s.map(lambda x: [tuple(q)
+                            for q in iterutils.chunked(sorted(x), size=2)])
+    else:
+        s = s.map(lambda x: [tuple(sorted(q))
+                            for q in iterutils.chunked(x, size=2)])
+
+    s = s.map(sorted)
+
+    if not disjoint:
+        # Remove cases with not sorted endtime
+        s = s.filter(lambda x: all([a[1] < b[1] for a, b in zip(x[:-1], x[1:])]))
+        # Remove cases without overlapping window
+        s = s.filter(lambda x: all([a[1] > b[0] for a, b in zip(x[:-1], x[1:])]))
 
     # Remove cases with zero-length intervals
     s = s.filter(lambda x: all([a[0] != a[1] for a in x]))
 
     if remove_duplicates:
         # (this will always succeed if disjoint=True)
         s = s.filter(lambda x: x == list(set(x)))
 
     # Sort intervals and result
-    return s.map(sorted)
+    return s
 
 
 ##
 # Fake intervals
 ##
```

### Comparing `strax-1.5.0/strax/utils.py` & `strax-1.5.1/strax/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -539,15 +539,15 @@
                         failures.append(_run_id)
                         continue
                     raise f.exception()
 
                 if throw_away_result:
                     continue
                 result = f.result()
- 
+
                 # Append the run id column
                 if add_run_id_field:
                     ids = np.array([_run_id] * len(result),
                                    dtype=[('run_id', run_id_numpy.dtype)])
                     result = merge_arrs([ids, result])
                 final_result.append(result)
                 run_id_output.append(_run_id)
```

### Comparing `strax-1.5.0/strax.egg-info/PKG-INFO` & `strax-1.5.1/strax.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strax
-Version: 1.5.0
+Version: 1.5.1
 Summary: Streaming analysis for xenon TPCs
 Home-page: https://github.com/AxFoundation/strax
 Author: Jelle Aalbers
 License: UNKNOWN
 Description: # strax
         Streaming analysis for xenon experiments
         
@@ -22,14 +22,35 @@
         
         Strax is an analysis framework for pulse-only digitization data, specialized for live data reduction at speeds of 50-100 MB(raw) / core / sec. For more information, please see the [strax documentation](https://strax.readthedocs.io).
         
         Strax' primary aim is to support noble liquid TPC dark matter searches, such as XENONnT. The XENON-specific algorithms live in the separate package [straxen](https://github.com/XENONnT/straxen). If you want to try out strax, you probably want to start there. This package only contains the core framework and basic algorithms any TPCs would want to use.
         
         
         
+        1.5.1 / 2023-06-22
+        ---------------------
+        * Fix argsort inside numba.jit using kind='mergesort' by @dachengx in https://github.com/AxFoundation/strax/pull/721
+        * Fix urllib3 version to 1.26.15 by @dachengx in https://github.com/AxFoundation/strax/pull/723
+        * Save other fields in the merged peaks to their default value by @dachengx in https://github.com/AxFoundation/strax/pull/722
+        * add a metadata comparison method by @KaraMelih in https://github.com/AxFoundation/strax/pull/706
+        * Accelerate select_runs by @shenyangshi in https://github.com/AxFoundation/strax/pull/727
+        * Stop assigning dependabot to Joran by @JoranAngevaare in https://github.com/AxFoundation/strax/pull/732
+        * Bump urllib3 from 1.26.15 to 2.0.2 in /extra_requirements by @dependabot in https://github.com/AxFoundation/strax/pull/729
+        * Add new general fucntion which computes dt to some interval by @WenzDaniel in https://github.com/AxFoundation/strax/pull/726
+        * Check whether `things` and `containers` are sorted by @dachengx in https://github.com/AxFoundation/strax/pull/725
+        * Set start of further chunk to be the smallest start of dependencies by @dachengx in https://github.com/AxFoundation/strax/pull/715
+        * Fix touching window by @dachengx in https://github.com/AxFoundation/strax/pull/736
+        
+        New Contributors
+        * @KaraMelih made their first contribution in https://github.com/AxFoundation/strax/pull/706
+        * @shenyangshi made their first contribution in https://github.com/AxFoundation/strax/pull/727
+        
+        **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.5.0...v1.5.1
+        
+        
         1.5.0 / 2023-05-02
         ---------------------
         * Fix ipython version by @dachengx in https://github.com/AxFoundation/strax/pull/719
         * Do not change channel when sort_by_time by @dachengx in https://github.com/AxFoundation/strax/pull/718
         * Save hits level information(hits time difference) in peaks by @dachengx in https://github.com/AxFoundation/strax/pull/716
         
         **Full Changelog**: https://github.com/AxFoundation/strax/compare/v1.4.3...v1.5.0
```

### Comparing `strax-1.5.0/strax.egg-info/SOURCES.txt` & `strax-1.5.1/strax.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_child_plugins.py` & `strax-1.5.1/tests/test_child_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_config.py` & `strax-1.5.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_context.py` & `strax-1.5.1/tests/test_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -435,14 +435,21 @@
             def compute(self, **kwargs):
                 res = super().compute(**kwargs)
                 return res
 
         st3 = st.new_context(register=DevelopRecords)
         assert key.lineage != st3.key_for(run_id, 'records').lineage
 
-
     @staticmethod
     def get_dummy_peaks_dependency():
         class DummyDependsOnPeaks(strax.CutPlugin):
             depends_on = 'peaks'
             provides = 'cut_peaks'
         return DummyDependsOnPeaks
+
+    def test_compare_metadata(self):
+        st = self.get_context(True)
+        st.register(Records)
+        st.make(run_id, 'records')
+        old_metadata = st.get_metadata(run_id, 'records')
+        old_metadata.pop('strax_version')
+        st.compare_metadata(run_id, 'records', old_metadata)
```

### Comparing `strax-1.5.0/tests/test_core.py` & `strax-1.5.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_corrections.py` & `strax-1.5.1/tests/test_corrections.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_cut_plugin.py` & `strax-1.5.1/tests/test_cut_plugin.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Initialize. We test both dt time-fields and time time-field
 _dtype_name = 'var'
 _cut_dtype = ('variable 0', _dtype_name)
 full_dt_dtype = [(_cut_dtype, np.float64)] + strax.time_dt_fields
 full_time_dtype = [(_cut_dtype, np.float64)] + strax.time_fields
 
 
-def get_some_array():
+def get_some_array(disjoint=True):
     # Either 0 or 1
     take_dt = np.random.choice(2)
 
     # Stolen from testutils.bounds_to_intervals
     def bounds_to_intervals(bs, dt=1):
         x = np.zeros(len(bs),
                      dtype=full_dt_dtype if take_dt else full_time_dtype)
@@ -24,15 +24,15 @@
             x['length'] = [x[1] - x[0] for x in bs]
             x['dt'] = 1
         else:
             x['endtime'] = x['time'] + ([x[1] - x[0] for x in bs]) * dt
         return x
 
     # Randomly input either of full_dt_dtype or full_time_dtype
-    sorted_intervals = testutils.sorted_bounds().map(bounds_to_intervals)
+    sorted_intervals = testutils.sorted_bounds(disjoint=disjoint).map(bounds_to_intervals)
     return sorted_intervals
 
 
 @given(get_some_array().filter(lambda x: len(x) >= 0),
        strategies.integers(min_value=-10, max_value=10))
 @settings(deadline=None)
 # Examples for readability
```

### Comparing `strax-1.5.0/tests/test_data_reduction.py` & `strax-1.5.1/tests/test_data_reduction.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_fixed_plugin_cache.py` & `strax-1.5.1/tests/test_fixed_plugin_cache.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_general_processing.py` & `strax-1.5.1/tests/test_general_processing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from hypothesis.extra import numpy as hyp_numpy
 import hypothesis.strategies
+
+import unittest
 import strax.testutils
 
 import numpy as np
 import strax
 
 
 @hypothesis.given(strax.testutils.sorted_intervals,
@@ -330,7 +332,110 @@
                            )
     dummy_array['time'] = time
     dummy_array['channel'] = -1
     
     res1 = strax.sort_by_time(dummy_array)
     res2 = np.sort(dummy_array, order='time')
     assert np.all(res1 == res2)
+
+    
+class Test_abs_time_to_prev_next_interval(unittest.TestCase):
+
+    def test_overlapping_raises_error(self):
+        events = np.zeros(2, strax.time_fields)
+        vetos = np.zeros(1, strax.time_fields)
+
+        events['time'] = [5, 10]
+        events['endtime'] = [15, 20]
+        self.assertRaises(AssertionError, strax.abs_time_to_prev_next_interval, events, vetos)
+
+        
+    def test_empty_inputs(self):
+        events = np.zeros(1, strax.time_fields)
+        vetos = np.zeros(0, strax.time_fields)
+
+        events['time'] = 1
+        events['endtime'] = 2
+        res_prev, res_next = strax.abs_time_to_prev_next_interval(events, vetos)
+        assert res_prev == res_next, f'{res_prev}, {res_next}'
+        assert np.all(res_prev == -1)
+
+        events = np.zeros(0, strax.time_fields)
+        vetos = np.zeros(1, strax.time_fields)
+
+        vetos['time'] = 1
+        vetos['endtime'] = 2
+        res_prev, res_next = strax.abs_time_to_prev_next_interval(events, vetos)
+
+        _results_are_empty = (len(res_prev) == 0) and (len(res_next) == 0) 
+        assert _results_are_empty
+
+        events = np.zeros(0, strax.time_fields)
+        vetos = np.zeros(0, strax.time_fields)
+        res_prev, res_next = strax.abs_time_to_prev_next_interval(events, vetos)
+
+    
+    def test_with_dt_fields(self):
+        pass
+    
+    @hypothesis.given(things=
+                      hyp_numpy.arrays(np.int64,
+                    hypothesis.strategies.integers(1, 10),
+                    elements=hypothesis.strategies.integers(0, 1000),
+                    unique=False),
+        intervals=
+                      hyp_numpy.arrays(np.int64,
+                       hypothesis.strategies.integers(1, 100),
+                       elements=hypothesis.strategies.integers(0, 100),
+                       unique=True),
+        )
+    
+    @hypothesis.settings(deadline=None)
+    def test_correct_time_delays(self, things, intervals):
+        _things, _intervals = self._make_correct_things_and_intervals(things, intervals)
+        res_prev, res_next = strax.abs_time_to_prev_next_interval(_things, _intervals)
+        
+        # Compare for each event:
+        for thing_i, e in enumerate(_things):
+            dt_prev = e['time'] - _intervals['endtime'] 
+            dt_prev[dt_prev < 0] = 99999
+            dt_prev = np.min(dt_prev)
+            
+            msg = (f'Found {res_prev[thing_i]}, but expected {dt_prev}'
+            f' for thing number {thing_i} of things: {_things} and intervals: {_intervals}')
+            if res_prev[thing_i] != -1:
+                assert dt_prev == res_prev[thing_i], msg
+            else:
+                assert dt_prev == 99999, msg
+            
+            dt_next = _intervals['time']  - e['endtime'] 
+            dt_next[dt_next < 0] = 99999
+            dt_next = np.min(dt_next)
+            
+            msg = (f'Found {res_next[thing_i]}, but expected {dt_next}'
+            f' for thing number {thing_i} of things: {_things} and intervals: {_intervals}')
+            if res_next[thing_i] != -1:
+                assert dt_next == res_next[thing_i], msg
+            else:
+                assert dt_next == 99999, msg
+                
+    def _make_correct_things_and_intervals(self, things, intervals):
+        _things = np.zeros(len(things), strax.time_fields)
+        _things['time'] = things
+        _things['endtime'] = things + 100
+        
+        _intervals = np.zeros(len(intervals), strax.time_fields)
+        _intervals['time'] = intervals
+        _intervals['endtime'] = intervals + 10
+        
+        _things = strax.sort_by_time(_things)
+        _intervals = strax.sort_by_time(_intervals)
+        
+        # Cut down overlapping _things and remove empty intervals to not 
+        # trigger overlapping error:
+        dt = _things['endtime'][:-1] - _things['time'][1:]
+        dt[dt < 0] = 0
+        _things['endtime'][:-1] = _things['endtime'][:-1] - dt
+        _is_not_empty_interval =( _things['endtime'] - _things['time']) > 0
+        _things = _things[_is_not_empty_interval]
+        
+        return _things, _intervals
```

### Comparing `strax-1.5.0/tests/test_get_zarr.py` & `strax-1.5.1/tests/test_get_zarr.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_helpers.py` & `strax-1.5.1/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_hitlet.py` & `strax-1.5.1/tests/test_hitlet.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_inline_plugin.py` & `strax-1.5.1/tests/test_inline_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_lone_hit_integration.py` & `strax-1.5.1/tests/test_lone_hit_integration.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_loop_plugins.py` & `strax-1.5.1/tests/test_loop_plugins.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_mailbox.py` & `strax-1.5.1/tests/test_mailbox.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_mongo_frontend.py` & `strax-1.5.1/tests/test_mongo_frontend.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_multi_output.py` & `strax-1.5.1/tests/test_multi_output.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_overlap_plugin.py` & `strax-1.5.1/tests/test_overlap_plugin.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_peak_merging.py` & `strax-1.5.1/tests/test_peak_merging.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_peak_processing.py` & `strax-1.5.1/tests/test_peak_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_peak_properties.py` & `strax-1.5.1/tests/test_peak_properties.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_peak_splitting.py` & `strax-1.5.1/tests/test_peak_splitting.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_pulse_processing.py` & `strax-1.5.1/tests/test_pulse_processing.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_saving.py` & `strax-1.5.1/tests/test_saving.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_statistics.py` & `strax-1.5.1/tests/test_statistics.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_storage.py` & `strax-1.5.1/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_superruns.py` & `strax-1.5.1/tests/test_superruns.py`

 * *Files identical despite different names*

### Comparing `strax-1.5.0/tests/test_utils.py` & `strax-1.5.1/tests/test_utils.py`

 * *Files identical despite different names*

