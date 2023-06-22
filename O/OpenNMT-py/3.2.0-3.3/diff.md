# Comparing `tmp/OpenNMT-py-3.2.0.tar.gz` & `tmp/OpenNMT-py-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenNMT-py-3.2.0.tar", last modified: Wed Jun  7 20:15:54 2023, max compression
+gzip compressed data, was "OpenNMT-py-3.3.tar", last modified: Thu Jun 22 11:34:32 2023, max compression
```

## Comparing `OpenNMT-py-3.2.0.tar` & `OpenNMT-py-3.3.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.871519 OpenNMT-py-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/LICENSE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.843519 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 20:15:54.000000 OpenNMT-py-3.2.0/OpenNMT_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-06-07 20:15:54.871519 OpenNMT-py-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.843519 OpenNMT-py-3.2.0/onmt/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.847519 OpenNMT-py-3.2.0/onmt/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1651 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/average_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/build_vocab.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/release_model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/bin/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.847519 OpenNMT-py-3.2.0/onmt/decoders/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/cnn_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)    28397 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/decoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.847519 OpenNMT-py-3.2.0/onmt/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/cnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/ggnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/mean_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/rnn_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7574 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/encoders/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.855519 OpenNMT-py-3.2.0/onmt/inputters/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/dynamic_iterator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7115 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/inputter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/text_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/inputters/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14427 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.855519 OpenNMT-py-3.2.0/onmt/models/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5706 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/models/model_saver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.859519 OpenNMT-py-3.2.0/onmt/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/alibi_position_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/average_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7778 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/bnb_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/conv_multi_step_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/copy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/global_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12494 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    13161 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/multi_headed_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/position_ffn.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/rmsnorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/sparse_activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/sparse_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/sru.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/stacked_rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/util_class.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/modules/weight_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    53100 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/opts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.859519 OpenNMT-py-3.2.0/onmt/scorers/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/scorers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/scorers/bleu.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/scorers/scorer.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/scorers/ter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.867519 OpenNMT-py-3.2.0/onmt/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    30982 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_copy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_data_prepare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-06-07 20:15:47.000000 OpenNMT-py-3.2.0/onmt/tests/test_greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_structured_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_subword_marker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_text_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_translation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/tests/utils_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/train_single.py
--rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.867519 OpenNMT-py-3.2.0/onmt/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/bart.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/docify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/fuzzymatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13648 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/inlinetags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/transforms/uppercase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.867519 OpenNMT-py-3.2.0/onmt/translate/
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/beam_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/decode_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/greedy_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/penalties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/process_zh.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)    36570 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/translation_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    41387 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/translate/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:15:54.871519 OpenNMT-py-3.2.0/onmt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/alignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/cnn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/earlystopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29800 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14395 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/report_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/rnn_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/scoring_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/onmt/utils/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-07 20:15:54.871519 OpenNMT-py-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 20:15:48.000000 OpenNMT-py-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.526389 OpenNMT-py-3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/LICENSE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.494390 OpenNMT-py-3.3/OpenNMT_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-22 11:34:32.000000 OpenNMT-py-3.3/OpenNMT_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-22 11:34:32.000000 OpenNMT-py-3.3/OpenNMT_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 11:34:32.000000 OpenNMT-py-3.3/OpenNMT_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-22 11:34:32.000000 OpenNMT-py-3.3/OpenNMT_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 11:34:32.000000 OpenNMT-py-3.3/OpenNMT_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 11:34:32.000000 OpenNMT-py-3.3/OpenNMT_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-06-22 11:34:32.526389 OpenNMT-py-3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.498390 OpenNMT-py-3.3/onmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.502389 OpenNMT-py-3.3/onmt/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1651 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/bin/average_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/bin/build_vocab.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1167 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/bin/release_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5237 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/bin/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/bin/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/bin/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.502389 OpenNMT-py-3.3/onmt/decoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/decoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/decoders/cnn_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14204 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/decoders/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/decoders/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29115 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/decoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.506389 OpenNMT-py-3.3/onmt/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/encoders/cnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/encoders/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/encoders/ggnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/encoders/mean_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/encoders/rnn_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7534 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/encoders/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.506389 OpenNMT-py-3.3/onmt/inputters/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/inputters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15085 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/inputters/dynamic_iterator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/inputters/inputter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/inputters/text_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/inputters/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15668 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.506389 OpenNMT-py-3.3/onmt/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10663 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/models/model_saver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.510389 OpenNMT-py-3.3/onmt/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/alibi_position_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/average_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/bnb_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/conv_multi_step_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/copy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6564 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/global_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12646 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/multi_headed_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/position_ffn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/rmsnorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/sparse_activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/sparse_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/sru.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/stacked_rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/util_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/modules/weight_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53735 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/opts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.514389 OpenNMT-py-3.3/onmt/scorers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/scorers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/scorers/bleu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/scorers/scorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/scorers/ter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.518389 OpenNMT-py-3.3/onmt/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/tests/test_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30982 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/tests/test_beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/tests/test_copy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/tests/test_data_prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6354 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/tests/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20167 2023-06-22 11:34:24.000000 OpenNMT-py-3.3/onmt/tests/test_greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7467 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/test_structured_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12006 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/test_subword_marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/test_text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10008 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/test_translation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/tests/utils_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/train_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23539 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.522389 OpenNMT-py-3.3/onmt/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/bart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/docify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/fuzzymatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13622 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/inlinetags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24101 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10123 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/transforms/uppercase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.522389 OpenNMT-py-3.3/onmt/translate/
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19571 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/beam_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/decode_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/greedy_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3630 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/penalties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/process_zh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36570 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/translation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41387 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/translate/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 11:34:32.526389 OpenNMT-py-3.3/onmt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/cnn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/earlystopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15753 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29800 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14487 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5546 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/report_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/rnn_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/scoring_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/onmt/utils/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 11:34:32.526389 OpenNMT-py-3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-22 11:34:25.000000 OpenNMT-py-3.3/setup.py
```

### Comparing `OpenNMT-py-3.2.0/LICENSE.md` & `OpenNMT-py-3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/OpenNMT_py.egg-info/PKG-INFO` & `OpenNMT-py-3.3/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: OpenNMT-py
-Version: 3.2.0
-Summary: A python implementation of OpenNMT
-Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
-Project-URL: Forum, http://forum.opennmt.net/
-Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
-Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # OpenNMT-py: Open-Source Neural Machine Translation and (Large) Language Models
 
 [![Build Status](https://github.com/OpenNMT/OpenNMT-py/workflows/Lint%20&%20Tests/badge.svg)](https://github.com/OpenNMT/OpenNMT-py/actions)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue.svg)](https://opennmt.net/OpenNMT-py/)
 [![Gitter](https://badges.gitter.im/OpenNMT/OpenNMT-py.svg)](https://gitter.im/OpenNMT/OpenNMT-py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![Forum](https://img.shields.io/discourse/status?server=https%3A%2F%2Fforum.opennmt.net%2F)](https://forum.opennmt.net/)
 
@@ -33,18 +21,21 @@
 Please try to read and/or follow before raising newbies issues.
 
 Otherwise you can just have a look at the [Quickstart](https://opennmt.net/OpenNMT-py/quickstart.html) steps
 
 ----
 ## New:
 
-LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
-Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
-You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
-Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+* Special note on Pytorch v2: up to v2.0.1 dynamic shapes are not handled properly, hence torch.compile() will not work with OpenNMT-py. We have tested nightly (in May) and it works with a small gain. Next version will be 2.1
+* LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
+* Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
+* You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
+* Inference can be forced in 4/8bit using the same layer quantization as in finetuning.
+* Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+* MMLU evaluation script, see results [here](https://github.com/OpenNMT/OpenNMT-py/blob/master/eval_llm/MMLU/readme.md)
 
 For all usecases including NMT, you can now use Multiquery instead of Multihead attention (faster at training and inference) and remove biases from all Linear (QKV as well as FeedForward modules).
 
 
 If you used previous versions of OpenNMT-py, you can check the [Changelog](https://github.com/OpenNMT/OpenNMT-py/blob/master/CHANGELOG.md) or the [Breaking Changes](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/changes.md)
 
 ----
@@ -60,15 +51,15 @@
 ----
 
 ## Setup
 
 OpenNMT-py requires:
 
 - Python >= 3.8
-- PyTorch >= 1.13 <2
+- PyTorch >= 1.13 <2.1
 
 Install `OpenNMT-py` from `pip`:
 ```bash
 pip install OpenNMT-py
 ```
 
 or from the sources:
@@ -82,44 +73,28 @@
 
 *(Optional)* Some advanced features (e.g. working pretrained models or specific transforms) require extra packages, you can install them with:
 
 ```bash
 pip install -r requirements.opt.txt
 ```
 
-## Features
-
-- [End-to-end training with on-the-fly data processing]([here](https://opennmt.net/OpenNMT-py/FAQ.html#what-are-the-readily-available-on-the-fly-data-transforms).)
-
-- [Transformer models](https://opennmt.net/OpenNMT-py/FAQ.html#how-do-i-use-the-transformer-model)
-- [Encoder-decoder models with multiple RNN cells (LSTM, GRU) and attention types (Luong, Bahdanau)](https://opennmt.net/OpenNMT-py/options/train.html#model-encoder-decoder)
-- [SRU "RNNs faster than CNN"](https://arxiv.org/abs/1709.02755)
-- [Conv2Conv convolution model](https://arxiv.org/abs/1705.03122)
-- [Copy and Coverage Attention](https://opennmt.net/OpenNMT-py/options/train.html#model-attention)
-- [Pretrained Embeddings](https://opennmt.net/OpenNMT-py/FAQ.html#how-do-i-use-pretrained-embeddings-e-g-glove)
-- [Source word features](https://opennmt.net/OpenNMT-py/options/train.html#model-embeddings)
-- [TensorBoard logging](https://opennmt.net/OpenNMT-py/options/train.html#logging)
-- Mixed-precision training with [APEX](https://github.com/NVIDIA/apex), optimized on [Tensor Cores](https://developer.nvidia.com/tensor-cores)
-- [Multi-GPU training](https://opennmt.net/OpenNMT-py/FAQ.html##do-you-support-multi-gpu)
-- [Inference (translation) with batching and beam search](https://opennmt.net/OpenNMT-py/options/translate.html)
-- Model export to [CTranslate2](https://github.com/OpenNMT/CTranslate2), a fast and efficient inference engine
-
-## Documentation
+## Documentation & FAQs
 
 [Full HTML Documentation](https://opennmt.net/OpenNMT-py/quickstart.html)
 
+[FAQs](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/FAQ.md)
+
 ## Acknowledgements
 
 OpenNMT-py is run as a collaborative open-source project.
 Project was incubated by Systran and Harvard NLP in 2016 in Lua and ported to Pytorch in 2017.
 
-Current maintainers:
-
-Ubiqus Team: [François Hernandez](https://github.com/francoishernandez) and Team.
+Current maintainers (since 2018):
 
+[François Hernandez](https://github.com/francoishernandez) and Ubiqus Team.
 [Vincent Nguyen](https://github.com/vince62s) (Seedfall)
 
 ## Citation
 
 If you are using OpenNMT-py for academic work, please cite the initial [system demonstration paper](https://www.aclweb.org/anthology/P17-4012) published in ACL 2017:
 
 ```
```

### Comparing `OpenNMT-py-3.2.0/OpenNMT_py.egg-info/SOURCES.txt` & `OpenNMT-py-3.3/OpenNMT_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/PKG-INFO` & `OpenNMT-py-3.3/OpenNMT_py.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenNMT-py
-Version: 3.2.0
+Version: 3.3
 Summary: A python implementation of OpenNMT
 Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
 Project-URL: Forum, http://forum.opennmt.net/
 Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
 Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -33,18 +33,21 @@
 Please try to read and/or follow before raising newbies issues.
 
 Otherwise you can just have a look at the [Quickstart](https://opennmt.net/OpenNMT-py/quickstart.html) steps
 
 ----
 ## New:
 
-LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
-Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
-You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
-Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+* Special note on Pytorch v2: up to v2.0.1 dynamic shapes are not handled properly, hence torch.compile() will not work with OpenNMT-py. We have tested nightly (in May) and it works with a small gain. Next version will be 2.1
+* LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
+* Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
+* You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
+* Inference can be forced in 4/8bit using the same layer quantization as in finetuning.
+* Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+* MMLU evaluation script, see results [here](https://github.com/OpenNMT/OpenNMT-py/blob/master/eval_llm/MMLU/readme.md)
 
 For all usecases including NMT, you can now use Multiquery instead of Multihead attention (faster at training and inference) and remove biases from all Linear (QKV as well as FeedForward modules).
 
 
 If you used previous versions of OpenNMT-py, you can check the [Changelog](https://github.com/OpenNMT/OpenNMT-py/blob/master/CHANGELOG.md) or the [Breaking Changes](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/changes.md)
 
 ----
@@ -60,15 +63,15 @@
 ----
 
 ## Setup
 
 OpenNMT-py requires:
 
 - Python >= 3.8
-- PyTorch >= 1.13 <2
+- PyTorch >= 1.13 <2.1
 
 Install `OpenNMT-py` from `pip`:
 ```bash
 pip install OpenNMT-py
 ```
 
 or from the sources:
@@ -82,44 +85,28 @@
 
 *(Optional)* Some advanced features (e.g. working pretrained models or specific transforms) require extra packages, you can install them with:
 
 ```bash
 pip install -r requirements.opt.txt
 ```
 
-## Features
-
-- [End-to-end training with on-the-fly data processing]([here](https://opennmt.net/OpenNMT-py/FAQ.html#what-are-the-readily-available-on-the-fly-data-transforms).)
-
-- [Transformer models](https://opennmt.net/OpenNMT-py/FAQ.html#how-do-i-use-the-transformer-model)
-- [Encoder-decoder models with multiple RNN cells (LSTM, GRU) and attention types (Luong, Bahdanau)](https://opennmt.net/OpenNMT-py/options/train.html#model-encoder-decoder)
-- [SRU "RNNs faster than CNN"](https://arxiv.org/abs/1709.02755)
-- [Conv2Conv convolution model](https://arxiv.org/abs/1705.03122)
-- [Copy and Coverage Attention](https://opennmt.net/OpenNMT-py/options/train.html#model-attention)
-- [Pretrained Embeddings](https://opennmt.net/OpenNMT-py/FAQ.html#how-do-i-use-pretrained-embeddings-e-g-glove)
-- [Source word features](https://opennmt.net/OpenNMT-py/options/train.html#model-embeddings)
-- [TensorBoard logging](https://opennmt.net/OpenNMT-py/options/train.html#logging)
-- Mixed-precision training with [APEX](https://github.com/NVIDIA/apex), optimized on [Tensor Cores](https://developer.nvidia.com/tensor-cores)
-- [Multi-GPU training](https://opennmt.net/OpenNMT-py/FAQ.html##do-you-support-multi-gpu)
-- [Inference (translation) with batching and beam search](https://opennmt.net/OpenNMT-py/options/translate.html)
-- Model export to [CTranslate2](https://github.com/OpenNMT/CTranslate2), a fast and efficient inference engine
-
-## Documentation
+## Documentation & FAQs
 
 [Full HTML Documentation](https://opennmt.net/OpenNMT-py/quickstart.html)
 
+[FAQs](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/FAQ.md)
+
 ## Acknowledgements
 
 OpenNMT-py is run as a collaborative open-source project.
 Project was incubated by Systran and Harvard NLP in 2016 in Lua and ported to Pytorch in 2017.
 
-Current maintainers:
-
-Ubiqus Team: [François Hernandez](https://github.com/francoishernandez) and Team.
+Current maintainers (since 2018):
 
+[François Hernandez](https://github.com/francoishernandez) and Ubiqus Team.
 [Vincent Nguyen](https://github.com/vince62s) (Seedfall)
 
 ## Citation
 
 If you are using OpenNMT-py for academic work, please cite the initial [system demonstration paper](https://www.aclweb.org/anthology/P17-4012) published in ACL 2017:
 
 ```
```

### Comparing `OpenNMT-py-3.2.0/README.md` & `OpenNMT-py-3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: OpenNMT-py
+Version: 3.3
+Summary: A python implementation of OpenNMT
+Project-URL: Documentation, http://opennmt.net/OpenNMT-py/
+Project-URL: Forum, http://forum.opennmt.net/
+Project-URL: Gitter, https://gitter.im/OpenNMT/OpenNMT-py
+Project-URL: Source, https://github.com/OpenNMT/OpenNMT-py/
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # OpenNMT-py: Open-Source Neural Machine Translation and (Large) Language Models
 
 [![Build Status](https://github.com/OpenNMT/OpenNMT-py/workflows/Lint%20&%20Tests/badge.svg)](https://github.com/OpenNMT/OpenNMT-py/actions)
 [![Documentation](https://img.shields.io/badge/docs-latest-blue.svg)](https://opennmt.net/OpenNMT-py/)
 [![Gitter](https://badges.gitter.im/OpenNMT/OpenNMT-py.svg)](https://gitter.im/OpenNMT/OpenNMT-py?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 [![Forum](https://img.shields.io/discourse/status?server=https%3A%2F%2Fforum.opennmt.net%2F)](https://forum.opennmt.net/)
 
@@ -21,18 +33,21 @@
 Please try to read and/or follow before raising newbies issues.
 
 Otherwise you can just have a look at the [Quickstart](https://opennmt.net/OpenNMT-py/quickstart.html) steps
 
 ----
 ## New:
 
-LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
-Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
-You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
-Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+* Special note on Pytorch v2: up to v2.0.1 dynamic shapes are not handled properly, hence torch.compile() will not work with OpenNMT-py. We have tested nightly (in May) and it works with a small gain. Next version will be 2.1
+* LLM support with converters for: Llama, OpenLlama, Redpajama, MPT-7B, Falcon.
+* Support for 8bit and 4bit quantization along with LoRA adapters, with or without checkpointing.
+* You can finetune 7B and 13B models on a single RTX 24GB with 4-bit quantization.
+* Inference can be forced in 4/8bit using the same layer quantization as in finetuning.
+* Once your model is finetuned you can run inference either with OpenNMT-py or faster with CTranslate2.
+* MMLU evaluation script, see results [here](https://github.com/OpenNMT/OpenNMT-py/blob/master/eval_llm/MMLU/readme.md)
 
 For all usecases including NMT, you can now use Multiquery instead of Multihead attention (faster at training and inference) and remove biases from all Linear (QKV as well as FeedForward modules).
 
 
 If you used previous versions of OpenNMT-py, you can check the [Changelog](https://github.com/OpenNMT/OpenNMT-py/blob/master/CHANGELOG.md) or the [Breaking Changes](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/changes.md)
 
 ----
@@ -48,15 +63,15 @@
 ----
 
 ## Setup
 
 OpenNMT-py requires:
 
 - Python >= 3.8
-- PyTorch >= 1.13 <2
+- PyTorch >= 1.13 <2.1
 
 Install `OpenNMT-py` from `pip`:
 ```bash
 pip install OpenNMT-py
 ```
 
 or from the sources:
@@ -70,44 +85,28 @@
 
 *(Optional)* Some advanced features (e.g. working pretrained models or specific transforms) require extra packages, you can install them with:
 
 ```bash
 pip install -r requirements.opt.txt
 ```
 
-## Features
-
-- [End-to-end training with on-the-fly data processing]([here](https://opennmt.net/OpenNMT-py/FAQ.html#what-are-the-readily-available-on-the-fly-data-transforms).)
-
-- [Transformer models](https://opennmt.net/OpenNMT-py/FAQ.html#how-do-i-use-the-transformer-model)
-- [Encoder-decoder models with multiple RNN cells (LSTM, GRU) and attention types (Luong, Bahdanau)](https://opennmt.net/OpenNMT-py/options/train.html#model-encoder-decoder)
-- [SRU "RNNs faster than CNN"](https://arxiv.org/abs/1709.02755)
-- [Conv2Conv convolution model](https://arxiv.org/abs/1705.03122)
-- [Copy and Coverage Attention](https://opennmt.net/OpenNMT-py/options/train.html#model-attention)
-- [Pretrained Embeddings](https://opennmt.net/OpenNMT-py/FAQ.html#how-do-i-use-pretrained-embeddings-e-g-glove)
-- [Source word features](https://opennmt.net/OpenNMT-py/options/train.html#model-embeddings)
-- [TensorBoard logging](https://opennmt.net/OpenNMT-py/options/train.html#logging)
-- Mixed-precision training with [APEX](https://github.com/NVIDIA/apex), optimized on [Tensor Cores](https://developer.nvidia.com/tensor-cores)
-- [Multi-GPU training](https://opennmt.net/OpenNMT-py/FAQ.html##do-you-support-multi-gpu)
-- [Inference (translation) with batching and beam search](https://opennmt.net/OpenNMT-py/options/translate.html)
-- Model export to [CTranslate2](https://github.com/OpenNMT/CTranslate2), a fast and efficient inference engine
-
-## Documentation
+## Documentation & FAQs
 
 [Full HTML Documentation](https://opennmt.net/OpenNMT-py/quickstart.html)
 
+[FAQs](https://github.com/OpenNMT/OpenNMT-py/blob/master/docs/source/FAQ.md)
+
 ## Acknowledgements
 
 OpenNMT-py is run as a collaborative open-source project.
 Project was incubated by Systran and Harvard NLP in 2016 in Lua and ported to Pytorch in 2017.
 
-Current maintainers:
-
-Ubiqus Team: [François Hernandez](https://github.com/francoishernandez) and Team.
+Current maintainers (since 2018):
 
+[François Hernandez](https://github.com/francoishernandez) and Ubiqus Team.
 [Vincent Nguyen](https://github.com/vince62s) (Seedfall)
 
 ## Citation
 
 If you are using OpenNMT-py for academic work, please cite the initial [system demonstration paper](https://www.aclweb.org/anthology/P17-4012) published in ACL 2017:
 
 ```
```

### Comparing `OpenNMT-py-3.2.0/onmt/bin/average_models.py` & `OpenNMT-py-3.3/onmt/bin/average_models.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/bin/build_vocab.py` & `OpenNMT-py-3.3/onmt/bin/build_vocab.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/bin/release_model.py` & `OpenNMT-py-3.3/onmt/bin/release_model.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/bin/server.py` & `OpenNMT-py-3.3/onmt/bin/server.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/bin/train.py` & `OpenNMT-py-3.3/onmt/bin/train.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/bin/translate.py` & `OpenNMT-py-3.3/onmt/bin/translate.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from onmt.utils.logging import init_logger
 from onmt.translate.translator import build_translator
 from onmt.inputters.dynamic_iterator import build_dynamic_dataset_iter
 from onmt.inputters.inputter import IterOnDevice
-from onmt.transforms import get_transforms_cls, TransformPipe
+from onmt.transforms import get_transforms_cls
 from onmt.constants import CorpusTask
 import onmt.opts as opts
 from onmt.utils.parse import ArgumentParser
 from onmt.utils.misc import use_gpu, set_random_seed
 
 
 def translate(opt):
@@ -28,27 +28,19 @@
         opt,
         transforms_cls,
         translator.vocabs,
         task=CorpusTask.INFER,
         copy=translator.copy_attn,
     )
 
-    data_transform = [
-        infer_iter.transforms[name]
-        for name in opt.transforms
-        if name in infer_iter.transforms
-    ]
-    transform = TransformPipe.build_from(data_transform)
-
-    if infer_iter is not None:
-        infer_iter = IterOnDevice(infer_iter, opt.gpu)
+    infer_iter = IterOnDevice(infer_iter, opt.gpu)
 
     _, _ = translator._translate(
         infer_iter,
-        transform=transform,
+        transform=infer_iter.transform,
         attn_debug=opt.attn_debug,
         align_debug=opt.align_debug,
     )
 
 
 def _get_parser():
     parser = ArgumentParser(description="translate.py")
```

### Comparing `OpenNMT-py-3.2.0/onmt/constants.py` & `OpenNMT-py-3.3/onmt/constants.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/decoders/cnn_decoder.py` & `OpenNMT-py-3.3/onmt/decoders/cnn_decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/decoders/decoder.py` & `OpenNMT-py-3.3/onmt/decoders/decoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/decoders/ensemble.py` & `OpenNMT-py-3.3/onmt/decoders/ensemble.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/decoders/transformer.py` & `OpenNMT-py-3.3/onmt/decoders/transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,18 @@
         self_attn_type="scaled-dot",
         max_relative_positions=0,
         aan_useffn=False,
         full_context_alignment=False,
         alignment_heads=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        multiquery=False,
+        num_kv=0,
         add_ffnbias=True,
         parallel_residual=False,
+        shared_layer_norm=False,
         layer_norm="standard",
         use_ckpting=[],
     ):
         """
         Args:
             d_model (int): the dimension of keys/values/queries in
                 :class:`MultiHeadedAttention`, also the input size of
@@ -70,15 +71,15 @@
             self.self_attn = MultiHeadedAttention(
                 heads,
                 d_model,
                 dropout=attention_dropout,
                 max_relative_positions=max_relative_positions,
                 attn_type="self",
                 add_qkvbias=add_qkvbias,
-                multiquery=multiquery,
+                num_kv=num_kv,
                 use_ckpting=use_ckpting,
             )
         elif self_attn_type == "average":
             self.self_attn = AverageAttention(
                 d_model, dropout=attention_dropout, aan_useffn=aan_useffn
             )
 
@@ -89,20 +90,26 @@
             pos_ffn_activation_fn,
             add_ffnbias,
             parallel_residual,
             layer_norm,
             use_ckpting=use_ckpting,
         )
         self.parallel_residual = parallel_residual
+        self.shared_layer_norm = shared_layer_norm
         if layer_norm == "standard":
             self.layer_norm_1 = nn.LayerNorm(d_model, eps=1e-6)
+            if parallel_residual and not shared_layer_norm:
+                self.layer_norm_res = nn.LayerNorm(d_model, eps=1e-6)
         elif layer_norm == "rms":
             self.layer_norm_1 = RMSNorm(d_model, eps=1e-6)
+            if parallel_residual and not shared_layer_norm:
+                self.layer_norm_res = RMSNorm(d_model, eps=1e-6)
         else:
             raise ValueError(f"{layer_norm} layer norm type is not supported")
+
         self.dropout = nn.Dropout(dropout)
         self.full_context_alignment = full_context_alignment
         self.alignment_heads = alignment_heads
 
     def forward(self, *args, **kwargs):
         """Extend `_forward` for (possibly) multiple decoder pass:
         Always a default (future masked) decoder forward pass,
@@ -195,17 +202,18 @@
         self_attn_type="scaled-dot",
         max_relative_positions=0,
         aan_useffn=False,
         full_context_alignment=False,
         alignment_heads=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        multiquery=False,
+        num_kv=0,
         add_ffnbias=True,
         parallel_residual=False,
+        shared_layer_norm=False,
         layer_norm="standard",
         use_ckpting=[],
     ):
         """
         Args:
             See TransformerDecoderLayerBase
         """
@@ -218,27 +226,28 @@
             self_attn_type,
             max_relative_positions,
             aan_useffn,
             full_context_alignment,
             alignment_heads,
             pos_ffn_activation_fn=pos_ffn_activation_fn,
             add_qkvbias=add_qkvbias,
-            multiquery=multiquery,
+            num_kv=num_kv,
             add_ffnbias=add_ffnbias,
             parallel_residual=parallel_residual,
+            shared_layer_norm=shared_layer_norm,
             layer_norm=layer_norm,
             use_ckpting=use_ckpting,
         )
         self.context_attn = MultiHeadedAttention(
             heads,
             d_model,
             dropout=attention_dropout,
             attn_type="context",
             add_qkvbias=add_qkvbias,
-            multiquery=multiquery,
+            num_kv=num_kv,
             use_ckpting=use_ckpting,
         )
         if layer_norm == "standard":
             self.layer_norm_2 = nn.LayerNorm(d_model, eps=1e-6)
         elif layer_norm == "rms":
             self.layer_norm_2 = RMSNorm(d_model, eps=1e-6)
         else:
@@ -355,17 +364,18 @@
             opt.max_relative_positions,
             opt.aan_useffn,
             opt.full_context_alignment,
             opt.alignment_layer,
             alignment_heads=opt.alignment_heads,
             pos_ffn_activation_fn=opt.pos_ffn_activation_fn,
             add_qkvbias=opt.add_qkvbias,
-            multiquery=opt.multiquery,
+            num_kv=opt.num_kv,
             add_ffnbias=opt.add_ffnbias,
             parallel_residual=opt.parallel_residual,
+            shared_layer_norm=opt.shared_layer_norm,
             layer_norm=opt.layer_norm,
             use_ckpting=opt.use_ckpting,
         )
 
     def init_state(self, src, enc_out, enc_final_hs):
         """Initialize decoder state."""
         self.state["src"] = src
@@ -442,17 +452,18 @@
         max_relative_positions,
         aan_useffn,
         full_context_alignment,
         alignment_layer,
         alignment_heads,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        multiquery=False,
+        num_kv=0,
         add_ffnbias=True,
         parallel_residual=False,
+        shared_layer_norm=False,
         layer_norm="standard",
         use_ckpting=[],
     ):
         super(TransformerDecoder, self).__init__(
             d_model, copy_attn, embeddings, alignment_layer, layer_norm
         )
 
@@ -467,17 +478,18 @@
                     self_attn_type=self_attn_type,
                     max_relative_positions=max_relative_positions,
                     aan_useffn=aan_useffn,
                     full_context_alignment=full_context_alignment,
                     alignment_heads=alignment_heads,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
                     add_qkvbias=add_qkvbias,
-                    multiquery=multiquery,
+                    num_kv=num_kv,
                     add_ffnbias=add_ffnbias,
                     parallel_residual=parallel_residual,
+                    shared_layer_norm=shared_layer_norm,
                     layer_norm=layer_norm,
                     use_ckpting=use_ckpting,
                 )
                 for i in range(num_layers)
             ]
         )
 
@@ -614,19 +626,21 @@
 
         norm_layer_in = self.layer_norm_1(layer_in)
 
         attn_output, attns = self._forward_self_attn(norm_layer_in, dec_mask, step)
 
         if self.parallel_residual:
             # feed_forward applies residual, so we remove and apply residual with un-normed
+            if not self.shared_layer_norm:
+                norm_res_layer_in = self.layer_norm_res(layer_in)
+                ff_in = norm_res_layer_in
+            else:
+                ff_in = norm_layer_in
             layer_out = (
-                self.feed_forward(norm_layer_in)
-                - norm_layer_in
-                + layer_in
-                + self.dropout(attn_output)
+                self.feed_forward(ff_in) - ff_in + layer_in + self.dropout(attn_output)
             )
         else:
             layer_out = self.dropout(attn_output) + layer_in
             layer_out = self.feed_forward(layer_out)
 
         return layer_out, attns
 
@@ -664,17 +678,18 @@
         max_relative_positions,
         aan_useffn,
         full_context_alignment=None,
         alignment_layer=None,
         alignment_heads=None,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        multiquery=False,
+        num_kv=0,
         add_ffnbias=True,
         parallel_residual=False,
+        shared_layer_norm=False,
         layer_norm="standard",
         use_ckpting=[],
     ):
         super(TransformerLMDecoder, self).__init__(
             d_model, copy_attn, embeddings, alignment_layer, layer_norm
         )
         self.transformer_layers = nn.ModuleList(
@@ -688,17 +703,18 @@
                     self_attn_type=self_attn_type,
                     max_relative_positions=max_relative_positions,
                     aan_useffn=aan_useffn,
                     full_context_alignment=None,
                     alignment_heads=None,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
                     add_qkvbias=add_qkvbias,
-                    multiquery=multiquery,
+                    num_kv=num_kv,
                     add_ffnbias=add_ffnbias,
                     parallel_residual=parallel_residual,
+                    shared_layer_norm=shared_layer_norm,
                     layer_norm=layer_norm,
                     use_ckpting=use_ckpting,
                 )
                 for i in range(num_layers)
             ]
         )
```

### Comparing `OpenNMT-py-3.2.0/onmt/encoders/cnn_encoder.py` & `OpenNMT-py-3.3/onmt/encoders/cnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/encoders/encoder.py` & `OpenNMT-py-3.3/onmt/encoders/encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/encoders/ggnn_encoder.py` & `OpenNMT-py-3.3/onmt/encoders/ggnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/encoders/mean_encoder.py` & `OpenNMT-py-3.3/onmt/encoders/mean_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/encoders/rnn_encoder.py` & `OpenNMT-py-3.3/onmt/encoders/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/encoders/transformer.py` & `OpenNMT-py-3.3/onmt/encoders/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,30 +33,30 @@
         heads,
         d_ff,
         dropout,
         attention_dropout,
         max_relative_positions=0,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        multiquery=False,
+        num_kv=0,
         add_ffnbias=True,
         parallel_residual=False,
         layer_norm="standard",
         use_ckpting=[],
     ):
         super(TransformerEncoderLayer, self).__init__()
 
         self.self_attn = MultiHeadedAttention(
             heads,
             d_model,
             dropout=attention_dropout,
             max_relative_positions=max_relative_positions,
             attn_type="self",
             add_qkvbias=add_qkvbias,
-            multiquery=multiquery,
+            num_kv=num_kv,
             use_ckpting=use_ckpting,
         )
         self.feed_forward = PositionwiseFeedForward(
             d_model,
             d_ff,
             dropout,
             pos_ffn_activation_fn,
@@ -139,15 +139,15 @@
         d_ff,
         dropout,
         attention_dropout,
         embeddings,
         max_relative_positions,
         pos_ffn_activation_fn=ActivationFunction.relu,
         add_qkvbias=False,
-        multiquery=False,
+        num_kv=0,
         add_ffnbias=True,
         parallel_residual=False,
         layer_norm="standard",
         use_ckpting=[],
     ):
         super(TransformerEncoder, self).__init__()
 
@@ -159,15 +159,15 @@
                     heads,
                     d_ff,
                     dropout,
                     attention_dropout,
                     max_relative_positions=max_relative_positions,
                     pos_ffn_activation_fn=pos_ffn_activation_fn,
                     add_qkvbias=add_qkvbias,
-                    multiquery=multiquery,
+                    num_kv=num_kv,
                     add_ffnbias=add_ffnbias,
                     parallel_residual=parallel_residual,
                     layer_norm=layer_norm,
                     use_ckpting=use_ckpting,
                 )
                 for i in range(num_layers)
             ]
@@ -191,15 +191,15 @@
             opt.attention_dropout[0]
             if type(opt.attention_dropout) is list
             else opt.attention_dropout,
             embeddings,
             opt.max_relative_positions,
             pos_ffn_activation_fn=opt.pos_ffn_activation_fn,
             add_qkvbias=opt.add_qkvbias,
-            multiquery=opt.multiquery,
+            num_kv=opt.num_kv,
             add_ffnbias=opt.add_ffnbias,
             parallel_residual=opt.parallel_residual,
             layer_norm=opt.layer_norm,
             use_ckpting=opt.use_ckpting,
         )
 
     def forward(self, src, src_len=None):
```

### Comparing `OpenNMT-py-3.2.0/onmt/inputters/__init__.py` & `OpenNMT-py-3.3/onmt/inputters/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/inputters/dynamic_iterator.py` & `OpenNMT-py-3.3/onmt/inputters/dynamic_iterator.py`

 * *Files 3% similar despite different names*

```diff
@@ -339,32 +339,43 @@
                 # within the batch
                 minibatch.sort(key=self.sort_key, reverse=True)
                 tensor_batch = tensorify(self.vocabs, minibatch)
                 yield tensor_batch
 
 
 def build_dynamic_dataset_iter(
-    opt, transforms_cls, vocabs, copy=False, task=CorpusTask.TRAIN, stride=1, offset=0
+    opt,
+    transforms_cls,
+    vocabs,
+    copy=False,
+    task=CorpusTask.TRAIN,
+    stride=1,
+    offset=0,
+    src=None,
+    tgt=None,
+    align=None,
 ):
     """
     Build `DynamicDatasetIter` from opt.
+    if src, tgt,align are passed then dataset is built from those lists
+    instead of opt.[src, tgt, align]
     Typically this function is called for CorpusTask.[TRAIN,VALID,INFER]
     from the main tain / translate scripts
     We disable automatic batching in the DataLoader.
     The custom optimized batching is performed by the
     custom class DynamicDatasetIter inherited from IterableDataset
     (and not by a custom collate function).
     We load opt.bucket_size examples, sort them and yield
     mini-batchs of size opt.batch_size.
     The bucket_size must be large enough to ensure homogeneous batches.
     Each worker will load opt.prefetch_factor mini-batches in
     advance to avoid the GPU waiting during the refilling of the bucket.
     """
     transforms = make_transforms(opt, transforms_cls, vocabs)
-    corpora = get_corpora(opt, task)
+    corpora = get_corpora(opt, task, src=src, tgt=tgt, align=align)
     if corpora is None:
         assert task != CorpusTask.TRAIN, "only valid corpus is ignorable."
         return None
     data_iter = DynamicDatasetIter.from_opt(
         corpora, transforms, vocabs, opt, task, copy=copy, stride=stride, offset=offset
     )
     data_iter.num_workers = opt.num_workers if hasattr(opt, "num_workers") else 0
```

### Comparing `OpenNMT-py-3.2.0/onmt/inputters/inputter.py` & `OpenNMT-py-3.3/onmt/inputters/inputter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 # -*- coding: utf-8 -*-
 import os
 import math
 import codecs
 import torch
 import pyonmttok
 from onmt.constants import DefaultTokens
+from onmt.transforms import TransformPipe
 
 
 class IterOnDevice(torch.utils.data.IterableDataset):
     """Sent items from `iterable` on `device_id` and yield."""
 
     def __init__(self, iterable, device_id):
         super(IterOnDevice).__init__()
         self.iterable = iterable
         self.device_id = device_id
+        # temporary as long as translation_server and scoring_preparator still use lists
+        if hasattr(iterable, "transforms"):
+            self.transform = TransformPipe.build_from(
+                [iterable.transforms[name] for name in iterable.transforms]
+            )
 
     @staticmethod
     def batch_to_device(tensor_batch, device_id):
         """Move `batch` to `device_id`, cpu if `device_id` < 0."""
         device = torch.device(device_id) if device_id >= 0 else torch.device("cpu")
         for key in tensor_batch.keys():
             if key != "src_ex_vocab":
```

### Comparing `OpenNMT-py-3.2.0/onmt/inputters/text_corpus.py` & `OpenNMT-py-3.3/onmt/inputters/text_corpus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Module that contain shard utils for dynamic data."""
 import os
 from onmt.utils.logging import logger
 from onmt.constants import CorpusName, CorpusTask
 from onmt.transforms import TransformPipe
 from onmt.inputters.text_utils import process, parse_features, append_features_to_text
 from contextlib import contextmanager
+import itertools
 
 
 @contextmanager
 def exfile_open(filename, *args, **kwargs):
     """Extended file opener enables open(filename=None).
 
     This context manager enables open(filename=None) as well as regular file.
@@ -53,55 +54,69 @@
 
     def load(self, offset=0, stride=1):
         """
         Load file and iterate by lines.
         `offset` and `stride` allow to iterate only on every
         `stride` example, starting from `offset`.
         """
-        with exfile_open(self.src, mode="rb") as fs, exfile_open(
-            self.tgt, mode="rb"
-        ) as ft, exfile_open(self.align, mode="rb") as fa:
-            for i, (sline, tline, align) in enumerate(zip(fs, ft, fa)):
+
+        def make_ex(sline, tline, align):
+            sline, sfeats = parse_features(
+                sline,
+                n_feats=self.n_src_feats,
+                defaults=self.src_feats_defaults,
+            )
+            # 'src_original' and 'tgt_original' store the
+            # original line before tokenization. These
+            # fields are used later on in the feature
+            # transforms.
+            example = {
+                "src": sline,
+                "tgt": tline,
+                "src_original": sline,
+                "tgt_original": tline,
+            }
+            if align is not None:
+                example["align"] = align
+            if sfeats is not None:
+                example["src_feats"] = [f for f in sfeats]
+            return example
+
+        if isinstance(self.src, list):
+            fs = self.src
+            ft = [] if self.tgt is None else self.tgt
+            fa = [] if self.align is None else self.align
+            for i, (sline, tline, align) in enumerate(
+                itertools.zip_longest(fs, ft, fa)
+            ):
                 if (i // stride) % stride == offset:
-                    sline = sline.decode("utf-8")
-                    sline, sfeats = parse_features(
-                        sline,
-                        n_feats=self.n_src_feats,
-                        defaults=self.src_feats_defaults,
-                    )
-                    if tline is not None:
-                        tline = tline.decode("utf-8")
-                    # 'src_original' and 'tgt_original' store the
-                    # original line before tokenization. These
-                    # fields are used later on in the feature
-                    # transforms.
-                    example = {
-                        "src": sline,
-                        "tgt": tline,
-                        "src_original": sline,
-                        "tgt_original": tline,
-                    }
-                    if align is not None:
-                        example["align"] = align.decode("utf-8")
-
-                    if sfeats is not None:
-                        example["src_feats"] = [f for f in sfeats]
-                    yield example
+                    yield make_ex(sline, tline, align)
+        else:
+            with exfile_open(self.src, mode="rb") as fs, exfile_open(
+                self.tgt, mode="rb"
+            ) as ft, exfile_open(self.align, mode="rb") as fa:
+                for i, (sline, tline, align) in enumerate(zip(fs, ft, fa)):
+                    if (i // stride) % stride == offset:
+                        if tline is not None:
+                            tline = tline.decode("utf-8")
+                        if align is not None:
+                            align = align.decode("utf-8")
+                        yield make_ex(sline.decode("utf-8"), tline, align)
 
     def __str__(self):
         cls_name = type(self).__name__
         return (
             f"{cls_name}({self.id}, {self.src}, {self.tgt}, "
             f"align={self.align}, "
             f"n_src_feats={self.n_src_feats}, "
             f'src_feats_defaults="{self.src_feats_defaults}")'
         )
 
 
-def get_corpora(opts, task=CorpusTask.TRAIN):
+def get_corpora(opts, task=CorpusTask.TRAIN, src=None, tgt=None, align=None):
     corpora_dict = {}
     if task == CorpusTask.TRAIN:
         for corpus_id, corpus_dict in opts.data.items():
             if corpus_id != CorpusName.VALID:
                 corpora_dict[corpus_id] = ParallelCorpus(
                     corpus_id,
                     corpus_dict["path_src"],
@@ -121,16 +136,17 @@
                 src_feats_defaults=opts.src_feats_defaults,
             )
         else:
             return None
     else:
         corpora_dict[CorpusName.INFER] = ParallelCorpus(
             CorpusName.INFER,
-            opts.src,
-            opts.tgt,
+            src if src else opts.src,
+            tgt if tgt else opts.tgt,
+            align if align else None,
             n_src_feats=opts.n_src_feats,
             src_feats_defaults=opts.src_feats_defaults,
         )
     return corpora_dict
 
 
 class ParallelCorpusIterator(object):
```

### Comparing `OpenNMT-py-3.2.0/onmt/inputters/text_utils.py` & `OpenNMT-py-3.3/onmt/inputters/text_utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/model_builder.py` & `OpenNMT-py-3.3/onmt/model_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 """
 This file is for models creation, which consults options
 and creates each encoder and decoder accordingly.
 """
-import re
-import os
-import importlib
 import torch
 import torch.nn as nn
 from torch.nn.init import xavier_uniform_, zeros_, uniform_
 import onmt.modules
 from onmt.encoders import str2enc
 from onmt.decoders import str2dec
 from onmt.inputters.inputter import dict_to_vocabs
@@ -93,40 +90,57 @@
 def load_test_model(opt, model_path=None):
     if model_path is None:
         model_path = opt.models[0]
     checkpoint = load_checkpoint(model_path)
 
     model_opt = ArgumentParser.ckpt_model_opts(checkpoint["opt"])
 
+    model_opt.quant_layers = opt.quant_layers
+    model_opt.quant_type = opt.quant_type
+
     ArgumentParser.update_model_opts(model_opt)
     ArgumentParser.validate_model_opts(model_opt)
     vocabs = dict_to_vocabs(checkpoint["vocab"])
 
     # Avoid functionality on inference
     model_opt.update_vocab = False
 
     model = build_base_model(model_opt, vocabs)
 
-    model.load_state_dict(
-        checkpoint, precision=torch.float32, device=torch.device("cpu"), strict=True
-    )
-
-    del checkpoint
+    precision = torch.float32
 
-    if opt.precision == "fp32":
-        model.float()
-    elif opt.precision == "fp16":
-        model.half()
+    if opt.precision == "fp16":
+        precision = torch.float16
     elif opt.precision == "int8":
         if opt.gpu >= 0:
             raise ValueError("Dynamic 8-bit quantization is not supported on GPU")
-        torch.quantization.quantize_dynamic(model, inplace=True)
+        else:
+            precision = torch.float16
 
     if use_gpu(opt) and opt.gpu >= 0:
-        model.to(torch.device("cuda", opt.gpu))
+        device = torch.device("cuda", opt.gpu)
+    else:
+        device = torch.device("cpu")
+
+    logger.info("Loading data into the model")
+    if "model" in checkpoint.keys():
+        # weights are in the .pt file
+        model.load_state_dict(
+            checkpoint, precision=precision, device=device, strict=True
+        )
+    else:
+        # weights are not in the .pt checkpoint but stored in the safetensors file
+        base_name = model_path[:-3] if model_path[-3:] == ".pt" else model_path
+        model.load_safe_state_dict(
+            base_name, precision=precision, device=device, strict=True
+        )
+
+    del checkpoint
+    if opt.precision == "int8":
+        torch.quantization.quantize_dynamic(model, inplace=True)
 
     model.eval()
     model.generator.eval()
     return vocabs, model, model_opt
 
 
 def build_src_emb(model_opt, vocabs):
@@ -251,16 +265,14 @@
 
     if hasattr(model_opt, "quant_layers") and len(nonlora_to_quant) > 0:
         if model_opt.quant_type in ["bnb_8bit", "bnb_FP4", "bnb_NF4"]:
             logger.info(
                 "%s compression of layer %s" % (model_opt.quant_type, nonlora_to_quant)
             )
             try:
-                os.environ["BITSANDBYTES_NOWELCOME"] = "1"
-                import bitsandbytes as bnb
                 from onmt.modules.bnb_linear import replace_bnb_linear
             except ImportError:
                 raise ImportError("Install bitsandbytes to use 4/8bit compression")
             model = replace_bnb_linear(
                 model, module_to_convert=nonlora_to_quant, q_type=model_opt.quant_type
             )
         else:
@@ -362,26 +374,47 @@
     if use_gpu(opt):
         device = torch.device("cuda")
     else:
         device = torch.device("cpu")
 
     if checkpoint is not None:
         if model_opt.update_vocab:
-            # Update model embeddings with those from the checkpoint
-            # after initialization
-            use_embeddings_from_checkpoint(vocabs, model, checkpoint)
-            # after this checkpoint contains no embeddings
+            if "model" in checkpoint.keys():
+                # Update model embeddings with those from the checkpoint
+                # after initialization
+                use_embeddings_from_checkpoint(vocabs, model, checkpoint)
+                # after this checkpoint contains no embeddings
+            else:
+                raise ValueError(
+                    "Update Vocab is not compatible with safetensors mode (yet"
+                )
 
         # when using LoRa or updating the vocab (no more embeddings in ckpt)
         # => strict=False when loading state_dict
         strict = not model_opt.update_vocab
 
-        model.load_state_dict(
-            checkpoint, precision=precision, device=device, strict=strict
-        )
+        if "model" in checkpoint.keys():
+            # weights are in the .pt file
+            model.load_state_dict(
+                checkpoint,
+                precision=precision,
+                device=device,
+                strict=strict,
+            )
+        else:
+            # weights are not in the .pt checkpoint but stored in the safetensors file
+            model_path = (
+                opt.train_from[:-3] if opt.train_from[-3:] == ".pt" else opt.train_from
+            )
+            model.load_safe_state_dict(
+                model_path,
+                precision=precision,
+                device=device,
+                strict=strict,
+            )
     else:
         model.to(precision)
         model.to(device)
 
     if model_opt.freeze_encoder:
         model.encoder.requires_grad_(False)
         model.encoder.embeddings.requires_grad_()
```

### Comparing `OpenNMT-py-3.2.0/onmt/models/model.py` & `OpenNMT-py-3.3/onmt/models/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Onmt NMT Model base class definition """
 import torch
 import torch.nn as nn
-from itertools import chain
+import glob
 
 
 class BaseModel(nn.Module):
     """Core trainable object in OpenNMT. Implements a trainable interface
     for a simple, generic encoder / decoder or decoder only model.
 
     Args:
@@ -51,30 +51,31 @@
         precision=torch.float32,
         device=torch.device("cpu"),
         strict=True,
     ):
         """Custom state_dict loading to enable moving module on device as they are loaded
 
         Args:
-            checkpoint:
-            precision:
-            device:
-            strict:
-
-        Return:
-
-            * Model"""
+            checkpoint: Pytorch serialized checkpoint
+            precision: precision to move each module to
+            device: device to move each module to
+            strict: if True checks model keys wrt state_dict (both ways)
+        """
 
         # bitsandbytes quantize weights when .cuda() is called
         # for huge models we need to save Ram
         # so we load the weights  module by module and transfer them to GPU for quantization
+        buf_list = []
         for name, module in self.named_modules():
-            for param_name, param in chain(
-                module.named_parameters(), module.named_buffers()
-            ):
+            for buf_name, buf in module.named_buffers():
+                buf_list.append(buf_name)
+                if len(buf_name.split(".")) == 1:  # only last key
+                    module.to(precision)
+                    module.to(device)
+            for param_name, param in module.named_parameters():
                 if len(param_name.split(".")) == 1:  # only last key
                     if name + "." + param_name in checkpoint["model"].keys():
                         param.data = checkpoint["model"][name + "." + param_name]
                         del checkpoint["model"][name + "." + param_name]
                     elif (
                         "generator" in checkpoint.keys()
                         and name == "generator"
@@ -85,24 +86,89 @@
                         del checkpoint["generator"][param_name]
                     elif strict and "lora" not in param_name:
                         raise ValueError(
                             "Missing key in checkpoint: %s" % name + "." + param_name
                         )
                     module.to(precision)
                     module.to(device)
-        if len(checkpoint["model"].keys()) > 0:
-            raise ValueError(
-                "Extra keys in model state_dict do not match the model config %s"
-                % checkpoint["model"].keys()
-            )
-        if len(checkpoint["generator"].keys()) > 0:
-            raise ValueError(
-                "Extra keys in generator state_dict do not match the model config %s"
-                % checkpoint["generator"].keys()
-            )
+        for key in checkpoint[
+            "model"
+        ].keys():  # if some keys are left in checkpoint after deletion
+            if key not in buf_list:
+                raise ValueError(
+                    "Extra keys in model state_dict do not match the model config %s"
+                    % checkpoint["model"].keys()
+                )
+        for key in checkpoint["generator"].keys():
+            if key not in buf_list:
+                raise ValueError(
+                    "Extra keys in generator state_dict do not match the model config %s"
+                    % checkpoint["generator"].keys()
+                )
+
+    def load_safe_state_dict(
+        self,
+        model_path,
+        precision=torch.float32,
+        device=torch.device("cpu"),
+        strict=True,
+    ):
+        """Custom state_dict loading to enable moving module on device as they are loaded
+
+        Args:
+            model_path: Model path
+            precision: same as above
+            device: same as above
+            strict: same as above
+        """
+        # bitsandbytes quantize weights when .cuda() is called
+        # for huge models we need to save Ram
+        # so we load the weights  module by module and transfer them to GPU for quantization
+        try:
+            import safetensors
+        except ImportError:
+            raise ImportError("run: pip install safetensors, to use safetensors")
+        keyfound = {}
+        shards = glob.glob(model_path + ".*.safetensors")
+        if len(shards) == 0:
+            raise ValueError("No safetensors file found")
+        f = []
+        keys_shard = {}
+        for i, shard in enumerate(shards):
+            f.append(safetensors.safe_open(shard, framework="pt", device="cpu"))
+            for key in f[i].keys():
+                keys_shard[key] = i
+        buf_list = []
+        for name, module in self.named_modules():
+            for buf_name, buf in module.named_buffers():
+                buf_list.append(buf_name)
+                if len(buf_name.split(".")) == 1:  # only last key
+                    module.to(precision)
+                    module.to(device)
+            for param_name, param in module.named_parameters():
+                if len(param_name.split(".")) == 1:  # only last key
+                    if name + "." + param_name in keys_shard.keys():
+                        param.data = f[keys_shard[name + "." + param_name]].get_tensor(
+                            name + "." + param_name
+                        )
+                        keyfound[name + "." + param_name] = True
+                    elif strict and "lora" not in param_name:
+                        raise ValueError(
+                            "Missing key in safetensors checkpoint: %s" % name
+                            + "."
+                            + param_name
+                        )
+                    module.to(precision)
+                    module.to(device)
+        for key in keys_shard.keys():
+            if key not in keyfound.keys() and key not in buf_list:
+                raise ValueError(
+                    "Extra keys in model state_dict do not match the model config %s"
+                    % key
+                )
 
 
 class NMTModel(BaseModel):
     """NMTModel Class
     See :class:`~onmt.models.BaseModel` for options."""
 
     def __init__(self, encoder, decoder):
```

### Comparing `OpenNMT-py-3.2.0/onmt/models/model_saver.py` & `OpenNMT-py-3.3/onmt/models/model_saver.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     model_saver = ModelSaver(
         opt.save_model,
         model,
         model_opt,
         vocabs,
         optim,
         opt.keep_checkpoint,
+        opt.save_format,
     )
     return model_saver
 
 
 def load_checkpoint(ckpt_path):
     """Load checkpoint from `ckpt_path` if any else return `None`."""
     checkpoint = None
@@ -66,24 +67,36 @@
     """Base class for model saving operations
 
     Inherited classes must implement private methods:
     * `_save`
     * `_rm_checkpoint
     """
 
-    def __init__(self, base_path, model, model_opt, vocabs, optim, keep_checkpoint=-1):
+    def __init__(
+        self,
+        base_path,
+        model,
+        model_opt,
+        vocabs,
+        optim,
+        keep_checkpoint=-1,
+        save_format="pytorch",
+    ):
         self.base_path = base_path
         self.model = model
         self.model_opt = model_opt
         self.vocabs = vocabs
         self.optim = optim
         self.last_saved_step = None
         self.keep_checkpoint = keep_checkpoint
+        self.save_format = save_format
         if keep_checkpoint > 0:
             self.checkpoint_queue = deque([], maxlen=keep_checkpoint)
+            if save_format == "safetensors":
+                self.model_queue = deque([], maxlen=keep_checkpoint)
 
     def save(self, step, moving_average=None):
         """Main entry point for model saver
 
         It wraps the `_save` method with checks and apply `keep_checkpoint`
         related logic
         """
@@ -94,39 +107,48 @@
         save_model = self.model
         if moving_average:
             model_params_data = []
             for avg, param in zip(moving_average, save_model.parameters()):
                 model_params_data.append(param.data)
                 param.data = avg.data
 
-        chkpt, chkpt_name = self._save(step, save_model)
+        if self.save_format == "pytorch":
+            ckpt_path, _ = self._save(step, save_model)
+        elif self.save_format == "safetensors":
+            ckpt_path, model_path = self._st_save(step, save_model)
+
         self.last_saved_step = step
 
         if moving_average:
             for param_data, param in zip(model_params_data, save_model.parameters()):
                 param.data = param_data
 
         if self.keep_checkpoint > 0:
             if len(self.checkpoint_queue) == self.checkpoint_queue.maxlen:
                 todel = self.checkpoint_queue.popleft()
                 self._rm_checkpoint(todel)
-            self.checkpoint_queue.append(chkpt_name)
+                if self.save_format == "safetensors":
+                    todel = self.model_queue.popleft()
+                    self._rm_checkpoint(todel)
+            self.checkpoint_queue.append(ckpt_path)
+            if self.save_format == "safetensors":
+                self.model_queue.append(model_path)
 
     def _save(self, step, model):
         """Save a resumable checkpoint.
 
         Args:
             step (int): step number
             model (nn.Module): torch model to save
 
         Returns:
-            (object, str):
+            (str, str):
 
-            * checkpoint: the saved object
             * checkpoint_name: name (or path) of the saved checkpoint
+            * model_name: name (or path) of the saved safetensors weights if applicable
         """
 
         raise NotImplementedError()
 
     def _rm_checkpoint(self, name):
         """Remove a checkpoint
 
@@ -162,14 +184,43 @@
             "generator": generator_state_dict,
             "vocab": vocabs_to_dict(self.vocabs),
             "opt": self.model_opt,
             "optim": self.optim.state_dict(),
         }
 
         logger.info("Saving checkpoint %s_step_%d.pt" % (self.base_path, step))
-        checkpoint_path = "%s_step_%d.pt" % (self.base_path, step)
-        torch.save(checkpoint, checkpoint_path)
-        return checkpoint, checkpoint_path
+        ckpt_path = "%s_step_%d.pt" % (self.base_path, step)
+        torch.save(checkpoint, ckpt_path)
+        return ckpt_path, None
+
+    def _st_save(self, step, model):
+        try:
+            from safetensors.torch import save_file
+        except ImportError:
+            raise ImportError("run: pip install safetensors, to use safetensors")
+        if (
+            hasattr(self.model_opt, "lora_layers")
+            and len(self.model_opt.lora_layers) > 0
+        ) or (
+            hasattr(self.model_opt, "lora_embedding") and self.model_opt.lora_embedding
+        ):
+            model_state_dict = lora_state_dict(model, bias="lora_only")
+        else:
+            model_state_dict = model.state_dict()
+
+        checkpoint = {
+            "vocab": vocabs_to_dict(self.vocabs),
+            "opt": self.model_opt,
+            "optim": self.optim.state_dict(),
+        }
+
+        logger.info("Saving checkpoint %s_step_%d.pt" % (self.base_path, step))
+        ckpt_path = "%s_step_%d.pt" % (self.base_path, step)
+        torch.save(checkpoint, ckpt_path)
+        logger.info("Saving safetensors %s_step_%d.pt" % (self.base_path, step))
+        model_path = "%s_step_%d.safetensors" % (self.base_path, step)
+        save_file(model_state_dict, model_path)
+        return ckpt_path, model_path
 
     def _rm_checkpoint(self, name):
         if os.path.exists(name):
             os.remove(name)
```

### Comparing `OpenNMT-py-3.2.0/onmt/modules/__init__.py` & `OpenNMT-py-3.3/onmt/modules/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """  Attention and normalization modules  """
-import importlib
-import os
 from onmt.modules.util_class import Elementwise
 from onmt.modules.gate import context_gate_factory, ContextGate
 from onmt.modules.global_attention import GlobalAttention
 from onmt.modules.conv_multi_step_attention import ConvMultiStepAttention
 from onmt.modules.copy_generator import CopyGenerator, CopyGeneratorLoss
 from onmt.modules.multi_headed_attn import MultiHeadedAttention
 from onmt.modules.embeddings import Embeddings, PositionalEncoding
```

### Comparing `OpenNMT-py-3.2.0/onmt/modules/alibi_position_bias.py` & `OpenNMT-py-3.3/onmt/modules/alibi_position_bias.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/average_attn.py` & `OpenNMT-py-3.3/onmt/modules/average_attn.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/bnb_linear.py` & `OpenNMT-py-3.3/onmt/modules/bnb_linear.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,19 +187,14 @@
 def replace_bnb_linear(
     model,
     module_to_convert=[],
     q_type="bnb_8bit",
     threshold=6.0,
     compute_dtype=torch.float16,  # we could also use bfloat16 when available
 ):
-    try:
-        os.environ["BITSANDBYTES_NOWELCOME"] = "1"
-        import bitsandbytes as bnb
-    except ImportError:
-        raise ImportError("Install bitsandbytes to use 4/8bit compression")
     for name, module in model.named_children():
         if len(list(module.children())) > 0:
             replace_bnb_linear(
                 module, module_to_convert, q_type, threshold, compute_dtype
             )
 
         if isinstance(module, nn.Linear) and name in module_to_convert:
```

### Comparing `OpenNMT-py-3.2.0/onmt/modules/conv_multi_step_attention.py` & `OpenNMT-py-3.3/onmt/modules/conv_multi_step_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/copy_generator.py` & `OpenNMT-py-3.3/onmt/modules/copy_generator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/embeddings.py` & `OpenNMT-py-3.3/onmt/modules/embeddings.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/gate.py` & `OpenNMT-py-3.3/onmt/modules/gate.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/global_attention.py` & `OpenNMT-py-3.3/onmt/modules/global_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/lora.py` & `OpenNMT-py-3.3/onmt/modules/lora.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 #  Licensed under the MIT License (MIT).
 # Support bnb quantization of nderlying layers
 #  --------------------------------------------------------------------------
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import math
-import importlib
 from torch.utils.checkpoint import checkpoint
-from typing import List, Dict
+from typing import Dict
 import os
 
 
 class LoRALayer:
     def __init__(
         self,
         r: int,
@@ -191,21 +190,26 @@
                                 ) * self.scaling
                             self.merged = True
                 else:
                     # cannot merge/unmerge quantized weigts with unquantized lora_X
                     pass
 
             def forward(self, x: torch.Tensor):
-                result = self.maybe_ckpt(super().forward, x)
                 if self.r > 0 and not self.merged:
-                    result += (
-                        self.lora_dropout(x)
-                        @ self.lora_A.transpose(0, 1)
-                        @ self.lora_B.transpose(0, 1)
-                    ) * self.scaling
+                    result = (
+                        self.maybe_ckpt(super().forward, x)
+                        + (
+                            self.lora_dropout(x)
+                            @ self.lora_A.transpose(0, 1)
+                            @ self.lora_B.transpose(0, 1)
+                        )
+                        * self.scaling
+                    )
+                else:
+                    result = self.maybe_ckpt(super().forward, x)
                 return result
 
         instance = QLoraLinear_cls.__new__(
             QLoraLinear_cls
         )  # Create a new instance of QLoraLinear_cls
         instance.__init__(
             *args, **kwargs
```

### Comparing `OpenNMT-py-3.2.0/onmt/modules/multi_headed_attn.py` & `OpenNMT-py-3.3/onmt/modules/multi_headed_attn.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,23 +149,23 @@
         self,
         head_count: int,
         model_dim: int,
         dropout: float = 0.1,
         max_relative_positions: int = 0,
         attn_type: str = None,
         add_qkvbias=False,
-        multiquery=False,
+        num_kv=0,
         use_ckpting=[],
     ) -> None:
         assert model_dim % head_count == 0
         self.dim_per_head = model_dim // head_count
         super(MultiHeadedAttention, self).__init__()
         self.head_count = head_count
-        self.multiquery = multiquery
-        if not multiquery:
+        self.num_kv = num_kv
+        if num_kv == 0:
             self.linear_keys = skip_init(
                 nn.Linear,
                 in_features=model_dim,
                 out_features=model_dim,
                 bias=add_qkvbias,
             )
             self.linear_values = skip_init(
@@ -174,21 +174,21 @@
                 out_features=model_dim,
                 bias=add_qkvbias,
             )
         else:
             self.linear_keys = skip_init(
                 nn.Linear,
                 in_features=model_dim,
-                out_features=self.dim_per_head,
+                out_features=self.dim_per_head * self.num_kv,
                 bias=add_qkvbias,
             )
             self.linear_values = skip_init(
                 nn.Linear,
                 in_features=model_dim,
-                out_features=self.dim_per_head,
+                out_features=self.dim_per_head * self.num_kv,
                 bias=add_qkvbias,
             )
         self.linear_query = skip_init(
             nn.Linear, in_features=model_dim, out_features=model_dim, bias=add_qkvbias
         )
         self.softmax = nn.Softmax(dim=-1)
         self.dropout = nn.Dropout(dropout)
@@ -315,14 +315,19 @@
                 query = query.transpose(1, 2)
                 key = key.transpose(1, 2)
                 query, key = apply_rotary_emb(query, key, rope=rope)
                 query = query.transpose(1, 2)
                 key = key.transpose(1, 2)
         # 2) Calculate and scale scores.
         query /= math.sqrt(self.dim_per_head)
+        # expand key on heads dimension when it's less than query heads (multi-query variant)
+        key = key.view(key.size(0), -1, 1, key.size(2), key.size(3)).repeat(
+            1, 1, query.size(1) // key.size(1), 1, 1
+        )
+        key = key.view(key.size(0), query.size(1), key.size(3), key.size(4))
         # batch x num_heads x query_len x key_len
         scores = torch.matmul(query, key.transpose(2, 3))
 
         if self.relative_positions_embeddings is not None:
             key_len = key.size(2)
             # 1 or key_len x key_len
             relative_positions_matrix = gen_relative_positions(
@@ -346,15 +351,19 @@
             mask = mask.expand(-1, self.head_count, -1, -1)
             # now mask and scores have the same shape
             scores = scores.masked_fill(mask, -1e18)
 
         # 3) Apply attention dropout and compute context vectors.
         attn = self.softmax(scores).to(query.dtype)
         drop_attn = self.dropout(attn)
-
+        # expand value on heads dimension when it's less than query heads (multi-query variant)
+        value = value.view(value.size(0), -1, 1, value.size(2), value.size(3)).repeat(
+            1, 1, query.size(1) // value.size(1), 1, 1
+        )
+        value = value.view(value.size(0), query.size(1), value.size(3), value.size(4))
         context_original = torch.matmul(drop_attn, value)
 
         if self.relative_positions_embeddings is not None:
             # We use the same embeddings for key and value
             relations_values = relations_keys
             context_original.add_(relative_matmul(drop_attn, relations_values, False))
```

### Comparing `OpenNMT-py-3.2.0/onmt/modules/position_ffn.py` & `OpenNMT-py-3.3/onmt/modules/position_ffn.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/rmsnorm.py` & `OpenNMT-py-3.3/onmt/modules/rmsnorm.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/sparse_activations.py` & `OpenNMT-py-3.3/onmt/modules/sparse_activations.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/sparse_losses.py` & `OpenNMT-py-3.3/onmt/modules/sparse_losses.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/sru.py` & `OpenNMT-py-3.3/onmt/modules/sru.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/stacked_rnn.py` & `OpenNMT-py-3.3/onmt/modules/stacked_rnn.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/structured_attention.py` & `OpenNMT-py-3.3/onmt/modules/structured_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/util_class.py` & `OpenNMT-py-3.3/onmt/modules/util_class.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/modules/weight_norm.py` & `OpenNMT-py-3.3/onmt/modules/weight_norm.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/opts.py` & `OpenNMT-py-3.3/onmt/opts.py`

 * *Files 0% similar despite different names*

```diff
@@ -581,27 +581,25 @@
     )
 
     group.add(
         "--encoder_type",
         "-encoder_type",
         type=str,
         default="rnn",
-        choices=["rnn", "brnn", "ggnn", "mean", "transformer", "cnn", "transformer_lm"],
         help="Type of encoder layer to use. Non-RNN layers "
-        "are experimental. Options are "
+        "are experimental. Default options are "
         "[rnn|brnn|ggnn|mean|transformer|cnn|transformer_lm].",
     )
     group.add(
         "--decoder_type",
         "-decoder_type",
         type=str,
         default="rnn",
-        choices=["rnn", "transformer", "cnn", "transformer_lm"],
         help="Type of decoder layer to use. Non-RNN layers "
-        "are experimental. Options are "
+        "are experimental. Default options are "
         "[rnn|transformer|cnn|transformer].",
     )
 
     # Freeze Encoder and/or Decoder
     group.add(
         "--freeze_encoder",
         "-freeze_encoder",
@@ -838,30 +836,43 @@
         help="Add bias to nn.linear of Query/Key/Value in MHA"
         "Note: this will add bias to output proj layer too",
     )
     group.add(
         "--multiquery",
         "-multiquery",
         action="store_true",
-        help="Use MultiQUery attention" "Note: https://arxiv.org/pdf/1911.02150.pdf",
+        help="Use MultiQuery attention" "Note: https://arxiv.org/pdf/1911.02150.pdf",
+    )
+    group.add(
+        "--num_kv",
+        "-num_kv",
+        type=int,
+        default=0,
+        help="Number of heads for KV in the variant of MultiQuery attention (egs: Falcon 40B)",
     )
     group.add(
         "--add_ffnbias",
         "-add_ffnbias",
         action="store_true",
         help="Add bias to nn.linear of Position_wise FFN",
     )
     group.add(
         "--parallel_residual",
         "-parallel_residual",
         action="store_true",
         help="Use Parallel residual in Decoder Layer"
         "Note: this is used by GPT-J / Falcon Architecture",
     )
-
+    group.add(
+        "--shared_layer_norm",
+        "-shared_layer_norm",
+        action="store_true",
+        help="Use a shared layer_norm in parallel residual attention"
+        "Note: must be true for Falcon 7B / false for Falcon 40B",
+    )
     # Alignement options
     group = parser.add_argument_group("Model - Alignement")
     group.add(
         "--lambda_align",
         "-lambda_align",
         type=float,
         default=0.0,
@@ -1012,14 +1023,22 @@
         default="model",
         help="Model filename (the model will be saved as "
         "<save_model>_N.pt where N is the number "
         "of steps",
     )
 
     group.add(
+        "--save_format",
+        "-save_format",
+        default="pytorch",
+        choices=["pytorch", "safetensors"],
+        help="Format to save the model weights",
+    )
+
+    group.add(
         "--save_checkpoint_steps",
         "-save_checkpoint_steps",
         type=int,
         default=5000,
         help="""Save a checkpoint every X steps""",
     )
     group.add(
@@ -1110,32 +1129,14 @@
         "--lora_dropout",
         "-lora_dropout",
         type=float,
         default=0.0,
         help="rule of thumb: same value as in main model",
     )
 
-    group.add(
-        "--quant_layers",
-        "-quant_layers",
-        default=[],
-        nargs="+",
-        type=str,
-        help="list of layers to be compressed in 4/8bit.",
-    )
-
-    group.add(
-        "--quant_type",
-        "-quant_type",
-        default="bnb_8bit",
-        choices=["bnb_8bit", "bnb_FP4", "bnb_NF4"],
-        type=str,
-        help="Type of compression.",
-    )
-
     _add_reproducibility_opts(parser)
 
     # Init options
     group = parser.add_argument_group("Initialization")
     group.add(
         "--param_init",
         "-param_init",
@@ -1510,22 +1511,44 @@
         type=int,
         default=200,
         help="""number of mini-batches loaded in advance to avoid the
                    GPU waiting during the refilling of the bucket.""",
     )
 
 
+def _add_quant_opts(parser):
+    group = parser.add_argument_group("Quant options")
+    group.add(
+        "--quant_layers",
+        "-quant_layers",
+        default=[],
+        nargs="+",
+        type=str,
+        help="list of layers to be compressed in 4/8bit.",
+    )
+
+    group.add(
+        "--quant_type",
+        "-quant_type",
+        default="bnb_8bit",
+        choices=["bnb_8bit", "bnb_FP4", "bnb_NF4"],
+        type=str,
+        help="Type of compression.",
+    )
+
+
 def train_opts(parser):
     """All options used in train."""
     # options relate to data preprare
     dynamic_prepare_opts(parser, build_vocab_only=False)
     # options relate to train
     model_opts(parser)
     _add_train_general_opts(parser)
     _add_train_dynamic_data(parser)
+    _add_quant_opts(parser)
 
 
 def _add_decoding_opts(parser):
     group = parser.add_argument_group("Beam Search")
     beam_size = group.add(
         "--beam_size", "-beam_size", type=int, default=5, help="Beam size"
     )
@@ -1805,14 +1828,16 @@
             choices=AVAILABLE_TRANSFORMS.keys(),
             help="Default transform pipeline to apply to data.",
         )
 
         # Adding options related to Transforms
         _add_dynamic_transform_opts(parser)
 
+    _add_quant_opts(parser)
+
 
 # Copyright 2016 The Chromium Authors. All rights reserved.
 # Use of this source code is governed by a BSD-style license that can be
 # found in the LICENSE file.
 
 
 class StoreLoggingLevelAction(configargparse.Action):
```

### Comparing `OpenNMT-py-3.2.0/onmt/scorers/__init__.py` & `OpenNMT-py-3.3/onmt/scorers/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/scorers/scorer.py` & `OpenNMT-py-3.3/onmt/scorers/scorer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_attention.py` & `OpenNMT-py-3.3/onmt/tests/test_attention.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_beam_search.py` & `OpenNMT-py-3.3/onmt/tests/test_beam_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_copy_generator.py` & `OpenNMT-py-3.3/onmt/tests/test_copy_generator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_data_prepare.py` & `OpenNMT-py-3.3/onmt/tests/test_data_prepare.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 class TestData(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super(TestData, self).__init__(*args, **kwargs)
         self.opt = default_opts
 
     def dataset_build(self, opt):
         try:
-            prepare_transforms_vocabs(opt)
+            prepare_transforms_vocabs(opt, {})
         except SystemExit as err:
             print(err)
         except IOError as err:
             if opt.skip_empty_level != "error":
                 raise err
             else:
                 print(f"Catched IOError: {err}")
```

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_embeddings.py` & `OpenNMT-py-3.3/onmt/tests/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_events.py` & `OpenNMT-py-3.3/onmt/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_greedy_search.py` & `OpenNMT-py-3.3/onmt/tests/test_greedy_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_models.py` & `OpenNMT-py-3.3/onmt/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_subword_marker.py` & `OpenNMT-py-3.3/onmt/tests/test_subword_marker.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_text_utils.py` & `OpenNMT-py-3.3/onmt/tests/test_text_utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_transform.py` & `OpenNMT-py-3.3/onmt/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_translation_server.py` & `OpenNMT-py-3.3/onmt/tests/test_translation_server.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/tests/test_translator.py` & `OpenNMT-py-3.3/onmt/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/train_single.py` & `OpenNMT-py-3.3/onmt/train_single.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,18 +21,16 @@
 from onmt.utils.optimizers import Optimizer
 from onmt.utils.misc import set_random_seed
 from onmt.trainer import build_trainer
 from onmt.models import build_model_saver
 from onmt.modules.embeddings import prepare_pretrained_embeddings
 
 
-def prepare_transforms_vocabs(opt):
+def prepare_transforms_vocabs(opt, transforms_cls):
     """Prepare or dump transforms before training."""
-    transforms_cls = get_transforms_cls(opt._all_transform)
-
     # if transform + options set in 'valid' we need to copy in main
     # transform / options for scoring considered as inference
     validset_transforms = opt.data.get("valid", {}).get("transforms", None)
     if validset_transforms:
         opt.transforms = validset_transforms
         if opt.data.get("valid", {}).get("tgt_prefix", None):
             opt.tgt_prefix = opt.data.get("valid", {}).get("tgt_prefix", None)
@@ -62,26 +60,30 @@
         logger.info("Sample saved, please check it before restart training.")
         sys.exit()
     logger.info(
         "The first 10 tokens of the vocabs are:"
         f"{vocabs_to_dict(vocabs)['src'][0:10]}"
     )
     logger.info(f"The decoder start token is: {opt.decoder_start_token}")
-    return vocabs, transforms_cls
+    return vocabs
 
 
 def _init_train(opt):
-    """Common initilization stuff for all training process."""
+    """Common initilization stuff for all training process.
+    We need to build or rebuild the vocab in 3 cases:
+    - training from scratch (train_from is false)
+    - resume training but transforms have changed
+    - resume training but vocab file has been modified
+    """
     ArgumentParser.validate_prepare_opts(opt)
-
+    transforms_cls = get_transforms_cls(opt._all_transform)
     if opt.train_from:
         # Load checkpoint if we resume from a previous training.
         checkpoint = load_checkpoint(ckpt_path=opt.train_from)
         vocabs = dict_to_vocabs(checkpoint["vocab"])
-        transforms_cls = get_transforms_cls(opt._all_transform)
         if (
             hasattr(checkpoint["opt"], "_all_transform")
             and len(
                 opt._all_transform.symmetric_difference(
                     checkpoint["opt"]._all_transform
                 )
             )
@@ -91,21 +93,21 @@
             new_transf = opt._all_transform.difference(checkpoint["opt"]._all_transform)
             old_transf = checkpoint["opt"]._all_transform.difference(opt._all_transform)
             if len(new_transf) != 0:
                 _msg += f" +{new_transf}"
             if len(old_transf) != 0:
                 _msg += f" -{old_transf}."
             logger.warning(_msg)
-            vocabs, transforms_cls = prepare_transforms_vocabs(opt)
+            vocabs = prepare_transforms_vocabs(opt, transforms_cls)
         if opt.update_vocab:
             logger.info("Updating checkpoint vocabulary with new vocabulary")
-            vocabs, transforms_cls = prepare_transforms_vocabs(opt)
+            vocabs = prepare_transforms_vocabs(opt, transforms_cls)
     else:
         checkpoint = None
-        vocabs, transforms_cls = prepare_transforms_vocabs(opt)
+        vocabs = prepare_transforms_vocabs(opt, transforms_cls)
 
     return checkpoint, vocabs, transforms_cls
 
 
 def configure_process(opt, device_id):
     if device_id >= 0:
         torch.cuda.set_device(device_id)
@@ -145,58 +147,47 @@
             model_opt.freeze_encoder = opt.freeze_encoder
             model_opt.freeze_decoder = opt.freeze_decoder
     else:
         model_opt = opt
     return model_opt
 
 
-def _build_valid_iter(opt, transforms_cls, vocabs):
-    """Build iterator used for validation."""
-    valid_iter = build_dynamic_dataset_iter(
-        opt, transforms_cls, vocabs, task=CorpusTask.VALID, copy=opt.copy_attn
-    )
-    return valid_iter
-
-
-def _build_train_iter(opt, transforms_cls, vocabs, stride=1, offset=0):
-    """Build training iterator."""
-    train_iter = build_dynamic_dataset_iter(
-        opt,
-        transforms_cls,
-        vocabs,
-        task=CorpusTask.TRAIN,
-        copy=opt.copy_attn,
-        stride=stride,
-        offset=offset,
-    )
-    return train_iter
-
-
 def main(opt, device_id):
     """Start training on `device_id`."""
     # NOTE: It's important that ``opt`` has been validated and updated
     # at this point.
 
     configure_process(opt, device_id)
     init_logger(opt.log_file)
     checkpoint, vocabs, transforms_cls = _init_train(opt)
     model_opt = _get_model_opts(opt, checkpoint=checkpoint)
 
     # Build model.
     model = build_model(model_opt, opt, vocabs, checkpoint)
 
     model.count_parameters(log=logger.info)
-    trainable, non_trainable = 0, 0
+    trainable = {
+        "torch.float32": 0,
+        "torch.float16": 0,
+        "torch.uint8": 0,
+        "torch.int8": 0,
+    }
+    non_trainable = {
+        "torch.float32": 0,
+        "torch.float16": 0,
+        "torch.uint8": 0,
+        "torch.int8": 0,
+    }
     for n, p in model.named_parameters():
         if p.requires_grad:
-            trainable += p.numel()
+            trainable[str(p.dtype)] += p.numel()
         else:
-            non_trainable += p.numel()
-    logger.info("Trainable parameters = %d" % trainable)
-    logger.info("Non trainable parameters = %d" % non_trainable)
+            non_trainable[str(p.dtype)] += p.numel()
+    logger.info("Trainable parameters = %s" % str(trainable))
+    logger.info("Non trainable parameters = %s" % str(non_trainable))
     logger.info(" * src vocab size = %d" % len(vocabs["src"]))
     logger.info(" * tgt vocab size = %d" % len(vocabs["tgt"]))
     if "src_feats" in vocabs:
         for i, feat_vocab in enumerate(vocabs["src_feats"]):
             logger.info(f"* src_feat {i} vocab size = {len(feat_vocab)}")
 
     # Build optimizer.
@@ -207,24 +198,29 @@
     # Build model saver
     model_saver = build_model_saver(model_opt, opt, model, vocabs, optim)
 
     trainer = build_trainer(
         opt, device_id, model, vocabs, optim, model_saver=model_saver
     )
 
-    _train_iter = _build_train_iter(
+    _train_iter = build_dynamic_dataset_iter(
         opt,
         transforms_cls,
         vocabs,
+        task=CorpusTask.TRAIN,
+        copy=opt.copy_attn,
         stride=max(1, len(opt.gpu_ranks)),
         offset=max(0, device_id),
     )
     train_iter = IterOnDevice(_train_iter, device_id)
 
-    valid_iter = _build_valid_iter(opt, transforms_cls, vocabs)
+    valid_iter = build_dynamic_dataset_iter(
+        opt, transforms_cls, vocabs, task=CorpusTask.VALID, copy=opt.copy_attn
+    )
+
     if valid_iter is not None:
         valid_iter = IterOnDevice(valid_iter, device_id)
 
     if len(opt.gpu_ranks):
         logger.info("Starting training on GPU: %s" % opt.gpu_ranks)
     else:
         logger.info("Starting training on CPU, could be very slow")
```

### Comparing `OpenNMT-py-3.2.0/onmt/trainer.py` & `OpenNMT-py-3.3/onmt/trainer.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/__init__.py` & `OpenNMT-py-3.3/onmt/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/bart.py` & `OpenNMT-py-3.3/onmt/transforms/bart.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/clean.py` & `OpenNMT-py-3.3/onmt/transforms/clean.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/docify.py` & `OpenNMT-py-3.3/onmt/transforms/docify.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/features.py` & `OpenNMT-py-3.3/onmt/transforms/features.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/fuzzymatch.py` & `OpenNMT-py-3.3/onmt/transforms/fuzzymatch.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/inlinetags.py` & `OpenNMT-py-3.3/onmt/transforms/inlinetags.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from onmt.utils.logging import logger
 from onmt.transforms import register_transform
 from .transform import Transform
-
 import random
 import ahocorasick
 import string
-from typing import Tuple
 
 
 class InlineTagger(object):
     """Class for augmenting source and target sentences
     with inline tags (placeholders).
 
     It requires a prepared tab-delimited dictionary of source-target
```

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/misc.py` & `OpenNMT-py-3.3/onmt/transforms/misc.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/normalize.py` & `OpenNMT-py-3.3/onmt/transforms/normalize.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/sampling.py` & `OpenNMT-py-3.3/onmt/transforms/sampling.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/tokenize.py` & `OpenNMT-py-3.3/onmt/transforms/tokenize.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/transform.py` & `OpenNMT-py-3.3/onmt/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/transforms/uppercase.py` & `OpenNMT-py-3.3/onmt/transforms/uppercase.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/__init__.py` & `OpenNMT-py-3.3/onmt/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/beam_search.py` & `OpenNMT-py-3.3/onmt/translate/beam_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/decode_strategy.py` & `OpenNMT-py-3.3/onmt/translate/decode_strategy.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/greedy_search.py` & `OpenNMT-py-3.3/onmt/translate/greedy_search.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/penalties.py` & `OpenNMT-py-3.3/onmt/translate/penalties.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/process_zh.py` & `OpenNMT-py-3.3/onmt/translate/process_zh.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/translation.py` & `OpenNMT-py-3.3/onmt/translate/translation.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/translation_server.py` & `OpenNMT-py-3.3/onmt/translate/translation_server.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/translate/translator.py` & `OpenNMT-py-3.3/onmt/translate/translator.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/__init__.py` & `OpenNMT-py-3.3/onmt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/alignment.py` & `OpenNMT-py-3.3/onmt/utils/alignment.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/cnn_factory.py` & `OpenNMT-py-3.3/onmt/utils/cnn_factory.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/distributed.py` & `OpenNMT-py-3.3/onmt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/earlystopping.py` & `OpenNMT-py-3.3/onmt/utils/earlystopping.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/logging.py` & `OpenNMT-py-3.3/onmt/utils/logging.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/loss.py` & `OpenNMT-py-3.3/onmt/utils/loss.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/misc.py` & `OpenNMT-py-3.3/onmt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/optimizers.py` & `OpenNMT-py-3.3/onmt/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/parse.py` & `OpenNMT-py-3.3/onmt/utils/parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -303,14 +303,16 @@
             raise ValueError(
                 "Cannot use absolute and relative position encoding at the"
                 "same time. Use either --position_encoding=true for legacy"
                 "absolute position encoding or --max_realtive_positions with"
                 " -1 for Rotary, or > 0 for Relative Position Representations"
                 "as in https://arxiv.org/pdf/1803.02155.pdf"
             )
+        if model_opt.multiquery and model_opt.num_kv == 0:
+            model_opt.num_kv = 1
 
     @classmethod
     def ckpt_model_opts(cls, ckpt_opt):
         # Load default opt values, then overwrite with the opts in
         # the checkpoint. That way, if there are new options added,
         # the defaults are used.
         opt = cls.defaults(opts.model_opts)
```

### Comparing `OpenNMT-py-3.2.0/onmt/utils/report_manager.py` & `OpenNMT-py-3.3/onmt/utils/report_manager.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/scoring_utils.py` & `OpenNMT-py-3.3/onmt/utils/scoring_utils.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/onmt/utils/statistics.py` & `OpenNMT-py-3.3/onmt/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `OpenNMT-py-3.2.0/setup.py` & `OpenNMT-py-3.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,25 @@
     long_description = f.read()
 
 setup(
     name="OpenNMT-py",
     description="A python implementation of OpenNMT",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="3.2.0",
+    version="3.3",
     packages=find_packages(),
     project_urls={
         "Documentation": "http://opennmt.net/OpenNMT-py/",
         "Forum": "http://forum.opennmt.net/",
         "Gitter": "https://gitter.im/OpenNMT/OpenNMT-py",
         "Source": "https://github.com/OpenNMT/OpenNMT-py/",
     },
     python_requires=">=3.8",
     install_requires=[
-        "torch>=1.13,<2",
+        "torch>=1.13,<2.1",
         "configargparse",
         "ctranslate2>=3.2,<4",
         "tensorboard>=2.3",
         "flask",
         "waitress",
         "pyonmttok>=1.35,<2",
         "pyyaml",
```

