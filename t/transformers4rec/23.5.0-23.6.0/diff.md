# Comparing `tmp/transformers4rec-23.5.0.tar.gz` & `tmp/transformers4rec-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transformers4rec-23.5.0.tar", last modified: Wed May 31 14:39:50 2023, max compression
+gzip compressed data, was "transformers4rec-23.6.0.tar", last modified: Thu Jun 22 20:59:39 2023, max compression
```

## Comparing `transformers4rec-23.5.0.tar` & `transformers4rec-23.6.0.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/CLA.md
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/_images/
--rw-r--r--   0 runner    (1001) docker     (123)    60445 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/DP_DDP_perf.png
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/nlp_x_recsys.png
--rw-r--r--   0 runner    (1001) docker     (123)    57700 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/pipeline.png
--rw-r--r--   0 runner    (1001) docker     (123)   139511 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/preproc_data_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/sequential_rec.png
--rw-r--r--   0 runner    (1001) docker     (123)   123737 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/_images/transformers4rec_metaarchitecture.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/merlin_standard_lib/
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/merlin_standard_lib/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34895 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/proto/schema_bp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/merlin_standard_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/schema/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/schema/tag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/merlin_standard_lib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/merlin_standard_lib/utils/embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/base_external.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/base_merlin.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/nvtabular.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/pytorch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.476529 transformers4rec-23.5.0/tests/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/integration/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/integration/notebooks/test_getting_started_session_based.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/integration/notebooks/test_notebooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/assets/data_schema/
--rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/data_schema/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/data_schema/data_schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/data_schema/data_seq.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/assets/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/config/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/config/test_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/config/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/data/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/data/testing/tabular_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/testing/tabular_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/testing/tabular_data/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/data/testing/test_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.480528 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/block/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/block/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/block/test_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/test_sequential.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/features/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/model/test_head.py
--rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/model/test_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/tabular/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/tabular/test_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/tabular/test_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_dataloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    10386 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_public_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_ranking_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_readme.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_torchscript.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_torchscript_with_topk.py
--rw-r--r--   0 runner    (1001) docker     (123)    20084 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/test_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/utils/test_schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/torch/utils/test_torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.484529 transformers4rec-23.5.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/utils/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tests/unit/utils/test_padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/config/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/config/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12661 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/config/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/data/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/data/testing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/
--rw-r--r--   0 runner    (1001) docker     (123)   279958 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/data.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/data/yoochoose.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/torch/
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/torch/block/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/block/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/block/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/block/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/block/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec/torch/features/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    20993 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    11125 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/features/text.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)    35959 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/masking.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/torch/model/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32200 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    27439 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/model/prediction_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/ranking_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/torch/tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/tabular/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/tabular/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/tabular/transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    35389 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/examples_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/padding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16202 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/torch/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.492529 transformers4rec-23.5.0/transformers4rec/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/transformers4rec/utils/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:50.488529 transformers4rec-23.5.0/transformers4rec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-31 14:39:50.000000 transformers4rec-23.5.0/transformers4rec.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-05-31 14:39:30.000000 transformers4rec-23.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/CLA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13359 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    60445 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/_images/DP_DDP_perf.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/_images/nlp_x_recsys.png
+-rw-r--r--   0 runner    (1001) docker     (123)    57700 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/_images/pipeline.png
+-rw-r--r--   0 runner    (1001) docker     (123)   139511 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/_images/preproc_data_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53017 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/_images/sequential_rec.png
+-rw-r--r--   0 runner    (1001) docker     (123)   123737 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/_images/transformers4rec_metaarchitecture.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/merlin_standard_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/merlin_standard_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/merlin_standard_lib/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/merlin_standard_lib/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34895 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/merlin_standard_lib/proto/schema_bp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/merlin_standard_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/merlin_standard_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/merlin_standard_lib/schema/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/merlin_standard_lib/schema/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/merlin_standard_lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/merlin_standard_lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/merlin_standard_lib/utils/embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/requirements/base_external.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/requirements/base_merlin.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/requirements/nvtabular.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/requirements/pytorch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.062079 transformers4rec-23.6.0/tests/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/tests/integration/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/integration/notebooks/test_getting_started_session_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/integration/notebooks/test_notebooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/tests/unit/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.066079 transformers4rec-23.6.0/tests/unit/assets/data_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/assets/data_schema/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/assets/data_schema/data_schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/assets/data_schema/data_seq.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/assets/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/config/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/config/test_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/config/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/data/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/data/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/data/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/data/testing/tabular_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/data/testing/tabular_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/data/testing/tabular_data/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/data/testing/test_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/merlin_standard_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/merlin_standard_lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/merlin_standard_lib/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/merlin_standard_lib/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/merlin_standard_lib/schema/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/torch/block/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/block/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/block/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/block/test_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/torch/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/features/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/features/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/features/test_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/features/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/torch/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/model/test_head.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15579 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/model/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/torch/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/tabular/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/tabular/test_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11257 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/tabular/test_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_dataloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10388 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_public_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_ranking_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_readme.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_torchscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_torchscript_with_topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/test_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.070079 transformers4rec-23.6.0/tests/unit/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/utils/test_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/torch/utils/test_torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.074080 transformers4rec-23.6.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/utils/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tests/unit/utils/test_padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3794 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/transformers4rec/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/transformers4rec/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.074080 transformers4rec-23.6.0/transformers4rec/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/config/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/config/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21097 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/config/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.074080 transformers4rec-23.6.0/transformers4rec/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5199 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.074080 transformers4rec-23.6.0/transformers4rec/data/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105788 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.074080 transformers4rec-23.6.0/transformers4rec/data/testing/music_streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)   279958 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/music_streaming/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/music_streaming/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/music_streaming/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.074080 transformers4rec-23.6.0/transformers4rec/data/testing/tabular_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/tabular_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42012 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/tabular_data/data.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/tabular_data/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/testing/tabular_data/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/data/yoochoose.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.074080 transformers4rec-23.6.0/transformers4rec/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/transformers4rec/torch/block/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/block/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14635 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/block/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/block/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/block/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/transformers4rec/torch/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/features/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/features/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28462 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/features/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11300 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/features/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/features/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/features/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36561 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/masking.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/transformers4rec/torch/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32200 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33390 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/model/prediction_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11734 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/ranking_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/transformers4rec/torch/tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6568 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/tabular/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22373 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/tabular/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/tabular/transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36492 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/transformers4rec/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19533 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/utils/examples_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/utils/padding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6369 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/utils/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16754 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/torch/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.078080 transformers4rec-23.6.0/transformers4rec/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13134 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/transformers4rec/utils/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:59:39.074080 transformers4rec-23.6.0/transformers4rec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-06-22 20:59:39.000000 transformers4rec-23.6.0/transformers4rec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-06-22 20:59:39.000000 transformers4rec-23.6.0/transformers4rec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:59:39.000000 transformers4rec-23.6.0/transformers4rec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-22 20:59:39.000000 transformers4rec-23.6.0/transformers4rec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 20:59:39.000000 transformers4rec-23.6.0/transformers4rec.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    81319 2023-06-22 20:59:17.000000 transformers4rec-23.6.0/versioneer.py
```

### Comparing `transformers4rec-23.5.0/.pre-commit-config.yaml` & `transformers4rec-23.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/CLA.md` & `transformers4rec-23.6.0/CLA.md`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/CONTRIBUTING.md` & `transformers4rec-23.6.0/CONTRIBUTING.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     - If you need more context on a particular issue, please ask and we shall
     provide.
 
 ## Code contributions
 
 ### Your first issue
 
-1. Read the project's [README.md](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/main/README.md)
+1. Read the project's [README.md](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/stable/README.md)
     to learn how to setup the development environment
 2. Find an issue to work on. The best way is to look for the [good first issue](https://github.com/NVIDIA-Merlin/Transformers4Rec/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
     or [help wanted](https://github.com/NVIDIA-Merlin/Transformers4Rec/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) labels
 3. Comment on the issue saying you are going to work on it
 4. Code! Make sure to update unit tests!
 5. When done, [create your pull request](https://github.com/NVIDIA-Merlin/Transformers4Rec/compare)
 6. Verify that CI passes all [status checks](https://help.github.com/articles/about-status-checks/). Fix if needed
```

### Comparing `transformers4rec-23.5.0/LICENSE` & `transformers4rec-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/MANIFEST.in` & `transformers4rec-23.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/PKG-INFO` & `transformers4rec-23.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers4rec
-Version: 23.5.0
+Version: 23.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/Transformers4Rec
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,16 @@
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 # [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/)
 
 [![PyPI](https://img.shields.io/pypi/v/Transformers4Rec?color=orange&label=version)](https://pypi.python.org/pypi/Transformers4Rec)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/Transformers4Rec)](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/Transformers4Rec/main/README.html)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/Transformers4Rec)](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/stable/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/Transformers4Rec/stable/README.html)
 
 Transformers4Rec is a flexible and efficient library for sequential and session-based recommendation and can work with PyTorch.
 
 The library works as a bridge between natural language processing (NLP) and recommender systems (RecSys) by integrating with one of the most popular NLP frameworks, [Hugging Face Transformers](https://github.com/huggingface/transformers) (HF).
 Transformers4Rec makes state-of-the-art transformer architectures available for RecSys researchers and industry practitioners.
 
 The following figure shows the use of the library in a recommender system.
@@ -70,15 +70,15 @@
 You can normalize and combine interaction and sequence-level input features in configurable ways.
 
 - **Seamless preprocessing and feature engineering**: As part of the Merlin ecosystem, Transformers4Rec is integrated with [NVTabular](https://github.com/NVIDIA-Merlin/NVTabular) and [Triton Inference Server](https://github.com/triton-inference-server/server).
 These components enable you to build a fully GPU-accelerated pipeline for sequential and session-based recommendation.
 NVTabular has common preprocessing operations for session-based recommendation and exports a dataset schema.
 The schema is compatible with Transformers4Rec so that input features can be configured automatically.
 You can export your trained models to serve with Triton Inference Server in a single pipeline that includes online feature preprocessing and model inference.
-For more information, refer to [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/main/pipeline.html).
+For more information, refer to [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/stable/pipeline.html).
 
 <img src="_images/pipeline.png" alt="GPU-accelerated Sequential and Session-based recommendation" style="width:600px;display:block;margin-left:auto;margin-right:auto;"/><br>
 <div style="text-align: center; margin: 20pt">
   <figcaption style="font-style: italic;">GPU-accelerated pipeline for Sequential and Session-based recommendation using NVIDIA Merlin components</figcaption>
 </div>
 
 ## Transformers4Rec Achievements
@@ -87,23 +87,23 @@
 The library provides higher accuracy for session-based recommendation than baseline algorithms and we performed extensive empirical analysis about the accuracy.
 These observations are published in our [ACM RecSys'21 paper](https://dl.acm.org/doi/10.1145/3460231.3474255).
 
 ## Sample Code: Defining and Training the Model
 
 Training a model with Transformers4Rec typically requires performing the following high-level steps:
 
-1. Provide the [schema](https://nvidia-merlin.github.io/Transformers4Rec/main/api/merlin_standard_lib.schema.html#merlin_standard_lib.schema.schema.Schema) and construct an input-module.
+1. Provide the [schema](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/merlin_standard_lib.schema.html#merlin_standard_lib.schema.schema.Schema) and construct an input-module.
 
    If you encounter session-based recommendation issues, you typically want to use the
-   [TabularSequenceFeatures](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.features.html#transformers4rec.torch.features.sequence.TabularSequenceFeatures)
+   [TabularSequenceFeatures](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.features.html#transformers4rec.torch.features.sequence.TabularSequenceFeatures)
    class because it merges context features with sequential features.
 
 2. Provide the prediction-tasks.
 
-   The tasks that are provided right out of the box are available from our [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.model.html#module-transformers4rec.torch.model.prediction_task).
+   The tasks that are provided right out of the box are available from our [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.model.html#module-transformers4rec.torch.model.prediction_task).
 
 3. Construct a transformer-body and convert this into a model.
 
 The following code sample shows how to define and train an XLNet model with PyTorch for next-item prediction task:
 
 ```python
 from transformers4rec import torch as tr
@@ -150,15 +150,15 @@
 model = tr.Model(head)
 ```
 
 > You can modify the preceding code to perform binary classification.
 > The masking in the input module can be set to `None` instead of `causal`.
 > When you define the head, you can replace the `NextItemPredictionTask`
 > with an instance of `BinaryClassificationTask`.
-> See the sample code in the [API documentation for the class](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.html#transformers4rec.torch.BinaryClassificationTask).
+> See the sample code in the [API documentation for the class](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.html#transformers4rec.torch.BinaryClassificationTask).
 
 ## Installation
 
 You can install Transformers4Rec with Pip, Conda, or run a Docker container.
 
 ### Installing Transformers4Rec Using Pip
 
@@ -194,29 +194,29 @@
     cudatoolkit=11.8 pytorch-cuda=11.8 `# NVIDIA CUDA version`
 ```
 
 ### Installing Transformers4Rec Using Docker
 
 Transformers4Rec is pre-installed in the `merlin-pytorch` container that is available from the NVIDIA GPU Cloud (NGC) catalog.
 
-Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
+Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/stable/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
 
 ## Notebook Examples and Tutorials
 
-The [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/main/pipeline.html) page
+The [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/stable/pipeline.html) page
 shows how to use Transformers4Rec and other Merlin libraries like NVTabular to build a complete recommender system.
 
 We have several [example](./examples) notebooks to help you build a recommender system or integrate Transformers4Rec into your system:
 
 - A getting started example that includes training a session-based model with an XLNET transformer architecture.
 - An end-to-end example that trains a model and takes the next step to serve inference with Triton Inference Server.
 - Another end-to-end example that trains and evaluates a session-based model on RNN and also serves inference with Triton Inference Server.
 - A notebook and scripts that reproduce the experiments presented in a paper for RecSys 2021.
 
 ## Feedback and Support
 
 If you'd like to make direct contributions to Transformers4Rec, refer to [Contributing to Transformers4Rec](CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin roadmap, we encourage you to share all the details regarding your recommender system pipeline by going to https://developer.nvidia.com/merlin-devzone-survey.
 
 If you're interested in learning more about how Transformers4Rec works, refer to our
-[Transformers4Rec documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/getting_started.html). We also have [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/api/modules.html) that outlines the specifics of the available modules and classes within Transformers4Rec.
+[Transformers4Rec documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/getting_started.html). We also have [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/modules.html) that outlines the specifics of the available modules and classes within Transformers4Rec.
```

### Comparing `transformers4rec-23.5.0/README.md` & `transformers4rec-23.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/)
 
 [![PyPI](https://img.shields.io/pypi/v/Transformers4Rec?color=orange&label=version)](https://pypi.python.org/pypi/Transformers4Rec)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/Transformers4Rec)](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/Transformers4Rec/main/README.html)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/Transformers4Rec)](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/stable/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/Transformers4Rec/stable/README.html)
 
 Transformers4Rec is a flexible and efficient library for sequential and session-based recommendation and can work with PyTorch.
 
 The library works as a bridge between natural language processing (NLP) and recommender systems (RecSys) by integrating with one of the most popular NLP frameworks, [Hugging Face Transformers](https://github.com/huggingface/transformers) (HF).
 Transformers4Rec makes state-of-the-art transformer architectures available for RecSys researchers and industry practitioners.
 
 The following figure shows the use of the library in a recommender system.
@@ -47,15 +47,15 @@
 You can normalize and combine interaction and sequence-level input features in configurable ways.
 
 - **Seamless preprocessing and feature engineering**: As part of the Merlin ecosystem, Transformers4Rec is integrated with [NVTabular](https://github.com/NVIDIA-Merlin/NVTabular) and [Triton Inference Server](https://github.com/triton-inference-server/server).
 These components enable you to build a fully GPU-accelerated pipeline for sequential and session-based recommendation.
 NVTabular has common preprocessing operations for session-based recommendation and exports a dataset schema.
 The schema is compatible with Transformers4Rec so that input features can be configured automatically.
 You can export your trained models to serve with Triton Inference Server in a single pipeline that includes online feature preprocessing and model inference.
-For more information, refer to [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/main/pipeline.html).
+For more information, refer to [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/stable/pipeline.html).
 
 <img src="_images/pipeline.png" alt="GPU-accelerated Sequential and Session-based recommendation" style="width:600px;display:block;margin-left:auto;margin-right:auto;"/><br>
 <div style="text-align: center; margin: 20pt">
   <figcaption style="font-style: italic;">GPU-accelerated pipeline for Sequential and Session-based recommendation using NVIDIA Merlin components</figcaption>
 </div>
 
 ## Transformers4Rec Achievements
@@ -64,23 +64,23 @@
 The library provides higher accuracy for session-based recommendation than baseline algorithms and we performed extensive empirical analysis about the accuracy.
 These observations are published in our [ACM RecSys'21 paper](https://dl.acm.org/doi/10.1145/3460231.3474255).
 
 ## Sample Code: Defining and Training the Model
 
 Training a model with Transformers4Rec typically requires performing the following high-level steps:
 
-1. Provide the [schema](https://nvidia-merlin.github.io/Transformers4Rec/main/api/merlin_standard_lib.schema.html#merlin_standard_lib.schema.schema.Schema) and construct an input-module.
+1. Provide the [schema](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/merlin_standard_lib.schema.html#merlin_standard_lib.schema.schema.Schema) and construct an input-module.
 
    If you encounter session-based recommendation issues, you typically want to use the
-   [TabularSequenceFeatures](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.features.html#transformers4rec.torch.features.sequence.TabularSequenceFeatures)
+   [TabularSequenceFeatures](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.features.html#transformers4rec.torch.features.sequence.TabularSequenceFeatures)
    class because it merges context features with sequential features.
 
 2. Provide the prediction-tasks.
 
-   The tasks that are provided right out of the box are available from our [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.model.html#module-transformers4rec.torch.model.prediction_task).
+   The tasks that are provided right out of the box are available from our [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.model.html#module-transformers4rec.torch.model.prediction_task).
 
 3. Construct a transformer-body and convert this into a model.
 
 The following code sample shows how to define and train an XLNet model with PyTorch for next-item prediction task:
 
 ```python
 from transformers4rec import torch as tr
@@ -127,15 +127,15 @@
 model = tr.Model(head)
 ```
 
 > You can modify the preceding code to perform binary classification.
 > The masking in the input module can be set to `None` instead of `causal`.
 > When you define the head, you can replace the `NextItemPredictionTask`
 > with an instance of `BinaryClassificationTask`.
-> See the sample code in the [API documentation for the class](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.html#transformers4rec.torch.BinaryClassificationTask).
+> See the sample code in the [API documentation for the class](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.html#transformers4rec.torch.BinaryClassificationTask).
 
 ## Installation
 
 You can install Transformers4Rec with Pip, Conda, or run a Docker container.
 
 ### Installing Transformers4Rec Using Pip
 
@@ -171,27 +171,27 @@
     cudatoolkit=11.8 pytorch-cuda=11.8 `# NVIDIA CUDA version`
 ```
 
 ### Installing Transformers4Rec Using Docker
 
 Transformers4Rec is pre-installed in the `merlin-pytorch` container that is available from the NVIDIA GPU Cloud (NGC) catalog.
 
-Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
+Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/stable/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
 
 ## Notebook Examples and Tutorials
 
-The [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/main/pipeline.html) page
+The [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/stable/pipeline.html) page
 shows how to use Transformers4Rec and other Merlin libraries like NVTabular to build a complete recommender system.
 
 We have several [example](./examples) notebooks to help you build a recommender system or integrate Transformers4Rec into your system:
 
 - A getting started example that includes training a session-based model with an XLNET transformer architecture.
 - An end-to-end example that trains a model and takes the next step to serve inference with Triton Inference Server.
 - Another end-to-end example that trains and evaluates a session-based model on RNN and also serves inference with Triton Inference Server.
 - A notebook and scripts that reproduce the experiments presented in a paper for RecSys 2021.
 
 ## Feedback and Support
 
 If you'd like to make direct contributions to Transformers4Rec, refer to [Contributing to Transformers4Rec](CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin roadmap, we encourage you to share all the details regarding your recommender system pipeline by going to https://developer.nvidia.com/merlin-devzone-survey.
 
 If you're interested in learning more about how Transformers4Rec works, refer to our
-[Transformers4Rec documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/getting_started.html). We also have [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/api/modules.html) that outlines the specifics of the available modules and classes within Transformers4Rec.
+[Transformers4Rec documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/getting_started.html). We also have [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/modules.html) that outlines the specifics of the available modules and classes within Transformers4Rec.
```

### Comparing `transformers4rec-23.5.0/_images/DP_DDP_perf.png` & `transformers4rec-23.6.0/_images/DP_DDP_perf.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/_images/nlp_x_recsys.png` & `transformers4rec-23.6.0/_images/nlp_x_recsys.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/_images/pipeline.png` & `transformers4rec-23.6.0/_images/pipeline.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/_images/preproc_data_example.png` & `transformers4rec-23.6.0/_images/preproc_data_example.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/_images/sequential_rec.png` & `transformers4rec-23.6.0/_images/sequential_rec.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/_images/transformers4rec_metaarchitecture.png` & `transformers4rec-23.6.0/_images/transformers4rec_metaarchitecture.png`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/merlin_standard_lib/__init__.py` & `transformers4rec-23.6.0/merlin_standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/merlin_standard_lib/proto/__init__.py` & `transformers4rec-23.6.0/merlin_standard_lib/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/merlin_standard_lib/proto/schema_bp.py` & `transformers4rec-23.6.0/merlin_standard_lib/proto/schema_bp.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/merlin_standard_lib/schema/__init__.py` & `transformers4rec-23.6.0/merlin_standard_lib/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/merlin_standard_lib/schema/schema.py` & `transformers4rec-23.6.0/merlin_standard_lib/schema/schema.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/merlin_standard_lib/schema/tag.py` & `transformers4rec-23.6.0/merlin_standard_lib/schema/tag.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/merlin_standard_lib/utils/__init__.py` & `transformers4rec-23.6.0/merlin_standard_lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/merlin_standard_lib/utils/embedding_utils.py` & `transformers4rec-23.6.0/merlin_standard_lib/utils/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/mypy.ini` & `transformers4rec-23.6.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/setup.cfg` & `transformers4rec-23.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/setup.py` & `transformers4rec-23.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/__init__.py` & `transformers4rec-23.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/conftest.py` & `transformers4rec-23.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/integration/notebooks/test_getting_started_session_based.py` & `transformers4rec-23.6.0/tests/integration/notebooks/test_getting_started_session_based.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/integration/notebooks/test_notebooks.py` & `transformers4rec-23.6.0/tests/integration/notebooks/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/assets/data_schema/data.parquet` & `transformers4rec-23.6.0/tests/unit/assets/data_schema/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/assets/data_schema/data_schema.pbtxt` & `transformers4rec-23.6.0/tests/unit/assets/data_schema/data_schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/assets/data_schema/data_seq.parquet` & `transformers4rec-23.6.0/tests/unit/assets/data_schema/data_seq.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt` & `transformers4rec-23.6.0/tests/unit/assets/data_schema/data_seq_schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/assets/schema.pbtxt` & `transformers4rec-23.6.0/tests/unit/assets/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/config/__init__.py` & `transformers4rec-23.6.0/tests/unit/config/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/config/test_schema.py` & `transformers4rec-23.6.0/tests/unit/config/test_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 from merlin.schema import Tags
 
 from merlin_standard_lib import categorical_cardinalities
 from merlin_standard_lib.utils.embedding_utils import get_embedding_sizes_from_schema
 
 
 def test_schema_from_yoochoose_schema(yoochoose_schema):
-    assert len(yoochoose_schema.column_names) == 22
+    assert len(yoochoose_schema.column_names) == 14
     assert len(yoochoose_schema.select_by_tag(Tags.CONTINUOUS).column_schemas) == 11
     assert len(yoochoose_schema.select_by_tag(Tags.CATEGORICAL).column_schemas) == 3
 
 
 def test_schema_cardinalities(yoochoose_schema):
     schema = yoochoose_schema
     assert categorical_cardinalities(schema) == {
```

### Comparing `transformers4rec-23.5.0/tests/unit/config/test_trainer.py` & `transformers4rec-23.6.0/tests/unit/config/test_trainer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/config/test_transformer.py` & `transformers4rec-23.6.0/tests/unit/config/test_transformer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/data/test_synthetic.py` & `transformers4rec-23.6.0/tests/unit/data/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/data/testing/tabular_data/test_dataset.py` & `transformers4rec-23.6.0/tests/unit/data/testing/tabular_data/test_dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/data/testing/test_dataset.py` & `transformers4rec-23.6.0/tests/unit/data/testing/test_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 def test_tabular_sequence_testing_data():
     assert isinstance(tabular_sequence_testing_data, ParquetDataset)
     assert tabular_sequence_testing_data.path.endswith("transformers4rec/data/testing/data.parquet")
     assert tabular_sequence_testing_data.schema_path.endswith(
         "transformers4rec/data/testing/schema.json"
     )
-    assert len(tabular_sequence_testing_data.schema) == 22
+    assert len(tabular_sequence_testing_data.schema) == 14
 
     torch_yoochoose_like = tabular_sequence_testing_data.torch_synthetic_data(
         num_rows=100, min_session_length=5, max_session_length=20
     )
 
     t4r_yoochoose_schema = tabular_sequence_testing_data.schema
```

### Comparing `transformers4rec-23.5.0/tests/unit/merlin_standard_lib/__init__.py` & `transformers4rec-23.6.0/tests/unit/merlin_standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/__init__.py` & `transformers4rec-23.6.0/tests/unit/merlin_standard_lib/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/merlin_standard_lib/schema/test_schema.py` & `transformers4rec-23.6.0/tests/unit/merlin_standard_lib/schema/test_schema.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/__init__.py` & `transformers4rec-23.6.0/tests/unit/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/_conftest.py` & `transformers4rec-23.6.0/tests/unit/torch/_conftest.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/block/__init__.py` & `transformers4rec-23.6.0/tests/unit/torch/block/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/block/test_base.py` & `transformers4rec-23.6.0/tests/unit/torch/block/test_base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/block/test_mlp.py` & `transformers4rec-23.6.0/tests/unit/torch/block/test_mlp.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/block/test_transformer.py` & `transformers4rec-23.6.0/tests/unit/torch/block/test_transformer.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/features/__init__.py` & `transformers4rec-23.6.0/tests/unit/torch/features/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/features/test_continuous.py` & `transformers4rec-23.6.0/tests/unit/torch/features/test_continuous.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/features/test_embedding.py` & `transformers4rec-23.6.0/tests/unit/torch/features/test_embedding.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/features/test_tabular.py` & `transformers4rec-23.6.0/tests/unit/torch/features/test_tabular.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/model/__init__.py` & `transformers4rec-23.6.0/tests/unit/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/model/test_head.py` & `transformers4rec-23.6.0/tests/unit/torch/model/test_head.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/model/test_model.py` & `transformers4rec-23.6.0/tests/unit/torch/model/test_model.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/tabular/__init__.py` & `transformers4rec-23.6.0/tests/unit/torch/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/tabular/test_aggregation.py` & `transformers4rec-23.6.0/tests/unit/torch/tabular/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/tabular/test_tabular.py` & `transformers4rec-23.6.0/tests/unit/torch/tabular/test_tabular.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/tabular/test_transformations.py` & `transformers4rec-23.6.0/tests/unit/torch/tabular/test_transformations.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_dataloader_utils.py` & `transformers4rec-23.6.0/tests/unit/torch/test_dataloader_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_experimental.py` & `transformers4rec-23.6.0/tests/unit/torch/test_experimental.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_losses.py` & `transformers4rec-23.6.0/tests/unit/torch/test_losses.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_masking.py` & `transformers4rec-23.6.0/tests/unit/torch/test_masking.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,29 +39,29 @@
 # Test only last item is masked when evaluating
 @pytest.mark.parametrize("task", lm_tasks)
 def test_mask_only_last_item_for_eval(torch_masking_inputs, task):
     hidden_dim = torch_masking_inputs["input_tensor"].size(2)
     lm = tr.masking.masking_registry[task](
         hidden_dim, padding_idx=torch_masking_inputs["padding_idx"]
     )
-    lm.compute_masked_targets(torch_masking_inputs["labels"], training=False)
+    lm.compute_masked_targets(torch_masking_inputs["labels"], training=False, testing=True)
     # get non padded last items
     non_padded_mask = torch_masking_inputs["labels"] != torch_masking_inputs["padding_idx"]
     rows_ids = torch.arange(
         torch_masking_inputs["labels"].size(0),
         dtype=torch.long,
         device=torch_masking_inputs["labels"].device,
     )
     last_item_sessions = non_padded_mask.sum(axis=1) - 1
     last_labels = torch_masking_inputs["labels"][rows_ids, last_item_sessions].flatten().numpy()
     # get the last labels from output
     trgt_pad = lm.masked_targets != torch_masking_inputs["padding_idx"]
     out_last = lm.masked_targets[trgt_pad].flatten().numpy()
     # check that only one item is masked for each session
-    assert lm.mask_schema.sum() == torch_masking_inputs["input_tensor"].size(0)
+    assert trgt_pad.sum() == torch_masking_inputs["input_tensor"].size(0)
     # check only the last non-paded item is masked
     assert all(last_labels == out_last)
 
 
 @pytest.mark.parametrize("task", lm_tasks)
 def test_mask_all_next_item_for_eval(torch_masking_inputs, task):
     hidden_dim = torch_masking_inputs["input_tensor"].size(2)
@@ -105,15 +105,15 @@
         device=torch_masking_inputs["labels"].device,
     )
     last_item_sessions = non_padded_mask.sum(axis=1) - 1
     last_labels = torch_masking_inputs["labels"][rows_ids, last_item_sessions].flatten().numpy()
     # last labels from output
     trgt_pad = lm.masked_targets != torch_masking_inputs["padding_idx"]
     out_last = lm.masked_targets[trgt_pad].flatten().numpy()
-    assert lm.mask_schema.sum() == torch_masking_inputs["input_tensor"].size(0)
+    assert trgt_pad.sum() == torch_masking_inputs["input_tensor"].size(0)
     assert all(last_labels == out_last)
 
 
 # Test at least one item is masked when training
 @pytest.mark.parametrize("task", lm_tasks)
 def test_at_least_one_masked_item_mlm(torch_masking_inputs, task):
     hidden_dim = torch_masking_inputs["input_tensor"].size(2)
```

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_public_api.py` & `transformers4rec-23.6.0/tests/unit/torch/test_public_api.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_readme.py` & `transformers4rec-23.6.0/tests/unit/torch/test_readme.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_torchscript.py` & `transformers4rec-23.6.0/tests/unit/torch/test_torchscript.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_torchscript_with_topk.py` & `transformers4rec-23.6.0/tests/unit/torch/test_torchscript_with_topk.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/test_trainer.py` & `transformers4rec-23.6.0/tests/unit/torch/test_trainer.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 import pytest
 import torch
 from merlin.schema import Schema
 
 import transformers4rec.torch as tr
 from transformers4rec.config import trainer
 from transformers4rec.config import transformer as tconf
+from transformers4rec.torch.ranking_metric import NDCGAt, RecallAt
 
 
 @pytest.mark.parametrize("batch_size", [16, 32])
 def test_set_train_eval_loaders_attributes(
     torch_yoochoose_like, torch_yoochoose_next_item_prediction_model, batch_size
 ):
     train_loader = torch.utils.data.DataLoader([torch_yoochoose_like], batch_size=batch_size)
@@ -324,14 +325,28 @@
                 "eval_/next-item/avg_precision_at_10",
                 "eval_/next-item/avg_precision_at_20",
                 "eval_/next-item/recall_at_10",
                 "eval_/next-item/recall_at_20",
             ],
         ),
         (
+            tr.NextItemPredictionTask(
+                weight_tying=False,
+                metrics=(
+                    NDCGAt(top_ks=[5, 10], labels_onehot=True),
+                    RecallAt(top_ks=[10], labels_onehot=True),
+                ),
+            ),
+            [
+                "eval_/next-item/ndcg_at_5",
+                "eval_/next-item/ndcg_at_10",
+                "eval_/next-item/recall_at_10",
+            ],
+        ),
+        (
             tr.BinaryClassificationTask("click", summary_type="mean"),
             [
                 "eval_/click/binary_classification_task/binary_accuracy",
                 "eval_/click/binary_classification_task/binary_precision",
                 "eval_/click/binary_classification_task/binary_recall",
             ],
         ),
@@ -343,15 +358,15 @@
         ),
     ],
 )
 def test_trainer_music_streaming(task_and_metrics):
     data = tr.data.music_streaming_testing_data
     schema = data.schema
     batch_size = 16
-    task, default_metric = task_and_metrics
+    task, expected_metrics = task_and_metrics
 
     inputs = tr.TabularSequenceFeatures.from_schema(
         schema,
         max_sequence_length=20,
         d_output=64,
         masking="mlm",
     )
@@ -384,21 +399,26 @@
     )
 
     recsys_trainer.train()
     eval_metrics = recsys_trainer.evaluate(eval_dataset=data.path, metric_key_prefix="eval")
     predictions = recsys_trainer.predict(data.path)
 
     assert isinstance(eval_metrics, dict)
-    assert set(default_metric).issubset(set(eval_metrics.keys()))
+    assert set(expected_metrics).issubset(set(eval_metrics.keys()))
     assert eval_metrics["eval_/loss"] is not None
 
     assert predictions is not None
+
+    DEFAULT_PREDICT_TOP_K = 100
+
     # 1000 is the total samples in the testing data
     if isinstance(task, tr.NextItemPredictionTask):
-        assert predictions.predictions.shape == (1000, task.target_dim)
+        top_predicted_item_ids, top_prediction_scores = predictions.predictions
+        assert top_predicted_item_ids.shape == (1000, DEFAULT_PREDICT_TOP_K)
+        assert top_prediction_scores.shape == (1000, DEFAULT_PREDICT_TOP_K)
     else:
         assert predictions.predictions.shape == (1000,)
 
 
 # This is broken out as a separate test since combining it leads to strange errors
 @pytest.mark.parametrize(
     "task_and_metrics",
@@ -554,25 +574,87 @@
 
     assert predictions is not None
     assert predictions.predictions["next-item"][0].shape == (1000, predict_top_k)
     assert predictions.predictions["play_percentage/regression_task"].shape == (1000,)
     assert predictions.predictions["click/binary_classification_task"].shape == (1000,)
 
 
-def test_trainer_trop_k_with_wrong_task():
+@pytest.mark.parametrize("predict_top_k", [20, None, "default"])
+def test_trainer_predict_topk(predict_top_k):
+    DEFAULT_PREDICT_TOP_K = 100
+
     data = tr.data.music_streaming_testing_data
     schema = data.schema
     batch_size = 16
-    predict_top_k = 20
 
-    task = tr.BinaryClassificationTask("click", summary_type="mean")
+    task = tr.NextItemPredictionTask(weight_tying=True)
     inputs = tr.TabularSequenceFeatures.from_schema(
         schema,
         max_sequence_length=20,
         d_output=64,
+        masking="clm",
+    )
+    transformer_config = tconf.XLNetConfig.build(64, 4, 2, 20)
+    model = transformer_config.to_torch_model(inputs, task)
+
+    additional_args = {}
+    if not isinstance(predict_top_k, str):
+        additional_args["predict_top_k"] = predict_top_k
+
+    args = trainer.T4RecTrainingArguments(
+        output_dir=".",
+        num_train_epochs=1,
+        per_device_train_batch_size=batch_size,
+        per_device_eval_batch_size=batch_size // 2,
+        data_loader_engine="merlin_dataloader",
+        max_sequence_length=20,
+        report_to=[],
+        debug=["r"],
+        **additional_args,
+    )
+
+    recsys_trainer = tr.Trainer(
+        model=model,
+        args=args,
+        schema=schema,
+        train_dataset_or_path=data.path,
+        eval_dataset_or_path=data.path,
+        test_dataset_or_path=data.path,
+        compute_metrics=True,
+    )
+
+    outputs = recsys_trainer.predict(data.path)
+
+    if predict_top_k is None:
+        assert outputs.predictions.shape[1] == 10001
+    else:
+        if predict_top_k == "default":
+            predict_top_k = DEFAULT_PREDICT_TOP_K
+
+        pred_item_ids, pred_scores = outputs.predictions
+        assert len(pred_item_ids.shape) == 2
+        assert pred_item_ids.shape[1] == predict_top_k
+        assert len(pred_scores.shape) == 2
+        assert pred_scores.shape[1] == predict_top_k
+
+
+@pytest.mark.parametrize("predict_top_k", [15, 20, 30, None])
+@pytest.mark.parametrize("top_k", [20, None])
+def test_trainer_predict_top_k_x_top_k(predict_top_k, top_k):
+    data = tr.data.music_streaming_testing_data
+    schema = data.schema
+    batch_size = 16
+
+    task = tr.NextItemPredictionTask(weight_tying=True)
+
+    inputs = tr.TabularSequenceFeatures.from_schema(
+        schema,
+        max_sequence_length=20,
+        d_output=64,
+        masking="clm",
     )
     transformer_config = tconf.XLNetConfig.build(64, 4, 2, 20)
     model = transformer_config.to_torch_model(inputs, task)
 
     args = trainer.T4RecTrainingArguments(
         output_dir=".",
         num_train_epochs=1,
@@ -590,11 +672,101 @@
         args=args,
         schema=schema,
         train_dataset_or_path=data.path,
         eval_dataset_or_path=data.path,
         test_dataset_or_path=data.path,
         compute_metrics=True,
     )
-    with pytest.raises(AssertionError) as excinfo:
-        recsys_trainer.predict(data.path)
 
-    assert "Top-k prediction is specific to NextItemPredictionTask" in str(excinfo.value)
+    model.top_k = top_k
+
+    if predict_top_k and top_k and predict_top_k > top_k:
+        with pytest.raises(ValueError) as excinfo:
+            recsys_trainer.predict(data.path)
+        assert "The args.predict_top_k should not be larger than model.top_k" in str(excinfo.value)
+
+    else:
+        outputs = recsys_trainer.predict(data.path)
+
+        if predict_top_k or top_k:
+            expected_top_k = predict_top_k or top_k
+
+            pred_item_ids, pred_scores = outputs.predictions
+            assert len(pred_item_ids.shape) == 2
+            assert pred_item_ids.shape[1] == expected_top_k
+            assert len(pred_scores.shape) == 2
+            assert pred_scores.shape[1] == expected_top_k
+        else:
+            ITEM_CARDINALITY = 10001
+            assert outputs.predictions.shape[1] == ITEM_CARDINALITY
+
+
+def test_trainer_with_pretrained_embeddings():
+    import numpy as np
+    from merlin.dataloader.ops.embeddings import EmbeddingOperator
+    from merlin.io import Dataset
+
+    from transformers4rec.torch.utils.data_utils import MerlinDataLoader
+
+    data = tr.data.music_streaming_testing_data
+    schema = data.merlin_schema.select_by_name(
+        ["item_id", "item_category", "item_recency", "item_genres", "user_id"]
+    )
+    batch_size, max_length, pretrained_dim = 128, 20, 16
+    item_cardinality = schema["item_id"].int_domain.max + 1
+    np_emb_item_id = np.random.rand(item_cardinality, pretrained_dim)
+
+    embeddings_op = EmbeddingOperator(
+        np_emb_item_id, lookup_key="item_id", embedding_name="pretrained_item_id_embeddings"
+    )
+    # set dataloader with pre-trained embeddings
+    data_loader = MerlinDataLoader.from_schema(
+        schema,
+        Dataset(data.path, schema=schema),
+        max_sequence_length=max_length,
+        batch_size=batch_size,
+        transforms=[embeddings_op],
+        shuffle=False,
+    )
+
+    # set the model schema from data-loader
+    model_schema = data_loader.output_schema
+    inputs = tr.TabularSequenceFeatures.from_schema(
+        model_schema,
+        max_sequence_length=max_length,
+        pretrained_output_dims=8,
+        normalizer="layer-norm",
+        d_output=64,
+        masking="mlm",
+    )
+    transformer_config = tconf.XLNetConfig.build(64, 4, 2, 20)
+    task = tr.NextItemPredictionTask(weight_tying=True)
+    model = transformer_config.to_torch_model(inputs, task, max_sequence_length=max_length)
+
+    assert isinstance(model.input_schema, Schema)
+
+    args = trainer.T4RecTrainingArguments(
+        output_dir=".",
+        max_steps=5,
+        num_train_epochs=1,
+        per_device_train_batch_size=batch_size,
+        per_device_eval_batch_size=batch_size // 2,
+        max_sequence_length=max_length,
+        fp16=False,
+        report_to=[],
+        debug=["r"],
+    )
+    # Explicitly pass the merlin dataloader with pre-trained embeddings
+    recsys_trainer = tr.Trainer(
+        model=model,
+        args=args,
+        schema=schema,
+        train_dataloader=data_loader,
+        eval_dataloader=data_loader,
+        compute_metrics=True,
+    )
+
+    recsys_trainer.train()
+    eval_metrics = recsys_trainer.evaluate(eval_dataset=data.path, metric_key_prefix="eval")
+
+    assert isinstance(eval_metrics, dict)
+    assert eval_metrics["eval_/loss"] is not None
```

### Comparing `transformers4rec-23.5.0/tests/unit/torch/utils/__init__.py` & `transformers4rec-23.6.0/tests/unit/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/utils/test_schema_utils.py` & `transformers4rec-23.6.0/tests/unit/torch/utils/test_schema_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/torch/utils/test_torch_utils.py` & `transformers4rec-23.6.0/tests/unit/torch/utils/test_torch_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/utils/__init__.py` & `transformers4rec-23.6.0/tests/unit/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/utils/test_data_utils.py` & `transformers4rec-23.6.0/tests/unit/utils/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tests/unit/utils/test_padding.py` & `transformers4rec-23.6.0/tests/unit/utils/test_padding.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/tox.ini` & `transformers4rec-23.6.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
     python -m pytest -rsx --cov-config tests/.coveragerc --cov-report term-missing --cov=. tests/unit
 
 [testenv:test-gpu-integration]
 sitepackages=true
 setenv = 
     TF_GPU_ALLOCATOR=cuda_malloc_async
+    LD_LIBRARY_PATH=/opt/tritonserver/backends/pytorch:{env:LD_LIBRARY_PATH}
 deps =
     -rrequirements/test.txt   
 commands =
     ; install latest Merlin libraries from source
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/NVTabular.git@{posargs:main}
     python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
```

### Comparing `transformers4rec-23.5.0/transformers4rec/__init__.py` & `transformers4rec-23.6.0/transformers4rec/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/config/__init__.py` & `transformers4rec-23.6.0/transformers4rec/config/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/config/schema.py` & `transformers4rec-23.6.0/transformers4rec/config/schema.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/config/trainer.py` & `transformers4rec-23.6.0/transformers4rec/config/trainer.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,17 @@
         -1 means no validation is used
         by default -1
     eval_on_test_set:
     eval_steps_on_train_set:
     predict_top_k:  Option[int], int
         Truncate recommendation list to the highest top-K predicted items,
         (do not affect evaluation metrics computation),
-        this parameter is specific to NextItemPredictionTask.
-        by default 0
+        This parameter is specific to NextItemPredictionTask and only affects
+        model.predict() and model.evaluate(), which both call `Trainer.evaluation_loop`.
+        By default 100.
     log_predictions : Optional[bool], bool
         log predictions, labels and metadata features each --compute_metrics_each_n_steps
         (for test set).
         by default False
     log_attention_weights : Optional[bool], bool
         Logs the inputs and attention weights
         each --eval_steps (only test set)"
@@ -86,18 +87,18 @@
 
     eval_steps_on_train_set: int = field(
         default=20,
         metadata={"help": "Number of steps to evaluate on train set (which is usually large)"},
     )
 
     predict_top_k: int = field(
-        default=0,
+        default=100,
         metadata={
             "help": "Truncate recommendation list to the highest top-K predicted items (do not affect evaluation metrics computation), "
-            "this parameter is specific to NextItemPredictionTask."
+            "this parameter is specific to NextItemPredictionTask. Default is 100."
         },
     )
 
     learning_rate_num_cosine_cycles_by_epoch: float = field(
         default=1.25,
         metadata={
             "help": "Number of cycles for by epoch when --learning_rate_schedule = cosine_with_warmup."
```

### Comparing `transformers4rec-23.5.0/transformers4rec/data/__init__.py` & `transformers4rec-23.6.0/transformers4rec/data/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/data/synthetic.py` & `transformers4rec-23.6.0/transformers4rec/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/data/testing/data.parquet` & `transformers4rec-23.6.0/transformers4rec/data/testing/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/data/testing/dataset.py` & `transformers4rec-23.6.0/transformers4rec/data/testing/dataset.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/data.parquet` & `transformers4rec-23.6.0/transformers4rec/data/testing/music_streaming/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/data/testing/music_streaming/schema.json` & `transformers4rec-23.6.0/transformers4rec/data/testing/music_streaming/schema.json`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/data/testing/schema.json` & `transformers4rec-23.6.0/transformers4rec/data/testing/schema.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8181818181818181%*

 * *Differences: {"'feature'": '{delete: [19, 17, 15, 14, 13, 2, 1, 0]}'}*

```diff
@@ -1,51 +1,12 @@
 {
     "feature": [
         {
             "annotation": {
                 "tag": [
-                    "groupby_col"
-                ]
-            },
-            "intDomain": {
-                "max": "11562158",
-                "min": "1",
-                "name": "session_id"
-            },
-            "name": "session_id",
-            "type": "INT"
-        },
-        {
-            "annotation": {
-                "tag": [
-                    "first"
-                ]
-            },
-            "name": "session_start"
-        },
-        {
-            "annotation": {
-                "tag": [
-                    "list"
-                ]
-            },
-            "intDomain": {
-                "max": "181",
-                "name": "timestamp/age_days/list"
-            },
-            "name": "timestamp/age_days/list",
-            "type": "INT",
-            "valueCount": {
-                "max": "185",
-                "min": "2"
-            }
-        },
-        {
-            "annotation": {
-                "tag": [
                     "continuous",
                     "list"
                 ]
             },
             "floatDomain": {
                 "max": 1.5231701135635376,
                 "min": -2.917729139328003,
@@ -237,63 +198,14 @@
                 "max": "185",
                 "min": "2"
             }
         },
         {
             "annotation": {
                 "tag": [
-                    "time",
-                    "list"
-                ]
-            },
-            "intDomain": {
-                "max": "1412045999",
-                "min": "1396321200",
-                "name": "ts/list"
-            },
-            "name": "ts/list",
-            "type": "INT",
-            "valueCount": {
-                "max": "185",
-                "min": "2"
-            }
-        },
-        {
-            "annotation": {
-                "tag": [
-                    "time",
-                    "last"
-                ]
-            },
-            "intDomain": {
-                "max": "1412045999",
-                "min": "1396321232",
-                "name": "ts/last"
-            },
-            "name": "ts/last",
-            "type": "INT"
-        },
-        {
-            "annotation": {
-                "tag": [
-                    "time",
-                    "first"
-                ]
-            },
-            "intDomain": {
-                "max": "1412045793",
-                "min": "1396321200",
-                "name": "ts/first"
-            },
-            "name": "ts/first",
-            "type": "INT"
-        },
-        {
-            "annotation": {
-                "tag": [
                     "item_id",
                     "list",
                     "categorical",
                     "item"
                 ]
             },
             "intDomain": {
@@ -308,28 +220,14 @@
                 "max": "185",
                 "min": "2"
             }
         },
         {
             "annotation": {
                 "tag": [
-                    "count"
-                ]
-            },
-            "intDomain": {
-                "max": "185",
-                "min": "2",
-                "name": "session_size"
-            },
-            "name": "session_size",
-            "type": "INT"
-        },
-        {
-            "annotation": {
-                "tag": [
                     "list",
                     "categorical",
                     "item"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
@@ -341,18 +239,14 @@
             "type": "INT",
             "valueCount": {
                 "max": "185",
                 "min": "2"
             }
         },
         {
-            "annotation": {},
-            "name": "day_idx"
-        },
-        {
             "annotation": {
                 "tag": [
                     "categorical"
                 ]
             },
             "intDomain": {
                 "isCategorical": true,
```

### Comparing `transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/data.parquet` & `transformers4rec-23.6.0/transformers4rec/data/testing/tabular_data/data.parquet`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/data/testing/tabular_data/schema.json` & `transformers4rec-23.6.0/transformers4rec/data/testing/tabular_data/schema.json`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/data/yoochoose.py` & `transformers4rec-23.6.0/transformers4rec/data/yoochoose.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/__init__.py` & `transformers4rec-23.6.0/transformers4rec/torch/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 from .block.transformer import TransformerBlock
 
 # Features related imports
 from .features.continuous import ContinuousFeatures
 from .features.embedding import (
     EmbeddingFeatures,
     FeatureConfig,
+    PretrainedEmbeddingFeatures,
     PretrainedEmbeddingsInitializer,
     SoftEmbedding,
     SoftEmbeddingFeatures,
     TableConfig,
 )
 from .features.sequence import SequenceEmbeddingFeatures, TabularSequenceFeatures
 from .features.tabular import TabularFeatures
@@ -100,14 +101,15 @@
     "TabularLayerNorm",
     "TabularDropout",
     "TransformerBlock",
     "ContinuousFeatures",
     "EmbeddingFeatures",
     "SoftEmbeddingFeatures",
     "PretrainedEmbeddingsInitializer",
+    "PretrainedEmbeddingFeatures",
     "TabularSequenceFeatures",
     "SequenceEmbeddingFeatures",
     "FeatureConfig",
     "TableConfig",
     "TabularFeatures",
     "Head",
     "Model",
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/block/__init__.py` & `transformers4rec-23.6.0/transformers4rec/torch/block/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/block/transformer.py` & `transformers4rec-23.6.0/transformers4rec/torch/block/transformer.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,24 +26,43 @@
 from ..utils.torch_utils import MappingTransformerMasking
 from .base import BlockBase
 
 TransformerBody = Union[PreTrainedModel, PretrainedConfig]
 
 
 class TransformerPrepare(torch.nn.Module):
-    def __init__(self, transformer, masking):
+    """
+    Base class to prepare additional inputs to the forward call of
+    the HF transformer layer.
+
+    Parameters
+    ----------
+    transformer : TransformerBody
+        The Transformer module.
+    masking : Optional[MaskSequence]
+        Masking block used to for masking input sequences.
+        By default None.
+    """
+
+    def __init__(self, transformer: TransformerBody, masking: Optional[MaskSequence] = None):
         super().__init__()
         self.transformer = transformer
         self.masking = masking
 
     def forward(self, inputs_embeds) -> Dict[str, Any]:
         raise NotImplementedError()
 
 
 class GPT2Prepare(TransformerPrepare):
+    """TransformerPrepare module for GPT-2.
+
+    This class extends the inputs for GPT-2 with a
+    triangular causal mask to the inputs.
+    """
+
     def forward(self, inputs_embeds) -> Dict[str, Any]:
         seq_len = inputs_embeds.shape[1]
         # head_mask has shape n_layer x batch x n_heads x N x N
         head_mask = (
             torch.tril(
                 torch.ones((seq_len, seq_len), dtype=torch.uint8, device=inputs_embeds.device)
             )
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/experimental.py` & `transformers4rec-23.6.0/transformers4rec/torch/experimental.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/features/__init__.py` & `transformers4rec-23.6.0/transformers4rec/torch/features/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/features/base.py` & `transformers4rec-23.6.0/transformers4rec/torch/features/base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/features/continuous.py` & `transformers4rec-23.6.0/transformers4rec/torch/features/continuous.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/features/embedding.py` & `transformers4rec-23.6.0/transformers4rec/torch/features/embedding.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 import torch
 from merlin.models.utils.doc_utils import docstring_parameter
 from merlin.schema import Tags, TagsType
 
 from merlin_standard_lib import Schema, categorical_cardinalities
 from merlin_standard_lib.utils.embedding_utils import get_embedding_sizes_from_schema
 
+from ..block.base import SequentialBlock
 from ..tabular.base import (
     TABULAR_MODULE_PARAMS_DOCSTRING,
     FilterFeatures,
     TabularAggregationType,
+    TabularTransformation,
     TabularTransformationType,
 )
 from ..utils.torch_utils import calculate_batch_size_from_input_size, get_output_sizes_from_schema
 from .base import InputBlock
 
 EMBEDDING_FEATURES_PARAMS_DOCSTRING = """
     feature_config: Dict[str, FeatureConfig]
@@ -252,14 +254,22 @@
         for name, feature in self.feature_config.items():
             sizes[name] = torch.Size([batch_size, feature.table.dim])
 
         return sizes
 
 
 class EmbeddingBagWrapper(torch.nn.EmbeddingBag):
+    """
+    Wrapper class for the PyTorch EmbeddingBag module.
+
+    This class extends the torch.nn.EmbeddingBag class and overrides
+    the forward method to handle 1D tensor inputs
+    by reshaping them to 2D as required by the EmbeddingBag.
+    """
+
     def forward(self, input, **kwargs):
         # EmbeddingBag requires 2D tensors (or offsets)
         if len(input.shape) == 1:
             input = input.unsqueeze(-1)
         return super().forward(input, **kwargs)
 
 
@@ -400,14 +410,37 @@
         return output
 
     def table_to_embedding_module(self, table: "TableConfig") -> "SoftEmbedding":
         return SoftEmbedding(table.vocabulary_size, table.dim, table.initializer)
 
 
 class TableConfig:
+    """
+    Class to configure the embeddings lookup table for a categorical feature.
+
+    Attributes
+    ----------
+    vocabulary_size : int
+        The size of the vocabulary,
+        i.e., the cardinality of the categorical feature.
+    dim : int
+        The dimensionality of the embedding vectors.
+    initializer : Optional[Callable[[torch.Tensor], None]]
+        The initializer function for the embedding weights.
+        If None, the weights are initialized using a normal
+        distribution with mean 0.0 and standard deviation 0.05.
+    combiner : Optional[str]
+        The combiner operation used to aggregate bag of embeddings.
+        Possible options are "mean", "sum", and "sqrtn".
+        By default "mean".
+    name : Optional[str]
+        The name of the lookup table.
+        By default None.
+    """
+
     def __init__(
         self,
         vocabulary_size: int,
         dim: int,
         initializer: Optional[Callable[[torch.Tensor], None]] = None,
         combiner: Text = "mean",
         name: Optional[Text] = None,
@@ -444,14 +477,31 @@
                 combiner=self.combiner,
                 name=self.name,
             )
         )
 
 
 class FeatureConfig:
+    """
+    Class to set the embeddings table of a categorical feature
+    with a maximum sequence length.
+
+    Attributes
+    ----------
+    table : TableConfig
+        Configuration for the lookup table,
+        which is used for embedding lookup and aggregation.
+    max_sequence_length : int, optional
+        Maximum sequence length for sequence features.
+        By default 0.
+    name : str, optional
+        The feature name.
+        By default None
+    """
+
     def __init__(
         self, table: TableConfig, max_sequence_length: int = 0, name: Optional[Text] = None
     ):
         self.table = table
         self.max_sequence_length = max_sequence_length
         self.name = name
 
@@ -537,7 +587,151 @@
         self.weight_matrix = torch.tensor(weight_matrix, device="cpu")
         self.trainable = trainable
 
     def forward(self, x):
         with torch.no_grad():
             x.copy_(self.weight_matrix)
         x.requires_grad = self.trainable
+
+
+@docstring_parameter(
+    tabular_module_parameters=TABULAR_MODULE_PARAMS_DOCSTRING,
+)
+class PretrainedEmbeddingFeatures(InputBlock):
+    """Input block for pre-trained embeddings features.
+
+    For 3-D features, if sequence_combiner is set, the features are aggregated
+    using the second dimension (sequence length)
+
+    Parameters
+    ----------
+    features: List[str]
+        A list of the pre-trained embeddings feature names.
+        You typically will pass schema.select_by_tag(Tags.EMBEDDING).column_names,
+        as that is the tag added to pre-trained embedding features when using the
+        merlin.dataloader.ops.embeddings.EmbeddingOperator
+    pretrained_output_dims: Optional[Union[int, Dict[str, int]]]
+        If provided, it projects features to specified dim(s).
+        If an int, all features are projected to that dim.
+        If a dict, only features provided in the dict will be mapped to the specified dim,
+    sequence_combiner: Optional[Union[str, torch.nn.Module]], optional
+       A string ("mean", "sum", "max", "min") or torch.nn.Module specifying
+       how to combine the second dimension of the pre-trained embeddings if it is 3D.
+       Default is None (no sequence combiner used)
+    normalizer: Optional[Union[str, TabularTransformationType]]
+       A tabular layer (e.g.tr.TabularLayerNorm()) or string ("layer-norm") to be applied
+       to pre-trained embeddings after projected and sequence combined
+       Default is None (no normalization)
+    schema (Optional[Schema]): the schema of the input data.
+    {tabular_module_parameters}
+    """
+
+    def __init__(
+        self,
+        features: List[str],
+        pretrained_output_dims: Optional[Union[int, Dict[str, int]]] = None,
+        sequence_combiner: Optional[Union[str, torch.nn.Module]] = None,
+        pre: Optional[TabularTransformationType] = None,
+        post: Optional[TabularTransformationType] = None,
+        aggregation: Optional[TabularAggregationType] = None,
+        normalizer: Optional[TabularTransformationType] = None,
+        schema: Optional[Schema] = None,
+    ):
+        if isinstance(normalizer, str):
+            normalizer = TabularTransformation.parse(normalizer)
+        if not post:
+            post = normalizer
+        elif normalizer:
+            post = SequentialBlock(normalizer, post)  # type: ignore
+
+        super().__init__(pre=pre, post=post, aggregation=aggregation, schema=schema)
+        self.features = features
+        self.filter_features = FilterFeatures(features)
+        self.pretrained_output_dims = pretrained_output_dims
+        self.sequence_combiner = self.parse_combiner(sequence_combiner)
+
+    def build(self, input_size, **kwargs):
+        if input_size is not None:
+            if self.pretrained_output_dims:
+                self.projection = torch.nn.ModuleDict()
+                if isinstance(self.pretrained_output_dims, int):
+                    for key in self.features:
+                        self.projection[key] = torch.nn.Linear(
+                            input_size[key][-1], self.pretrained_output_dims
+                        )
+
+                elif isinstance(self.pretrained_output_dims, dict):
+                    for key in self.features:
+                        self.projection[key] = torch.nn.Linear(
+                            input_size[key][-1], self.pretrained_output_dims[key]
+                        )
+
+        return super().build(input_size, **kwargs)
+
+    @classmethod
+    def from_schema(
+        cls,
+        schema: Schema,
+        tags: Optional[TagsType] = None,
+        pretrained_output_dims=None,
+        sequence_combiner=None,
+        normalizer: Optional[Union[str, TabularTransformationType]] = None,
+        pre: Optional[TabularTransformationType] = None,
+        post: Optional[TabularTransformationType] = None,
+        aggregation: Optional[TabularAggregationType] = None,
+        **kwargs,
+    ):  # type: ignore
+        if tags:
+            schema = schema.select_by_tag(tags)
+
+        features = schema.column_names
+        return cls(
+            features=features,
+            pretrained_output_dims=pretrained_output_dims,
+            sequence_combiner=sequence_combiner,
+            pre=pre,
+            post=post,
+            aggregation=aggregation,
+            normalizer=normalizer,
+        )
+
+    def forward(self, inputs):
+        output = self.filter_features(inputs)
+        if self.pretrained_output_dims:
+            output = {key: self.projection[key](val) for key, val in output.items()}
+        if self.sequence_combiner:
+            for key, val in output.items():
+                if val.dim() > 2:
+                    output[key] = self.sequence_combiner(val, axis=1)
+
+        return output
+
+    def forward_output_size(self, input_sizes):
+        sizes = self.filter_features.forward_output_size(input_sizes)
+        if self.pretrained_output_dims:
+            if isinstance(self.pretrained_output_dims, dict):
+                sizes.update(
+                    {
+                        key: torch.Size(list(sizes[key][:-1]) + [self.pretrained_output_dims[key]])
+                        for key in self.features
+                    }
+                )
+            else:
+                sizes.update(
+                    {
+                        key: torch.Size(list(sizes[key][:-1]) + [self.pretrained_output_dims])
+                        for key in self.features
+                    }
+                )
+        return sizes
+
+    def parse_combiner(self, combiner):
+        if isinstance(combiner, str):
+            if combiner == "sum":
+                combiner = torch.sum
+            elif combiner == "max":
+                combiner = torch.max
+            elif combiner == "min":
+                combiner = torch.min
+            elif combiner == "mean":
+                combiner = torch.mean
+        return combiner
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/features/sequence.py` & `transformers4rec-23.6.0/transformers4rec/torch/features/sequence.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,27 +111,27 @@
 
     EMBEDDING_MODULE_CLASS = SequenceEmbeddingFeatures
 
     def __init__(
         self,
         continuous_module: Optional[TabularModule] = None,
         categorical_module: Optional[TabularModule] = None,
-        text_embedding_module: Optional[TabularModule] = None,
+        pretrained_embedding_module: Optional[TabularModule] = None,
         projection_module: Optional[BlockOrModule] = None,
         masking: Optional[MaskSequence] = None,
         pre: Optional[TabularTransformationType] = None,
         post: Optional[TabularTransformationType] = None,
         aggregation: Optional[TabularAggregationType] = None,
         schema: Optional[Schema] = None,
         **kwargs
     ):
         super().__init__(
             continuous_module,
             categorical_module,
-            text_embedding_module,
+            pretrained_embedding_module,
             pre=pre,
             post=post,
             aggregation=aggregation,
             schema=schema,
             **kwargs
         )
         self.projection_module = projection_module
@@ -139,14 +139,15 @@
 
     @classmethod
     def from_schema(  # type: ignore
         cls,
         schema: Schema,
         continuous_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CONTINUOUS,),
         categorical_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CATEGORICAL,),
+        pretrained_embeddings_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.EMBEDDING,),
         aggregation: Optional[str] = None,
         automatic_build: bool = True,
         max_sequence_length: Optional[int] = None,
         continuous_projection: Optional[Union[List[int], int]] = None,
         continuous_soft_embeddings: bool = False,
         projection: Optional[Union[torch.nn.Module, BuildableBlock]] = None,
         d_output: Optional[int] = None,
@@ -190,14 +191,15 @@
         TabularFeatures
             Returns ``TabularFeatures`` from a dataset schema
         """
         output: TabularSequenceFeatures = super().from_schema(  # type: ignore
             schema=schema,
             continuous_tags=continuous_tags,
             categorical_tags=categorical_tags,
+            pretrained_embeddings_tags=pretrained_embeddings_tags,
             aggregation=aggregation,
             automatic_build=automatic_build,
             max_sequence_length=max_sequence_length,
             continuous_projection=continuous_projection,
             continuous_soft_embeddings=continuous_soft_embeddings,
             **kwargs
         )
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/features/tabular.py` & `transformers4rec-23.6.0/transformers4rec/torch/features/tabular.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     MergeTabular,
     TabularAggregationType,
     TabularModule,
     TabularTransformationType,
 )
 from ..utils.torch_utils import get_output_sizes_from_schema
 from .continuous import ContinuousFeatures
-from .embedding import EmbeddingFeatures, SoftEmbeddingFeatures
+from .embedding import EmbeddingFeatures, PretrainedEmbeddingFeatures, SoftEmbeddingFeatures
 
 TABULAR_FEATURES_PARAMS_DOCSTRING = """
     continuous_module: TabularModule, optional
         Module used to process continuous features.
     categorical_module: TabularModule, optional
         Module used to process categorical features.
     text_embedding_module: TabularModule, optional
@@ -57,33 +57,34 @@
     {tabular_features_parameters}
     {tabular_module_parameters}
     """
 
     CONTINUOUS_MODULE_CLASS: Type[TabularModule] = ContinuousFeatures
     EMBEDDING_MODULE_CLASS: Type[TabularModule] = EmbeddingFeatures
     SOFT_EMBEDDING_MODULE_CLASS: Type[TabularModule] = SoftEmbeddingFeatures
+    PRETRAINED_EMBEDDING_MODULE_CLASS: Type[TabularModule] = PretrainedEmbeddingFeatures
 
     def __init__(
         self,
         continuous_module: Optional[TabularModule] = None,
         categorical_module: Optional[TabularModule] = None,
-        text_embedding_module: Optional[TabularModule] = None,
+        pretrained_embedding_module: Optional[TabularModule] = None,
         pre: Optional[TabularTransformationType] = None,
         post: Optional[TabularTransformationType] = None,
         aggregation: Optional[TabularAggregationType] = None,
         schema: Optional[Schema] = None,
         **kwargs,
     ):
         to_merge = {}
         if continuous_module:
             to_merge["continuous_module"] = continuous_module
         if categorical_module:
             to_merge["categorical_module"] = categorical_module
-        if text_embedding_module:
-            to_merge["text_embedding_module"] = text_embedding_module
+        if pretrained_embedding_module:
+            to_merge["pretrained_embedding_module"] = pretrained_embedding_module
 
         assert to_merge != {}, "Please provide at least one input layer"
         super(TabularFeatures, self).__init__(
             to_merge, pre=pre, post=post, aggregation=aggregation, schema=schema, **kwargs
         )
 
     def project_continuous_features(
@@ -117,14 +118,15 @@
 
     @classmethod
     def from_schema(  # type: ignore
         cls,
         schema: Schema,
         continuous_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CONTINUOUS,),
         categorical_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CATEGORICAL,),
+        pretrained_embeddings_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.EMBEDDING,),
         aggregation: Optional[str] = None,
         automatic_build: bool = True,
         max_sequence_length: Optional[int] = None,
         continuous_projection: Optional[Union[List[int], int]] = None,
         continuous_soft_embeddings: bool = False,
         **kwargs,
     ) -> "TabularFeatures":
@@ -152,15 +154,20 @@
             represent continuous features, by default False
 
         Returns
         -------
         TabularFeatures
             Returns ``TabularFeatures`` from a dataset schema
         """
-        maybe_continuous_module, maybe_categorical_module = None, None
+        maybe_continuous_module, maybe_categorical_module, maybe_pretrained_module = (
+            None,
+            None,
+            None,
+        )
+
         if continuous_tags:
             if continuous_soft_embeddings:
                 maybe_continuous_module = cls.SOFT_EMBEDDING_MODULE_CLASS.from_schema(
                     schema,
                     tags=continuous_tags,
                     **kwargs,
                 )
@@ -168,19 +175,23 @@
                 maybe_continuous_module = cls.CONTINUOUS_MODULE_CLASS.from_schema(
                     schema, tags=continuous_tags, **kwargs
                 )
         if categorical_tags:
             maybe_categorical_module = cls.EMBEDDING_MODULE_CLASS.from_schema(
                 schema, tags=categorical_tags, **kwargs
             )
+        if pretrained_embeddings_tags:
+            maybe_pretrained_module = cls.PRETRAINED_EMBEDDING_MODULE_CLASS.from_schema(
+                schema, tags=pretrained_embeddings_tags, **kwargs
+            )
 
         output = cls(
             continuous_module=maybe_continuous_module,
             categorical_module=maybe_categorical_module,
-            text_embedding_module=None,
+            pretrained_embedding_module=maybe_pretrained_module,
             aggregation=aggregation,
         )
 
         if automatic_build and schema:
             output.build(
                 get_output_sizes_from_schema(
                     schema,
@@ -215,7 +226,14 @@
 
     @property
     def categorical_module(self) -> Optional[TabularModule]:
         if "categorical_module" in self.to_merge:
             return self.to_merge["categorical_module"]
 
         return None
+
+    @property
+    def pretrained_module(self) -> Optional[TabularModule]:
+        if "pretrained_embedding_module" in self.to_merge:
+            return self.to_merge["pretrained_embedding_module"]
+
+        return None
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/features/text.py` & `transformers4rec-23.6.0/transformers4rec/torch/features/text.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/losses.py` & `transformers4rec-23.6.0/transformers4rec/torch/losses.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/masking.py` & `transformers4rec-23.6.0/transformers4rec/torch/masking.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,14 +270,18 @@
             kwargs=kwargs,
         )
         self.train_on_last_item_seq_only = train_on_last_item_seq_only
 
     def _compute_masked_targets(
         self, item_ids: torch.Tensor, training: bool = False, testing: bool = False
     ) -> MaskingInfo:
+        if not training and not testing:
+            mask_labels = item_ids != self.padding_idx
+            return MaskingInfo(mask_labels, item_ids)
+
         masking_info = self.predict_all(item_ids)
         mask_labels, labels = masking_info.schema, masking_info.targets
 
         if (self.eval_on_last_item_seq_only and not training) or (
             self.train_on_last_item_seq_only and training
         ):
             rows_ids = torch.arange(
@@ -286,41 +290,49 @@
             last_item_sessions = mask_labels.sum(dim=1) - 1
             label_seq_trg_eval = torch.zeros(
                 labels.shape, dtype=labels.dtype, device=item_ids.device
             )
             label_seq_trg_eval[rows_ids, last_item_sessions] = labels[rows_ids, last_item_sessions]
             # Updating labels and mask
             labels = label_seq_trg_eval
-            mask_labels = label_seq_trg_eval != self.padding_idx
+            # We only mask padded positions
+            mask_labels = item_ids != self.padding_idx
 
         return MaskingInfo(mask_labels, labels)
 
     def apply_mask_to_inputs(
         self,
         inputs: torch.Tensor,
         mask_schema: torch.Tensor,
         training: bool = False,
         testing: bool = False,
     ) -> torch.Tensor:
         if not training and not testing:
+            # Replacing the inputs corresponding to padded items with a trainable embedding
+            # To mimic training and evaluation masking strategy
+            inputs = torch.where(
+                mask_schema.unsqueeze(-1).bool(),
+                inputs,
+                self.masked_item_embedding.to(inputs.dtype),
+            )
             return inputs
         # shift sequence of interaction embeddings
         pos_emb_inp = inputs[:, :-1]
         # Adding a masked item in the sequence to return to the initial sequence.
         pos_emb_inp = torch.cat(  # type: ignore
             [
                 pos_emb_inp,
                 torch.zeros(
                     (pos_emb_inp.shape[0], 1, pos_emb_inp.shape[2]),
                     dtype=pos_emb_inp.dtype,
                 ).to(inputs.device),
             ],
             axis=1,
         )
-        # Replacing the inputs corresponding to masked label with a trainable embedding
+        # Replacing the inputs corresponding to padded items with a trainable embedding
         pos_emb_inp = torch.where(
             mask_schema.unsqueeze(-1).bool(),
             pos_emb_inp,
             self.masked_item_embedding.to(pos_emb_inp.dtype),
         )
         return pos_emb_inp
 
@@ -597,22 +609,24 @@
                         # Reserve a context
                         # to surround span to be masked
                         context_length = int(span_length / self.plm_probability)
                         # Sample a starting point `start_index`
                         # from the interval `[cur_len, cur_len + context_length - span_length]`
                         start_index = (
                             cur_len
-                            + torch.randint(  # type: ignore
-                                context_length - span_length + 1, (1,)
+                            + torch.randint(
+                                context_length - span_length + 1, (1,)  # type: ignore
                             ).item()
                         )
                         if start_index < max_len:
                             # Mask the span of non-padded items
                             #   `start_index:start_index + span_length`
-                            mask_labels[i, start_index : start_index + span_length] = 1
+                            mask_labels[
+                                i, start_index : start_index + span_length  # type: ignore
+                            ] = 1
                         # Set `cur_len = cur_len + context_length`
                         cur_len += context_length
                     # if no item was masked:
                     if mask_labels[i].sum() == 0:
                         # Set at least one item in the sequence to mask, so that the network can
                         # learn something with this session
                         one_random_index_by_session = torch.multinomial(
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/model/__init__.py` & `transformers4rec-23.6.0/transformers4rec/torch/model/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/model/base.py` & `transformers4rec-23.6.0/transformers4rec/torch/model/base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/model/prediction_task.py` & `transformers4rec-23.6.0/transformers4rec/torch/model/prediction_task.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,15 +29,34 @@
 from ..utils.torch_utils import LambdaModule
 from .base import BlockType, PredictionTask
 
 LOG = logging.getLogger("transformers4rec")
 
 
 class BinaryClassificationPrepareBlock(BuildableBlock):
+    """Prepares the output layer of the binary classification prediction task.
+    The output layer is a SequentialBlock of a torch linear
+    layer followed by a sigmoid activation and a squeeze operation.
+    """
+
     def build(self, input_size) -> SequentialBlock:
+        """Builds the output layer of binary classification based on the input_size.
+
+        Parameters
+        ----------
+        input_size: Tuple[int]
+            The size of the input tensor, specifically the last dimension is
+            used for setting the input dimension of the linear layer.
+
+        Returns
+        -------
+        SequentialBlock
+            A SequentialBlock consisting of a linear layer (with input dimension equal to the last
+            dimension of input_size), a sigmoid activation, and a squeeze operation.
+        """
         return SequentialBlock(
             torch.nn.Linear(input_size[-1], 1, bias=False),
             torch.nn.Sigmoid(),
             LambdaModule(lambda x: torch.squeeze(x, -1)),
             output_size=[
                 None,
             ],
@@ -151,25 +170,119 @@
             task_block=task_block,
             pre=BinaryClassificationPrepareBlock(),
             forward_to_prediction_fn=lambda x: torch.round(x).int(),
         )
 
 
 class RegressionPrepareBlock(BuildableBlock):
+    """Prepares the output layer of the regression prediction task.
+    The output layer is a SequentialBlock of a torch linear
+    layer followed by a squeeze operation.
+    """
+
     def build(self, input_size) -> SequentialBlock:
+        """Builds the output layer of regression based on the input_size.
+
+        Parameters
+        ----------
+        input_size: Tuple[int]
+            The size of the input tensor, specifically the last dimension is
+            used for setting the input dimension of the linear layer.
+
+        Returns
+        -------
+        SequentialBlock
+            A SequentialBlock consisting of a linear layer (with input dimension equal to
+            the last dimension of input_size), and a squeeze operation.
+        """
         return SequentialBlock(
             torch.nn.Linear(input_size[-1], 1),
             LambdaModule(lambda x: torch.squeeze(x, -1)),
             output_size=[
                 None,
             ],
         )
 
 
 class RegressionTask(PredictionTask):
+    """Returns a ``PredictionTask`` for regression.
+
+    Example usage::
+
+        # Define the input module to process the tabular input features.
+        input_module = tr.TabularSequenceFeatures.from_schema(
+            schema,
+            max_sequence_length=max_sequence_length,
+            continuous_projection=d_model,
+            aggregation="concat",
+            masking=None,
+        )
+
+        # Define XLNetConfig class and set default parameters for HF XLNet config.
+        transformer_config = tr.XLNetConfig.build(
+            d_model=d_model, n_head=4, n_layer=2, total_seq_length=max_sequence_length
+        )
+
+        # Define the model block including: inputs, projection and transformer block.
+        body = tr.SequentialBlock(
+            input_module,
+            tr.MLPBlock([64]),
+            tr.TransformerBlock(
+                transformer_config,
+            )
+        )
+
+        # Define a head with BinaryClassificationTask.
+        head = tr.Head(
+            body,
+            tr.RegressionTask(
+                "watch_time",
+                summary_type="mean",
+                metrics=[tm.regression.MeanSquaredError()]
+            ),
+            inputs=input_module,
+        )
+
+        # Get the end-to-end Model class.
+        model = tr.Model(head)
+
+    Parameters
+    ----------
+
+    target_name: Optional[str]
+        Specifies the variable name that represents the continuous value to predict.
+        By default None
+
+    task_name: Optional[str]
+        Specifies the name of the prediction task. If this parameter is not specified,
+        a name is automatically constructed based on ``target_name`` and the Python
+        class name of the model.
+        By default None
+
+    task_block: Optional[BlockType] = None
+        Specifies a module to transform the input tensor before computing predictions.
+
+    loss: torch.nn.Module
+        Specifies the loss function for the task.
+        The default class is ``torch.nn.MSELoss``.
+
+    metrics: Tuple[torch.nn.Module, ...]
+        Specifies the metrics to calculate during training and evaluation.
+        The default metric is MeanSquaredError.
+
+    summary_type: str
+        Summarizes a sequence into a single tensor. Accepted values are:
+
+            - ``last`` -- Take the last token hidden state (like XLNet)
+            - ``first`` -- Take the first token hidden state (like Bert)
+            - ``mean`` -- Take the mean of all tokens hidden states
+            - ``cls_index`` -- Supply a Tensor of classification token position (GPT/GPT-2)
+            - ``attn`` -- Not implemented now, use multi-head attention
+    """
+
     DEFAULT_LOSS = torch.nn.MSELoss()
     DEFAULT_METRICS = (tm.regression.MeanSquaredError(),)
 
     def __init__(
         self,
         target_name: Optional[str] = None,
         task_name: Optional[str] = None,
@@ -190,15 +303,15 @@
         )
 
 
 class NextItemPredictionTask(PredictionTask):
     """This block performs item prediction task for session and sequential-based models.
     It requires a body containing a masking schema to use for training and target generation.
     For the supported masking schemes, please refers to:
-    https://nvidia-merlin.github.io/Transformers4Rec/main/model_definition.html#sequence-masking
+    https://nvidia-merlin.github.io/Transformers4Rec/stable/model_definition.html#sequence-masking
 
     Parameters
     ----------
     loss: torch.nn.Module
         Loss function to use. Defaults to NLLLos.
     metrics: Iterable[torchmetrics.Metric]
         List of ranking metrics to use for evaluation.
@@ -369,15 +482,16 @@
         if isinstance(targets, dict) and self.target_name:
             targets = targets[self.target_name]
 
         outputs = {}
         predictions = self.forward_to_prediction_fn(predictions)
 
         for metric in self.metrics:
-            outputs[self.metric_name(metric)] = metric(predictions, targets)
+            result = metric(predictions, targets)
+            outputs[self.metric_name(metric)] = result
 
         return outputs
 
     def compute_metrics(self):
         metrics = {
             self.metric_name(metric): metric.compute()
             for metric in self.metrics
@@ -385,20 +499,50 @@
         }
         # Explode metrics for each cut-off
         # TODO make result generic:
         # To accept a mix of ranking metrics and others not requiring top_ks ?
         topks = {self.metric_name(metric): metric.top_ks for metric in self.metrics}
         results = {}
         for name, metric in metrics.items():
+            # Fix for when using a single cut-off, as torch metrics convert results to scalar
+            # when a single element vector is returned
+            if len(metric.size()) == 0:
+                metric = metric.unsqueeze(0)
             for measure, k in zip(metric, topks[name]):
                 results[f"{name}_{k}"] = measure
         return results
 
 
 class NextItemPredictionPrepareBlock(BuildableBlock):
+    """Prepares the output layer of the next item prediction task.
+    The output layer is a an instance of `_NextItemPredictionTask` class.
+
+    Parameters
+    ----------
+    target_dim: int
+        The output dimension for next-item predictions.
+    weight_tying: bool, optional
+        If true, ties the weights of the prediction layer and the item embedding layer.
+        By default False.
+    item_embedding_table: torch.nn.Module, optional
+        The module containing the item embedding table.
+        By default None.
+    softmax_temperature: float, optional
+        The temperature to be applied to the softmax function. Defaults to 0.
+    sampled_softmax: bool, optional
+        If true, sampled softmax is used for approximating the full softmax function.
+        By default False.
+    max_n_samples: int, optional
+        The maximum number of samples when using sampled softmax.
+        By default 100.
+    min_id: int, optional
+        The minimum value of the range for the log-uniform sampling.
+        By default 0.
+    """
+
     def __init__(
         self,
         target_dim: int,
         weight_tying: bool = False,
         item_embedding_table: Optional[torch.nn.Module] = None,
         softmax_temperature: float = 0,
         sampled_softmax: Optional[bool] = False,
@@ -411,14 +555,26 @@
         self.item_embedding_table = item_embedding_table
         self.softmax_temperature = softmax_temperature
         self.sampled_softmax = sampled_softmax
         self.max_n_samples = max_n_samples
         self.min_id = min_id
 
     def build(self, input_size) -> Block:
+        """Builds the output layer of next-item prediction based on the input_size.
+
+        Parameters
+        ----------
+        input_size : Tuple[int]
+            The size of the input tensor, specifically the last dimension is
+            used for setting the input dimension of the output layer.
+        Returns
+        -------
+        Block[_NextItemPredictionTask]
+            an instance of _NextItemPredictionTask
+        """
         return Block(
             _NextItemPredictionTask(
                 input_size,
                 self.target_dim,
                 self.weight_tying,
                 self.item_embedding_table,
                 self.softmax_temperature,
@@ -501,15 +657,15 @@
             output_weights = self.item_embedding_table.weight
         else:
             output_weights = self.output_layer
 
         if self.sampled_softmax and training:
             logits, targets = self.sampled(inputs, targets, output_weights)
         else:
-            logits = inputs @ output_weights.t()
+            logits = inputs @ output_weights.t()  # type: ignore
 
         if self.softmax_temperature:
             # Softmax temperature to reduce model overconfidence
             # and better calibrate probs and accuracy
             logits = torch.div(logits, self.softmax_temperature)
 
         return logits, targets
@@ -621,15 +777,17 @@
         -------
         torch.Tensor
             Returns the log uniform probability distribution
         """
         log_indices = torch.arange(1.0, max_id - min_id + 2.0, 1.0).log_()
         probs = (log_indices[1:] - log_indices[:-1]) / log_indices[-1]
         if min_id > 0:
-            probs = torch.cat([torch.zeros([min_id], dtype=probs.dtype), probs], axis=0)
+            probs = torch.cat(
+                [torch.zeros([min_id], dtype=probs.dtype), probs], axis=0
+            )  # type: ignore
         return probs
 
     def get_unique_sampling_distr(self, dist, n_sample):
         """Returns the probability that each item is sampled at least once
         given the specified number of trials. This is meant to be used when
         self.unique_sampling == True.
         That probability can be approximated by by 1 - (1 - p)^n
@@ -678,26 +836,26 @@
             raise ValueError("Labels must not be an empty tensor.")
         if (labels < 0).any() or (labels > self.max_id).any():
             raise ValueError("All label values must be within the range [0, max_id].")
 
         n_tries = self.n_sample
 
         with torch.no_grad():
-            neg_samples = torch.multinomial(self.dist, n_tries, replacement=True).unique()[
-                : self.max_n_samples
-            ]
+            neg_samples = torch.multinomial(
+                self.dist, n_tries, replacement=True  # type: ignore
+            ).unique()[: self.max_n_samples]
 
             device = labels.device
             neg_samples = neg_samples.to(device)
 
             if self.unique_sampling:
                 dist = self.unique_sampling_dist
             else:
                 dist = self.dist
 
-            true_probs = dist[labels]
-            samples_probs = dist[neg_samples]
+            true_probs = dist[labels]  # type: ignore
+            samples_probs = dist[neg_samples]  # type: ignore
 
             return neg_samples, true_probs, samples_probs
 
     def forward(self, labels):
         return self.sample(labels)
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/ranking_metric.py` & `transformers4rec-23.6.0/transformers4rec/torch/ranking_metric.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,28 @@
     labels_onehot : bool
         Enable transform the labels to one-hot representation
     """
 
     def __init__(self, top_ks=None, labels_onehot=False):
         super(RankingMetric, self).__init__()
         self.top_ks = top_ks or [2, 5]
+        if not isinstance(self.top_ks, (list, tuple)):
+            self.top_ks = [self.top_ks]
+
         self.labels_onehot = labels_onehot
         # Store the mean of the batch metrics (for each cut-off at topk)
         self.add_state("metric_mean", default=[], dist_reduce_fx="cat")
 
     def update(self, preds: torch.Tensor, target: torch.Tensor, **kwargs):  # type: ignore
         # Computing the metrics at different cut-offs
         if self.labels_onehot:
             target = torch_utils.tranform_label_to_onehot(target, preds.size(-1))
-        metric = self._metric(self.top_ks, preds.view(-1, preds.size(-1)), target)
+        metric = self._metric(
+            self.top_ks, preds.view(-1, preds.size(-1)), target.view(-1, target.size(-1))
+        )
         self.metric_mean.append(metric)  # type: ignore
 
     def compute(self):
         # Computing the mean of the batch metrics (for each cut-off at topk)
         return dim_zero_cat(self.metric_mean).mean(0)
 
     @abstractmethod
@@ -122,25 +127,25 @@
 
         ks, scores, labels = torch_utils.check_inputs(ks, scores, labels)
         _, _, topk_labels = torch_utils.extract_topk(ks, scores, labels)
         recalls = torch_utils.create_output_placeholder(scores, ks)
 
         # Compute recalls at K
         num_relevant = torch.sum(labels, dim=-1)
-        rel_indices = (num_relevant != 0).nonzero()
-        rel_count = num_relevant[rel_indices].squeeze()
+        rel_indices = (num_relevant != 0).nonzero().squeeze()
+        rel_count = num_relevant[rel_indices]
 
         if rel_indices.shape[0] > 0:
             for index, k in enumerate(ks):
-                rel_labels = topk_labels[rel_indices, : int(k)].squeeze()
+                rel_labels = topk_labels[rel_indices, : int(k)]
 
-                recalls[rel_indices, index] = (
-                    torch.div(torch.sum(rel_labels, dim=-1), rel_count)
-                    .reshape(len(rel_indices), 1)
-                    .to(dtype=torch.float32)
+                recalls[rel_indices, index] = torch.div(
+                    torch.sum(rel_labels, dim=-1), rel_count
+                ).to(
+                    dtype=torch.float32
                 )  # Ensuring type is double, because it can be float if --fp16
 
         return recalls
 
 
 @ranking_metrics_registry.register_with_multiple_names("avg_precision_at", "avg_precision", "map")
 class AvgPrecisionAt(RankingMetric):
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/tabular/__init__.py` & `transformers4rec-23.6.0/transformers4rec/torch/tabular/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/tabular/aggregation.py` & `transformers4rec-23.6.0/transformers4rec/torch/tabular/aggregation.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,23 +94,44 @@
         else:
             output_size.insert(self.axis, num_features)
 
         return tuple(output_size)
 
 
 class ElementwiseFeatureAggregation(TabularAggregation):
-    def _check_input_shapes_equal(self, inputs):
+    """Base class for aggregation methods that aggregates
+    features element-wise.
+    It implements two check methods to ensure inputs have the correct shape.
+    """
+
+    def _check_input_shapes_equal(self, inputs: TabularData):
+        """Checks if the shapes of all inputs are equal.
+
+        Parameters
+        ----------
+        inputs : TabularData
+            Dictionary of tensors.
+
+        """
         all_input_shapes_equal = len(set([x.shape for x in inputs.values()])) == 1
         if not all_input_shapes_equal:
             raise ValueError(
                 "The shapes of all input features are not equal, which is required for"
                 " element-wise aggregation: {}".format({k: v.shape for k, v in inputs.items()})
             )
 
     def _check_inputs_last_dim_equal(self, inputs_sizes):
+        """
+        Checks if the last dimensions of all inputs are equal.
+
+        Parameters
+        ----------
+        inputs_sizes : dict[str, Union[List[int], torch.Size]]
+            A dictionary containing the sizes of the inputs.
+        """
         all_input_last_dim_equal = len(set([x[-1] for x in inputs_sizes.values()])) == 1
         if not all_input_last_dim_equal:
             raise ValueError(
                 f"The last dim of all input features is not equal, which is"
                 f" required for element-wise aggregation: {inputs_sizes}"
             )
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/tabular/base.py` & `transformers4rec-23.6.0/transformers4rec/torch/tabular/base.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/tabular/transformations.py` & `transformers4rec-23.6.0/transformers4rec/torch/tabular/transformations.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/trainer.py` & `transformers4rec-23.6.0/transformers4rec/torch/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -524,58 +524,76 @@
                 labels = self._pad_across_processes(labels)
                 labels = self._nested_gather(labels)
                 labels_host = (
                     labels
                     if labels_host is None
                     else nested_concat(labels_host, labels, padding_index=0)
                 )
-            if preds is not None and self.args.predict_top_k > 0:
-                if self.model.top_k:
-                    raise ValueError(
-                        "you cannot set top_k argument in the model class and the, "
-                        "predict_top_k  in the trainer at the same time. Please ensure setting "
-                        "only predict_top_k"
-                    )
+
+            if (
+                preds is not None
+                and any(isinstance(x, NextItemPredictionTask) for x in model.prediction_tasks)
+                and (self.args.predict_top_k or self.model.top_k)
+            ):
                 # get outputs of next-item scores
                 if isinstance(preds, dict):
-                    assert any(
-                        isinstance(x, NextItemPredictionTask) for x in model.prediction_tasks
-                    ), "Top-k prediction is specific to NextItemPredictionTask, "
-                    "Please ensure `self.args.predict_top_k == 0` "
                     pred_next_item = preds["next-item"]
                 else:
-                    assert isinstance(
-                        model.prediction_tasks[0], NextItemPredictionTask
-                    ), "Top-k prediction is specific to NextItemPredictionTask, "
-                    "Please ensure `self.args.predict_top_k == 0` "
                     pred_next_item = preds
 
-                preds_sorted_item_scores, preds_sorted_item_ids = torch.topk(
-                    pred_next_item, k=self.args.predict_top_k, dim=-1
-                )
-                self._maybe_log_predictions(
-                    labels,
-                    preds_sorted_item_ids,
-                    preds_sorted_item_scores,
-                    # outputs["pred_metadata"],
-                    metrics_results_detailed,
-                    metric_key_prefix,
-                )
-                # The output predictions will be a tuple with the ranked top-n item ids,
-                # and item recommendation scores
-                if isinstance(preds, dict):
-                    preds["next-item"] = (
-                        preds_sorted_item_ids,
-                        preds_sorted_item_scores,
+                preds_sorted_item_scores = None
+                preds_sorted_item_ids = None
+
+                if self.model.top_k is not None and isinstance(pred_next_item, (list, tuple)):
+                    preds_sorted_item_scores, preds_sorted_item_ids = pred_next_item
+
+                    if self.args.predict_top_k:
+                        if self.args.predict_top_k > self.model.top_k:
+                            raise ValueError(
+                                "The args.predict_top_k should not be larger than model.top_k. "
+                                "The model.top_k is available to support inference (e.g. when "
+                                "serving with Triton Inference Server) to return only the top-k "
+                                "predicted items ids and their scores."
+                                "When doing offline predictions with `trainer.predict(), "
+                                "if you set model.top_k, the model will also limit the number of "
+                                "predictions output from trainer.predict(). "
+                                "In that case, you want either to reduce args.predict_top_k or "
+                                "increase model.top_k, so that args.predict_top_k is "
+                                "not larger than model.top_k."
+                            )
+                        preds_sorted_item_scores = preds_sorted_item_scores[
+                            :, : self.args.predict_top_k
+                        ]
+                        preds_sorted_item_ids = preds_sorted_item_ids[:, : self.args.predict_top_k]
+                elif self.args.predict_top_k:
+                    preds_sorted_item_scores, preds_sorted_item_ids = torch.topk(
+                        pred_next_item, k=self.args.predict_top_k, dim=-1
                     )
-                else:
-                    preds = (
+
+                if preds_sorted_item_scores is not None:
+                    self._maybe_log_predictions(
+                        labels,
                         preds_sorted_item_ids,
                         preds_sorted_item_scores,
+                        # outputs["pred_metadata"],
+                        metrics_results_detailed,
+                        metric_key_prefix,
                     )
+                    # The output predictions will be a tuple with the ranked top-n item ids,
+                    # and item recommendation scores
+                    if isinstance(preds, dict):
+                        preds["next-item"] = (
+                            preds_sorted_item_ids,
+                            preds_sorted_item_scores,
+                        )
+                    else:
+                        preds = (
+                            preds_sorted_item_ids,
+                            preds_sorted_item_scores,
+                        )
 
             preds_host = (
                 preds
                 if preds_host is None
                 else nested_concat(
                     preds_host,
                     preds,
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/typing.py` & `transformers4rec-23.6.0/transformers4rec/torch/typing.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/utils/__init__.py` & `transformers4rec-23.6.0/transformers4rec/torch/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/utils/data_utils.py` & `transformers4rec-23.6.0/transformers4rec/torch/utils/data_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
 import numpy as np
 import torch
 from merlin.dataloader.torch import Loader
 from merlin.models.utils.misc_utils import validate_dataset
 from merlin.models.utils.registry import Registry
 from merlin.schema import Tags
+from merlin.schema.io.tensorflow_metadata import TensorflowMetadata
 from torch.utils.data import DataLoader as PyTorchDataLoader
 from torch.utils.data import Dataset, IterableDataset
 
 from merlin_standard_lib import Schema
 from transformers4rec.torch.utils.padding import pad_batch
 
 from ...utils import dependencies
@@ -211,15 +212,15 @@
 
 @dataloader_registry.register_with_multiple_names(
     "merlin_dataloader", "merlin", "nvtabular_dataloader", "nvtabular"
 )
 class MerlinDataLoader(T4RecDataLoader, DLDataLoader):
     """
     This class extends the [Merlin data loader]
-    (https://github.com/NVIDIA-Merlin/dataloader/blob/main/merlin/dataloader/torch.py).
+    (https://github.com/NVIDIA-Merlin/dataloader/blob/stable/merlin/dataloader/torch.py).
     The data input requires a merlin.io.Dataset or a path to the data files.
     It also sets the dataset's schema with the necessary properties to prepare the input
     list features as dense tensors (i.e. padded to the specified `max_sequence_length`).
     The dense representation is required by the Transformers4Rec input modules.
 
     Parameters
     ----------
@@ -235,33 +236,26 @@
         By default None.
     conts: List[str], optional
         The list of continuous columns in the dataset.
         By default None.
     labels : List[str], optional
         The list of label columns in the dataset.
         By default None.
+    lists : List[str], optional
+        The list of sequential columns in the dataset.
+        By default None.
     shuffle : bool, optional
         Enable/disable shuffling of dataset.
         By default False.
     parts_per_chunk : int, optional
         The number of partitions from the iterator, an Merlin Dataset,
         to concatenate into a "chunk". By default 1.
     device : int, optional
         The device id of the selected GPU
         By default None.
-    sparse_names : [str], optional
-        List with column names of columns that should be represented as sparse tensors.
-        By default None.
-    sparse_max : Dict[str, int], optional
-        A dictionary of key: column_name + value: integer representing the max sequence
-        length for a list column.
-        By default None.
-    sparse_as_dense : bool, optional
-        Boolean value to activate transforming sparse tensors to dense ones.
-        By default None.
     drop_last: bool, optional
         Whether or not to drop the last batch in an epoch. This is useful when you need to
         guarantee that each batch contains exactly `batch_size` rows - since the last batch
         will usually contain fewer rows.
     seed_fn: callable
         Function used to initialize random state
     parts_per_chunk: int
@@ -279,53 +273,55 @@
         Extra arguments to pass to the merlin.io.Dataset object, when the path to data files
         is provided in `paths_or_dataset` argument.
     row_groups_per_part: bool, optional
         If true, preserve the group partitions when loading the dataset from parquet files.
     collate_fn: Callable, optional
         A processing function to collect and prepare the list samples
         (tuple of (input, target) Tensor(s)) returned by the Merlin DataLoader.
+    transforms: List[merlin.dag.BaseOperator]
+        A list of operators that the Merlin dataloader applies on top of the loaded
+        batch, which is a tuple of input and target tensors.
     """
 
     def __init__(
         self,
         paths_or_dataset,
         batch_size,
-        max_sequence_length,
+        max_sequence_length=None,
         conts=None,
         cats=None,
         labels=None,
+        lists=None,
         collate_fn=lambda x: x[0],
         engine=None,
         buffer_size=0.1,
         reader_kwargs=None,
         shuffle=False,
         seed_fn=None,
         parts_per_chunk=1,
         device=None,
         global_size=None,
         global_rank=None,
-        sparse_names=None,
-        sparse_max=None,
-        sparse_as_dense=True,
         drop_last=False,
         schema=None,
         row_groups_per_part=True,
+        transforms=None,
         **kwargs,
     ):
         T4RecDataLoader.__init__(self)
 
         self.paths_or_dataset = paths_or_dataset
         self.batch_size = batch_size
         self.shuffle = shuffle
         self.max_sequence_length = max_sequence_length
         self.drop_last = drop_last
 
         reader_kwargs = reader_kwargs or {}
         reader_kwargs["row_groups_per_part"] = row_groups_per_part
-        self.set_dataset(buffer_size, engine, reader_kwargs)
+        self.set_dataset(buffer_size, engine, reader_kwargs, schema=schema)
 
         if (global_rank is not None) and (self.dataset.npartitions < global_size):
             logger.warning(
                 "UserWarning: User is advised to repartition the parquet file before training "
                 "so npartitions>=global_size. Cudf or pandas can be used for repartitioning "
                 "eg. pdf.to_parquet('file.parquet',row_group_size=N_ROWS/NPARTITIONS) for pandas "
                 "or gdf.to_parquet('file.parquet',row_group_size_rows=N_ROWS/NPARTITIONS) for cudf "
@@ -339,28 +335,39 @@
                 f"UserWarning: User is advised to set the number of partitions"
                 f" ({self.dataset.npartitions}) divisible by the number of available"
                 f" GPUs ({global_size}). This will divide the work equally among GPUs"
                 " for DDP training and ensure optimal performance."
             )
 
         self.dataset.schema = self._augment_schema(
-            self.dataset.schema, cats=cats, conts=conts, labels=labels
+            self.dataset.schema,
+            cats=cats,
+            conts=conts,
+            labels=labels,
+            lists=lists,
         )
 
         loader = Loader(
             self.dataset,
             self.batch_size,
             shuffle,
             seed_fn=seed_fn,
             parts_per_chunk=parts_per_chunk,
             device=device,
             global_size=global_size,
             global_rank=global_rank,
             drop_last=drop_last,
-        ).map(self._get_pad_fn(sparse_max))
+            transforms=transforms,
+        )
+        if max_sequence_length:
+            # Apply padding
+            output_schema = loader.output_schema
+            sparse_feats = [col.name for col in output_schema if Tags.LIST in col.tags]
+            sparse_max = {name: max_sequence_length for name in sparse_feats}
+            loader = loader.map(self._get_pad_fn(sparse_max))
 
         DLDataLoader.__init__(
             self,
             loader,
             collate_fn=collate_fn,
             batch_size=self.batch_size,
             drop_last=self.drop_last,
@@ -382,102 +389,114 @@
 
     @staticmethod
     def _augment_schema(
         schema,
         cats=None,
         conts=None,
         labels=None,
+        lists=None,
     ):
         cats = cats or []
         conts = conts or []
         labels = labels or []
 
-        schema = schema.select_by_name(conts + cats + labels)
+        schema = schema.select_by_name(conts + cats + labels + lists)
 
         labels = [labels] if isinstance(labels, str) else labels
         for label in labels:
             schema[label] = schema[label].with_tags(Tags.TARGET)
         for label in cats:
             schema[label] = schema[label].with_tags(Tags.CATEGORICAL)
         for label in conts:
             schema[label] = schema[label].with_tags(Tags.CONTINUOUS)
+        for col in lists:
+            schema[col] = schema[col].with_tags(Tags.LIST)
 
         return schema
 
-    def set_dataset(self, buffer_size, engine, reader_kwargs):
+    def set_dataset(self, buffer_size, engine, reader_kwargs, schema=None):
         dataset = validate_dataset(
             self.paths_or_dataset,
             self.batch_size,
             buffer_size,
             engine,
             reader_kwargs,
         )
+        if schema:
+            # set the dataset schema based on the provided one to keep all original information
+            if isinstance(schema, Schema):
+                # convert merlin-standardlib schema to merlin-core schema
+                schema = to_core_schema(schema)
+            dataset.schema = schema
         self.dataset = dataset
 
     @classmethod
     def from_schema(
         cls,
         schema: Schema,
         paths_or_dataset,
         batch_size,
-        max_sequence_length,
+        max_sequence_length=None,
         continuous_features=None,
         categorical_features=None,
+        list_features=None,
         targets=None,
         collate_fn=lambda x: x[0],
         shuffle=True,
         buffer_size=0.06,
         parts_per_chunk=1,
-        sparse_names=None,
-        sparse_max=None,
+        transforms=None,
         **kwargs,
     ):
         """
             Instantitates `MerlinDataLoader` from a ``DatasetSchema``.
         Parameters
         ----------
             schema: DatasetSchema
                 Dataset schema
             paths_or_dataset: Union[str, Dataset]
                 Path to paquet data of Dataset object.
             batch_size: int
                 batch size of Dataloader.
-            max_sequence_length: int
-                The maximum length of list features.
         """
         categorical_features = (
             categorical_features or schema.select_by_tag(Tags.CATEGORICAL).column_names
         )
         continuous_features = (
             continuous_features or schema.select_by_tag(Tags.CONTINUOUS).column_names
         )
         targets = targets or schema.select_by_tag(Tags.TARGET).column_names
-        schema = schema.select_by_name(categorical_features + continuous_features + targets)
-        sparse_names = sparse_names or schema.select_by_tag(Tags.LIST).column_names
-        sparse_max = sparse_max or {name: max_sequence_length for name in sparse_names}
+        list_features = list_features or schema.select_by_tag(Tags.LIST).column_names
+        schema = schema.select_by_name(
+            categorical_features + continuous_features + targets + list_features
+        )
         loader = cls(
             paths_or_dataset,
             batch_size=batch_size,
-            max_sequence_length=max_sequence_length,
             labels=targets,
+            max_sequence_length=max_sequence_length,
             cats=categorical_features,
             conts=continuous_features,
+            lists=list_features,
             collate_fn=collate_fn,
             engine="parquet",
             shuffle=shuffle,
             buffer_size=buffer_size,  # how many batches to load at once
             parts_per_chunk=parts_per_chunk,
-            sparse_names=sparse_names,
-            sparse_max=sparse_max,
             schema=schema,
+            transforms=transforms,
             **kwargs,
         )
 
         return loader
 
+    @property
+    def output_schema(self):
+        return self.dataset.output_schema
+
 
 class ParquetDataset(Dataset):
     def __init__(self, parquet_file, cols_to_read, target_names, seq_features_len_pad_trim):
         self.cols_to_read = cols_to_read
         self.target_names = target_names
         self.data = pq.ParquetDataset(parquet_file).read(columns=self.cols_to_read).to_pandas()
         self.seq_features_len_pad_trim = seq_features_len_pad_trim
@@ -516,7 +535,11 @@
         logger.info("[SHUFFLE] INITIALIZING BUFFER_SIZE: {}".format(self.buffer_size))
 
         raise StopIteration()
         # TODO define The shuffle method for pyarrow dataloader
 
     def __len__(self):
         return len(self.dataset)
+
+
+def to_core_schema(t4rec_schema):
+    return TensorflowMetadata.from_json(t4rec_schema.to_json()).to_merlin_schema()
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/utils/examples_utils.py` & `transformers4rec-23.6.0/transformers4rec/torch/utils/examples_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/utils/padding.py` & `transformers4rec-23.6.0/transformers4rec/torch/utils/padding.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,19 @@
 import torch.nn.functional as F
 
 
 def _pad_dense_tensor(t: torch.Tensor, length: int) -> torch.Tensor:
     if len(t.shape) == 2:
         pad_diff = length - t.shape[1]
         return F.pad(input=t, pad=(0, pad_diff, 0, 0))
-    return t
+    elif len(t.shape) == 3:
+        pad_diff = length - t.shape[1]
+        return F.pad(input=t, pad=(0, pad_diff, 0, 0, 0, 0))
+    else:
+        return t
 
 
 def _squeeze(tensor: torch.Tensor):
     if len(tensor.shape) == 2:
         return tensor.squeeze(1)
     return tensor
 
@@ -44,17 +48,27 @@
 def _pad_ragged_tensor(values: torch.Tensor, offsets: torch.Tensor, padding_length: int):
     values = _squeeze(values)
     offsets = _squeeze(offsets)
     num_rows = len(offsets) - 1
     diff_offsets = offsets[1:] - offsets[:-1]
     max_length = int(diff_offsets.max())
     indices = _get_indices(offsets, diff_offsets)
-    sparse_tensor = torch.sparse_coo_tensor(
-        indices.T, values, torch.Size([num_rows, max_length]), device=values.device
-    )
+
+    if values.ndim == 2:
+        # 3D ragged inputs
+        sparse_tensor = torch.sparse_coo_tensor(
+            indices.T,
+            values,
+            torch.Size([num_rows, max_length, values.shape[-1]]),
+            device=values.device,
+        )
+    else:
+        sparse_tensor = torch.sparse_coo_tensor(
+            indices.T, values, torch.Size([num_rows, max_length]), device=values.device
+        )
     return _pad_dense_tensor(sparse_tensor.to_dense(), padding_length)
 
 
 @torch.jit.script
 def pad_batch(
     batch: Dict[str, torch.Tensor], padding_lengths: Dict[str, int]
 ) -> Dict[str, torch.Tensor]:
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/utils/schema_utils.py` & `transformers4rec-23.6.0/transformers4rec/torch/utils/schema_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,46 @@
     num_rows: int,
     max_session_length: Optional[int] = None,
     min_session_length: int = 5,
     device=None,
     ragged=False,
     seed=0,
 ) -> TabularData:
+    """Generates random tabular data based on a given schema.
+    The generated data can be used for testing
+    data preprocessing or model training pipelines.
+
+    Parameters
+    ----------
+    schema : Schema
+        The schema to be used for generating the random tabular data.
+    num_rows : int
+        The number of rows.
+    max_session_length : Optional[int]
+        The maximum session length.
+        If None, the session length will not be limited.
+        By default None
+    min_session_length : int
+        The minimum session length.
+        By default 5
+    device : torch.device
+        The device on which the synthetic data should be created.
+        If None, the synthetic data will be created on the CPU.
+        By default None
+    ragged : bool
+        If True, the sequence features will be represented with __values and __offsets.
+        By default False
+
+    Returns
+    -------
+    TabularData
+        A dictionary where each key is a feature name and each value is the generated
+        tensor.
+
+    """
     data: Dict[str, Any] = {}
 
     random.seed(seed)
     np.random.seed(seed)
     if seed:
         torch.manual_seed(seed)
```

### Comparing `transformers4rec-23.5.0/transformers4rec/torch/utils/torch_utils.py` & `transformers4rec-23.6.0/transformers4rec/torch/utils/torch_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 from dataclasses import dataclass
 from typing import Dict, Optional, Union
 
 import numpy as np
 import torch
 from merlin.schema import Schema as CoreSchema
 from merlin.schema.io.proto_utils import has_field
+from merlin.schema.tags import Tags
 
 from merlin_standard_lib import Schema
 from merlin_standard_lib.schema.schema import ColumnSchema
 
 from ...config.schema import SchemaMixin
 from ..typing import TabularData
 
@@ -163,22 +164,36 @@
 def get_output_sizes_from_schema(schema: Schema, batch_size=-1, max_sequence_length=None):
     sizes = {}
 
     features = schema if isinstance(schema, CoreSchema) else schema.feature
 
     for feature in features:
         name = feature.name
+        # Pretrained embeddings (2-D or 3-D)
+        if Tags.EMBEDDING in feature.tags:
+            if len(feature.shape.dims) > 2:
+                sizes[name] = torch.Size(
+                    [
+                        batch_size,
+                        max_sequence_length if max_sequence_length else feature.value_count.max,
+                        feature.shape[-1].min,
+                    ]
+                )
+            else:
+                sizes[name] = torch.Size([batch_size, feature.shape[-1].min])
+
         # Sequential or multi-hot feature
-        if _has_field(feature, "value_count"):
+        elif _has_field(feature, "value_count"):
             sizes[name] = torch.Size(
                 [
                     batch_size,
                     max_sequence_length if max_sequence_length else feature.value_count.max,
                 ]
             )
+
         else:
             sizes[name] = _get_size_from_shape(feature, batch_size)
 
     return sizes
 
 
 def calculate_batch_size_from_input_size(input_size):
```

### Comparing `transformers4rec-23.5.0/transformers4rec/types.py` & `transformers4rec-23.6.0/transformers4rec/types.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/utils/__init__.py` & `transformers4rec-23.6.0/transformers4rec/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/utils/data_utils.py` & `transformers4rec-23.6.0/transformers4rec/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec/utils/dependencies.py` & `transformers4rec-23.6.0/transformers4rec/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec.egg-info/PKG-INFO` & `transformers4rec-23.6.0/transformers4rec.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers4rec
-Version: 23.5.0
+Version: 23.6.0
 Summary: UNKNOWN
 Home-page: https://github.com/NVIDIA-Merlin/Transformers4Rec
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -20,16 +20,16 @@
 Provides-Extra: dev
 Provides-Extra: all
 License-File: LICENSE
 
 # [Transformers4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/)
 
 [![PyPI](https://img.shields.io/pypi/v/Transformers4Rec?color=orange&label=version)](https://pypi.python.org/pypi/Transformers4Rec)
-[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/Transformers4Rec)](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/main/LICENSE)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/Transformers4Rec/main/README.html)
+[![LICENSE](https://img.shields.io/github/license/NVIDIA-Merlin/Transformers4Rec)](https://github.com/NVIDIA-Merlin/Transformers4Rec/blob/stable/LICENSE)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/Transformers4Rec/stable/README.html)
 
 Transformers4Rec is a flexible and efficient library for sequential and session-based recommendation and can work with PyTorch.
 
 The library works as a bridge between natural language processing (NLP) and recommender systems (RecSys) by integrating with one of the most popular NLP frameworks, [Hugging Face Transformers](https://github.com/huggingface/transformers) (HF).
 Transformers4Rec makes state-of-the-art transformer architectures available for RecSys researchers and industry practitioners.
 
 The following figure shows the use of the library in a recommender system.
@@ -70,15 +70,15 @@
 You can normalize and combine interaction and sequence-level input features in configurable ways.
 
 - **Seamless preprocessing and feature engineering**: As part of the Merlin ecosystem, Transformers4Rec is integrated with [NVTabular](https://github.com/NVIDIA-Merlin/NVTabular) and [Triton Inference Server](https://github.com/triton-inference-server/server).
 These components enable you to build a fully GPU-accelerated pipeline for sequential and session-based recommendation.
 NVTabular has common preprocessing operations for session-based recommendation and exports a dataset schema.
 The schema is compatible with Transformers4Rec so that input features can be configured automatically.
 You can export your trained models to serve with Triton Inference Server in a single pipeline that includes online feature preprocessing and model inference.
-For more information, refer to [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/main/pipeline.html).
+For more information, refer to [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/stable/pipeline.html).
 
 <img src="_images/pipeline.png" alt="GPU-accelerated Sequential and Session-based recommendation" style="width:600px;display:block;margin-left:auto;margin-right:auto;"/><br>
 <div style="text-align: center; margin: 20pt">
   <figcaption style="font-style: italic;">GPU-accelerated pipeline for Sequential and Session-based recommendation using NVIDIA Merlin components</figcaption>
 </div>
 
 ## Transformers4Rec Achievements
@@ -87,23 +87,23 @@
 The library provides higher accuracy for session-based recommendation than baseline algorithms and we performed extensive empirical analysis about the accuracy.
 These observations are published in our [ACM RecSys'21 paper](https://dl.acm.org/doi/10.1145/3460231.3474255).
 
 ## Sample Code: Defining and Training the Model
 
 Training a model with Transformers4Rec typically requires performing the following high-level steps:
 
-1. Provide the [schema](https://nvidia-merlin.github.io/Transformers4Rec/main/api/merlin_standard_lib.schema.html#merlin_standard_lib.schema.schema.Schema) and construct an input-module.
+1. Provide the [schema](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/merlin_standard_lib.schema.html#merlin_standard_lib.schema.schema.Schema) and construct an input-module.
 
    If you encounter session-based recommendation issues, you typically want to use the
-   [TabularSequenceFeatures](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.features.html#transformers4rec.torch.features.sequence.TabularSequenceFeatures)
+   [TabularSequenceFeatures](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.features.html#transformers4rec.torch.features.sequence.TabularSequenceFeatures)
    class because it merges context features with sequential features.
 
 2. Provide the prediction-tasks.
 
-   The tasks that are provided right out of the box are available from our [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.model.html#module-transformers4rec.torch.model.prediction_task).
+   The tasks that are provided right out of the box are available from our [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.model.html#module-transformers4rec.torch.model.prediction_task).
 
 3. Construct a transformer-body and convert this into a model.
 
 The following code sample shows how to define and train an XLNet model with PyTorch for next-item prediction task:
 
 ```python
 from transformers4rec import torch as tr
@@ -150,15 +150,15 @@
 model = tr.Model(head)
 ```
 
 > You can modify the preceding code to perform binary classification.
 > The masking in the input module can be set to `None` instead of `causal`.
 > When you define the head, you can replace the `NextItemPredictionTask`
 > with an instance of `BinaryClassificationTask`.
-> See the sample code in the [API documentation for the class](https://nvidia-merlin.github.io/Transformers4Rec/main/api/transformers4rec.torch.html#transformers4rec.torch.BinaryClassificationTask).
+> See the sample code in the [API documentation for the class](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/transformers4rec.torch.html#transformers4rec.torch.BinaryClassificationTask).
 
 ## Installation
 
 You can install Transformers4Rec with Pip, Conda, or run a Docker container.
 
 ### Installing Transformers4Rec Using Pip
 
@@ -194,29 +194,29 @@
     cudatoolkit=11.8 pytorch-cuda=11.8 `# NVIDIA CUDA version`
 ```
 
 ### Installing Transformers4Rec Using Docker
 
 Transformers4Rec is pre-installed in the `merlin-pytorch` container that is available from the NVIDIA GPU Cloud (NGC) catalog.
 
-Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
+Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/stable/containers.html) documentation page for information about the Merlin container names, URLs to container images in the catalog, and key Merlin components.
 
 ## Notebook Examples and Tutorials
 
-The [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/main/pipeline.html) page
+The [End-to-end pipeline with NVIDIA Merlin](https://nvidia-merlin.github.io/Transformers4Rec/stable/pipeline.html) page
 shows how to use Transformers4Rec and other Merlin libraries like NVTabular to build a complete recommender system.
 
 We have several [example](./examples) notebooks to help you build a recommender system or integrate Transformers4Rec into your system:
 
 - A getting started example that includes training a session-based model with an XLNET transformer architecture.
 - An end-to-end example that trains a model and takes the next step to serve inference with Triton Inference Server.
 - Another end-to-end example that trains and evaluates a session-based model on RNN and also serves inference with Triton Inference Server.
 - A notebook and scripts that reproduce the experiments presented in a paper for RecSys 2021.
 
 ## Feedback and Support
 
 If you'd like to make direct contributions to Transformers4Rec, refer to [Contributing to Transformers4Rec](CONTRIBUTING.md). We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations. To further advance our Merlin roadmap, we encourage you to share all the details regarding your recommender system pipeline by going to https://developer.nvidia.com/merlin-devzone-survey.
 
 If you're interested in learning more about how Transformers4Rec works, refer to our
-[Transformers4Rec documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/getting_started.html). We also have [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/main/api/modules.html) that outlines the specifics of the available modules and classes within Transformers4Rec.
+[Transformers4Rec documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/getting_started.html). We also have [API documentation](https://nvidia-merlin.github.io/Transformers4Rec/stable/api/modules.html) that outlines the specifics of the available modules and classes within Transformers4Rec.
```

### Comparing `transformers4rec-23.5.0/transformers4rec.egg-info/SOURCES.txt` & `transformers4rec-23.6.0/transformers4rec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `transformers4rec-23.5.0/transformers4rec.egg-info/requires.txt` & `transformers4rec-23.6.0/transformers4rec.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 transformers[torch]<5,>=4.12
 tqdm>=4.27
 pyarrow>=1.0
 torchmetrics>=0.10.0
-merlin-models>=0.11
+merlin-models<23.07,>=23.06
 
 [all]
 transformers[torch]<5,>=4.12
 tqdm>=4.27
 pyarrow>=1.0
 torchmetrics>=0.10.0
-merlin-models>=0.11
+merlin-models<23.07,>=23.06
 torch>=1.0
 torchmetrics>=0.10.0
 nvtabular
 Sphinx<3.6
 sphinx_rtd_theme==1.0.0
 sphinx-multiversion@ git+https://github.com/mikemckiernan/sphinx-multiversion.git
 sphinxcontrib-copydirs@ git+https://github.com/mikemckiernan/sphinxcontrib-copydirs.git
@@ -28,15 +28,15 @@
 bandit
 
 [base]
 transformers[torch]<5,>=4.12
 tqdm>=4.27
 pyarrow>=1.0
 torchmetrics>=0.10.0
-merlin-models>=0.11
+merlin-models<23.07,>=23.06
 
 [dev]
 check-manifest
 bandit
 
 [docs]
 Sphinx<3.6
```

### Comparing `transformers4rec-23.5.0/versioneer.py` & `transformers4rec-23.6.0/versioneer.py`

 * *Files identical despite different names*

