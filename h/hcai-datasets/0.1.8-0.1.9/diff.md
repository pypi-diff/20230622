# Comparing `tmp/hcai-datasets-0.1.8.tar.gz` & `tmp/hcai-datasets-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-datasets-0.1.8.tar", last modified: Thu May 25 09:59:23 2023, max compression
+gzip compressed data, was "hcai-datasets-0.1.9.tar", last modified: Fri Jun  2 12:33:08 2023, max compression
```

## Comparing `hcai-datasets-0.1.8.tar` & `hcai-datasets-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.022498 hcai-datasets-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-05-25 09:59:23.022498 hcai-datasets-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.014498 hcai-datasets-0.1.8/hcai_dataset_utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_dataset_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_dataset_utils/bridge_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_dataset_utils/bridge_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_dataset_utils/dataset_indexed.py
--rw-r--r--   0 runner    (1001) docker     (122)      735 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_dataset_utils/import_validator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_dataset_utils/pytorch_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_dataset_utils/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.014498 hcai-datasets-0.1.8/hcai_datasets/
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.014498 hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.018499 hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/Ignore_Lists/
--rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
--rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/hcai_affectnet.py
--rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.018499 hcai-datasets-0.1.8/hcai_datasets/hcai_audioset/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_audioset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_audioset/hcai_audioset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.018499 hcai-datasets-0.1.8/hcai_datasets/hcai_ckplus/
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_ckplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_ckplus/hcai_ckplus.py
--rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.018499 hcai-datasets-0.1.8/hcai_datasets/hcai_faces/
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_faces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_faces/hcai_faces.py
--rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_faces/hcai_faces_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.018499 hcai-datasets-0.1.8/hcai_datasets/hcai_is2021_ess/
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_is2021_ess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.022498 hcai-datasets-0.1.8/hcai_datasets/hcai_librispeech/
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_librispeech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_librispeech/hcai_librispeech.py
--rw-r--r--   0 runner    (1001) docker     (122)      711 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_librispeech/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.022498 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/
--rw-r--r--   0 runner    (1001) docker     (122)       83 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    22727 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
--rw-r--r--   0 runner    (1001) docker     (122)    25025 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.022498 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12645 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    19552 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      216 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 09:59:23.014498 hcai-datasets-0.1.8/hcai_datasets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-05-25 09:59:22.000000 hcai-datasets-0.1.8/hcai_datasets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-05-25 09:59:22.000000 hcai-datasets-0.1.8/hcai_datasets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 09:59:22.000000 hcai-datasets-0.1.8/hcai_datasets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-05-25 09:59:22.000000 hcai-datasets-0.1.8/hcai_datasets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       33 2023-05-25 09:59:22.000000 hcai-datasets-0.1.8/hcai_datasets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 09:59:23.022498 hcai-datasets-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-05-25 09:59:14.000000 hcai-datasets-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.373614 hcai-datasets-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-06-02 12:33:08.373614 hcai-datasets-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8154 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.361614 hcai-datasets-0.1.9/hcai_dataset_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_dataset_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1094 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_dataset_utils/bridge_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      928 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_dataset_utils/bridge_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_dataset_utils/dataset_indexed.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_dataset_utils/import_validator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_dataset_utils/pytorch_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2770 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_dataset_utils/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.361614 hcai-datasets-0.1.9/hcai_datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.365614 hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.365614 hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/Ignore_Lists/
+-rw-r--r--   0 runner    (1001) docker     (122)  2377285 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json
+-rw-r--r--   0 runner    (1001) docker     (122)     6234 2023-06-02 12:32:52.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/hcai_affectnet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5919 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.369614 hcai-datasets-0.1.9/hcai_datasets/hcai_audioset/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_audioset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2412 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_audioset/hcai_audioset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.369614 hcai-datasets-0.1.9/hcai_datasets/hcai_ckplus/
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_ckplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3017 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_ckplus/hcai_ckplus.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1943 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.369614 hcai-datasets-0.1.9/hcai_datasets/hcai_faces/
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_faces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3303 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_faces/hcai_faces.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2054 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_faces/hcai_faces_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.369614 hcai-datasets-0.1.9/hcai_datasets/hcai_is2021_ess/
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_is2021_ess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.373614 hcai-datasets-0.1.9/hcai_datasets/hcai_librispeech/
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_librispeech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4323 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_librispeech/hcai_librispeech.py
+-rw-r--r--   0 runner    (1001) docker     (122)      711 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_librispeech/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.373614 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22809 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25026 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.373614 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12724 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19619 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/utils/nova_string_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 12:33:08.365614 hcai-datasets-0.1.9/hcai_datasets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9065 2023-06-02 12:33:08.000000 hcai-datasets-0.1.9/hcai_datasets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1770 2023-06-02 12:33:08.000000 hcai-datasets-0.1.9/hcai_datasets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 12:33:08.000000 hcai-datasets-0.1.9/hcai_datasets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-02 12:33:08.000000 hcai-datasets-0.1.9/hcai_datasets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       33 2023-06-02 12:33:08.000000 hcai-datasets-0.1.9/hcai_datasets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 12:33:08.373614 hcai-datasets-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-06-02 12:32:53.000000 hcai-datasets-0.1.9/setup.py
```

### Comparing `hcai-datasets-0.1.8/PKG-INFO` & `hcai-datasets-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets
-Version: 0.1.8
+Version: 0.1.9
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-0.1.8/README.md` & `hcai-datasets-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_dataset_utils/bridge_pytorch.py` & `hcai-datasets-0.1.9/hcai_dataset_utils/bridge_pytorch.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_dataset_utils/bridge_tf.py` & `hcai-datasets-0.1.9/hcai_dataset_utils/bridge_tf.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_dataset_utils/import_validator.py` & `hcai-datasets-0.1.9/hcai_dataset_utils/import_validator.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_dataset_utils/pytorch_dataset_wrapper.py` & `hcai-datasets-0.1.9/hcai_dataset_utils/pytorch_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_dataset_utils/statistics.py` & `hcai-datasets-0.1.9/hcai_dataset_utils/statistics.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/__init__.py` & `hcai-datasets-0.1.9/hcai_datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json` & `hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_duplicates.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json` & `hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/Ignore_Lists/affect_net_ignore_list_wrong_format.json`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/hcai_affectnet.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/hcai_affectnet.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_affectnet/hcai_affectnet_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_audioset/hcai_audioset.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_audioset/hcai_audioset.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_ckplus/hcai_ckplus.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_ckplus/hcai_ckplus.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_ckplus/hcai_ckplus_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_faces/hcai_faces.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_faces/hcai_faces.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_faces/hcai_faces_iterable.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_faces/hcai_faces_iterable.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_is2021_ess/hcai_is2021_ess.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_librispeech/hcai_librispeech.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_librispeech/hcai_librispeech.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_librispeech/preprocessing.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_librispeech/preprocessing.py`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/hcai_nova_dynamic_iterable.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,16 @@
         sessions=None,
         annotator=None,
         schemes=None,
         roles=None,
         data_streams=None,
         start=None,
         end=None,
-        left_context="0s",
-        right_context="0s",
+        left_context=None,
+        right_context=None,
         frame_size=None,
         stride=None,
         add_rest_class=True,
         flatten_samples=False,
         supervised_keys=None,
         lazy_loading=False,
         fake_missing_data=True,
@@ -76,17 +76,19 @@
         self.sessions = sessions
         self.roles = roles
         self.schemes = schemes
         self.data_streams = data_streams
         self.annotator = annotator
 
         # Sliding window parameters for the main stream
-        self.left_context, self.left_context_unit = ndu.parse_time_str(left_context)
-        self.right_context, self.right_context_unit = ndu.parse_time_str(right_context)
+        self.left_context, self.left_context_unit = ndu.parse_time_str(left_context if left_context else '0')
+        self.right_context, self.right_context_unit = ndu.parse_time_str(right_context if right_context else '0')
         self.frame_size, self.frame_size_unit = ndu.parse_time_str(frame_size)
+
+        # Framesize 0 or None indicates that the whole session should be returned as one sample
         if self.frame_size == 0:
             print(
                 "WARNING: Frame size 0 is invalid. Returning whole session as sample."
             )
             self.frame_size = None
         self.stride, self.stride_unit = ndu.parse_time_str(stride) if stride else self.frame_size, self.frame_size_unit
 
@@ -377,30 +379,28 @@
                     raise fnf
 
     def _build_sample_dict(self, labels_for_frame, data_for_frame):
         sample_dict = {}
 
         garbage_detected = False
         for label_id, label_value in labels_for_frame:
-            # check for nan
+            # if value is not list type check for nan
             if (
                     type(label_value) != list
                     and type(label_value) != str
                     and type(label_value) != np.ndarray
             ):
-                try:
-                    if label_value != label_value:
-                        garbage_detected = True
-                except:
-                    breakpoint()
+                if label_value != label_value:
+                    garbage_detected = True
+
             sample_dict.update({label_id: label_value})
 
         # If at least one label is a garbage label we skip this iteration
         if garbage_detected:
-            return sample_dict
+            return None
 
         for d in data_for_frame:
             sample_dict.update(d)
 
         # if self.flatten_samples:
         #
         #     # grouping labels and data according to roles
```

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/nova_db_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,15 +207,15 @@
         mongo_sessions,
         mongo_annotators,
         mongo_roles,
         database,
         collection,
     ):
         """
-        Fetches all annotationobjects that match the specified criteria from the nova database
+        Fetches all annotation objects that match the specified criteria from the nova database
         Args:
           mongo_schemes:
           mongo_sessions:
           mongo_annotators:
           mongo_roles:
           database:
           collection:
```

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/utils/nova_anno_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 import pandas as pd
+import sys
 from numba import njit
 from abc import ABC, abstractmethod
 from hcai_datasets.hcai_nova_dynamic.utils.nova_string_utils import merge_role_key
 from nova_utils.db_utils import nova_types as nt
 
 # TODO: Currently we do not take the rest class into account when calculating the label for the frame. Maybe we should do this
 @njit
@@ -302,15 +303,17 @@
     def postprocess(self):
         pass
 
 
 class ContinuousAnnotation(Annotation):
 
     # Class ids and string names as provided from NOVA-DB and required by SSI
-    NOVA_GARBAGE_LABEL_ID = np.NAN
+    NOVA_GARBAGE_LABEL_VALUE = np.NAN
+
+    MISSING_DATA_LABEL_VALUE = sys.float_info.min
 
     def __init__(self, sr=0, min_val=0, max_val=0, **kwargs):
         super().__init__(**kwargs)
         self.type = nt.AnnoTypes.CONTINUOUS
         self.sr = sr
         self.min_val = min_val
         self.max_val = max_val
@@ -329,23 +332,23 @@
         e = int(end * self.sr / 1000)
 
         if len(self.data) >= e:
             frame = self.data[s:e]
             frame_data = frame[:, 0]
             frame_conf = frame[:, 1]
         else:
-            return self.NOVA_GARBAGE_LABEL_ID
+            return self.MISSING_DATA_LABEL_VALUE
 
         # TODO: Return timeseries instead of average
         conf = sum(frame_conf) / max(len(frame_conf), 1)
         label = sum(frame_data) / max(len(frame_data), 1)
 
         # If frame evaluates to garbage label discard sample
-        if _is_garbage(label, self.NOVA_GARBAGE_LABEL_ID):
-            return Annotation.GARBAGE_LABEL_ID
+        if _is_garbage(label, self.NOVA_GARBAGE_LABEL_VALUE):
+            return Annotation.NOVA_GARBAGE_LABEL_VALUE
         else:
             return label
 
     def postprocess(self):
         pass
```

### Comparing `hcai-datasets-0.1.8/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py` & `hcai-datasets-0.1.9/hcai_datasets/hcai_nova_dynamic/utils/nova_data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,18 +190,19 @@
         """
 
         Args:
             **kwargs ():
         """
         # Overwrite default
         if kwargs.get("sample_data_shape") is None:
-            self.sample_data_shape = (1,)
+            sample_data_shape = (1,)
+            kwargs.update({"sample_data_shape": sample_data_shape})
         if kwargs.get("np_data_type") is None:
             kwargs.update({"np_data_type": np.float32})
-        kwargs.update({"data_type": nt.DataTypes.AUDIO})
+            kwargs.update({"data_type": nt.DataTypes.AUDIO})
 
         super().__init__(**kwargs)
 
     def _get_info_hook(self):
         return merge_role_key(self.role, self.name), {
             "shape": self.sample_data_shape,
             "dtype": np.float32,
```

### Comparing `hcai-datasets-0.1.8/hcai_datasets.egg-info/PKG-INFO` & `hcai-datasets-0.1.9/hcai_datasets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-datasets
-Version: 0.1.8
+Version: 0.1.9
 Summary: !Alpha Version! - This repository contains the backend server for the nova annotation ui (https://github.com/hcmlab/nova)
 Home-page: https://github.com/hcmlab/nova-server
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-datasets-0.1.8/hcai_datasets.egg-info/SOURCES.txt` & `hcai-datasets-0.1.9/hcai_datasets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-datasets-0.1.8/setup.py` & `hcai-datasets-0.1.9/setup.py`

 * *Files identical despite different names*

