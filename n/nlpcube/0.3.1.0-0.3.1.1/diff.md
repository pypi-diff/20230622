# Comparing `tmp/nlpcube-0.3.1.0.tar.gz` & `tmp/nlpcube-0.3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpcube-0.3.1.0.tar", last modified: Sun Aug 15 06:20:00 2021, max compression
+gzip compressed data, was "nlpcube-0.3.1.1.tar", last modified: Mon Oct 18 19:54:15 2021, max compression
```

## Comparing `nlpcube-0.3.1.0.tar` & `nlpcube-0.3.1.1.tar`

### file list

```diff
@@ -1,88 +1,86 @@
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.243075 nlpcube-0.3.1.0/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    11421 2021-08-15 06:20:00.243075 nlpcube-0.3.1.0/PKG-INFO
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     9632 2021-08-15 06:13:36.000000 nlpcube-0.3.1.0/README.md
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.235075 nlpcube-0.3.1.0/_cube/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    12727 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/api.py
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.239075 nlpcube-0.3.1.0/_cube/generic_networks/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     6045 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/character_embeddings.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    17323 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/crf.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    23623 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/lemmatizers.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    13178 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/ner.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    18284 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/parsers.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    12376 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/taggers.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    13015 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/token_expanders.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    63083 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/tokenizers.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    10392 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/translators.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     1905 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/utils.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     3419 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/generic_networks/wrappers.py
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.239075 nlpcube-0.3.1.0/_cube/graph/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/graph/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2931 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/graph/decoders.py
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.239075 nlpcube-0.3.1.0/_cube/io_utils/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    10669 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/config.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     5983 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/conll.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2682 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/cupt.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     6700 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/embeddings.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    10390 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/encodings.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    34717 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/model_store.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2768 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/mt.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    60731 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/io_utils/trainers.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    34616 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/main.py
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.239075 nlpcube-0.3.1.0/_cube/misc/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/misc/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     1302 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/misc/conll17_ud_eval_wrapper.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    27549 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/misc/conll18_ud_eval.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     1234 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/misc/conll18_ud_eval_wrapper.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2691 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/misc/misc.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     4246 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/_cube/webserver.py
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.239075 nlpcube-0.3.1.0/cube/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)      359 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     9320 2021-08-13 19:09:00.000000 nlpcube-0.3.1.0/cube/api.py
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.239075 nlpcube-0.3.1.0/cube/io_utils/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/io_utils/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2645 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/io_utils/components.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     9975 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/io_utils/config.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    10195 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/io_utils/encodings.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2229 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/io_utils/misc.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    12588 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/io_utils/modelstore.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     6079 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/io_utils/objects.py
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.243075 nlpcube-0.3.1.0/cube/networks/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/networks/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    14323 2021-08-11 15:55:55.000000 nlpcube-0.3.1.0/cube/networks/compound.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    13657 2021-08-11 15:55:45.000000 nlpcube-0.3.1.0/cube/networks/lemmatizer.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     7710 2021-08-12 18:05:34.000000 nlpcube-0.3.1.0/cube/networks/lm.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    23357 2021-08-15 05:39:59.000000 nlpcube-0.3.1.0/cube/networks/modules.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    23554 2021-08-11 15:55:29.000000 nlpcube-0.3.1.0/cube/networks/parser.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    18905 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/networks/tagger.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    16895 2021-08-15 06:07:17.000000 nlpcube-0.3.1.0/cube/networks/tokenizer.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    22963 2021-08-11 16:01:45.000000 nlpcube-0.3.1.0/cube/networks/utils.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    24125 2021-08-14 06:52:00.000000 nlpcube-0.3.1.0/cube/networks/utils_tokenizer.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    13282 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/trainer.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)       17 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/version.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     4246 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/cube/webserver.py
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.243075 nlpcube-0.3.1.0/nlpcube.egg-info/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    11421 2021-08-15 06:20:00.000000 nlpcube-0.3.1.0/nlpcube.egg-info/PKG-INFO
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2004 2021-08-15 06:20:00.000000 nlpcube-0.3.1.0/nlpcube.egg-info/SOURCES.txt
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        1 2021-08-15 06:20:00.000000 nlpcube-0.3.1.0/nlpcube.egg-info/dependency_links.txt
--rw-rw-r--   0 tibi      (1000) tibi      (1000)      236 2021-08-15 06:20:00.000000 nlpcube-0.3.1.0/nlpcube.egg-info/requires.txt
--rw-rw-r--   0 tibi      (1000) tibi      (1000)       19 2021-08-15 06:20:00.000000 nlpcube-0.3.1.0/nlpcube.egg-info/top_level.txt
-drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-08-15 06:20:00.243075 nlpcube-0.3.1.0/scripts/
--rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2020-04-29 20:01:27.000000 nlpcube-0.3.1.0/scripts/__init__.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     5346 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/scripts/_del_pack_models_for_upload.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2590 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/download_data.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2002 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/download_model.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     2621 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/export_model.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     7067 2021-08-09 13:42:53.000000 nlpcube-0.3.1.0/scripts/generate_catalog_from_models.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)    12246 2021-02-22 07:11:02.000000 nlpcube-0.3.1.0/scripts/generate_training_yamls.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)      921 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/import_model.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     7631 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/list2train.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     5389 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/package_ud_models.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     1649 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/reshape_unimorf.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     1784 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/result_mdtable_generator.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     8996 2021-01-31 19:12:59.000000 nlpcube-0.3.1.0/scripts/test_all_models.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     1715 2020-04-29 20:01:27.000000 nlpcube-0.3.1.0/scripts/utils.py
--rw-rw-r--   0 tibi      (1000) tibi      (1000)       38 2021-08-15 06:20:00.243075 nlpcube-0.3.1.0/setup.cfg
--rw-rw-r--   0 tibi      (1000) tibi      (1000)     1067 2021-08-15 06:19:50.000000 nlpcube-0.3.1.0/setup.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.356156 nlpcube-0.3.1.1/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    11734 2021-10-18 19:54:15.356156 nlpcube-0.3.1.1/PKG-INFO
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     9946 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/README.md
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.136155 nlpcube-0.3.1.1/_cube/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    12727 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/api.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.168155 nlpcube-0.3.1.1/_cube/generic_networks/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     6045 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/character_embeddings.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    17323 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/crf.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    23623 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/lemmatizers.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    13178 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/ner.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    18284 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/parsers.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    12376 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/taggers.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    13015 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/token_expanders.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    63115 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/tokenizers.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    10392 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/translators.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     1905 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/utils.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     3419 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/generic_networks/wrappers.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.168155 nlpcube-0.3.1.1/_cube/graph/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/graph/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     2931 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/graph/decoders.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.208155 nlpcube-0.3.1.1/_cube/io_utils/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    10669 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/config.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     4093 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/conll.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     2682 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/cupt.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     6700 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/embeddings.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    10390 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/encodings.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    34717 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/model_store.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     2768 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/mt.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    60731 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/io_utils/trainers.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    34616 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/main.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.232156 nlpcube-0.3.1.1/_cube/misc/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/misc/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     1302 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/misc/conll17_ud_eval_wrapper.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    27549 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/misc/conll18_ud_eval.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     1234 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/misc/conll18_ud_eval_wrapper.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     2691 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/misc/misc.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     4246 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/_cube/webserver.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.256156 nlpcube-0.3.1.1/cube/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)      359 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     9460 2021-10-18 19:53:40.000000 nlpcube-0.3.1.1/cube/api.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.296156 nlpcube-0.3.1.1/cube/io_utils/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-08-08 07:13:45.000000 nlpcube-0.3.1.1/cube/io_utils/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     2645 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/io_utils/components.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     9975 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/io_utils/config.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    10195 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/io_utils/encodings.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     2229 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/io_utils/misc.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    12588 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/io_utils/modelstore.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     6079 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/io_utils/objects.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.320156 nlpcube-0.3.1.1/cube/networks/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)        0 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    14323 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/compound.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    13657 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/lemmatizer.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     7710 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/lm.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    23357 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/modules.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    23570 2021-10-13 20:17:01.000000 nlpcube-0.3.1.1/cube/networks/parser.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    18905 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/tagger.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    16895 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/tokenizer.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    22963 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/utils.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    24125 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/networks/utils_tokenizer.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    13282 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/trainer.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)       17 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/cube/version.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     4246 2021-08-08 07:13:45.000000 nlpcube-0.3.1.1/cube/webserver.py
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.324156 nlpcube-0.3.1.1/nlpcube.egg-info/
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    11734 2021-10-18 19:54:14.000000 nlpcube-0.3.1.1/nlpcube.egg-info/PKG-INFO
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     1953 2021-10-18 19:54:15.000000 nlpcube-0.3.1.1/nlpcube.egg-info/SOURCES.txt
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)        1 2021-10-18 19:54:14.000000 nlpcube-0.3.1.1/nlpcube.egg-info/dependency_links.txt
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)      236 2021-10-18 19:54:14.000000 nlpcube-0.3.1.1/nlpcube.egg-info/requires.txt
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)       19 2021-10-18 19:54:14.000000 nlpcube-0.3.1.1/nlpcube.egg-info/top_level.txt
+drwxrwxr-x   0 tibi      (1000) tibi      (1000)        0 2021-10-18 19:54:15.348156 nlpcube-0.3.1.1/scripts/
+-rw-r--r--   0 tibi      (1000) tibi      (1000)        0 2018-03-23 20:16:04.000000 nlpcube-0.3.1.1/scripts/__init__.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     5346 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/scripts/_del_pack_models_for_upload.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     2621 2021-08-08 07:13:45.000000 nlpcube-0.3.1.1/scripts/export_model.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     7067 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/scripts/generate_catalog_from_models.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)    12246 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/scripts/generate_training_yamls.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)      921 2021-08-08 07:13:45.000000 nlpcube-0.3.1.1/scripts/import_model.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     7631 2021-10-12 09:55:00.000000 nlpcube-0.3.1.1/scripts/list2train.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     5389 2021-08-08 07:13:45.000000 nlpcube-0.3.1.1/scripts/package_ud_models.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     1649 2021-08-08 07:13:45.000000 nlpcube-0.3.1.1/scripts/reshape_unimorf.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     1784 2021-08-08 07:13:45.000000 nlpcube-0.3.1.1/scripts/result_mdtable_generator.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     8996 2021-08-08 07:13:45.000000 nlpcube-0.3.1.1/scripts/test_all_models.py
+-rw-r--r--   0 tibi      (1000) tibi      (1000)     1715 2018-03-23 20:16:04.000000 nlpcube-0.3.1.1/scripts/utils.py
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)       38 2021-10-18 19:54:15.356156 nlpcube-0.3.1.1/setup.cfg
+-rw-rw-r--   0 tibi      (1000) tibi      (1000)     1066 2021-10-18 19:53:53.000000 nlpcube-0.3.1.1/setup.py
```

### Comparing `nlpcube-0.3.1.0/PKG-INFO` & `nlpcube-0.3.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nlpcube
-Version: 0.3.1.0
-Summary: Natural Language Procecssing Toolkit with support for tokenization, sentence splitting, lemmatization, tagging and parsing for more than 60 languages
+Version: 0.3.1.1
+Summary: Natural Language Processing Toolkit with support for tokenization, sentence splitting, lemmatization, tagging and parsing for more than 60 languages
 Home-page: https://github.com/adobe/NLP-Cube
 Author: Multiple authors
 Author-email: tiberiu44@gmail.com
 License: UNKNOWN
-Description: ![Monthly](https://img.shields.io/pypi/dm/nlpcube.svg) ![Weekly](https://img.shields.io/pypi/dw/nlpcube.svg) ![daily](https://img.shields.io/pypi/dd/nlpcube.svg)
-        ![Version](https://badge.fury.io/py/nlpcube.svg) [![Python 3](https://img.shields.io/badge/python-3-blue.svg)](https://www.python.org/downloads/release/python-360/) 
+Description: [![Downloads](https://pepy.tech/badge/nlpcube)](https://pepy.tech/project/nlpcube) [![Downloads](https://pepy.tech/badge/nlpcube/month)](https://pepy.tech/project/nlpcube/month) ![Weekly](https://img.shields.io/pypi/dw/nlpcube.svg) ![daily](https://img.shields.io/pypi/dd/nlpcube.svg)
+        ![Version](https://badge.fury.io/py/nlpcube.svg) [![Python 3](https://img.shields.io/badge/python-3-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub stars](https://img.shields.io/github/stars/adobe/NLP-Cube.svg?style=social&label=Star&maxAge=2592000)](https://github.com/adobe/NLP-Cube/stargazers/)
         
         ## News
         **[05 August 2021]** - We are releasing version 3.0 of NLPCube and models and introducing [FLAVOURS](#flavours). This is a major update, but we did our best to maintain the same API, so previous implementation will not crash. The supported language list is smaller, but you can open an issue for unsupported languages, and we will do our best to add them. Other options include fixing the pip package version 1.0.8 ```pip install nlpcube==0.1.0.8```. 
         
-        **[15 April 2019]** - We are releasing version 1.1 models - check all [supported languages below](#languages). Both models 1.0 and 1.1 are trained on the same UD2.2 corpus; however, models 1.1 do not use vector embeddings, thus reducing the time and disk space required to download them. Some languages actually have a slightly increased accuracy, some a bit decreased. By default, NLP Cube will use the latest (at this time) 1.1 models.
+        **[15 April 2019]** - We are releasing version 1.1 models - check all [supported languages below](#languages). Both 1.0 and 1.1 models are trained on the same [UD2.2 corpus](http://hdl.handle.net/11234/1-2837); however, models 1.1 do not use vector embeddings, thus reducing disk space and time required to use them. Some languages actually have a slightly increased accuracy, some a bit decreased. By default, NLP Cube will use the latest (at this time) 1.1 models.
         
-        To use the older 1.0 models just specify this version in the ``load`` call: ``cube.load("en",1.0)`` (``en`` for English, or any other language code). This will download (if not already downloaded) and use _this_ specific model version. Same goes for any language/version you want to use.
+        To use the older 1.0 models just specify this version in the ``load`` call: ``cube.load("en", 1.0)`` (``en`` for English, or any other language code). This will download (if not already downloaded) and use _this_ specific model version. Same goes for any language/version you want to use.
         
-        If you already have NLP Cube installed and **want to use the newer 1.1 models**, type either ``cube.load("en",1.1)`` or ``cube.load("en","latest")`` to auto-download them. After this, calling ``cube.load("en")`` without version number will automatically use the latest ones from your disk.
+        If you already have NLP Cube installed and **want to use the newer 1.1 models**, type either ``cube.load("en", 1.1)`` or ``cube.load("en", "latest")`` to auto-download them. After this, calling ``cube.load("en")`` without version number will automatically use the latest ones from your disk.
         
         <hr>
         
         # NLP-Cube
         
         NLP-Cube is an opensource Natural Language Processing Framework with support for languages which are included in the [UD Treebanks](http://universaldependencies.org/) (list of all available languages below). Use NLP-Cube if you need:
         * Sentence segmentation
```

### Comparing `nlpcube-0.3.1.0/README.md` & `nlpcube-0.3.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-![Monthly](https://img.shields.io/pypi/dm/nlpcube.svg) ![Weekly](https://img.shields.io/pypi/dw/nlpcube.svg) ![daily](https://img.shields.io/pypi/dd/nlpcube.svg)
-![Version](https://badge.fury.io/py/nlpcube.svg) [![Python 3](https://img.shields.io/badge/python-3-blue.svg)](https://www.python.org/downloads/release/python-360/) 
+[![Downloads](https://pepy.tech/badge/nlpcube)](https://pepy.tech/project/nlpcube) [![Downloads](https://pepy.tech/badge/nlpcube/month)](https://pepy.tech/project/nlpcube/month) ![Weekly](https://img.shields.io/pypi/dw/nlpcube.svg) ![daily](https://img.shields.io/pypi/dd/nlpcube.svg)
+![Version](https://badge.fury.io/py/nlpcube.svg) [![Python 3](https://img.shields.io/badge/python-3-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub stars](https://img.shields.io/github/stars/adobe/NLP-Cube.svg?style=social&label=Star&maxAge=2592000)](https://github.com/adobe/NLP-Cube/stargazers/)
 
 ## News
 **[05 August 2021]** - We are releasing version 3.0 of NLPCube and models and introducing [FLAVOURS](#flavours). This is a major update, but we did our best to maintain the same API, so previous implementation will not crash. The supported language list is smaller, but you can open an issue for unsupported languages, and we will do our best to add them. Other options include fixing the pip package version 1.0.8 ```pip install nlpcube==0.1.0.8```. 
 
-**[15 April 2019]** - We are releasing version 1.1 models - check all [supported languages below](#languages). Both models 1.0 and 1.1 are trained on the same UD2.2 corpus; however, models 1.1 do not use vector embeddings, thus reducing the time and disk space required to download them. Some languages actually have a slightly increased accuracy, some a bit decreased. By default, NLP Cube will use the latest (at this time) 1.1 models.
+**[15 April 2019]** - We are releasing version 1.1 models - check all [supported languages below](#languages). Both 1.0 and 1.1 models are trained on the same [UD2.2 corpus](http://hdl.handle.net/11234/1-2837); however, models 1.1 do not use vector embeddings, thus reducing disk space and time required to use them. Some languages actually have a slightly increased accuracy, some a bit decreased. By default, NLP Cube will use the latest (at this time) 1.1 models.
 
-To use the older 1.0 models just specify this version in the ``load`` call: ``cube.load("en",1.0)`` (``en`` for English, or any other language code). This will download (if not already downloaded) and use _this_ specific model version. Same goes for any language/version you want to use.
+To use the older 1.0 models just specify this version in the ``load`` call: ``cube.load("en", 1.0)`` (``en`` for English, or any other language code). This will download (if not already downloaded) and use _this_ specific model version. Same goes for any language/version you want to use.
 
-If you already have NLP Cube installed and **want to use the newer 1.1 models**, type either ``cube.load("en",1.1)`` or ``cube.load("en","latest")`` to auto-download them. After this, calling ``cube.load("en")`` without version number will automatically use the latest ones from your disk.
+If you already have NLP Cube installed and **want to use the newer 1.1 models**, type either ``cube.load("en", 1.1)`` or ``cube.load("en", "latest")`` to auto-download them. After this, calling ``cube.load("en")`` without version number will automatically use the latest ones from your disk.
 
 <hr>
 
 # NLP-Cube
 
 NLP-Cube is an opensource Natural Language Processing Framework with support for languages which are included in the [UD Treebanks](http://universaldependencies.org/) (list of all available languages below). Use NLP-Cube if you need:
 * Sentence segmentation
```

### Comparing `nlpcube-0.3.1.0/_cube/api.py` & `nlpcube-0.3.1.1/_cube/api.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/character_embeddings.py` & `nlpcube-0.3.1.1/_cube/generic_networks/character_embeddings.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/crf.py` & `nlpcube-0.3.1.1/_cube/generic_networks/crf.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/lemmatizers.py` & `nlpcube-0.3.1.1/_cube/generic_networks/lemmatizers.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/ner.py` & `nlpcube-0.3.1.1/_cube/generic_networks/ner.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/parsers.py` & `nlpcube-0.3.1.1/_cube/generic_networks/parsers.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/taggers.py` & `nlpcube-0.3.1.1/_cube/generic_networks/taggers.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/token_expanders.py` & `nlpcube-0.3.1.1/_cube/generic_networks/token_expanders.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/tokenizers.py` & `nlpcube-0.3.1.1/_cube/generic_networks/tokenizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -859,15 +859,16 @@
                 if np.argmax(y.npvalue()) == 1:
                     space_after_end_of_sentence = False
                     if index < len(
                             input_string) - 1:  # compare with input_string not with current_string for whitespace after current sentence
                         if input_string[index + 1] in string.whitespace:
                             space_after_end_of_sentence = True
                     seq = self._get_tokens(w.strip(), space_after_end_of_sentence=space_after_end_of_sentence)
-                    sequences.append(seq)
+                    if seq:
+                        sequences.append(seq)
                     w = ""
                     last_ss_break = index
                 last_checked_index = index
 
             if last_ss_break == -1:  # no sentence break applied
                 last_ss_break = last_checked_index
             else:
```

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/translators.py` & `nlpcube-0.3.1.1/_cube/generic_networks/translators.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/utils.py` & `nlpcube-0.3.1.1/_cube/generic_networks/utils.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/generic_networks/wrappers.py` & `nlpcube-0.3.1.1/_cube/generic_networks/wrappers.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/graph/decoders.py` & `nlpcube-0.3.1.1/_cube/graph/decoders.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/io_utils/config.py` & `nlpcube-0.3.1.1/_cube/io_utils/config.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/io_utils/cupt.py` & `nlpcube-0.3.1.1/_cube/io_utils/cupt.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/io_utils/embeddings.py` & `nlpcube-0.3.1.1/_cube/io_utils/embeddings.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/io_utils/encodings.py` & `nlpcube-0.3.1.1/_cube/io_utils/encodings.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/io_utils/model_store.py` & `nlpcube-0.3.1.1/_cube/io_utils/model_store.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/io_utils/mt.py` & `nlpcube-0.3.1.1/_cube/io_utils/mt.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/io_utils/trainers.py` & `nlpcube-0.3.1.1/_cube/io_utils/trainers.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/main.py` & `nlpcube-0.3.1.1/_cube/main.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/misc/conll17_ud_eval_wrapper.py` & `nlpcube-0.3.1.1/_cube/misc/conll17_ud_eval_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/misc/conll18_ud_eval.py` & `nlpcube-0.3.1.1/_cube/misc/conll18_ud_eval.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/misc/conll18_ud_eval_wrapper.py` & `nlpcube-0.3.1.1/_cube/misc/conll18_ud_eval_wrapper.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/misc/misc.py` & `nlpcube-0.3.1.1/_cube/misc/misc.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/_cube/webserver.py` & `nlpcube-0.3.1.1/_cube/webserver.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/api.py` & `nlpcube-0.3.1.1/cube/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,14 +122,18 @@
                 doc = self._cwe.process(doc, self._lemmatizer_collate, num_workers=0)
         else:
             doc = text
 
         self._lm_helper.apply(doc)
         self._parser.process(doc, self._parser_collate, num_workers=0)
         self._lemmatizer.process(doc, self._lemmatizer_collate, num_workers=0)
+        for seq in doc.sentences:
+            for w in seq.words:
+                if w.upos =='PUNCT':
+                    w.lemma = w.word
         return doc
 
 
 def _download_file(url: str, filename: str, description=None):
     r = requests.get(url, stream=True)
     if r.status_code != 200:
         raise Exception(f"Error getting {url}, received status_code {r.status_code}")
```

### Comparing `nlpcube-0.3.1.0/cube/io_utils/components.py` & `nlpcube-0.3.1.1/cube/io_utils/components.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/io_utils/config.py` & `nlpcube-0.3.1.1/cube/io_utils/config.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/io_utils/encodings.py` & `nlpcube-0.3.1.1/cube/io_utils/encodings.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/io_utils/misc.py` & `nlpcube-0.3.1.1/cube/io_utils/misc.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/io_utils/modelstore.py` & `nlpcube-0.3.1.1/cube/io_utils/modelstore.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/io_utils/objects.py` & `nlpcube-0.3.1.1/cube/io_utils/objects.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/networks/compound.py` & `nlpcube-0.3.1.1/cube/networks/compound.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/networks/lemmatizer.py` & `nlpcube-0.3.1.1/cube/networks/lemmatizer.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/networks/lm.py` & `nlpcube-0.3.1.1/cube/networks/lm.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/networks/modules.py` & `nlpcube-0.3.1.1/cube/networks/modules.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/networks/parser.py` & `nlpcube-0.3.1.1/cube/networks/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,17 +133,17 @@
 
         char_emb = unpack(char_emb_packed, sl, x_sents.shape[1], device=self._get_device())
         word_emb_ext = None
 
         for ii in range(len(x_word_emb_packed)):
             we = unpack(x_word_emb_packed[ii], sl, x_sents.shape[1], self._get_device())
             if word_emb_ext is None:
-                word_emb_ext = self._ext_proj[ii](we)
+                word_emb_ext = self._ext_proj[ii](we.float())
             else:
-                word_emb_ext = word_emb_ext + self._ext_proj[ii](we)
+                word_emb_ext = word_emb_ext + self._ext_proj[ii](we.float())
 
         word_emb_ext = word_emb_ext / len(x_word_emb_packed)
         word_emb_ext = torch.tanh(word_emb_ext)
 
         lang_emb = self._lang_emb(x_lang_sent)
         lang_emb = lang_emb.unsqueeze(1).repeat(1, char_emb.shape[1] + 1, 1)
```

### Comparing `nlpcube-0.3.1.0/cube/networks/tagger.py` & `nlpcube-0.3.1.1/cube/networks/tagger.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/networks/tokenizer.py` & `nlpcube-0.3.1.1/cube/networks/tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/networks/utils.py` & `nlpcube-0.3.1.1/cube/networks/utils.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/networks/utils_tokenizer.py` & `nlpcube-0.3.1.1/cube/networks/utils_tokenizer.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/trainer.py` & `nlpcube-0.3.1.1/cube/trainer.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/cube/webserver.py` & `nlpcube-0.3.1.1/cube/webserver.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/nlpcube.egg-info/PKG-INFO` & `nlpcube-0.3.1.1/nlpcube.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: nlpcube
-Version: 0.3.1.0
-Summary: Natural Language Procecssing Toolkit with support for tokenization, sentence splitting, lemmatization, tagging and parsing for more than 60 languages
+Version: 0.3.1.1
+Summary: Natural Language Processing Toolkit with support for tokenization, sentence splitting, lemmatization, tagging and parsing for more than 60 languages
 Home-page: https://github.com/adobe/NLP-Cube
 Author: Multiple authors
 Author-email: tiberiu44@gmail.com
 License: UNKNOWN
-Description: ![Monthly](https://img.shields.io/pypi/dm/nlpcube.svg) ![Weekly](https://img.shields.io/pypi/dw/nlpcube.svg) ![daily](https://img.shields.io/pypi/dd/nlpcube.svg)
-        ![Version](https://badge.fury.io/py/nlpcube.svg) [![Python 3](https://img.shields.io/badge/python-3-blue.svg)](https://www.python.org/downloads/release/python-360/) 
+Description: [![Downloads](https://pepy.tech/badge/nlpcube)](https://pepy.tech/project/nlpcube) [![Downloads](https://pepy.tech/badge/nlpcube/month)](https://pepy.tech/project/nlpcube/month) ![Weekly](https://img.shields.io/pypi/dw/nlpcube.svg) ![daily](https://img.shields.io/pypi/dd/nlpcube.svg)
+        ![Version](https://badge.fury.io/py/nlpcube.svg) [![Python 3](https://img.shields.io/badge/python-3-blue.svg)](https://www.python.org/downloads/release/python-360/) [![GitHub stars](https://img.shields.io/github/stars/adobe/NLP-Cube.svg?style=social&label=Star&maxAge=2592000)](https://github.com/adobe/NLP-Cube/stargazers/)
         
         ## News
         **[05 August 2021]** - We are releasing version 3.0 of NLPCube and models and introducing [FLAVOURS](#flavours). This is a major update, but we did our best to maintain the same API, so previous implementation will not crash. The supported language list is smaller, but you can open an issue for unsupported languages, and we will do our best to add them. Other options include fixing the pip package version 1.0.8 ```pip install nlpcube==0.1.0.8```. 
         
-        **[15 April 2019]** - We are releasing version 1.1 models - check all [supported languages below](#languages). Both models 1.0 and 1.1 are trained on the same UD2.2 corpus; however, models 1.1 do not use vector embeddings, thus reducing the time and disk space required to download them. Some languages actually have a slightly increased accuracy, some a bit decreased. By default, NLP Cube will use the latest (at this time) 1.1 models.
+        **[15 April 2019]** - We are releasing version 1.1 models - check all [supported languages below](#languages). Both 1.0 and 1.1 models are trained on the same [UD2.2 corpus](http://hdl.handle.net/11234/1-2837); however, models 1.1 do not use vector embeddings, thus reducing disk space and time required to use them. Some languages actually have a slightly increased accuracy, some a bit decreased. By default, NLP Cube will use the latest (at this time) 1.1 models.
         
-        To use the older 1.0 models just specify this version in the ``load`` call: ``cube.load("en",1.0)`` (``en`` for English, or any other language code). This will download (if not already downloaded) and use _this_ specific model version. Same goes for any language/version you want to use.
+        To use the older 1.0 models just specify this version in the ``load`` call: ``cube.load("en", 1.0)`` (``en`` for English, or any other language code). This will download (if not already downloaded) and use _this_ specific model version. Same goes for any language/version you want to use.
         
-        If you already have NLP Cube installed and **want to use the newer 1.1 models**, type either ``cube.load("en",1.1)`` or ``cube.load("en","latest")`` to auto-download them. After this, calling ``cube.load("en")`` without version number will automatically use the latest ones from your disk.
+        If you already have NLP Cube installed and **want to use the newer 1.1 models**, type either ``cube.load("en", 1.1)`` or ``cube.load("en", "latest")`` to auto-download them. After this, calling ``cube.load("en")`` without version number will automatically use the latest ones from your disk.
         
         <hr>
         
         # NLP-Cube
         
         NLP-Cube is an opensource Natural Language Processing Framework with support for languages which are included in the [UD Treebanks](http://universaldependencies.org/) (list of all available languages below). Use NLP-Cube if you need:
         * Sentence segmentation
```

### Comparing `nlpcube-0.3.1.0/nlpcube.egg-info/SOURCES.txt` & `nlpcube-0.3.1.1/nlpcube.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,14 @@
 nlpcube.egg-info/PKG-INFO
 nlpcube.egg-info/SOURCES.txt
 nlpcube.egg-info/dependency_links.txt
 nlpcube.egg-info/requires.txt
 nlpcube.egg-info/top_level.txt
 scripts/__init__.py
 scripts/_del_pack_models_for_upload.py
-scripts/download_data.py
-scripts/download_model.py
 scripts/export_model.py
 scripts/generate_catalog_from_models.py
 scripts/generate_training_yamls.py
 scripts/import_model.py
 scripts/list2train.py
 scripts/package_ud_models.py
 scripts/reshape_unimorf.py
```

### Comparing `nlpcube-0.3.1.0/scripts/_del_pack_models_for_upload.py` & `nlpcube-0.3.1.1/scripts/_del_pack_models_for_upload.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/export_model.py` & `nlpcube-0.3.1.1/scripts/export_model.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/generate_catalog_from_models.py` & `nlpcube-0.3.1.1/scripts/generate_catalog_from_models.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/generate_training_yamls.py` & `nlpcube-0.3.1.1/scripts/generate_training_yamls.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/import_model.py` & `nlpcube-0.3.1.1/scripts/import_model.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/list2train.py` & `nlpcube-0.3.1.1/scripts/list2train.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/package_ud_models.py` & `nlpcube-0.3.1.1/scripts/package_ud_models.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/reshape_unimorf.py` & `nlpcube-0.3.1.1/scripts/reshape_unimorf.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/result_mdtable_generator.py` & `nlpcube-0.3.1.1/scripts/result_mdtable_generator.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/test_all_models.py` & `nlpcube-0.3.1.1/scripts/test_all_models.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/scripts/utils.py` & `nlpcube-0.3.1.1/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `nlpcube-0.3.1.0/setup.py` & `nlpcube-0.3.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,18 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nlpcube",
-    version="0.3.1.0",
+    version="0.3.1.1",
     author="Multiple authors",
     author_email="tiberiu44@gmail.com",
-    description="Natural Language Procecssing Toolkit with support for tokenization, sentence splitting, lemmatization, tagging and parsing for more than 60 languages",
+    description="Natural Language Processing Toolkit with support for tokenization, sentence splitting, lemmatization, tagging and parsing for more than 60 languages",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/adobe/NLP-Cube",
     packages=setuptools.find_packages(),
     install_requires = parse_requirements('requirements.txt', session=False),
     classifiers=(
         "Programming Language :: Python :: 3.0",
```

