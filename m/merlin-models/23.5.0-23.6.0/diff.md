# Comparing `tmp/merlin-models-23.5.0.tar.gz` & `tmp/merlin-models-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merlin-models-23.5.0.tar", last modified: Wed May 31 14:39:51 2023, max compression
+gzip compressed data, was "merlin-models-23.6.0.tar", last modified: Thu Jun 22 20:53:53 2023, max compression
```

## Comparing `merlin-models-23.5.0.tar` & `merlin-models-23.6.0.tar`

### file list

```diff
@@ -1,428 +1,468 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-31 14:39:25.000000 merlin-models-23.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-05-31 14:39:25.000000 merlin-models-23.5.0/CLA.md
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-31 14:39:25.000000 merlin-models-23.5.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-05-31 14:39:25.000000 merlin-models-23.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-31 14:39:25.000000 merlin-models-23.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-31 14:39:25.000000 merlin-models-23.5.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-31 14:39:51.915997 merlin-models-23.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-05-31 14:39:25.000000 merlin-models-23.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.815997 merlin-models-23.5.0/conda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/conda/recipes/
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-31 14:39:25.000000 merlin-models-23.5.0/conda/recipes/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.815997 merlin-models-23.5.0/merlin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/advertising/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/advertising/criteo/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/criteo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/criteo/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25620 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/ecommerce/
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14826 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.823997 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/transformed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/transformed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/large/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/large/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/large/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/small/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/small/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/small/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/entertainment/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.827997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/movielens/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.831997 merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/datasets/social/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/social/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/social/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/datasets/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/merlin/models/
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-31 14:39:51.915997 merlin-models-23.5.0/merlin/models/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/models/config/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/config/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/models/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/implicit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.835997 merlin-models-23.5.0/merlin/models/lightfm/
--rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/lightfm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.839997 merlin-models-23.5.0/merlin/models/loader/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/loader/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.839997 merlin-models-23.5.0/merlin/models/tf/
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.839997 merlin-models-23.5.0/merlin/models/tf/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/dlrm.py
--rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    21771 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.843997 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/two_tower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.843997 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/blocks/sampling/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29012 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/combinators.py
--rw-r--r--   0 runner    (1001) docker     (123)    20418 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/core/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/distributed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/distributed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/distributed/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/distributed/embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/experimental/sample_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13298 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/inputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/inputs/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    51818 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/inputs/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.847997 merlin-models-23.5.0/merlin/models/tf/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/logging/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.851997 merlin-models-23.5.0/merlin/models/tf/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/losses/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/losses/listwise.py
--rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/losses/pairwise.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.851997 merlin-models-23.5.0/merlin/models/tf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/metrics/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20291 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/metrics/topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.851997 merlin-models-23.5.0/merlin/models/tf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    99187 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    23318 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)    21734 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.855997 merlin-models-23.5.0/merlin/models/tf/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11003 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12173 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/block.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17911 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.855997 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/sampling/popularity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12246 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/outputs/topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.859997 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     9831 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/next_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     6705 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/prediction_tasks/retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.859997 merlin-models-23.5.0/merlin/models/tf/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transformers/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transformers/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.859997 merlin-models-23.5.0/merlin/models/tf/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/bias.py
--rw-r--r--   0 runner    (1001) docker     (123)    54513 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/negative_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/noise.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/regularization.py
--rw-r--r--   0 runner    (1001) docker     (123)    46941 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/transforms/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.863997 merlin-models-23.5.0/merlin/models/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/repr_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18552 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17673 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/tf/utils/tf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.863997 merlin-models-23.5.0/merlin/models/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     9935 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/block.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.863997 merlin-models-23.5.0/merlin/models/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6465 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/utils/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/torch/utils/torchscript_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.867997 merlin-models-23.5.0/merlin/models/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/doc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/example_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/nvt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/utils/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.867997 merlin-models-23.5.0/merlin/models/xgb/
--rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-05-31 14:39:25.000000 merlin-models-23.5.0/merlin/models/xgb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.871997 merlin-models-23.5.0/merlin_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 14:39:51.000000 merlin-models-23.5.0/merlin_models.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-31 14:39:25.000000 merlin-models-23.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 14:39:25.000000 merlin-models-23.5.0/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.871997 merlin-models-23.5.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/horovod-cpu-environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/horovod.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/implicit.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/lightfm.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/nvtabular.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/pytorch.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/tensorflow.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/transformers.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-31 14:39:25.000000 merlin-models-23.5.0/requirements/xgboost.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-31 14:39:51.915997 merlin-models-23.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-31 14:39:25.000000 merlin-models-23.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/common/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/common/tf/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_tests_common.py
--rw-r--r--   0 runner    (1001) docker     (123)    25747 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/common/tf/tests_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.875997 merlin-models-23.5.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/integration/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/integration/tf/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/retrieval/test_integration_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_01_getting_started.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_02_dataschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_03_exploring_different_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_04_export_ranking_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_05_export_retrieval_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/unit/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/config/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/unit/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_advertising.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_ecommerce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_entertainment.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_social.py
--rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/datasets/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.879997 merlin-models-23.5.0/tests/unit/implicit/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/implicit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/implicit/test_implicit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.883997 merlin-models-23.5.0/tests/unit/lightfm/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/lightfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/lightfm/test_lightfm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.883997 merlin-models-23.5.0/tests/unit/tf/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/_conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.883997 merlin-models-23.5.0/tests/unit/tf/blocks/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.887997 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_two_tower.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.887997 merlin-models-23.5.0/tests/unit/tf/blocks/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/sampling/test_cross_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/sampling/test_in_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_cross.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_dlrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/blocks/test_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.891997 merlin-models-23.5.0/tests/unit/tf/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_combinators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/core/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.895997 merlin-models-23.5.0/tests/unit/tf/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_01_getting_started.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_02_dataschema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_03_exploring_different_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_04_export_ranking_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_05_export_retrieval_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_07_train_traditional_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_incremental_training_layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_pretrained_embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.895997 merlin-models-23.5.0/tests/unit/tf/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/experimental/test_sample_weight.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.895997 merlin-models-23.5.0/tests/unit/tf/horovod/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/horovod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/horovod/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/horovod/test_horovod.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.899997 merlin-models-23.5.0/tests/unit/tf/inputs/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/inputs/test_tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.899997 merlin-models-23.5.0/tests/unit/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/layers/test_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.899997 merlin-models-23.5.0/tests/unit/tf/losses/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/losses/test_losses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.899997 merlin-models-23.5.0/tests/unit/tf/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/metrics/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/metrics/test_metrics_topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.903997 merlin-models-23.5.0/tests/unit/tf/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54988 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    18802 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/test_ranking.py
--rw-r--r--   0 runner    (1001) docker     (123)    36718 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/models/test_retrieval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.903997 merlin-models-23.5.0/tests/unit/tf/outputs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_contrastive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/outputs/test_topk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.907997 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_classification.py
--rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_multi_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_next_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/test_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/test_public_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.907997 merlin-models-23.5.0/tests/unit/tf/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24815 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transformers/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transformers/test_transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.911997 merlin-models-23.5.0/tests/unit/tf/transforms/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)    52913 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_negative_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/transforms/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.911997 merlin-models-23.5.0/tests/unit/tf/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/utils/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/utils/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/tf/utils/test_tf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/tests/unit/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/test_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/tests/unit/torch/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6612 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/utils/test_module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/torch/utils/test_torchscript_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/utils/test_schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 14:39:51.915997 merlin-models-23.5.0/tests/unit/xgb/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/xgb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tests/unit/xgb/test_xgboost.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-31 14:39:25.000000 merlin-models-23.5.0/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)    81912 2023-05-31 14:39:25.000000 merlin-models-23.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-22 20:53:30.000000 merlin-models-23.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-06-22 20:53:30.000000 merlin-models-23.6.0/CLA.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-22 20:53:30.000000 merlin-models-23.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-06-22 20:53:30.000000 merlin-models-23.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-22 20:53:30.000000 merlin-models-23.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-22 20:53:30.000000 merlin-models-23.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-06-22 20:53:53.007253 merlin-models-23.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7616 2023-06-22 20:53:30.000000 merlin-models-23.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.971253 merlin-models-23.6.0/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/conda/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-22 20:53:30.000000 merlin-models-23.6.0/conda/recipes/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.975253 merlin-models-23.6.0/merlin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/advertising/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/advertising/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/advertising/criteo/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/advertising/criteo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8197 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/advertising/criteo/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/advertising/criteo/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/advertising/criteo/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25620 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20713 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21339 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10120 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/transformed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/transformed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/preprocessed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19855 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/large/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/large/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13094 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/large/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/small/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/small/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/small/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/ecommerce/transactions/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/ecommerce/transactions/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/entertainment/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.979253 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/100k/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/100k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/100k/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9487 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m-raw/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/25m/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/25m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14821 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/movielens/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/entertainment/music_streaming/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/music_streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/music_streaming/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/entertainment/tenrec_video/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/tenrec_video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/social/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/social/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8744 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/social/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/datasets/testing/sequence_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/testing/sequence_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/datasets/testing/sequence_testing/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/merlin/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 20:53:53.007253 merlin-models-23.6.0/merlin/models/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/models/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/config/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/models/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7474 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/implicit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/models/lightfm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7730 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/lightfm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/models/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/loader/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/models/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/models/tf/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8708 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/dlrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20727 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17064 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21771 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.983253 merlin-models-23.6.0/merlin/models/tf/blocks/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19772 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/retrieval/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/retrieval/two_tower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/blocks/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/sampling/cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/sampling/in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13239 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/blocks/sampling/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16244 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/core/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18151 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29125 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/core/combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27360 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/core/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/core/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21033 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/core/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/distributed/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/distributed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/distributed/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/distributed/embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/experimental/sample_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13409 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/inputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/inputs/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58247 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/inputs/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17233 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/logging/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/losses/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/losses/listwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16402 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/losses/pairwise.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/metrics/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20293 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/metrics/topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103689 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/models/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23319 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/models/ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21909 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/models/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13144 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13175 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17911 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.987253 merlin-models-23.6.0/merlin/models/tf/outputs/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/sampling/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/sampling/in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/sampling/popularity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/outputs/topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/tf/prediction_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/prediction_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17597 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/prediction_tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/prediction_tasks/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/prediction_tasks/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/prediction_tasks/next_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/prediction_tasks/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/prediction_tasks/retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/tf/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17700 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transformers/block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9888 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transformers/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/tf/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12085 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transforms/bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54513 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transforms/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transforms/negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transforms/noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transforms/regularization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47410 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transforms/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/transforms/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/utils/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/utils/repr_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/utils/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18553 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/utils/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17676 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/tf/utils/tf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11664 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10834 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/torch/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/blocks/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11870 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/torch/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/outputs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/outputs/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/outputs/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/torch/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/transforms/agg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.991253 merlin-models-23.6.0/merlin/models/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9686 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/utils/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/utils/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/utils/selection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/torch/utils/torchscript_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/merlin/models/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/ci_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/doc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/example_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/nvt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/utils/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/merlin/models/xgb/
+-rw-r--r--   0 runner    (1001) docker     (123)    12576 2023-06-22 20:53:30.000000 merlin-models-23.6.0/merlin/models/xgb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/merlin_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-06-22 20:53:52.000000 merlin-models-23.6.0/merlin_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14254 2023-06-22 20:53:52.000000 merlin-models-23.6.0/merlin_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:53:52.000000 merlin-models-23.6.0/merlin_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-22 20:53:52.000000 merlin-models-23.6.0/merlin_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 20:53:52.000000 merlin-models-23.6.0/merlin_models.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-22 20:53:30.000000 merlin-models-23.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-22 20:53:30.000000 merlin-models-23.6.0/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/horovod-cpu-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/horovod.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/implicit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/lightfm.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/nvtabular.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/pytorch.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/tensorflow.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/transformers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 20:53:30.000000 merlin-models-23.6.0/requirements/xgboost.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-22 20:53:53.007253 merlin-models-23.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-22 20:53:30.000000 merlin-models-23.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/tests/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/benchmark/test_asvdb_transformers_next_item_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/tests/common/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/common/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/tests/common/tf/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/common/tf/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/common/tf/retrieval/retrieval_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/common/tf/retrieval/retrieval_tests_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25747 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/common/tf/retrieval/retrieval_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/common/tf/tests_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/tests/integration/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.995253 merlin-models-23.6.0/tests/integration/tf/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/retrieval/test_integration_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/test_ci_01_getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/test_ci_02_dataschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/test_ci_03_exploring_different_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/test_ci_04_export_ranking_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/test_ci_05_export_retrieval_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/config/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/datasets/test_advertising.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/datasets/test_ecommerce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/datasets/test_entertainment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/datasets/test_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/datasets/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/implicit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3183 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/implicit/test_implicit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/lightfm/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/lightfm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/lightfm/test_lightfm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/_conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/tf/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/tf/blocks/retrieval/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/retrieval/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8275 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/retrieval/test_two_tower.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/tf/blocks/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/sampling/test_cross_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/sampling/test_in_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/test_cross.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/test_dlrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/test_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8395 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27984 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/blocks/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:52.999253 merlin-models-23.6.0/tests/unit/tf/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/core/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/core/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11391 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/core/test_combinators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/core/test_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/core/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/core/test_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/core/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_01_getting_started.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_02_dataschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_03_exploring_different_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_04_export_ranking_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_05_export_retrieval_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_07_train_traditional_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_incremental_training_layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_pretrained_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/experimental/test_sample_weight.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/horovod/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/horovod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/horovod/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/horovod/test_horovod.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/inputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/inputs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7266 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/inputs/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/inputs/test_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28964 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/inputs/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9230 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/inputs/test_tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/layers/test_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/losses/test_losses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/metrics/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9430 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/metrics/test_metrics_topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54988 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/models/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18802 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/models/test_ranking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36718 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/models/test_retrieval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/outputs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31962 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/outputs/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/outputs/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9079 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/outputs/test_contrastive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/outputs/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/outputs/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/outputs/test_topk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/prediction_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/prediction_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21525 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_multi_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_next_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10694 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/test_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/test_public_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.003253 merlin-models-23.6.0/tests/unit/tf/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24838 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transformers/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transformers/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/tf/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transforms/test_bias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52913 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transforms/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transforms/test_negative_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transforms/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12259 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transforms/test_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/transforms/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/tf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/utils/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/utils/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/tf/utils/test_tf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/torch/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/blocks/test_mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/torch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/models/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/torch/outputs/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/outputs/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/outputs/test_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/outputs/test_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8953 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7708 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8288 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/test_router.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/torch/transforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/transforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/transforms/test_agg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/torch/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8901 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/utils/test_module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/utils/test_schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/utils/test_selection_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/torch/utils/test_torchscript_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/utils/test_schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:53.007253 merlin-models-23.6.0/tests/unit/xgb/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/xgb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tests/unit/xgb/test_xgboost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-06-22 20:53:30.000000 merlin-models-23.6.0/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    81912 2023-06-22 20:53:30.000000 merlin-models-23.6.0/versioneer.py
```

### Comparing `merlin-models-23.5.0/.pre-commit-config.yaml` & `merlin-models-23.6.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         exclude: ^(docs|examples|tests|setup.py|versioneer.py)
         args: [--config=pyproject.toml]
   # yaml formatting
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: v3.0.0-alpha.4
     hooks:
       - id: prettier
-        types: [yaml]
-        exclude: ^.github|^conda
+        types_or: [yaml, markdown]
+        exclude: ^conda
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.2
     hooks:
       - id: codespell
         exclude: retrieval-with-hyperparameter-optimization
   - repo: local
     hooks:
```

### Comparing `merlin-models-23.5.0/CLA.md` & `merlin-models-23.6.0/CLA.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,38 +20,40 @@
 discussing and improving that Project, but excluding communication that is conspicuously marked or
 otherwise designated in writing by You as “Not a Submission.”
 
 “Submission” means the Code and any other copyrightable material Submitted by You, including any
 associated comments and documentation.
 
 ## 2. Your Submission
+
 You must agree to the terms of this Agreement before making a Submission to any
 Project. This Agreement covers any and all Submissions that You, now or in the future (except as
 described in Section 4 below), Submit to any Project.
 
 ## 3. Originality of Work
+
 You represent that each of Your Submissions is entirely Your original work.
 Should You wish to Submit materials that are not Your original work, You may Submit them separately
 to the Project if You (a) retain all copyright and license information that was in the materials as You
 received them, (b) in the description accompanying Your Submission, include the phrase “Submission
 containing materials of a third party:” followed by the names of the third party and any licenses or other
 restrictions of which You are aware, and (c) follow any other instructions in the Project’s written
 guidelines concerning Submissions.
 
 ## 4. Your Employer
+
 References to “employer” in this Agreement include Your employer or anyone else
 for whom You are acting in making Your Submission, e.g. as a contractor, vendor, or agent. If Your
 Submission is made in the course of Your work for an employer or Your employer has intellectual
 property rights in Your Submission by contract or applicable law, You must secure permission from Your
 employer to make the Submission before signing this Agreement. In that case, the term “You” in this
 Agreement will refer to You and the employer collectively. If You change employers in the future and
 desire to Submit additional Submissions for the new employer, then You agree to sign a new Agreement
 and secure permission from the new employer before Submitting those Submissions.
 
-
 ## 5. Licenses
 
 a. Copyright License. You grant NVIDIA, and those who receive the Submission directly or
 indirectly from NVIDIA, a perpetual, worldwide, non-exclusive, royalty-free, irrevocable license in the
 Submission to reproduce, prepare derivative works of, publicly display, publicly perform, and distribute
 the Submission and such derivative works, and to sublicense any or all of the foregoing rights to third
 parties.
@@ -63,37 +65,42 @@
 import or otherwise dispose of the Submission alone or with the Project.
 
 c. Other Rights Reserved. Each party reserves all rights not expressly granted in this Agreement.
 No additional licenses or rights whatsoever (including, without limitation, any implied licenses) are
 granted by implication, exhaustion, estoppel or otherwise.
 
 ## 6. Representations and Warranties
+
 You represent that You are legally entitled to grant the above
 licenses. You represent that each of Your Submissions is entirely Your original work (except as You may
 have disclosed under Section 3). You represent that You have secured permission from Your employer to
 make the Submission in cases where Your Submission is made in the course of Your work for Your
 employer or Your employer has intellectual property rights in Your Submission by contract or applicable
 law. If You are signing this Agreement on behalf of Your employer, You represent and warrant that You
 have the necessary authority to bind the listed employer to the obligations contained in this Agreement.
 You are not expected to provide support for Your Submission, unless You choose to do so. UNLESS
 REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING, AND EXCEPT FOR THE WARRANTIES
 EXPRESSLY STATED IN SECTIONS 3, 4, AND 6, THE SUBMISSION PROVIDED UNDER THIS AGREEMENT IS
 PROVIDED WITHOUT WARRANTY OF ANY KIND, INCLUDING, BUT NOT LIMITED TO, ANY WARRANTY OF
 NONINFRINGEMENT, MERCHANTABILITY, OR FITNESS FOR A PARTICULAR PURPOSE.
 
 ## 7. Notice to NVIDIA
+
 You agree to notify NVIDIA in writing of any facts or circumstances of which
 You later become aware that would make Your representations in this Agreement inaccurate in any
 respect.
 
 ## 8. Information about Submissions
+
 You agree that contributions to Projects and information about
 contributions may be maintained indefinitely and disclosed publicly, including Your name and other
 information that You submit with Your Submission.
 
-## 9. Governing Law/Jurisdiction. 
+## 9. Governing Law/Jurisdiction.
+
 Claims arising under this Agreement shall be governed by the laws of Delaware, excluding its principles of conflict of laws and the United Nations Convention on Contracts for the Sale of Goods. The state and/or federal courts residing in Santa Clara County, California shall have exclusive jurisdiction over any dispute or claim arising out of this Agreement. You may not export the Software in violation of applicable export laws and regulations.
 
 ## 10. Entire Agreement/Assignment
+
 This Agreement is the entire agreement between the parties, and
 supersedes any and all prior agreements, understandings or communications, written or oral, between
-the parties relating to the subject matter hereof. This Agreement may be assigned by NVIDIA.
+the parties relating to the subject matter hereof. This Agreement may be assigned by NVIDIA.
```

### Comparing `merlin-models-23.5.0/CONTRIBUTING.md` & `merlin-models-23.6.0/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
    - If you need more context on a particular issue, please ask and the
      NVIDIA-Merlin team will provide the context.
 
 ## Code contributions
 
 ### Your first issue
 
-1. Read the project's [README.md](https://github.com/NVIDIA-Merlin/models/blob/main/README.md)
+1. Read the project's [README.md](https://github.com/NVIDIA-Merlin/models/blob/stable/README.md)
    to learn how to setup the development environment.
 2. Find an issue to work on. The best way is to look for the [good first issue](https://github.com/NVIDIA-Merlin/models/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22)
    or [help wanted](https://github.com/NVIDIA-Merlin/models/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) labels.
 3. Comment on the issue to say that you are going to work on it.
 4. Code! Make sure to update unit tests!
 5. When done, [create your pull request](https://github.com/NVIDIA-Merlin/models/compare).
 6. Verify that CI passes all [status checks](https://help.github.com/articles/about-status-checks/). Fix if needed.
@@ -61,15 +61,15 @@
 - `bug` -- The PR fixes a problem with the code.
 - `feature` or `enhancement` -- The PR introduces a backward-compatible feature.
 - `documentation` or `examples` -- The PR is an addition or update to documentation.
 - `build`, `dependencies`, `chore`, or `ci` -- The PR is related to maintaining the
   repository or the project.
 
 By default, an unlabeled PR is listed at the top of the change log and is not
-grouped under a heading like *Features* that groups similar PRs.
+grouped under a heading like _Features_ that groups similar PRs.
 Labeling the PRs so we can categorize them is preferred.
 
 If, for some reason, you do not believe your PR should be included in the change
 log, you can add the `skip-changelog` label.
 This label excludes the PR from the change log.
 
 For more information, see `.github/release-drafter.yml` in the repository
@@ -112,13 +112,13 @@
 schema : ~merlin.schema.Schema
     The `Schema` with the input features
 deep_block: Block
     Block (structure) of deep model.
 ```
 
 The [Intersphinx](https://docs.readthedocs.io/en/stable/guides/intersphinx.html)
-extension truncates the text to [Schema](https://nvidia-merlin.github.io/core/main/api/merlin.schema.html)
+extension truncates the text to [Schema](https://nvidia-merlin.github.io/core/stable/api/merlin.schema.html)
 and makes it a link.
 
 ## Attribution
 
 Portions adopted from https://github.com/pytorch/pytorch/blob/master/CONTRIBUTING.md
```

### Comparing `merlin-models-23.5.0/LICENSE` & `merlin-models-23.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/MANIFEST.in` & `merlin-models-23.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/Makefile` & `merlin-models-23.6.0/Makefile`

 * *Files 26% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 	mypy transformers4rec --install-types --non-interactive --no-strict-optional --ignore-missing-imports
 
 tests:
 	coverage run -m pytest -rsx || exit 1
 	coverage report --include 'merlin/models/*'
 	coverage html --include 'merlin/models/*'
 
+tests-changed:
+	coverage run -m pytest -rsx -m "changed" || exit 1
+	coverage report --include 'merlin/models/*'
+	coverage html --include 'merlin/models/*'
+
 tests-tf:
 	coverage run -m pytest --durations=100 --dist=loadfile --numprocesses=auto -rsx tests -m "tensorflow and not (integration or example)" || exit 1
 	coverage report --include 'merlin/models/*'
 	coverage html --include 'merlin/models/*'
 
 tests-tf-examples:
 	coverage run -m pytest -rsx tests -m "tensorflow and example" || exit 1
@@ -27,39 +32,80 @@
 	coverage html --include 'merlin/models/*'
 
 tests-tf-integration:
 	coverage run -m pytest -rsx tests -m "tensorflow and integration" || exit 1
 	coverage report --include 'merlin/models/*'
 	coverage html --include 'merlin/models/*'
 
+tests-tf-changed:
+	coverage run -m pytest --durations=100 --dist=loadfile --numprocesses=auto -rsx tests -m "tensorflow and changed and not (integration or example) or always" || exit 1
+	coverage report --include 'merlin/models/*'
+	coverage html --include 'merlin/models/*'
+
+tests-tf-examples-changed:
+	coverage run -m pytest -rsx tests -m "tensorflow and changed and example" || exit 1
+	coverage report --include 'merlin/models/*'
+	coverage html --include 'merlin/models/*'
+
+tests-tf-integration-changed:
+	coverage run -m pytest -rsx tests -m "tensorflow and changed and integration" || exit 1
+	coverage report --include 'merlin/models/*'
+	coverage html --include 'merlin/models/*'
+
+
 tests-torch:
 	coverage run -m pytest -rsx tests -m "torch" || exit 1
 	coverage report --include 'merlin/models/torch/*'
 	coverage html --include 'merlin/models/torch/*'
 
+tests-torch-changed:
+	coverage run -m pytest -rsx tests -m "torch and changed" || exit 1
+	coverage report --include 'merlin/models/torch/*'
+	coverage html --include 'merlin/models/torch/*'
+
 tests-implicit:
 	coverage run -m pytest -rsx tests -m "implicit" || exit 1
 	coverage report --include 'merlin/models/*'
 	coverage html --include 'merlin/models/*'
 
+tests-implicit-changed:
+	coverage run -m pytest -rsx tests -m "implicit and changed" || exit 1
+	coverage report --include 'merlin/models/*'
+	coverage html --include 'merlin/models/*'
+
 tests-lightfm:
 	coverage run -m pytest -rsx tests -m "lightfm" || exit 1
 	coverage report --include 'merlin/models/*'
 	coverage html --include 'merlin/models/*'
 
+tests-lightfm-changed:
+	coverage run -m pytest -rsx tests -m "lightfm and changed" || exit 1
+	coverage report --include 'merlin/models/*'
+	coverage html --include 'merlin/models/*'
+
 tests-xgboost:
 	coverage run -m pytest -rsx tests -m "xgboost" || exit 1
 	coverage report --include 'merlin/models/*'
 	coverage html --include 'merlin/models/*'
 
+tests-xgboost-changed:
+	coverage run -m pytest -rsx tests -m "xgboost and changed" || exit 1
+	coverage report --include 'merlin/models/*'
+	coverage html --include 'merlin/models/*'
+
 tests-datasets:
 	coverage run -m pytest -rsx tests -m "datasets" || exit 1
 	coverage report --include 'merlin/models/*'
 	coverage html --include 'merlin/models/*'
 
+tests-datasets-changed:
+	coverage run -m pytest -rsx tests -m "datasets and changed" || exit 1
+	coverage report --include 'merlin/models/*'
+	coverage html --include 'merlin/models/*'
+
 jenkins-tf:
 	coverage run -m pytest -rsx tests -m "tensorflow and not integration" || exit 1
 	coverage report --include 'merlin/models/*'
 	coverage html --include 'merlin/models/*'
 
 dist:
 	python setup.py sdist
```

### Comparing `merlin-models-23.5.0/PKG-INFO` & `merlin-models-23.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-models
-Version: 23.5.0
+Version: 23.6.0
 Summary: Merlin recommender system models
 Home-page: https://github.com/NVIDIA-Merlin/models
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -33,53 +33,53 @@
 Provides-Extra: all
 License-File: LICENSE
 
 ## Merlin Models
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
 ![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/models)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/main/)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/)
 
 The Merlin Models library provides standard models for recommender systems with an aim for high-quality implementations
 that range from classic machine learning models to highly-advanced deep learning models.
 
 The goal of this library is to make it easy for users in the industry to train and deploy recommender models with the best
 practices that are already baked into the library. The library simplifies how users in the industry can train standard models against their dataset and put high-performance, GPU-accelerated models into production. The library also enables researchers to build custom
 models by incorporating standard components of deep learning recommender models and then researchers can benchmark the new models on
 example offline
 datasets.
 
 In our initial releases, Merlin Models features a TensorFlow API. The PyTorch API is initiated, but incomplete. We have PyTorch support for transformer-based, session-based recommender systems in the [Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/) library.
 
 ### Benefits of Merlin Models
 
-**[RecSys model implementations](https://nvidia-merlin.github.io/models/main/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
+**[RecSys model implementations](https://nvidia-merlin.github.io/models/stable/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
 These models include both retrieval (e.g. Matrix Factorization, Two tower, YouTube DNN, ..) and ranking (e.g. DLRM, DCN-v2, DeepFM, ...) models.
 
 **Building blocks** - Within Merlin Models, recommender models are built on reusable building blocks.
 The design makes it easy to combine the blocks to define new architectures.
 The library provides model definition blocks (MLP layers, factorization layers, input blocks, negative samplers, loss functions), training models (data loaders from Parquet files), and evaluation (e.g. ranking metrics).
 
 **Integration with Merlin platform** - Merlin Models is deeply integrated with the other Merlin components.
 For example, models depend on NVTabular for pre-processing and integrate easily with Merlin Systems for inference.
 The thoughtfully-designed integration makes it straightforward to build performant end-to-end RecSys pipelines.
 
-**[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/main/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
+**[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/stable/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
 When training deep learning recommender system models, data loading can be a bottleneck.
 To address the challenge, Merlin has custom, highly-optimized dataloaders to accelerate existing TensorFlow and PyTorch training pipelines.
 The Merlin dataloaders can lead to a speedup that is nine times faster than the same training pipeline used with the GPU.
 
 With the Merlin dataloaders, you can:
 
 - Remove bottlenecks from data loading by processing large chunks of data at a time instead of item by item.
 - Process datasets that don't fit within the GPU or CPU memory by streaming from the disk.
 - Prepare batches asynchronously into the GPU to avoid CPU-to-GPU communication.
 - Integrate easily into existing TensorFlow or PyTorch training pipelines by using a similar API.
 
-To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/main/models_overview.html) page.
+To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/stable/models_overview.html) page.
 
 ### Installation
 
 #### Installing Merlin Models Using Pip
 
 Merlin Models can be installed with `pip` by running the following command:
 
@@ -90,15 +90,15 @@
 > Installing Merlin Models with `pip` does not install some additional GPU dependencies, such as the CUDA Toolkit.
 > When you run Merlin Models in one of our Docker containers, the dependencies are already installed.
 
 #### Docker Containers that include Merlin Models
 
 Merlin Models is included in the Merlin Containers.
 
-Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
+Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/stable/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
 
 #### Installing Merlin Models from Source
 
 Merlin Models can be installed from source by running the following commands:
 
 ```shell
 git clone https://github.com/NVIDIA-Merlin/models
@@ -106,15 +106,15 @@
 ```
 
 ### Getting Started
 
 Merlin Models makes it straightforward to define architectures that adapt to different input features.
 This adaptability is provided by building on a core feature of the NVTabular library.
 When you use NVTabular for feature engineering, NVTabular creates a schema that identifies the input features.
-You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/main/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
+You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/stable/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
 
 You can easily build popular RecSys architectures like [DLRM](http://arxiv.org/abs/1906.00091), as shown in the following code sample.
 After you define the model, you can train and evaluate it with a typical Keras model.
 
 ```python
 import merlin.models.tf as mm
 from merlin.io.dataset import Dataset
@@ -138,19 +138,19 @@
 1.  To build the internal input layer, the model identifies them from the schema object.
     The schema identifies the continuous features and categorical features, for which embedding tables are created.
 2.  To define the body of the architecture, MLP layers are used with configurable dimensions.
 3.  The head of the architecture is created from the chosen task, `BinaryClassificationTask` in this example.
     The target binary feature is also inferred from the schema (i.e., tagged as 'TARGET').
 
 You can find more details and information about a low-level API in our overview of the
-[Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
+[Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/stable/models_overview.html#deep-learning-recommender-model).
 
 ### Notebook Examples and Tutorials
 
-View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
+View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/stable/examples/README.html) to help you become familiar with Merlin Models.
 
 The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
 
 ### Feedback and Support
 
 If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
```

### Comparing `merlin-models-23.5.0/README.md` & `merlin-models-23.6.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 ## Merlin Models
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
 ![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/models)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/main/)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/)
 
 The Merlin Models library provides standard models for recommender systems with an aim for high-quality implementations
 that range from classic machine learning models to highly-advanced deep learning models.
 
 The goal of this library is to make it easy for users in the industry to train and deploy recommender models with the best
 practices that are already baked into the library. The library simplifies how users in the industry can train standard models against their dataset and put high-performance, GPU-accelerated models into production. The library also enables researchers to build custom
 models by incorporating standard components of deep learning recommender models and then researchers can benchmark the new models on
 example offline
 datasets.
 
 In our initial releases, Merlin Models features a TensorFlow API. The PyTorch API is initiated, but incomplete. We have PyTorch support for transformer-based, session-based recommender systems in the [Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/) library.
 
 ### Benefits of Merlin Models
 
-**[RecSys model implementations](https://nvidia-merlin.github.io/models/main/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
+**[RecSys model implementations](https://nvidia-merlin.github.io/models/stable/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
 These models include both retrieval (e.g. Matrix Factorization, Two tower, YouTube DNN, ..) and ranking (e.g. DLRM, DCN-v2, DeepFM, ...) models.
 
 **Building blocks** - Within Merlin Models, recommender models are built on reusable building blocks.
 The design makes it easy to combine the blocks to define new architectures.
 The library provides model definition blocks (MLP layers, factorization layers, input blocks, negative samplers, loss functions), training models (data loaders from Parquet files), and evaluation (e.g. ranking metrics).
 
 **Integration with Merlin platform** - Merlin Models is deeply integrated with the other Merlin components.
 For example, models depend on NVTabular for pre-processing and integrate easily with Merlin Systems for inference.
 The thoughtfully-designed integration makes it straightforward to build performant end-to-end RecSys pipelines.
 
-**[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/main/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
+**[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/stable/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
 When training deep learning recommender system models, data loading can be a bottleneck.
 To address the challenge, Merlin has custom, highly-optimized dataloaders to accelerate existing TensorFlow and PyTorch training pipelines.
 The Merlin dataloaders can lead to a speedup that is nine times faster than the same training pipeline used with the GPU.
 
 With the Merlin dataloaders, you can:
 
 - Remove bottlenecks from data loading by processing large chunks of data at a time instead of item by item.
 - Process datasets that don't fit within the GPU or CPU memory by streaming from the disk.
 - Prepare batches asynchronously into the GPU to avoid CPU-to-GPU communication.
 - Integrate easily into existing TensorFlow or PyTorch training pipelines by using a similar API.
 
-To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/main/models_overview.html) page.
+To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/stable/models_overview.html) page.
 
 ### Installation
 
 #### Installing Merlin Models Using Pip
 
 Merlin Models can be installed with `pip` by running the following command:
 
@@ -55,15 +55,15 @@
 > Installing Merlin Models with `pip` does not install some additional GPU dependencies, such as the CUDA Toolkit.
 > When you run Merlin Models in one of our Docker containers, the dependencies are already installed.
 
 #### Docker Containers that include Merlin Models
 
 Merlin Models is included in the Merlin Containers.
 
-Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
+Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/stable/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
 
 #### Installing Merlin Models from Source
 
 Merlin Models can be installed from source by running the following commands:
 
 ```shell
 git clone https://github.com/NVIDIA-Merlin/models
@@ -71,15 +71,15 @@
 ```
 
 ### Getting Started
 
 Merlin Models makes it straightforward to define architectures that adapt to different input features.
 This adaptability is provided by building on a core feature of the NVTabular library.
 When you use NVTabular for feature engineering, NVTabular creates a schema that identifies the input features.
-You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/main/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
+You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/stable/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
 
 You can easily build popular RecSys architectures like [DLRM](http://arxiv.org/abs/1906.00091), as shown in the following code sample.
 After you define the model, you can train and evaluate it with a typical Keras model.
 
 ```python
 import merlin.models.tf as mm
 from merlin.io.dataset import Dataset
@@ -103,19 +103,19 @@
 1.  To build the internal input layer, the model identifies them from the schema object.
     The schema identifies the continuous features and categorical features, for which embedding tables are created.
 2.  To define the body of the architecture, MLP layers are used with configurable dimensions.
 3.  The head of the architecture is created from the chosen task, `BinaryClassificationTask` in this example.
     The target binary feature is also inferred from the schema (i.e., tagged as 'TARGET').
 
 You can find more details and information about a low-level API in our overview of the
-[Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
+[Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/stable/models_overview.html#deep-learning-recommender-model).
 
 ### Notebook Examples and Tutorials
 
-View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
+View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/stable/examples/README.html) to help you become familiar with Merlin Models.
 
 The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
 
 ### Feedback and Support
 
 If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
```

### Comparing `merlin-models-23.5.0/conda/recipes/meta.yaml` & `merlin-models-23.6.0/conda/recipes/meta.yaml`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/__init__.py` & `merlin-models-23.6.0/merlin/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/advertising/__init__.py` & `merlin-models-23.6.0/merlin/datasets/advertising/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/advertising/criteo/__init__.py` & `merlin-models-23.6.0/merlin/datasets/advertising/criteo/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/advertising/criteo/dataset.py` & `merlin-models-23.6.0/merlin/datasets/advertising/criteo/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/__init__.py` & `merlin-models-23.6.0/merlin/datasets/advertising/criteo/transformed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/advertising/criteo/transformed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,22 +13,22 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from merlin.datasets.ecommerce.aliccp.dataset import (
     default_aliccp_transformation,
     get_aliccp,
-    prepare_alliccp,
+    prepare_aliccp,
     transform_aliccp,
 )
 from merlin.datasets.ecommerce.booking.dataset import get_booking, transform_booking
 from merlin.datasets.ecommerce.dressipi.dataset import get_dressipi2022
 
 __all__ = [
-    "prepare_alliccp",
+    "prepare_aliccp",
     "transform_aliccp",
     "get_aliccp",
     "default_aliccp_transformation",
     "get_dressipi2022",
     "get_booking",
     "transform_booking",
 ]
```

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/dataset.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,821 +107,819 @@
 000006a0: 6869 2e61 6c69 7975 6e2e 636f 6d2f 6461  hi.aliyun.com/da
 000006b0: 7461 7365 742f 6461 7461 4465 7461 696c  taset/dataDetail
 000006c0: 3f64 6174 6149 643d 3430 3823 3129 2e0a  ?dataId=408#1)..
 000006d0: 2020 2020 322e 2055 6e7a 6970 2074 6865      2. Unzip the
 000006e0: 2072 6177 2064 6174 6120 746f 2061 2064   raw data to a d
 000006f0: 6972 6563 746f 7279 2e0a 2020 2020 332e  irectory..    3.
 00000700: 2052 756e 2060 7072 6570 6172 655f 616c   Run `prepare_al
-00000710: 6c69 6363 7028 6461 7461 5f64 6972 2960  liccp(data_dir)`
-00000720: 2074 6f20 636f 6e76 6572 7420 7468 6520   to convert the 
-00000730: 7261 7720 6461 7461 2074 6f20 7061 7271  raw data to parq
-00000740: 7565 7420 6669 6c65 732e 0a0a 2020 2020  uet files...    
-00000750: 446f 776e 6c6f 6164 696e 6720 2620 7072  Downloading & pr
-00000760: 6570 6172 696e 6720 7468 6520 6461 7461  eparing the data
-00000770: 2063 616e 2074 616b 6520 7175 6974 6520   can take quite 
-00000780: 6120 7768 696c 652e 0a20 2020 2049 6e20  a while..    In 
-00000790: 6361 7365 2079 6f75 2077 616e 7420 746f  case you want to
-000007a0: 2075 7365 2074 6869 7320 6461 7461 7365   use this datase
-000007b0: 7420 746f 2072 756e 206f 7572 2074 7574  t to run our tut
-000007c0: 6f72 6961 6c73 2c20 796f 7520 6361 6e20  orials, you can 
-000007d0: 616c 736f 206f 7074 2066 6f72 2073 796e  also opt for syn
-000007e0: 7468 6574 6963 2064 6174 612e 0a20 2020  thetic data..   
-000007f0: 2053 796e 7468 6574 6963 2064 6174 6120   Synthetic data 
-00000800: 6361 6e20 6265 2067 656e 6572 6174 6564  can be generated
-00000810: 2062 7920 7275 6e6e 696e 673a 3a0a 2020   by running::.  
-00000820: 2020 2020 2020 6672 6f6d 206d 6572 6c69        from merli
-00000830: 6e2e 6d6f 6465 6c73 2e64 6174 612e 7379  n.models.data.sy
-00000840: 6e74 6865 7469 6320 696d 706f 7274 2067  nthetic import g
-00000850: 656e 6572 6174 655f 6461 7461 0a0a 2020  enerate_data..  
-00000860: 2020 2020 2020 6461 7461 203d 2067 656e        data = gen
-00000870: 6572 6174 655f 6461 7461 2822 616c 6963  erate_data("alic
-00000880: 6370 2229 0a0a 2020 2020 4e6f 7465 2c20  cp")..    Note, 
-00000890: 7275 6e6e 696e 6720 7468 6973 2066 756e  running this fun
-000008a0: 6374 696f 6e20 7265 7175 6972 6573 2074  ction requires t
-000008b0: 6865 0a20 2020 205b 6e76 7461 6275 6c61  he.    [nvtabula
-000008c0: 725d 2868 7474 7073 3a2f 2f67 6974 6875  r](https://githu
-000008d0: 622e 636f 6d2f 4e56 4944 4941 2d4d 6572  b.com/NVIDIA-Mer
-000008e0: 6c69 6e2f 4e56 5461 6275 6c61 7229 206c  lin/NVTabular) l
-000008f0: 6962 7261 7279 2e0a 0a20 2020 2050 6172  ibrary...    Par
-00000900: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00000910: 2d2d 2d2d 2d2d 0a20 2020 2070 6174 683a  ------.    path:
-00000920: 2055 6e69 6f6e 5b73 7472 2c20 5061 7468   Union[str, Path
-00000930: 5d0a 2020 2020 2020 2020 4469 7265 6374  ].        Direct
-00000940: 6f72 7920 746f 206c 6f61 6420 7468 6520  ory to load the 
-00000950: 7261 7720 6461 7461 2066 726f 6d2e 0a20  raw data from.. 
-00000960: 2020 206f 7665 7277 7269 7465 3a20 626f     overwrite: bo
-00000970: 6f6c 0a20 2020 2020 2020 2057 6865 7468  ol.        Wheth
-00000980: 6572 2074 6f20 6f76 6572 7772 6974 6520  er to overwrite 
-00000990: 7468 6520 7472 616e 7366 6f72 6d65 6420  the transformed 
-000009a0: 6461 7461 2e0a 2020 2020 7472 616e 7366  data..    transf
-000009b0: 6f72 6d65 645f 6e61 6d65 3a20 7374 720a  ormed_name: str.
-000009c0: 2020 2020 2020 2020 4e61 6d65 206f 6620          Name of 
-000009d0: 7468 6520 7472 616e 7366 6f72 6d65 6420  the transformed 
-000009e0: 6461 7461 2e0a 2020 2020 2020 2020 5468  data..        Th
-000009f0: 6973 2069 7320 7573 6566 756c 2077 6865  is is useful whe
-00000a00: 6e20 796f 7520 7761 6e74 2074 6f20 6c6f  n you want to lo
-00000a10: 6164 2074 6865 2074 7261 6e73 666f 726d  ad the transform
-00000a20: 6564 2064 6174 610a 2020 2020 2020 2020  ed data.        
-00000a30: 6d75 6c74 6970 6c65 2074 696d 6573 2075  multiple times u
-00000a40: 7369 6e67 2064 6966 6665 7265 6e74 2077  sing different w
-00000a50: 6f72 6b66 6c6f 7773 2e0a 2020 2020 6e76  orkflows..    nv
-00000a60: 745f 776f 726b 666c 6f77 3a20 4f70 7469  t_workflow: Opti
-00000a70: 6f6e 616c 5b57 6f72 6b66 6c6f 775d 0a20  onal[Workflow]. 
-00000a80: 2020 2020 2020 2057 6f72 6b66 6c6f 7720         Workflow 
-00000a90: 746f 2074 7261 6e73 666f 726d 2074 6865  to transform the
-00000aa0: 2072 6177 2064 6174 612e 0a20 2020 2020   raw data..     
-00000ab0: 2020 2049 6620 4e6f 6e65 2c20 7468 6520     If None, the 
-00000ac0: 6465 6661 756c 7420 776f 726b 666c 6f77  default workflow
-00000ad0: 2077 696c 6c20 6265 2075 7365 6420 6672   will be used fr
-00000ae0: 6f6d 2060 6465 6661 756c 745f 616c 6963  om `default_alic
-00000af0: 6370 5f74 7261 6e73 666f 726d 6174 696f  cp_transformatio
-00000b00: 6e60 2e0a 2020 2020 6669 6c65 5f73 697a  n`..    file_siz
-00000b10: 653a 2069 6e74 0a20 2020 2020 2020 2053  e: int.        S
-00000b20: 697a 6520 6f66 2074 6865 2070 6172 7175  ize of the parqu
-00000b30: 6574 2066 696c 6573 2074 6f20 6265 206c  et files to be l
-00000b40: 6f61 6465 6420 7768 656e 2070 7265 7061  oaded when prepa
-00000b50: 7269 6e67 2074 6865 2064 6174 612e 0a0a  ring the data...
-00000b60: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00000b70: 2d2d 2d2d 2d2d 2d0a 2020 2020 7472 6169  -------.    trai
-00000b80: 6e3a 206d 6572 6c69 6e2e 696f 2e44 6174  n: merlin.io.Dat
-00000b90: 6173 6574 0a20 2020 2020 2020 2054 7261  aset.        Tra
-00000ba0: 696e 696e 6720 6461 7461 7365 742e 0a20  ining dataset.. 
-00000bb0: 2020 2076 616c 6964 3a20 6d65 726c 696e     valid: merlin
-00000bc0: 2e69 6f2e 4461 7461 7365 740a 2020 2020  .io.Dataset.    
-00000bd0: 2020 2020 5465 7374 2064 6174 6173 6574      Test dataset
-00000be0: 2e0a 2020 2020 2222 220a 0a20 2020 2072  ..    """..    r
-00000bf0: 6571 7569 7265 5f6e 7674 2829 0a0a 2020  equire_nvt()..  
-00000c00: 2020 7020 3d20 5061 7468 2870 6174 6829    p = Path(path)
-00000c10: 0a20 2020 2072 6177 5f70 6174 6820 3d20  .    raw_path = 
-00000c20: 7020 2f20 2272 6177 220a 2020 2020 6966  p / "raw".    if
-00000c30: 206e 6f74 2072 6177 5f70 6174 682e 6578   not raw_path.ex
-00000c40: 6973 7473 2829 3a0a 2020 2020 2020 2020  ists():.        
-00000c50: 7261 775f 7061 7468 2e6d 6b64 6972 2870  raw_path.mkdir(p
-00000c60: 6172 656e 7473 3d54 7275 6529 0a20 2020  arents=True).   
-00000c70: 2020 2020 2070 7265 7061 7265 5f61 6c6c       prepare_all
-00000c80: 6963 6370 2870 6174 682c 206f 7574 7075  iccp(path, outpu
-00000c90: 745f 6469 723d 7261 775f 7061 7468 2c20  t_dir=raw_path, 
-00000ca0: 6669 6c65 5f73 697a 653d 6669 6c65 5f73  file_size=file_s
-00000cb0: 697a 652c 202a 2a6b 7761 7267 7329 0a0a  ize, **kwargs)..
-00000cc0: 2020 2020 6e76 745f 7061 7468 203d 2070      nvt_path = p
-00000cd0: 202f 2074 7261 6e73 666f 726d 6564 5f6e   / transformed_n
-00000ce0: 616d 650a 2020 2020 7472 6169 6e5f 7061  ame.    train_pa
-00000cf0: 7468 2c20 7661 6c69 645f 7061 7468 203d  th, valid_path =
-00000d00: 206e 7674 5f70 6174 6820 2f20 2274 7261   nvt_path / "tra
-00000d10: 696e 222c 206e 7674 5f70 6174 6820 2f20  in", nvt_path / 
-00000d20: 2276 616c 6964 220a 2020 2020 6e76 745f  "valid".    nvt_
-00000d30: 7061 7468 5f65 7869 7374 7320 3d20 7472  path_exists = tr
-00000d40: 6169 6e5f 7061 7468 2e65 7869 7374 7328  ain_path.exists(
-00000d50: 2920 616e 6420 7661 6c69 645f 7061 7468  ) and valid_path
-00000d60: 2e65 7869 7374 7328 290a 2020 2020 6966  .exists().    if
-00000d70: 206e 6f74 206e 7674 5f70 6174 685f 6578   not nvt_path_ex
-00000d80: 6973 7473 206f 7220 6f76 6572 7772 6974  ists or overwrit
-00000d90: 653a 0a20 2020 2020 2020 2074 7261 6e73  e:.        trans
-00000da0: 666f 726d 5f61 6c69 6363 7028 7261 775f  form_aliccp(raw_
-00000db0: 7061 7468 2c20 6e76 745f 7061 7468 2c20  path, nvt_path, 
-00000dc0: 6e76 745f 776f 726b 666c 6f77 3d6e 7674  nvt_workflow=nvt
-00000dd0: 5f77 6f72 6b66 6c6f 7729 0a0a 2020 2020  _workflow)..    
-00000de0: 7472 6169 6e20 3d20 6d65 726c 696e 2e69  train = merlin.i
-00000df0: 6f2e 4461 7461 7365 7428 7374 7228 7472  o.Dataset(str(tr
-00000e00: 6169 6e5f 7061 7468 292c 2065 6e67 696e  ain_path), engin
-00000e10: 653d 2270 6172 7175 6574 2229 0a20 2020  e="parquet").   
-00000e20: 2076 616c 6964 203d 206d 6572 6c69 6e2e   valid = merlin.
-00000e30: 696f 2e44 6174 6173 6574 2873 7472 2876  io.Dataset(str(v
-00000e40: 616c 6964 5f70 6174 6829 2c20 656e 6769  alid_path), engi
-00000e50: 6e65 3d22 7061 7271 7565 7422 290a 0a20  ne="parquet").. 
-00000e60: 2020 2072 6574 7572 6e20 7472 6169 6e2c     return train,
-00000e70: 2076 616c 6964 0a0a 0a64 6566 2070 7265   valid...def pre
-00000e80: 7061 7265 5f61 6c6c 6963 6370 280a 2020  pare_alliccp(.  
-00000e90: 2020 6461 7461 5f64 6972 3a20 556e 696f    data_dir: Unio
-00000ea0: 6e5b 7374 722c 2050 6174 685d 2c0a 2020  n[str, Path],.  
-00000eb0: 2020 636f 6e76 6572 745f 7472 6169 6e3a    convert_train:
-00000ec0: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
-00000ed0: 2020 636f 6e76 6572 745f 7465 7374 3a20    convert_test: 
-00000ee0: 626f 6f6c 203d 2054 7275 652c 0a20 2020  bool = True,.   
-00000ef0: 2066 696c 655f 7369 7a65 3a20 696e 7420   file_size: int 
-00000f00: 3d20 3130 3030 3030 2c0a 2020 2020 6d61  = 100000,.    ma
-00000f10: 785f 6e75 6d5f 726f 7773 3a20 4f70 7469  x_num_rows: Opti
-00000f20: 6f6e 616c 5b69 6e74 5d20 3d20 4e6f 6e65  onal[int] = None
-00000f30: 2c0a 2020 2020 7069 636b 6c65 5f63 6f6d  ,.    pickle_com
-00000f40: 6d6f 6e5f 6665 6174 7572 6573 3d54 7275  mon_features=Tru
-00000f50: 652c 0a20 2020 206f 7574 7075 745f 6469  e,.    output_di
-00000f60: 723a 204f 7074 696f 6e61 6c5b 556e 696f  r: Optional[Unio
-00000f70: 6e5b 7374 722c 2050 6174 685d 5d20 3d20  n[str, Path]] = 
-00000f80: 4e6f 6e65 2c0a 293a 0a20 2020 2022 2222  None,.):.    """
-00000f90: 0a20 2020 2043 6f6e 7665 7274 2041 6c69  .    Convert Ali
-00000fa0: 2d43 5050 2064 6174 6120 746f 2070 6172  -CPP data to par
-00000fb0: 7175 6574 2066 696c 6573 2e0a 0a20 2020  quet files...   
-00000fc0: 2054 6f20 646f 776e 6c6f 6164 2074 6865   To download the
-00000fd0: 2072 6177 2074 6865 2041 6c69 2d43 4350   raw the Ali-CCP
-00000fe0: 2074 7261 696e 696e 6720 616e 6420 7465   training and te
-00000ff0: 7374 2064 6174 6173 6574 7320 7669 7369  st datasets visi
-00001000: 740a 2020 2020 5b74 6961 6e63 6869 2e61  t.    [tianchi.a
-00001010: 6c69 7975 6e2e 636f 6d5d 2868 7474 7073  liyun.com](https
-00001020: 3a2f 2f74 6961 6e63 6869 2e61 6c69 7975  ://tianchi.aliyu
-00001030: 6e2e 636f 6d2f 6461 7461 7365 742f 6461  n.com/dataset/da
-00001040: 7461 4465 7461 696c 3f64 6174 6149 643d  taDetail?dataId=
-00001050: 3430 3823 3129 2e0a 0a20 2020 2050 6172  408#1)...    Par
-00001060: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00001070: 2d2d 2d2d 2d2d 0a20 2020 2064 6174 615f  ------.    data_
-00001080: 6469 723a 2055 6e69 6f6e 5b73 7472 2c20  dir: Union[str, 
-00001090: 5061 7468 5d0a 2020 2020 2020 2020 4469  Path].        Di
-000010a0: 7265 6374 6f72 7920 746f 206c 6f61 6420  rectory to load 
-000010b0: 7468 6520 7261 7720 6461 7461 2066 726f  the raw data fro
-000010c0: 6d2e 0a20 2020 2063 6f6e 7665 7274 5f74  m..    convert_t
-000010d0: 7261 696e 3a20 626f 6f6c 0a20 2020 2020  rain: bool.     
-000010e0: 2020 2057 6865 7468 6572 2074 6f20 636f     Whether to co
-000010f0: 6e76 6572 7420 7468 6520 7472 6169 6e69  nvert the traini
-00001100: 6e67 2064 6174 612e 0a20 2020 2063 6f6e  ng data..    con
-00001110: 7665 7274 5f74 6573 743a 2062 6f6f 6c0a  vert_test: bool.
-00001120: 2020 2020 2020 2020 5768 6574 6865 7220          Whether 
-00001130: 746f 2063 6f6e 7665 7274 2074 6865 2074  to convert the t
-00001140: 6573 7420 6461 7461 2e0a 2020 2020 6669  est data..    fi
-00001150: 6c65 5f73 697a 653a 2069 6e74 0a20 2020  le_size: int.   
-00001160: 2020 2020 204e 756d 6265 7220 6f66 2072       Number of r
-00001170: 6f77 7320 746f 2077 7269 7465 2074 6f20  ows to write to 
-00001180: 6561 6368 2070 6172 7175 6574 2066 696c  each parquet fil
-00001190: 652e 0a20 2020 206d 6178 5f6e 756d 5f72  e..    max_num_r
-000011a0: 6f77 733a 2069 6e74 2c20 6f70 7469 6f6e  ows: int, option
-000011b0: 616c 0a20 2020 2020 2020 204d 6178 696d  al.        Maxim
-000011c0: 756d 206e 756d 6265 7220 6f66 2072 6f77  um number of row
-000011d0: 7320 746f 2072 6561 6420 6672 6f6d 2074  s to read from t
-000011e0: 6865 2072 6177 2064 6174 612e 0a20 2020  he raw data..   
-000011f0: 2070 6963 6b6c 655f 636f 6d6d 6f6e 5f66   pickle_common_f
-00001200: 6561 7475 7265 733a 2062 6f6f 6c0a 2020  eatures: bool.  
-00001210: 2020 2020 2020 5768 6574 6865 7220 746f        Whether to
-00001220: 2070 6963 6b6c 6520 7468 6520 636f 6d6d   pickle the comm
-00001230: 6f6e 2066 6561 7475 7265 732e 0a20 2020  on features..   
-00001240: 2020 2020 2057 6865 6e20 656e 6162 6c65       When enable
-00001250: 6420 6974 2077 696c 6c20 6d61 6b65 2074  d it will make t
-00001260: 6865 2063 6f6e 7665 7273 696f 6e20 6661  he conversion fa
-00001270: 7374 6572 2069 6620 6974 2077 6f75 6c64  ster if it would
-00001280: 2062 6520 7275 6e20 6167 6169 6e2e 0a20   be run again.. 
-00001290: 2020 206f 7574 7075 745f 6469 723a 2055     output_dir: U
-000012a0: 6e69 6f6e 5b73 7472 2c20 5061 7468 5d2c  nion[str, Path],
-000012b0: 206f 7074 696f 6e61 6c0a 2020 2020 2020   optional.      
-000012c0: 2020 4469 7265 6374 6f72 7920 746f 2077    Directory to w
-000012d0: 7269 7465 2074 6865 2063 6f6e 7665 7274  rite the convert
-000012e0: 6564 2064 6174 6120 746f 2e0a 2020 2020  ed data to..    
-000012f0: 2020 2020 4966 206e 6f74 2073 7065 6369      If not speci
-00001300: 6669 6564 2074 6865 2064 6174 6120 7769  fied the data wi
-00001310: 6c6c 2062 6520 7772 6974 7465 6e20 746f  ll be written to
-00001320: 2074 6865 2073 616d 6520 6469 7265 6374   the same direct
-00001330: 6f72 7920 6173 2074 6865 2072 6177 2064  ory as the raw d
-00001340: 6174 612e 0a0a 2020 2020 5265 7475 726e  ata...    Return
-00001350: 730a 2020 2020 2d2d 2d2d 2d2d 2d0a 2020  s.    -------.  
-00001360: 2020 6461 7461 5f64 6972 0a20 2020 2022    data_dir.    "
-00001370: 2222 0a0a 2020 2020 6966 2063 6f6e 7665  ""..    if conve
-00001380: 7274 5f74 7261 696e 3a0a 2020 2020 2020  rt_train:.      
-00001390: 2020 5f63 6f6e 7665 7274 5f64 6174 6128    _convert_data(
-000013a0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-000013b0: 2864 6174 615f 6469 7229 2c0a 2020 2020  (data_dir),.    
-000013c0: 2020 2020 2020 2020 6669 6c65 5f73 697a          file_siz
-000013d0: 652c 0a20 2020 2020 2020 2020 2020 2069  e,.            i
-000013e0: 735f 7472 6169 6e3d 5472 7565 2c0a 2020  s_train=True,.  
-000013f0: 2020 2020 2020 2020 2020 6d61 785f 6e75            max_nu
-00001400: 6d5f 726f 7773 3d6d 6178 5f6e 756d 5f72  m_rows=max_num_r
-00001410: 6f77 732c 0a20 2020 2020 2020 2020 2020  ows,.           
-00001420: 2070 6963 6b6c 655f 636f 6d6d 6f6e 5f66   pickle_common_f
-00001430: 6561 7475 7265 733d 7069 636b 6c65 5f63  eatures=pickle_c
-00001440: 6f6d 6d6f 6e5f 6665 6174 7572 6573 2c0a  ommon_features,.
-00001450: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00001460: 7574 5f64 6972 3d6f 7574 7075 745f 6469  ut_dir=output_di
-00001470: 722c 0a20 2020 2020 2020 2029 0a20 2020  r,.        ).   
-00001480: 2069 6620 636f 6e76 6572 745f 7465 7374   if convert_test
-00001490: 3a0a 2020 2020 2020 2020 5f63 6f6e 7665  :.        _conve
-000014a0: 7274 5f64 6174 6128 0a20 2020 2020 2020  rt_data(.       
-000014b0: 2020 2020 2073 7472 2864 6174 615f 6469       str(data_di
-000014c0: 7229 2c0a 2020 2020 2020 2020 2020 2020  r),.            
-000014d0: 6669 6c65 5f73 697a 652c 0a20 2020 2020  file_size,.     
-000014e0: 2020 2020 2020 2069 735f 7472 6169 6e3d         is_train=
-000014f0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00001500: 2020 206d 6178 5f6e 756d 5f72 6f77 733d     max_num_rows=
-00001510: 6d61 785f 6e75 6d5f 726f 7773 2c0a 2020  max_num_rows,.  
-00001520: 2020 2020 2020 2020 2020 7069 636b 6c65            pickle
-00001530: 5f63 6f6d 6d6f 6e5f 6665 6174 7572 6573  _common_features
-00001540: 3d70 6963 6b6c 655f 636f 6d6d 6f6e 5f66  =pickle_common_f
-00001550: 6561 7475 7265 732c 0a20 2020 2020 2020  eatures,.       
-00001560: 2020 2020 206f 7574 7075 745f 6469 723d       output_dir=
-00001570: 6f75 7470 7574 5f64 6972 2c0a 2020 2020  output_dir,.    
-00001580: 2020 2020 290a 0a20 2020 2072 6574 7572      )..    retur
-00001590: 6e20 6461 7461 5f64 6972 0a0a 0a64 6566  n data_dir...def
-000015a0: 2064 6566 6175 6c74 5f61 6c69 6363 705f   default_aliccp_
-000015b0: 7472 616e 7366 6f72 6d61 7469 6f6e 2861  transformation(a
-000015c0: 6464 5f74 6172 6765 745f 656e 636f 6469  dd_target_encodi
-000015d0: 6e67 3d54 7275 652c 202a 2a6b 7761 7267  ng=True, **kwarg
-000015e0: 7329 3a0a 2020 2020 696d 706f 7274 206e  s):.    import n
-000015f0: 7674 6162 756c 6172 2061 7320 6e76 740a  vtabular as nvt.
-00001600: 2020 2020 6672 6f6d 206e 7674 6162 756c      from nvtabul
-00001610: 6172 2069 6d70 6f72 7420 6f70 7320 6173  ar import ops as
-00001620: 206e 7674 5f6f 7073 0a0a 2020 2020 6361   nvt_ops..    ca
-00001630: 7420 3d20 6c61 6d62 6461 3a20 6e76 745f  t = lambda: nvt_
-00001640: 6f70 732e 4361 7465 676f 7269 6679 2864  ops.Categorify(d
-00001650: 7479 7065 3d22 696e 7433 3222 2920 2023  type="int32")  #
-00001660: 206e 6f71 613a 2045 3733 310a 0a20 2020   noqa: E731..   
-00001670: 2075 7365 725f 6964 203d 205b 2275 7365   user_id = ["use
-00001680: 725f 6964 225d 203e 3e20 6361 7428 2920  r_id"] >> cat() 
-00001690: 3e3e 206e 7674 5f6f 7073 2e54 6167 4173  >> nvt_ops.TagAs
-000016a0: 5573 6572 4944 2829 0a20 2020 2069 7465  UserID().    ite
-000016b0: 6d5f 6964 203d 205b 2269 7465 6d5f 6964  m_id = ["item_id
-000016c0: 225d 203e 3e20 6361 7428 2920 3e3e 206e  "] >> cat() >> n
-000016d0: 7674 5f6f 7073 2e54 6167 4173 4974 656d  vt_ops.TagAsItem
-000016e0: 4944 2829 0a0a 2020 2020 6974 656d 5f66  ID()..    item_f
-000016f0: 6561 7475 7265 7320 3d20 280a 2020 2020  eatures = (.    
-00001700: 2020 2020 5b22 6974 656d 5f63 6174 6567      ["item_categ
-00001710: 6f72 7922 2c20 2269 7465 6d5f 7368 6f70  ory", "item_shop
-00001720: 222c 2022 6974 656d 5f62 7261 6e64 222c  ", "item_brand",
-00001730: 2022 6974 656d 5f69 6e74 656e 7469 6f6e   "item_intention
-00001740: 225d 0a20 2020 2020 2020 203e 3e20 6361  "].        >> ca
-00001750: 7428 290a 2020 2020 2020 2020 3e3e 206e  t().        >> n
-00001760: 7674 5f6f 7073 2e54 6167 4173 4974 656d  vt_ops.TagAsItem
-00001770: 4665 6174 7572 6573 2829 0a20 2020 2029  Features().    )
-00001780: 0a0a 2020 2020 7573 6572 5f66 6561 7475  ..    user_featu
-00001790: 7265 7320 3d20 280a 2020 2020 2020 2020  res = (.        
-000017a0: 5b0a 2020 2020 2020 2020 2020 2020 2275  [.            "u
-000017b0: 7365 725f 7368 6f70 7322 2c0a 2020 2020  ser_shops",.    
-000017c0: 2020 2020 2020 2020 2275 7365 725f 7072          "user_pr
-000017d0: 6f66 696c 6522 2c0a 2020 2020 2020 2020  ofile",.        
-000017e0: 2020 2020 2275 7365 725f 6772 6f75 7022      "user_group"
-000017f0: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
-00001800: 7365 725f 6765 6e64 6572 222c 0a20 2020  ser_gender",.   
-00001810: 2020 2020 2020 2020 2022 7573 6572 5f61           "user_a
-00001820: 6765 222c 0a20 2020 2020 2020 2020 2020  ge",.           
-00001830: 2022 7573 6572 5f63 6f6e 7375 6d70 7469   "user_consumpti
-00001840: 6f6e 5f31 222c 0a20 2020 2020 2020 2020  on_1",.         
-00001850: 2020 2022 7573 6572 5f63 6f6e 7375 6d70     "user_consump
-00001860: 7469 6f6e 5f32 222c 0a20 2020 2020 2020  tion_2",.       
-00001870: 2020 2020 2022 7573 6572 5f69 735f 6f63       "user_is_oc
-00001880: 6375 7069 6564 222c 0a20 2020 2020 2020  cupied",.       
-00001890: 2020 2020 2022 7573 6572 5f67 656f 6772       "user_geogr
-000018a0: 6170 6879 222c 0a20 2020 2020 2020 2020  aphy",.         
-000018b0: 2020 2022 7573 6572 5f69 6e74 656e 7469     "user_intenti
-000018c0: 6f6e 7322 2c0a 2020 2020 2020 2020 2020  ons",.          
-000018d0: 2020 2275 7365 725f 6272 616e 6473 222c    "user_brands",
-000018e0: 0a20 2020 2020 2020 2020 2020 2022 7573  .            "us
-000018f0: 6572 5f63 6174 6567 6f72 6965 7322 2c0a  er_categories",.
-00001900: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
-00001910: 2020 3e3e 2063 6174 2829 0a20 2020 2020    >> cat().     
-00001920: 2020 203e 3e20 6e76 745f 6f70 732e 5461     >> nvt_ops.Ta
-00001930: 6741 7355 7365 7246 6561 7475 7265 7328  gAsUserFeatures(
-00001940: 290a 2020 2020 290a 0a20 2020 2075 7365  ).    )..    use
-00001950: 725f 6974 656d 5f66 6561 7475 7265 7320  r_item_features 
-00001960: 3d20 280a 2020 2020 2020 2020 5b0a 2020  = (.        [.  
-00001970: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
-00001980: 6974 656d 5f63 6174 6567 6f72 6965 7322  item_categories"
-00001990: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
-000019a0: 7365 725f 6974 656d 5f73 686f 7073 222c  ser_item_shops",
-000019b0: 0a20 2020 2020 2020 2020 2020 2022 7573  .            "us
-000019c0: 6572 5f69 7465 6d5f 6272 616e 6473 222c  er_item_brands",
-000019d0: 0a20 2020 2020 2020 2020 2020 2022 7573  .            "us
-000019e0: 6572 5f69 7465 6d5f 696e 7465 6e74 696f  er_item_intentio
-000019f0: 6e73 222c 0a20 2020 2020 2020 205d 0a20  ns",.        ]. 
-00001a00: 2020 2020 2020 203e 3e20 6361 7428 290a         >> cat().
-00001a10: 2020 2020 2020 2020 3e3e 206e 7674 5f6f          >> nvt_o
-00001a20: 7073 2e41 6464 4d65 7461 6461 7461 2874  ps.AddMetadata(t
-00001a30: 6167 733d 5b22 7573 6572 5f69 7465 6d22  ags=["user_item"
-00001a40: 5d29 0a20 2020 2029 0a0a 2020 2020 636f  ]).    )..    co
-00001a50: 6e74 6578 745f 6665 6174 7572 6573 203d  ntext_features =
-00001a60: 205b 2270 6f73 6974 696f 6e22 5d20 3e3e   ["position"] >>
-00001a70: 2063 6174 2829 203e 3e20 6e76 745f 6f70   cat() >> nvt_op
-00001a80: 732e 4164 644d 6574 6164 6174 6128 7461  s.AddMetadata(ta
-00001a90: 6773 3d5b 5461 6773 2e43 4f4e 5445 5854  gs=[Tags.CONTEXT
-00001aa0: 5d29 0a0a 2020 2020 7461 7267 6574 7320  ])..    targets 
-00001ab0: 3d20 5b22 636c 6963 6b22 2c20 2263 6f6e  = ["click", "con
-00001ac0: 7665 7273 696f 6e22 5d20 3e3e 206e 7674  version"] >> nvt
-00001ad0: 5f6f 7073 2e41 6464 4d65 7461 6461 7461  _ops.AddMetadata
-00001ae0: 280a 2020 2020 2020 2020 7461 6773 3d5b  (.        tags=[
-00001af0: 5461 6773 2e42 494e 4152 595f 434c 4153  Tags.BINARY_CLAS
-00001b00: 5349 4649 4341 5449 4f4e 2c20 2274 6172  SIFICATION, "tar
-00001b10: 6765 7422 5d0a 2020 2020 290a 2020 2020  get"].    ).    
-00001b20: 6f75 7470 7574 7320 3d20 280a 2020 2020  outputs = (.    
-00001b30: 2020 2020 7573 6572 5f69 640a 2020 2020      user_id.    
-00001b40: 2020 2020 2b20 6974 656d 5f69 640a 2020      + item_id.  
-00001b50: 2020 2020 2020 2b20 6974 656d 5f66 6561        + item_fea
-00001b60: 7475 7265 730a 2020 2020 2020 2020 2b20  tures.        + 
-00001b70: 7573 6572 5f66 6561 7475 7265 730a 2020  user_features.  
-00001b80: 2020 2020 2020 2b20 7573 6572 5f69 7465        + user_ite
-00001b90: 6d5f 6665 6174 7572 6573 0a20 2020 2020  m_features.     
-00001ba0: 2020 202b 2063 6f6e 7465 7874 5f66 6561     + context_fea
-00001bb0: 7475 7265 730a 2020 2020 2020 2020 2b20  tures.        + 
-00001bc0: 7461 7267 6574 730a 2020 2020 290a 0a20  targets.    ).. 
-00001bd0: 2020 2069 6620 6164 645f 7461 7267 6574     if add_target
-00001be0: 5f65 6e63 6f64 696e 673a 0a20 2020 2020  _encoding:.     
-00001bf0: 2020 2063 6f6e 7469 6e75 6f75 7320 3d20     continuous = 
-00001c00: 280a 2020 2020 2020 2020 2020 2020 5b22  (.            ["
-00001c10: 7573 6572 5f69 6422 2c20 2269 7465 6d5f  user_id", "item_
-00001c20: 6964 225d 0a20 2020 2020 2020 2020 2020  id"].           
-00001c30: 203e 3e20 6e76 745f 6f70 732e 5461 7267   >> nvt_ops.Targ
-00001c40: 6574 456e 636f 6469 6e67 285b 2263 6c69  etEncoding(["cli
-00001c50: 636b 225d 2c20 6b66 6f6c 643d 312c 2070  ck"], kfold=1, p
-00001c60: 5f73 6d6f 6f74 683d 3230 290a 2020 2020  _smooth=20).    
-00001c70: 2020 2020 2020 2020 3e3e 206e 7674 5f6f          >> nvt_o
-00001c80: 7073 2e4e 6f72 6d61 6c69 7a65 2829 0a20  ps.Normalize(). 
-00001c90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00001ca0: 206f 7574 7075 7473 202b 3d20 636f 6e74   outputs += cont
-00001cb0: 696e 756f 7573 0a0a 2020 2020 7265 7475  inuous..    retu
-00001cc0: 726e 206e 7674 2e57 6f72 6b66 6c6f 7728  rn nvt.Workflow(
-00001cd0: 6f75 7470 7574 7329 0a0a 0a64 6566 2074  outputs)...def t
-00001ce0: 7261 6e73 666f 726d 5f61 6c69 6363 7028  ransform_aliccp(
-00001cf0: 0a20 2020 2064 6174 613a 2055 6e69 6f6e  .    data: Union
-00001d00: 5b73 7472 2c20 5061 7468 2c20 5475 706c  [str, Path, Tupl
-00001d10: 655b 6d65 726c 696e 2e69 6f2e 4461 7461  e[merlin.io.Data
-00001d20: 7365 742c 206d 6572 6c69 6e2e 696f 2e44  set, merlin.io.D
-00001d30: 6174 6173 6574 5d5d 2c0a 2020 2020 6f75  ataset]],.    ou
-00001d40: 7470 7574 5f70 6174 683a 2055 6e69 6f6e  tput_path: Union
-00001d50: 5b73 7472 2c20 5061 7468 5d2c 0a20 2020  [str, Path],.   
-00001d60: 206e 7674 5f77 6f72 6b66 6c6f 773d 4e6f   nvt_workflow=No
-00001d70: 6e65 2c0a 2020 2020 2a2a 6b77 6172 6773  ne,.    **kwargs
-00001d80: 2c0a 293a 0a20 2020 206e 7674 5f77 6f72  ,.):.    nvt_wor
-00001d90: 6b66 6c6f 7720 3d20 6e76 745f 776f 726b  kflow = nvt_work
-00001da0: 666c 6f77 206f 7220 6465 6661 756c 745f  flow or default_
-00001db0: 616c 6963 6370 5f74 7261 6e73 666f 726d  aliccp_transform
-00001dc0: 6174 696f 6e28 2a2a 6c6f 6361 6c73 2829  ation(**locals()
-00001dd0: 290a 0a20 2020 2069 6620 6973 696e 7374  )..    if isinst
-00001de0: 616e 6365 2864 6174 612c 2028 7374 722c  ance(data, (str,
-00001df0: 2050 6174 6829 293a 0a20 2020 2020 2020   Path)):.       
-00001e00: 205f 7472 6169 6e20 3d20 676c 6f62 2873   _train = glob(s
-00001e10: 7472 2864 6174 6120 2f20 2274 7261 696e  tr(data / "train
-00001e20: 2f2a 2e70 6172 7175 6574 2229 290a 2020  /*.parquet")).  
-00001e30: 2020 2020 2020 5f76 616c 6964 203d 2067        _valid = g
-00001e40: 6c6f 6228 7374 7228 6461 7461 202f 2022  lob(str(data / "
-00001e50: 7465 7374 2f2a 2e70 6172 7175 6574 2229  test/*.parquet")
-00001e60: 290a 2020 2020 656c 6966 2028 0a20 2020  ).    elif (.   
-00001e70: 2020 2020 2069 7369 6e73 7461 6e63 6528       isinstance(
-00001e80: 6461 7461 2c20 7475 706c 6529 0a20 2020  data, tuple).   
-00001e90: 2020 2020 2061 6e64 206c 656e 2864 6174       and len(dat
-00001ea0: 6129 203d 3d20 320a 2020 2020 2020 2020  a) == 2.        
-00001eb0: 616e 6420 616c 6c28 6973 696e 7374 616e  and all(isinstan
-00001ec0: 6365 2878 2c20 6d65 726c 696e 2e69 6f2e  ce(x, merlin.io.
-00001ed0: 4461 7461 7365 7429 2066 6f72 2078 2069  Dataset) for x i
-00001ee0: 6e20 6461 7461 290a 2020 2020 293a 0a20  n data).    ):. 
-00001ef0: 2020 2020 2020 205f 7472 6169 6e2c 205f         _train, _
-00001f00: 7661 6c69 6420 3d20 6461 7461 0a20 2020  valid = data.   
-00001f10: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
-00001f20: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00001f30: 2264 6174 6120 6d75 7374 2062 6520 6120  "data must be a 
-00001f40: 7061 7468 206f 7220 6120 7475 706c 6520  path or a tuple 
-00001f50: 6f66 2074 7261 696e 2061 6e64 2076 616c  of train and val
-00001f60: 6964 2064 6174 6173 6574 7322 290a 0a20  id datasets").. 
-00001f70: 2020 2077 6f72 6b66 6c6f 775f 6669 745f     workflow_fit_
-00001f80: 7472 616e 7366 6f72 6d28 6e76 745f 776f  transform(nvt_wo
-00001f90: 726b 666c 6f77 2c20 5f74 7261 696e 2c20  rkflow, _train, 
-00001fa0: 5f76 616c 6964 2c20 7374 7228 6f75 7470  _valid, str(outp
-00001fb0: 7574 5f70 6174 6829 2c20 2a2a 6b77 6172  ut_path), **kwar
-00001fc0: 6773 290a 0a0a 4064 6174 6163 6c61 7373  gs)...@dataclass
-00001fd0: 0a63 6c61 7373 205f 4665 6174 7572 653a  .class _Feature:
-00001fe0: 0a20 2020 206e 616d 653a 2073 7472 0a20  .    name: str. 
-00001ff0: 2020 2069 643a 2073 7472 0a20 2020 2074     id: str.    t
-00002000: 6167 733a 204c 6973 745b 556e 696f 6e5b  ags: List[Union[
-00002010: 7374 722c 2054 6167 735d 5d0a 2020 2020  str, Tags]].    
-00002020: 6465 7363 7269 7074 696f 6e3a 2073 7472  description: str
-00002030: 0a0a 0a63 6c61 7373 205f 4665 6174 7572  ...class _Featur
-00002040: 6573 3a0a 2020 2020 6465 6620 5f5f 696e  es:.    def __in
-00002050: 6974 5f5f 2873 656c 6629 3a0a 2020 2020  it__(self):.    
-00002060: 2020 2020 7365 6c66 2e66 6561 7475 7265      self.feature
-00002070: 733a 204c 6973 745b 5f46 6561 7475 7265  s: List[_Feature
-00002080: 5d20 3d20 5b0a 2020 2020 2020 2020 2020  ] = [.          
-00002090: 2020 2320 5573 6572 0a20 2020 2020 2020    # User.       
-000020a0: 2020 2020 205f 4665 6174 7572 6528 2275       _Feature("u
-000020b0: 7365 725f 6964 222c 2022 3130 3122 2c20  ser_id", "101", 
-000020c0: 5b54 6167 732e 5553 4552 5f49 442c 2054  [Tags.USER_ID, T
-000020d0: 6167 732e 5553 4552 5d2c 2022 5573 6572  ags.USER], "User
-000020e0: 2049 4422 292c 0a20 2020 2020 2020 2020   ID"),.         
-000020f0: 2020 205f 4665 6174 7572 6528 0a20 2020     _Feature(.   
-00002100: 2020 2020 2020 2020 2020 2020 2022 7573               "us
-00002110: 6572 5f63 6174 6567 6f72 6965 7322 2c0a  er_categories",.
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2231 3039 5f31 3422 2c0a 2020 2020 2020  "109_14",.      
-00002140: 2020 2020 2020 2020 2020 5b54 6167 732e            [Tags.
-00002150: 5553 4552 5d2c 0a20 2020 2020 2020 2020  USER],.         
-00002160: 2020 2020 2020 2022 5573 6572 2068 6973         "User his
-00002170: 746f 7269 6361 6c20 6265 6861 7669 6f72  torical behavior
-00002180: 7320 6f66 2063 6174 6567 6f72 7920 4944  s of category ID
-00002190: 2061 6e64 2063 6f75 6e74 222c 0a20 2020   and count",.   
-000021a0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-000021b0: 2020 2020 2020 2020 5f46 6561 7475 7265          _Feature
-000021c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000021d0: 2020 2275 7365 725f 7368 6f70 7322 2c0a    "user_shops",.
-000021e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021f0: 2231 3130 5f31 3422 2c0a 2020 2020 2020  "110_14",.      
-00002200: 2020 2020 2020 2020 2020 5b54 6167 732e            [Tags.
-00002210: 5553 4552 5d2c 0a20 2020 2020 2020 2020  USER],.         
-00002220: 2020 2020 2020 2022 5573 6572 2068 6973         "User his
-00002230: 746f 7269 6361 6c20 6265 6861 7669 6f72  torical behavior
-00002240: 7320 6f66 2073 686f 7020 4944 2061 6e64  s of shop ID and
-00002250: 2063 6f75 6e74 222c 0a20 2020 2020 2020   count",.       
-00002260: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00002270: 2020 2020 5f46 6561 7475 7265 280a 2020      _Feature(.  
-00002280: 2020 2020 2020 2020 2020 2020 2020 2275                "u
-00002290: 7365 725f 6272 616e 6473 222c 0a20 2020  ser_brands",.   
-000022a0: 2020 2020 2020 2020 2020 2020 2022 3132               "12
-000022b0: 375f 3134 222c 0a20 2020 2020 2020 2020  7_14",.         
-000022c0: 2020 2020 2020 205b 5461 6773 2e55 5345         [Tags.USE
-000022d0: 525d 2c0a 2020 2020 2020 2020 2020 2020  R],.            
-000022e0: 2020 2020 2255 7365 7220 6869 7374 6f72      "User histor
-000022f0: 6963 616c 2062 6568 6176 696f 7273 206f  ical behaviors o
-00002300: 6620 6272 616e 6420 4944 2061 6e64 2063  f brand ID and c
-00002310: 6f75 6e74 222c 0a20 2020 2020 2020 2020  ount",.         
-00002320: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00002330: 2020 5f46 6561 7475 7265 280a 2020 2020    _Feature(.    
-00002340: 2020 2020 2020 2020 2020 2020 2275 7365              "use
-00002350: 725f 696e 7465 6e74 696f 6e73 222c 0a20  r_intentions",. 
-00002360: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002370: 3135 305f 3134 222c 0a20 2020 2020 2020  150_14",.       
-00002380: 2020 2020 2020 2020 205b 5461 6773 2e55           [Tags.U
-00002390: 5345 525d 2c0a 2020 2020 2020 2020 2020  SER],.          
-000023a0: 2020 2020 2020 2255 7365 7220 6869 7374        "User hist
-000023b0: 6f72 6963 616c 2062 6568 6176 696f 7273  orical behaviors
-000023c0: 206f 6620 696e 7465 6e74 696f 6e20 6e6f   of intention no
-000023d0: 6465 2049 4420 616e 6420 636f 756e 7422  de ID and count"
-000023e0: 2c0a 2020 2020 2020 2020 2020 2020 292c  ,.            ),
-000023f0: 0a20 2020 2020 2020 2020 2020 205f 4665  .            _Fe
-00002400: 6174 7572 6528 2275 7365 725f 7072 6f66  ature("user_prof
-00002410: 696c 6522 2c20 2231 3231 222c 205b 5461  ile", "121", [Ta
-00002420: 6773 2e55 5345 525d 2c20 2243 6174 6567  gs.USER], "Categ
-00002430: 6f72 6963 616c 2049 4420 6f66 2055 7365  orical ID of Use
-00002440: 7220 5072 6f66 696c 6522 292c 0a20 2020  r Profile"),.   
-00002450: 2020 2020 2020 2020 205f 4665 6174 7572           _Featur
-00002460: 6528 2275 7365 725f 6772 6f75 7022 2c20  e("user_group", 
-00002470: 2231 3232 222c 205b 5461 6773 2e55 5345  "122", [Tags.USE
-00002480: 525d 2c20 2243 6174 6567 6f72 6963 616c  R], "Categorical
-00002490: 2067 726f 7570 2049 4420 6f66 2055 7365   group ID of Use
-000024a0: 7220 5072 6f66 696c 6522 292c 0a20 2020  r Profile"),.   
-000024b0: 2020 2020 2020 2020 205f 4665 6174 7572           _Featur
-000024c0: 6528 2275 7365 725f 6765 6e64 6572 222c  e("user_gender",
-000024d0: 2022 3132 3422 2c20 5b54 6167 732e 5553   "124", [Tags.US
-000024e0: 4552 5d2c 2022 5573 6572 7320 4765 6e64  ER], "Users Gend
-000024f0: 6572 2049 4422 292c 0a20 2020 2020 2020  er ID"),.       
-00002500: 2020 2020 205f 4665 6174 7572 6528 2275       _Feature("u
-00002510: 7365 725f 6167 6522 2c20 2231 3235 222c  ser_age", "125",
-00002520: 205b 5461 6773 2e55 5345 525d 2c20 2255   [Tags.USER], "U
-00002530: 7365 7273 2041 6765 2049 4422 292c 0a20  sers Age ID"),. 
-00002540: 2020 2020 2020 2020 2020 205f 4665 6174             _Feat
-00002550: 7572 6528 2275 7365 725f 636f 6e73 756d  ure("user_consum
-00002560: 7074 696f 6e5f 3122 2c20 2231 3236 222c  ption_1", "126",
-00002570: 205b 5461 6773 2e55 5345 525d 2c20 2255   [Tags.USER], "U
-00002580: 7365 7273 2043 6f6e 7375 6d70 7469 6f6e  sers Consumption
-00002590: 204c 6576 656c 2054 7970 6520 4922 292c   Level Type I"),
-000025a0: 0a20 2020 2020 2020 2020 2020 205f 4665  .            _Fe
-000025b0: 6174 7572 6528 2275 7365 725f 636f 6e73  ature("user_cons
-000025c0: 756d 7074 696f 6e5f 3222 2c20 2231 3237  umption_2", "127
-000025d0: 222c 205b 5461 6773 2e55 5345 525d 2c20  ", [Tags.USER], 
-000025e0: 2255 7365 7273 2043 6f6e 7375 6d70 7469  "Users Consumpti
-000025f0: 6f6e 204c 6576 656c 2054 7970 6520 4949  on Level Type II
-00002600: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-00002610: 5f46 6561 7475 7265 280a 2020 2020 2020  _Feature(.      
-00002620: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
-00002630: 6973 5f6f 6363 7570 6965 6422 2c20 2231  is_occupied", "1
-00002640: 3238 222c 205b 5461 6773 2e55 5345 525d  28", [Tags.USER]
-00002650: 2c20 2255 7365 7273 204f 6363 7570 6174  , "Users Occupat
-00002660: 696f 6e3a 2077 6865 7468 6572 206f 7220  ion: whether or 
-00002670: 6e6f 7420 746f 2077 6f72 6b22 0a20 2020  not to work".   
-00002680: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
-00002690: 2020 2020 2020 2020 5f46 6561 7475 7265          _Feature
-000026a0: 2822 7573 6572 5f67 656f 6772 6170 6879  ("user_geography
-000026b0: 222c 2022 3132 3922 2c20 5b54 6167 732e  ", "129", [Tags.
-000026c0: 5553 4552 5d2c 2022 5573 6572 7320 4765  USER], "Users Ge
-000026d0: 6f67 7261 7068 7920 496e 666f 726d 6174  ography Informat
-000026e0: 696f 6e22 292c 0a20 2020 2020 2020 2020  ion"),.         
-000026f0: 2020 2023 2049 7465 6d0a 2020 2020 2020     # Item.      
-00002700: 2020 2020 2020 5f46 6561 7475 7265 2822        _Feature("
-00002710: 6974 656d 5f69 6422 2c20 2232 3035 222c  item_id", "205",
-00002720: 205b 5461 6773 2e49 5445 4d2c 2054 6167   [Tags.ITEM, Tag
-00002730: 732e 4954 454d 5f49 445d 2c20 2249 7465  s.ITEM_ID], "Ite
-00002740: 6d20 4944 2229 2c0a 2020 2020 2020 2020  m ID"),.        
-00002750: 2020 2020 5f46 6561 7475 7265 280a 2020      _Feature(.  
-00002760: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00002770: 7465 6d5f 6361 7465 676f 7279 222c 2022  tem_category", "
-00002780: 3230 3622 2c20 5b54 6167 732e 4954 454d  206", [Tags.ITEM
-00002790: 5d2c 2022 4361 7465 676f 7279 2049 4420  ], "Category ID 
-000027a0: 746f 2077 6869 6368 2074 6865 2069 7465  to which the ite
-000027b0: 6d20 6265 6c6f 6e67 7320 746f 220a 2020  m belongs to".  
-000027c0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-000027d0: 2020 2020 2020 2020 205f 4665 6174 7572           _Featur
-000027e0: 6528 2269 7465 6d5f 7368 6f70 222c 2022  e("item_shop", "
-000027f0: 3230 3722 2c20 5b54 6167 732e 4954 454d  207", [Tags.ITEM
-00002800: 5d2c 2022 5368 6f70 2049 4420 746f 2077  ], "Shop ID to w
-00002810: 6869 6368 2069 7465 6d20 6265 6c6f 6e67  hich item belong
-00002820: 7320 746f 2229 2c0a 2020 2020 2020 2020  s to"),.        
-00002830: 2020 2020 5f46 6561 7475 7265 280a 2020      _Feature(.  
-00002840: 2020 2020 2020 2020 2020 2020 2020 2269                "i
-00002850: 7465 6d5f 696e 7465 6e74 696f 6e22 2c20  tem_intention", 
-00002860: 2232 3130 222c 205b 5461 6773 2e49 5445  "210", [Tags.ITE
-00002870: 4d5d 2c20 2249 6e74 656e 7469 6f6e 206e  M], "Intention n
-00002880: 6f64 6520 4944 2077 6869 6368 2074 6865  ode ID which the
-00002890: 2069 7465 6d20 6265 6c6f 6e67 7320 746f   item belongs to
-000028a0: 220a 2020 2020 2020 2020 2020 2020 292c  ".            ),
-000028b0: 0a20 2020 2020 2020 2020 2020 205f 4665  .            _Fe
-000028c0: 6174 7572 6528 2269 7465 6d5f 6272 616e  ature("item_bran
-000028d0: 6422 2c20 2232 3136 222c 205b 5461 6773  d", "216", [Tags
-000028e0: 2e49 5445 4d5d 2c20 2242 7261 6e64 2049  .ITEM], "Brand I
-000028f0: 4420 6f66 2074 6865 2069 7465 6d22 292c  D of the item"),
-00002900: 0a20 2020 2020 2020 2020 2020 2023 2055  .            # U
-00002910: 7365 722d 4974 656d 0a20 2020 2020 2020  ser-Item.       
-00002920: 2020 2020 205f 4665 6174 7572 6528 0a20       _Feature(. 
-00002930: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002940: 7573 6572 5f69 7465 6d5f 6361 7465 676f  user_item_catego
-00002950: 7269 6573 222c 0a20 2020 2020 2020 2020  ries",.         
-00002960: 2020 2020 2020 2022 3530 3822 2c0a 2020         "508",.  
-00002970: 2020 2020 2020 2020 2020 2020 2020 5b22                ["
-00002980: 7573 6572 5f69 7465 6d22 5d2c 0a20 2020  user_item"],.   
-00002990: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
-000029a0: 6520 636f 6d62 696e 6174 696f 6e20 6f66  e combination of
-000029b0: 2066 6561 7475 7265 7320 7769 7468 2031   features with 1
-000029c0: 3039 5f31 3420 616e 6420 3230 3622 2c0a  09_14 and 206",.
-000029d0: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
-000029e0: 2020 2020 2020 2020 2020 205f 4665 6174             _Feat
-000029f0: 7572 6528 0a20 2020 2020 2020 2020 2020  ure(.           
-00002a00: 2020 2020 2022 7573 6572 5f69 7465 6d5f       "user_item_
-00002a10: 7368 6f70 7322 2c0a 2020 2020 2020 2020  shops",.        
-00002a20: 2020 2020 2020 2020 2235 3039 222c 0a20          "509",. 
-00002a30: 2020 2020 2020 2020 2020 2020 2020 205b                 [
-00002a40: 2275 7365 725f 6974 656d 225d 2c0a 2020  "user_item"],.  
-00002a50: 2020 2020 2020 2020 2020 2020 2020 2254                "T
-00002a60: 6865 2063 6f6d 6269 6e61 7469 6f6e 206f  he combination o
-00002a70: 6620 6665 6174 7572 6573 2077 6974 6820  f features with 
-00002a80: 3131 305f 3134 2061 6e64 2032 3037 222c  110_14 and 207",
-00002a90: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
-00002aa0: 2020 2020 2020 2020 2020 2020 5f46 6561              _Fea
-00002ab0: 7475 7265 280a 2020 2020 2020 2020 2020  ture(.          
-00002ac0: 2020 2020 2020 2275 7365 725f 6974 656d        "user_item
-00002ad0: 5f62 7261 6e64 7322 2c0a 2020 2020 2020  _brands",.      
-00002ae0: 2020 2020 2020 2020 2020 2237 3032 222c            "702",
-00002af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002b00: 205b 2275 7365 725f 6974 656d 225d 2c0a   ["user_item"],.
-00002b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b20: 2254 6865 2063 6f6d 6269 6e61 7469 6f6e  "The combination
-00002b30: 206f 6620 6665 6174 7572 6573 2077 6974   of features wit
-00002b40: 6820 3132 375f 3134 2061 6e64 2032 3136  h 127_14 and 216
-00002b50: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-00002b60: 2c0a 2020 2020 2020 2020 2020 2020 5f46  ,.            _F
-00002b70: 6561 7475 7265 280a 2020 2020 2020 2020  eature(.        
-00002b80: 2020 2020 2020 2020 2275 7365 725f 6974          "user_it
-00002b90: 656d 5f69 6e74 656e 7469 6f6e 7322 2c0a  em_intentions",.
-00002ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002bb0: 2238 3533 222c 0a20 2020 2020 2020 2020  "853",.         
-00002bc0: 2020 2020 2020 205b 2275 7365 725f 6974         ["user_it
-00002bd0: 656d 225d 2c0a 2020 2020 2020 2020 2020  em"],.          
-00002be0: 2020 2020 2020 2254 6865 2063 6f6d 6269        "The combi
-00002bf0: 6e61 7469 6f6e 206f 6620 6665 6174 7572  nation of featur
-00002c00: 6573 2077 6974 6820 3135 305f 3134 2061  es with 150_14 a
-00002c10: 6e64 2032 3130 222c 0a20 2020 2020 2020  nd 210",.       
-00002c20: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00002c30: 2020 2020 2320 436f 6e74 6578 740a 2020      # Context.  
-00002c40: 2020 2020 2020 2020 2020 5f46 6561 7475            _Featu
-00002c50: 7265 2822 706f 7369 7469 6f6e 222c 2022  re("position", "
-00002c60: 3330 3122 2c20 5b54 6167 732e 434f 4e54  301", [Tags.CONT
-00002c70: 4558 545d 2c20 2241 2063 6174 6567 6f72  EXT], "A categor
-00002c80: 6963 616c 2065 7870 7265 7373 696f 6e20  ical expression 
-00002c90: 6f66 2070 6f73 6974 696f 6e22 292c 0a20  of position"),. 
-00002ca0: 2020 2020 2020 205d 0a0a 2020 2020 4070         ]..    @p
-00002cb0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-00002cc0: 6279 5f69 6428 7365 6c66 293a 0a20 2020  by_id(self):.   
-00002cd0: 2020 2020 2072 6574 7572 6e20 7b66 6561       return {fea
-00002ce0: 7475 7265 2e69 643a 2066 6561 7475 7265  ture.id: feature
-00002cf0: 2e6e 616d 6520 666f 7220 6665 6174 7572  .name for featur
-00002d00: 6520 696e 2073 656c 662e 6665 6174 7572  e in self.featur
-00002d10: 6573 7d0a 0a0a 6465 6620 5f63 6f6e 7665  es}...def _conve
-00002d20: 7274 5f63 6f6d 6d6f 6e5f 6665 6174 7572  rt_common_featur
-00002d30: 6573 2863 6f6d 6d6f 6e5f 7061 7468 2c20  es(common_path, 
-00002d40: 7069 636b 6c65 5f70 6174 683d 4e6f 6e65  pickle_path=None
-00002d50: 293a 0a20 2020 2063 6f6d 6d6f 6e20 3d20  ):.    common = 
-00002d60: 7b7d 0a0a 2020 2020 7769 7468 206f 7065  {}..    with ope
-00002d70: 6e28 636f 6d6d 6f6e 5f70 6174 682c 2022  n(common_path, "
-00002d80: 7222 2920 6173 2063 6f6d 6d6f 6e5f 6665  r") as common_fe
-00002d90: 6174 7572 6573 3a0a 2020 2020 2020 2020  atures:.        
-00002da0: 666f 7220 6373 765f 6c69 6e65 2069 6e20  for csv_line in 
-00002db0: 7471 646d 2863 6f6d 6d6f 6e5f 6665 6174  tqdm(common_feat
-00002dc0: 7572 6573 2c20 6465 7363 3d22 5265 6164  ures, desc="Read
-00002dd0: 696e 6720 636f 6d6d 6f6e 2066 6561 7475  ing common featu
-00002de0: 7265 732e 2e2e 2229 3a0a 2020 2020 2020  res..."):.      
-00002df0: 2020 2020 2020 6c69 6e65 203d 2063 7376        line = csv
-00002e00: 5f6c 696e 652e 7374 7269 7028 292e 7370  _line.strip().sp
-00002e10: 6c69 7428 222c 2229 0a20 2020 2020 2020  lit(",").       
-00002e20: 2020 2020 206b 7620 3d20 6e70 2e61 7272       kv = np.arr
-00002e30: 6179 2872 652e 7370 6c69 7428 225b 0102  ay(re.split("[..
-00002e40: 035d 222c 206c 696e 655b 325d 2929 0a20  .]", line[2])). 
-00002e50: 2020 2020 2020 2020 2020 206b 6579 7320             keys 
-00002e60: 3d20 6b76 5b72 616e 6765 2830 2c20 6c65  = kv[range(0, le
-00002e70: 6e28 6b76 292c 2033 295d 0a20 2020 2020  n(kv), 3)].     
-00002e80: 2020 2020 2020 2076 616c 7565 7320 3d20         values = 
-00002e90: 6b76 5b72 616e 6765 2831 2c20 6c65 6e28  kv[range(1, len(
-00002ea0: 6b76 292c 2033 295d 0a20 2020 2020 2020  kv), 3)].       
-00002eb0: 2020 2020 2063 6f6d 6d6f 6e5b 6c69 6e65       common[line
-00002ec0: 5b30 5d5d 203d 2064 6963 7428 7a69 7028  [0]] = dict(zip(
-00002ed0: 6b65 7973 2c20 7661 6c75 6573 2929 0a0a  keys, values))..
-00002ee0: 2020 2020 2020 2020 6966 2070 6963 6b6c          if pickl
-00002ef0: 655f 7061 7468 3a0a 2020 2020 2020 2020  e_path:.        
-00002f00: 2020 2020 7769 7468 206f 7065 6e28 7069      with open(pi
-00002f10: 636b 6c65 5f70 6174 682c 2022 7762 2229  ckle_path, "wb")
-00002f20: 2061 7320 6861 6e64 6c65 3a0a 2020 2020   as handle:.    
-00002f30: 2020 2020 2020 2020 2020 2020 7069 636b              pick
-00002f40: 6c65 2e64 756d 7028 636f 6d6d 6f6e 2c20  le.dump(common, 
-00002f50: 6861 6e64 6c65 2c20 7072 6f74 6f63 6f6c  handle, protocol
-00002f60: 3d70 6963 6b6c 652e 4849 4748 4553 545f  =pickle.HIGHEST_
-00002f70: 5052 4f54 4f43 4f4c 290a 0a20 2020 2072  PROTOCOL)..    r
-00002f80: 6574 7572 6e20 636f 6d6d 6f6e 0a0a 0a23  eturn common...#
-00002f90: 2054 4f44 4f3a 204f 7074 696d 697a 6520   TODO: Optimize 
-00002fa0: 7468 6973 2066 756e 6374 696f 6e2c 2072  this function, r
-00002fb0: 6967 6874 206e 6f77 2069 7427 7320 746f  ight now it's to
-00002fc0: 6f20 736c 6f77 2e0a 6465 6620 5f63 6f6e  o slow..def _con
-00002fd0: 7665 7274 5f64 6174 6128 0a20 2020 2064  vert_data(.    d
-00002fe0: 6174 615f 6469 722c 0a20 2020 2066 696c  ata_dir,.    fil
-00002ff0: 655f 7369 7a65 2c0a 2020 2020 6973 5f74  e_size,.    is_t
-00003000: 7261 696e 3d54 7275 652c 0a20 2020 2070  rain=True,.    p
-00003010: 6963 6b6c 655f 636f 6d6d 6f6e 5f66 6561  ickle_common_fea
-00003020: 7475 7265 733d 5472 7565 2c0a 2020 2020  tures=True,.    
-00003030: 6d61 785f 6e75 6d5f 726f 7773 3d4e 6f6e  max_num_rows=Non
-00003040: 652c 0a20 2020 206f 7574 7075 745f 6469  e,.    output_di
-00003050: 723d 4e6f 6e65 2c0a 293a 0a20 2020 2064  r=None,.):.    d
-00003060: 6174 615f 7479 7065 203d 2022 7472 6169  ata_type = "trai
-00003070: 6e22 2069 6620 6973 5f74 7261 696e 2065  n" if is_train e
-00003080: 6c73 6520 2274 6573 7422 0a20 2020 206f  lse "test".    o
-00003090: 7574 7075 745f 6469 7220 3d20 6f75 7470  utput_dir = outp
-000030a0: 7574 5f64 6972 206f 7220 6461 7461 5f64  ut_dir or data_d
-000030b0: 6972 0a0a 2020 2020 636f 6d6d 6f6e 5f70  ir..    common_p
-000030c0: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-000030d0: 696e 2864 6174 615f 6469 722c 2064 6174  in(data_dir, dat
-000030e0: 615f 7479 7065 2c20 6622 636f 6d6d 6f6e  a_type, f"common
-000030f0: 5f66 6561 7475 7265 735f 7b64 6174 615f  _features_{data_
-00003100: 7479 7065 7d2e 6373 7622 290a 2020 2020  type}.csv").    
-00003110: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
-00003120: 6f69 6e28 6461 7461 5f64 6972 2c20 6461  oin(data_dir, da
-00003130: 7461 5f74 7970 652c 2066 2273 616d 706c  ta_type, f"sampl
-00003140: 655f 736b 656c 6574 6f6e 5f7b 6461 7461  e_skeleton_{data
-00003150: 5f74 7970 657d 2e63 7376 2229 0a20 2020  _type}.csv").   
-00003160: 2063 6f6d 6d6f 6e5f 6665 6174 7572 6573   common_features
-00003170: 5f70 6174 6820 3d20 6f73 2e70 6174 682e  _path = os.path.
-00003180: 6a6f 696e 2864 6174 615f 6469 722c 2064  join(data_dir, d
-00003190: 6174 615f 7479 7065 2c20 2263 6f6d 6d6f  ata_type, "commo
-000031a0: 6e5f 6665 6174 7572 6573 2e70 6963 6b6c  n_features.pickl
-000031b0: 6522 290a 0a20 2020 2063 6f6d 6d6f 6e20  e")..    common 
-000031c0: 3d20 7b7d 0a20 2020 2069 6620 7069 636b  = {}.    if pick
-000031d0: 6c65 5f63 6f6d 6d6f 6e5f 6665 6174 7572  le_common_featur
-000031e0: 6573 3a0a 2020 2020 2020 2020 6966 206f  es:.        if o
-000031f0: 732e 7061 7468 2e65 7869 7374 7328 636f  s.path.exists(co
-00003200: 6d6d 6f6e 5f66 6561 7475 7265 735f 7061  mmon_features_pa
-00003210: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
-00003220: 2077 6974 6820 6f70 656e 2863 6f6d 6d6f   with open(commo
-00003230: 6e5f 6665 6174 7572 6573 5f70 6174 682c  n_features_path,
-00003240: 2022 7262 2229 2061 7320 663a 0a20 2020   "rb") as f:.   
-00003250: 2020 2020 2020 2020 2020 2020 2063 6f6d               com
-00003260: 6d6f 6e20 3d20 7069 636b 6c65 2e6c 6f61  mon = pickle.loa
-00003270: 6428 6629 0a0a 2020 2020 6966 206e 6f74  d(f)..    if not
-00003280: 2063 6f6d 6d6f 6e3a 0a20 2020 2020 2020   common:.       
-00003290: 2070 6963 6b6c 655f 7061 7468 203d 2063   pickle_path = c
-000032a0: 6f6d 6d6f 6e5f 6665 6174 7572 6573 5f70  ommon_features_p
-000032b0: 6174 6820 6966 2070 6963 6b6c 655f 636f  ath if pickle_co
-000032c0: 6d6d 6f6e 5f66 6561 7475 7265 7320 656c  mmon_features el
-000032d0: 7365 204e 6f6e 650a 2020 2020 2020 2020  se None.        
-000032e0: 636f 6d6d 6f6e 203d 205f 636f 6e76 6572  common = _conver
-000032f0: 745f 636f 6d6d 6f6e 5f66 6561 7475 7265  t_common_feature
-00003300: 7328 636f 6d6d 6f6e 5f70 6174 682c 2070  s(common_path, p
-00003310: 6963 6b6c 655f 7061 7468 290a 0a20 2020  ickle_path)..   
-00003320: 2063 7572 7265 6e74 203d 205b 5d0a 2020   current = [].  
-00003330: 2020 6279 5f69 6420 3d20 5f46 6561 7475    by_id = _Featu
-00003340: 7265 7328 292e 6279 5f69 640a 0a20 2020  res().by_id..   
-00003350: 206f 7574 5f64 6972 203d 206f 732e 7061   out_dir = os.pa
-00003360: 7468 2e6a 6f69 6e28 7374 7228 6f75 7470  th.join(str(outp
-00003370: 7574 5f64 6972 292c 2064 6174 615f 7479  ut_dir), data_ty
-00003380: 7065 290a 2020 2020 746d 705f 6469 7220  pe).    tmp_dir 
-00003390: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
-000033a0: 7574 5f64 6972 2c20 2274 6d70 2229 0a20  ut_dir, "tmp"). 
-000033b0: 2020 2069 6620 6e6f 7420 6f73 2e70 6174     if not os.pat
-000033c0: 682e 6578 6973 7473 2874 6d70 5f64 6972  h.exists(tmp_dir
-000033d0: 293a 0a20 2020 2020 2020 206f 732e 6d61  ):.        os.ma
-000033e0: 6b65 6469 7273 2874 6d70 5f64 6972 290a  kedirs(tmp_dir).
-000033f0: 0a20 2020 2077 6974 6820 6f70 656e 2870  .    with open(p
-00003400: 6174 682c 2022 7222 2920 6173 2073 6b65  ath, "r") as ske
-00003410: 6c65 746f 6e3a 0a20 2020 2020 2020 2066  leton:.        f
-00003420: 6f72 2069 2c20 6373 765f 6c69 6e65 2069  or i, csv_line i
-00003430: 6e20 7471 646d 2865 6e75 6d65 7261 7465  n tqdm(enumerate
-00003440: 2873 6b65 6c65 746f 6e29 2c20 6465 7363  (skeleton), desc
-00003450: 3d22 5072 6f63 6573 7369 6e67 2064 6174  ="Processing dat
-00003460: 612e 2e2e 2229 3a0a 2020 2020 2020 2020  a..."):.        
-00003470: 2020 2020 6966 206d 6178 5f6e 756d 5f72      if max_num_r
-00003480: 6f77 7320 616e 6420 6920 3e3d 206d 6178  ows and i >= max
-00003490: 5f6e 756d 5f72 6f77 733a 0a20 2020 2020  _num_rows:.     
-000034a0: 2020 2020 2020 2020 2020 2062 7265 616b             break
-000034b0: 0a0a 2020 2020 2020 2020 2020 2020 6c69  ..            li
-000034c0: 6e65 203d 2063 7376 5f6c 696e 652e 7374  ne = csv_line.st
-000034d0: 7269 7028 292e 7370 6c69 7428 222c 2229  rip().split(",")
-000034e0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000034f0: 6c69 6e65 5b31 5d20 3d3d 2022 3022 2061  line[1] == "0" a
-00003500: 6e64 206c 696e 655b 325d 203d 3d20 2231  nd line[2] == "1
-00003510: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00003520: 2020 2063 6f6e 7469 6e75 650a 2020 2020     continue.    
-00003530: 2020 2020 2020 2020 6b76 203d 206e 702e          kv = np.
-00003540: 6172 7261 7928 7265 2e73 706c 6974 2822  array(re.split("
-00003550: 5b01 0203 5d22 2c20 6c69 6e65 5b35 5d29  [...]", line[5])
-00003560: 290a 2020 2020 2020 2020 2020 2020 6b65  ).            ke
-00003570: 7920 3d20 6b76 5b72 616e 6765 2830 2c20  y = kv[range(0, 
-00003580: 6c65 6e28 6b76 292c 2033 295d 0a20 2020  len(kv), 3)].   
-00003590: 2020 2020 2020 2020 2076 616c 7565 203d           value =
-000035a0: 206b 765b 7261 6e67 6528 312c 206c 656e   kv[range(1, len
-000035b0: 286b 7629 2c20 3329 5d0a 2020 2020 2020  (kv), 3)].      
-000035c0: 2020 2020 2020 6665 6174 5f64 6963 7420        feat_dict 
-000035d0: 3d20 6469 6374 287a 6970 286b 6579 2c20  = dict(zip(key, 
-000035e0: 7661 6c75 6529 290a 2020 2020 2020 2020  value)).        
-000035f0: 2020 2020 6665 6174 5f64 6963 742e 7570      feat_dict.up
-00003600: 6461 7465 2863 6f6d 6d6f 6e5b 6c69 6e65  date(common[line
-00003610: 5b33 5d5d 290a 2020 2020 2020 2020 2020  [3]]).          
-00003620: 2020 6665 6174 5f64 6963 745b 2263 6c69    feat_dict["cli
-00003630: 636b 225d 203d 2069 6e74 286c 696e 655b  ck"] = int(line[
-00003640: 315d 290a 2020 2020 2020 2020 2020 2020  1]).            
-00003650: 6665 6174 5f64 6963 745b 2263 6f6e 7665  feat_dict["conve
-00003660: 7273 696f 6e22 5d20 3d20 696e 7428 6c69  rsion"] = int(li
-00003670: 6e65 5b32 5d29 0a0a 2020 2020 2020 2020  ne[2])..        
-00003680: 2020 2020 6375 7272 656e 742e 6170 7065      current.appe
-00003690: 6e64 2866 6561 745f 6469 6374 290a 0a20  nd(feat_dict).. 
-000036a0: 2020 2020 2020 2020 2020 2069 6620 6920             if i 
-000036b0: 3e20 3020 616e 6420 6920 2520 6669 6c65  > 0 and i % file
-000036c0: 5f73 697a 6520 3d3d 2030 3a0a 2020 2020  _size == 0:.    
-000036d0: 2020 2020 2020 2020 2020 2020 6466 203d              df =
-000036e0: 2067 6574 5f6c 6962 2829 2e44 6174 6146   get_lib().DataF
-000036f0: 7261 6d65 2863 7572 7265 6e74 290a 2020  rame(current).  
-00003700: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00003710: 6c73 203d 205b 5d0a 2020 2020 2020 2020  ls = [].        
-00003720: 2020 2020 2020 2020 666f 7220 636f 6c20          for col 
-00003730: 696e 206c 6973 7428 6466 2e63 6f6c 756d  in list(df.colum
-00003740: 6e73 293a 0a20 2020 2020 2020 2020 2020  ns):.           
-00003750: 2020 2020 2020 2020 2069 6620 636f 6c20           if col 
-00003760: 3d3d 2022 636c 6963 6b22 206f 7220 636f  == "click" or co
-00003770: 6c20 3d3d 2022 636f 6e76 6572 7369 6f6e  l == "conversion
-00003780: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00003790: 2020 2020 2020 2020 2020 2063 6f6c 732e             cols.
-000037a0: 6170 7065 6e64 2863 6f6c 290a 2020 2020  append(col).    
-000037b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000037c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000037d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000037e0: 6c73 2e61 7070 656e 6428 6279 5f69 645b  ls.append(by_id[
-000037f0: 636f 6c5d 290a 0a20 2020 2020 2020 2020  col])..         
-00003800: 2020 2020 2020 2064 662e 636f 6c75 6d6e         df.column
-00003810: 7320 3d20 636f 6c73 0a20 2020 2020 2020  s = cols.       
-00003820: 2020 2020 2020 2020 2069 6e64 6578 203d           index =
-00003830: 2069 6e74 2828 6920 2f20 6669 6c65 5f73   int((i / file_s
-00003840: 697a 6529 202d 2031 290a 2020 2020 2020  ize) - 1).      
-00003850: 2020 2020 2020 2020 2020 6466 2e74 6f5f            df.to_
-00003860: 7061 7271 7565 7428 0a20 2020 2020 2020  parquet(.       
-00003870: 2020 2020 2020 2020 2020 2020 206f 732e               os.
-00003880: 7061 7468 2e6a 6f69 6e28 746d 705f 6469  path.join(tmp_di
-00003890: 722c 2066 227b 6461 7461 5f74 7970 657d  r, f"{data_type}
-000038a0: 5f7b 696e 6465 787d 2e70 6172 7175 6574  _{index}.parquet
-000038b0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
-000038c0: 2020 2020 2020 2020 6f76 6572 7772 6974          overwrit
-000038d0: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
-000038e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000038f0: 2020 2020 2020 2020 2020 6375 7272 656e            curren
-00003900: 7420 3d20 5b5d 0a0a 2020 2020 746d 705f  t = []..    tmp_
-00003910: 6669 6c65 7320 3d20 676c 6f62 286f 732e  files = glob(os.
-00003920: 7061 7468 2e6a 6f69 6e28 746d 705f 6469  path.join(tmp_di
-00003930: 722c 2066 227b 6461 7461 5f74 7970 657d  r, f"{data_type}
-00003940: 5f2a 2e70 6172 7175 6574 2229 290a 2020  _*.parquet")).  
-00003950: 2020 6474 7970 6573 203d 207b 662e 6e61    dtypes = {f.na
-00003960: 6d65 3a20 2269 6e74 3332 2220 666f 7220  me: "int32" for 
-00003970: 6620 696e 205f 4665 6174 7572 6573 2829  f in _Features()
-00003980: 2e66 6561 7475 7265 737d 0a20 2020 206d  .features}.    m
-00003990: 6572 6c69 6e2e 696f 2e44 6174 6173 6574  erlin.io.Dataset
-000039a0: 2874 6d70 5f66 696c 6573 2c20 6474 7970  (tmp_files, dtyp
-000039b0: 6573 3d64 7479 7065 7329 2e74 6f5f 7061  es=dtypes).to_pa
-000039c0: 7271 7565 7428 6f75 745f 6469 7229 0a20  rquet(out_dir). 
-000039d0: 2020 2073 6875 7469 6c2e 726d 7472 6565     shutil.rmtree
-000039e0: 2874 6d70 5f64 6972 290a                 (tmp_dir).
+00000710: 6963 6370 2864 6174 615f 6469 7229 6020  iccp(data_dir)` 
+00000720: 746f 2063 6f6e 7665 7274 2074 6865 2072  to convert the r
+00000730: 6177 2064 6174 6120 746f 2070 6172 7175  aw data to parqu
+00000740: 6574 2066 696c 6573 2e0a 0a20 2020 2044  et files...    D
+00000750: 6f77 6e6c 6f61 6469 6e67 2026 2070 7265  ownloading & pre
+00000760: 7061 7269 6e67 2074 6865 2064 6174 6120  paring the data 
+00000770: 6361 6e20 7461 6b65 2071 7569 7465 2061  can take quite a
+00000780: 2077 6869 6c65 2e0a 2020 2020 496e 2063   while..    In c
+00000790: 6173 6520 796f 7520 7761 6e74 2074 6f20  ase you want to 
+000007a0: 7573 6520 7468 6973 2064 6174 6173 6574  use this dataset
+000007b0: 2074 6f20 7275 6e20 6f75 7220 7475 746f   to run our tuto
+000007c0: 7269 616c 732c 2079 6f75 2063 616e 2061  rials, you can a
+000007d0: 6c73 6f20 6f70 7420 666f 7220 7379 6e74  lso opt for synt
+000007e0: 6865 7469 6320 6461 7461 2e0a 2020 2020  hetic data..    
+000007f0: 5379 6e74 6865 7469 6320 6461 7461 2063  Synthetic data c
+00000800: 616e 2062 6520 6765 6e65 7261 7465 6420  an be generated 
+00000810: 6279 2072 756e 6e69 6e67 3a3a 0a20 2020  by running::.   
+00000820: 2020 2020 2066 726f 6d20 6d65 726c 696e       from merlin
+00000830: 2e6d 6f64 656c 732e 6461 7461 2e73 796e  .models.data.syn
+00000840: 7468 6574 6963 2069 6d70 6f72 7420 6765  thetic import ge
+00000850: 6e65 7261 7465 5f64 6174 610a 0a20 2020  nerate_data..   
+00000860: 2020 2020 2064 6174 6120 3d20 6765 6e65       data = gene
+00000870: 7261 7465 5f64 6174 6128 2261 6c69 6363  rate_data("alicc
+00000880: 7022 290a 0a20 2020 204e 6f74 652c 2072  p")..    Note, r
+00000890: 756e 6e69 6e67 2074 6869 7320 6675 6e63  unning this func
+000008a0: 7469 6f6e 2072 6571 7569 7265 7320 7468  tion requires th
+000008b0: 650a 2020 2020 5b6e 7674 6162 756c 6172  e.    [nvtabular
+000008c0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008d0: 2e63 6f6d 2f4e 5649 4449 412d 4d65 726c  .com/NVIDIA-Merl
+000008e0: 696e 2f4e 5654 6162 756c 6172 2920 6c69  in/NVTabular) li
+000008f0: 6272 6172 792e 0a0a 2020 2020 5061 7261  brary...    Para
+00000900: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
+00000910: 2d2d 2d2d 2d0a 2020 2020 7061 7468 3a20  -----.    path: 
+00000920: 556e 696f 6e5b 7374 722c 2050 6174 685d  Union[str, Path]
+00000930: 0a20 2020 2020 2020 2044 6972 6563 746f  .        Directo
+00000940: 7279 2074 6f20 6c6f 6164 2074 6865 2072  ry to load the r
+00000950: 6177 2064 6174 6120 6672 6f6d 2e0a 2020  aw data from..  
+00000960: 2020 6f76 6572 7772 6974 653a 2062 6f6f    overwrite: boo
+00000970: 6c0a 2020 2020 2020 2020 5768 6574 6865  l.        Whethe
+00000980: 7220 746f 206f 7665 7277 7269 7465 2074  r to overwrite t
+00000990: 6865 2074 7261 6e73 666f 726d 6564 2064  he transformed d
+000009a0: 6174 612e 0a20 2020 2074 7261 6e73 666f  ata..    transfo
+000009b0: 726d 6564 5f6e 616d 653a 2073 7472 0a20  rmed_name: str. 
+000009c0: 2020 2020 2020 204e 616d 6520 6f66 2074         Name of t
+000009d0: 6865 2074 7261 6e73 666f 726d 6564 2064  he transformed d
+000009e0: 6174 612e 0a20 2020 2020 2020 2054 6869  ata..        Thi
+000009f0: 7320 6973 2075 7365 6675 6c20 7768 656e  s is useful when
+00000a00: 2079 6f75 2077 616e 7420 746f 206c 6f61   you want to loa
+00000a10: 6420 7468 6520 7472 616e 7366 6f72 6d65  d the transforme
+00000a20: 6420 6461 7461 0a20 2020 2020 2020 206d  d data.        m
+00000a30: 756c 7469 706c 6520 7469 6d65 7320 7573  ultiple times us
+00000a40: 696e 6720 6469 6666 6572 656e 7420 776f  ing different wo
+00000a50: 726b 666c 6f77 732e 0a20 2020 206e 7674  rkflows..    nvt
+00000a60: 5f77 6f72 6b66 6c6f 773a 204f 7074 696f  _workflow: Optio
+00000a70: 6e61 6c5b 576f 726b 666c 6f77 5d0a 2020  nal[Workflow].  
+00000a80: 2020 2020 2020 576f 726b 666c 6f77 2074        Workflow t
+00000a90: 6f20 7472 616e 7366 6f72 6d20 7468 6520  o transform the 
+00000aa0: 7261 7720 6461 7461 2e0a 2020 2020 2020  raw data..      
+00000ab0: 2020 4966 204e 6f6e 652c 2074 6865 2064    If None, the d
+00000ac0: 6566 6175 6c74 2077 6f72 6b66 6c6f 7720  efault workflow 
+00000ad0: 7769 6c6c 2062 6520 7573 6564 2066 726f  will be used fro
+00000ae0: 6d20 6064 6566 6175 6c74 5f61 6c69 6363  m `default_alicc
+00000af0: 705f 7472 616e 7366 6f72 6d61 7469 6f6e  p_transformation
+00000b00: 602e 0a20 2020 2066 696c 655f 7369 7a65  `..    file_size
+00000b10: 3a20 696e 740a 2020 2020 2020 2020 5369  : int.        Si
+00000b20: 7a65 206f 6620 7468 6520 7061 7271 7565  ze of the parque
+00000b30: 7420 6669 6c65 7320 746f 2062 6520 6c6f  t files to be lo
+00000b40: 6164 6564 2077 6865 6e20 7072 6570 6172  aded when prepar
+00000b50: 696e 6720 7468 6520 6461 7461 2e0a 0a20  ing the data... 
+00000b60: 2020 2052 6574 7572 6e73 0a20 2020 202d     Returns.    -
+00000b70: 2d2d 2d2d 2d2d 0a20 2020 2074 7261 696e  ------.    train
+00000b80: 3a20 6d65 726c 696e 2e69 6f2e 4461 7461  : merlin.io.Data
+00000b90: 7365 740a 2020 2020 2020 2020 5472 6169  set.        Trai
+00000ba0: 6e69 6e67 2064 6174 6173 6574 2e0a 2020  ning dataset..  
+00000bb0: 2020 7661 6c69 643a 206d 6572 6c69 6e2e    valid: merlin.
+00000bc0: 696f 2e44 6174 6173 6574 0a20 2020 2020  io.Dataset.     
+00000bd0: 2020 2054 6573 7420 6461 7461 7365 742e     Test dataset.
+00000be0: 0a20 2020 2022 2222 0a0a 2020 2020 7265  .    """..    re
+00000bf0: 7175 6972 655f 6e76 7428 290a 0a20 2020  quire_nvt()..   
+00000c00: 2070 203d 2050 6174 6828 7061 7468 290a   p = Path(path).
+00000c10: 2020 2020 7261 775f 7061 7468 203d 2070      raw_path = p
+00000c20: 202f 2022 7261 7722 0a20 2020 2069 6620   / "raw".    if 
+00000c30: 6e6f 7420 7261 775f 7061 7468 2e65 7869  not raw_path.exi
+00000c40: 7374 7328 293a 0a20 2020 2020 2020 2072  sts():.        r
+00000c50: 6177 5f70 6174 682e 6d6b 6469 7228 7061  aw_path.mkdir(pa
+00000c60: 7265 6e74 733d 5472 7565 290a 2020 2020  rents=True).    
+00000c70: 2020 2020 7072 6570 6172 655f 616c 6963      prepare_alic
+00000c80: 6370 2870 6174 682c 206f 7574 7075 745f  cp(path, output_
+00000c90: 6469 723d 7261 775f 7061 7468 2c20 6669  dir=raw_path, fi
+00000ca0: 6c65 5f73 697a 653d 6669 6c65 5f73 697a  le_size=file_siz
+00000cb0: 652c 202a 2a6b 7761 7267 7329 0a0a 2020  e, **kwargs)..  
+00000cc0: 2020 6e76 745f 7061 7468 203d 2070 202f    nvt_path = p /
+00000cd0: 2074 7261 6e73 666f 726d 6564 5f6e 616d   transformed_nam
+00000ce0: 650a 2020 2020 7472 6169 6e5f 7061 7468  e.    train_path
+00000cf0: 2c20 7661 6c69 645f 7061 7468 203d 206e  , valid_path = n
+00000d00: 7674 5f70 6174 6820 2f20 2274 7261 696e  vt_path / "train
+00000d10: 222c 206e 7674 5f70 6174 6820 2f20 2276  ", nvt_path / "v
+00000d20: 616c 6964 220a 2020 2020 6e76 745f 7061  alid".    nvt_pa
+00000d30: 7468 5f65 7869 7374 7320 3d20 7472 6169  th_exists = trai
+00000d40: 6e5f 7061 7468 2e65 7869 7374 7328 2920  n_path.exists() 
+00000d50: 616e 6420 7661 6c69 645f 7061 7468 2e65  and valid_path.e
+00000d60: 7869 7374 7328 290a 2020 2020 6966 206e  xists().    if n
+00000d70: 6f74 206e 7674 5f70 6174 685f 6578 6973  ot nvt_path_exis
+00000d80: 7473 206f 7220 6f76 6572 7772 6974 653a  ts or overwrite:
+00000d90: 0a20 2020 2020 2020 2074 7261 6e73 666f  .        transfo
+00000da0: 726d 5f61 6c69 6363 7028 7261 775f 7061  rm_aliccp(raw_pa
+00000db0: 7468 2c20 6e76 745f 7061 7468 2c20 6e76  th, nvt_path, nv
+00000dc0: 745f 776f 726b 666c 6f77 3d6e 7674 5f77  t_workflow=nvt_w
+00000dd0: 6f72 6b66 6c6f 7729 0a0a 2020 2020 7472  orkflow)..    tr
+00000de0: 6169 6e20 3d20 6d65 726c 696e 2e69 6f2e  ain = merlin.io.
+00000df0: 4461 7461 7365 7428 7374 7228 7472 6169  Dataset(str(trai
+00000e00: 6e5f 7061 7468 292c 2065 6e67 696e 653d  n_path), engine=
+00000e10: 2270 6172 7175 6574 2229 0a20 2020 2076  "parquet").    v
+00000e20: 616c 6964 203d 206d 6572 6c69 6e2e 696f  alid = merlin.io
+00000e30: 2e44 6174 6173 6574 2873 7472 2876 616c  .Dataset(str(val
+00000e40: 6964 5f70 6174 6829 2c20 656e 6769 6e65  id_path), engine
+00000e50: 3d22 7061 7271 7565 7422 290a 0a20 2020  ="parquet")..   
+00000e60: 2072 6574 7572 6e20 7472 6169 6e2c 2076   return train, v
+00000e70: 616c 6964 0a0a 0a64 6566 2070 7265 7061  alid...def prepa
+00000e80: 7265 5f61 6c69 6363 7028 0a20 2020 2064  re_aliccp(.    d
+00000e90: 6174 615f 6469 723a 2055 6e69 6f6e 5b73  ata_dir: Union[s
+00000ea0: 7472 2c20 5061 7468 5d2c 0a20 2020 2063  tr, Path],.    c
+00000eb0: 6f6e 7665 7274 5f74 7261 696e 3a20 626f  onvert_train: bo
+00000ec0: 6f6c 203d 2054 7275 652c 0a20 2020 2063  ol = True,.    c
+00000ed0: 6f6e 7665 7274 5f74 6573 743a 2062 6f6f  onvert_test: boo
+00000ee0: 6c20 3d20 5472 7565 2c0a 2020 2020 6669  l = True,.    fi
+00000ef0: 6c65 5f73 697a 653a 2069 6e74 203d 2031  le_size: int = 1
+00000f00: 3030 3030 302c 0a20 2020 206d 6178 5f6e  00000,.    max_n
+00000f10: 756d 5f72 6f77 733a 204f 7074 696f 6e61  um_rows: Optiona
+00000f20: 6c5b 696e 745d 203d 204e 6f6e 652c 0a20  l[int] = None,. 
+00000f30: 2020 2070 6963 6b6c 655f 636f 6d6d 6f6e     pickle_common
+00000f40: 5f66 6561 7475 7265 733d 5472 7565 2c0a  _features=True,.
+00000f50: 2020 2020 6f75 7470 7574 5f64 6972 3a20      output_dir: 
+00000f60: 4f70 7469 6f6e 616c 5b55 6e69 6f6e 5b73  Optional[Union[s
+00000f70: 7472 2c20 5061 7468 5d5d 203d 204e 6f6e  tr, Path]] = Non
+00000f80: 652c 0a29 3a0a 2020 2020 2222 220a 2020  e,.):.    """.  
+00000f90: 2020 436f 6e76 6572 7420 416c 692d 4350    Convert Ali-CP
+00000fa0: 5020 6461 7461 2074 6f20 7061 7271 7565  P data to parque
+00000fb0: 7420 6669 6c65 732e 0a0a 2020 2020 546f  t files...    To
+00000fc0: 2064 6f77 6e6c 6f61 6420 7468 6520 7261   download the ra
+00000fd0: 7720 7468 6520 416c 692d 4343 5020 7472  w the Ali-CCP tr
+00000fe0: 6169 6e69 6e67 2061 6e64 2074 6573 7420  aining and test 
+00000ff0: 6461 7461 7365 7473 2076 6973 6974 0a20  datasets visit. 
+00001000: 2020 205b 7469 616e 6368 692e 616c 6979     [tianchi.aliy
+00001010: 756e 2e63 6f6d 5d28 6874 7470 733a 2f2f  un.com](https://
+00001020: 7469 616e 6368 692e 616c 6979 756e 2e63  tianchi.aliyun.c
+00001030: 6f6d 2f64 6174 6173 6574 2f64 6174 6144  om/dataset/dataD
+00001040: 6574 6169 6c3f 6461 7461 4964 3d34 3038  etail?dataId=408
+00001050: 2331 292e 0a0a 2020 2020 5061 7261 6d65  #1)...    Parame
+00001060: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
+00001070: 2d2d 2d0a 2020 2020 6461 7461 5f64 6972  ---.    data_dir
+00001080: 3a20 556e 696f 6e5b 7374 722c 2050 6174  : Union[str, Pat
+00001090: 685d 0a20 2020 2020 2020 2044 6972 6563  h].        Direc
+000010a0: 746f 7279 2074 6f20 6c6f 6164 2074 6865  tory to load the
+000010b0: 2072 6177 2064 6174 6120 6672 6f6d 2e0a   raw data from..
+000010c0: 2020 2020 636f 6e76 6572 745f 7472 6169      convert_trai
+000010d0: 6e3a 2062 6f6f 6c0a 2020 2020 2020 2020  n: bool.        
+000010e0: 5768 6574 6865 7220 746f 2063 6f6e 7665  Whether to conve
+000010f0: 7274 2074 6865 2074 7261 696e 696e 6720  rt the training 
+00001100: 6461 7461 2e0a 2020 2020 636f 6e76 6572  data..    conver
+00001110: 745f 7465 7374 3a20 626f 6f6c 0a20 2020  t_test: bool.   
+00001120: 2020 2020 2057 6865 7468 6572 2074 6f20       Whether to 
+00001130: 636f 6e76 6572 7420 7468 6520 7465 7374  convert the test
+00001140: 2064 6174 612e 0a20 2020 2066 696c 655f   data..    file_
+00001150: 7369 7a65 3a20 696e 740a 2020 2020 2020  size: int.      
+00001160: 2020 4e75 6d62 6572 206f 6620 726f 7773    Number of rows
+00001170: 2074 6f20 7772 6974 6520 746f 2065 6163   to write to eac
+00001180: 6820 7061 7271 7565 7420 6669 6c65 2e0a  h parquet file..
+00001190: 2020 2020 6d61 785f 6e75 6d5f 726f 7773      max_num_rows
+000011a0: 3a20 696e 742c 206f 7074 696f 6e61 6c0a  : int, optional.
+000011b0: 2020 2020 2020 2020 4d61 7869 6d75 6d20          Maximum 
+000011c0: 6e75 6d62 6572 206f 6620 726f 7773 2074  number of rows t
+000011d0: 6f20 7265 6164 2066 726f 6d20 7468 6520  o read from the 
+000011e0: 7261 7720 6461 7461 2e0a 2020 2020 7069  raw data..    pi
+000011f0: 636b 6c65 5f63 6f6d 6d6f 6e5f 6665 6174  ckle_common_feat
+00001200: 7572 6573 3a20 626f 6f6c 0a20 2020 2020  ures: bool.     
+00001210: 2020 2057 6865 7468 6572 2074 6f20 7069     Whether to pi
+00001220: 636b 6c65 2074 6865 2063 6f6d 6d6f 6e20  ckle the common 
+00001230: 6665 6174 7572 6573 2e0a 2020 2020 2020  features..      
+00001240: 2020 5768 656e 2065 6e61 626c 6564 2069    When enabled i
+00001250: 7420 7769 6c6c 206d 616b 6520 7468 6520  t will make the 
+00001260: 636f 6e76 6572 7369 6f6e 2066 6173 7465  conversion faste
+00001270: 7220 6966 2069 7420 776f 756c 6420 6265  r if it would be
+00001280: 2072 756e 2061 6761 696e 2e0a 2020 2020   run again..    
+00001290: 6f75 7470 7574 5f64 6972 3a20 556e 696f  output_dir: Unio
+000012a0: 6e5b 7374 722c 2050 6174 685d 2c20 6f70  n[str, Path], op
+000012b0: 7469 6f6e 616c 0a20 2020 2020 2020 2044  tional.        D
+000012c0: 6972 6563 746f 7279 2074 6f20 7772 6974  irectory to writ
+000012d0: 6520 7468 6520 636f 6e76 6572 7465 6420  e the converted 
+000012e0: 6461 7461 2074 6f2e 0a20 2020 2020 2020  data to..       
+000012f0: 2049 6620 6e6f 7420 7370 6563 6966 6965   If not specifie
+00001300: 6420 7468 6520 6461 7461 2077 696c 6c20  d the data will 
+00001310: 6265 2077 7269 7474 656e 2074 6f20 7468  be written to th
+00001320: 6520 7361 6d65 2064 6972 6563 746f 7279  e same directory
+00001330: 2061 7320 7468 6520 7261 7720 6461 7461   as the raw data
+00001340: 2e0a 0a20 2020 2052 6574 7572 6e73 0a20  ...    Returns. 
+00001350: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2064     -------.    d
+00001360: 6174 615f 6469 720a 2020 2020 2222 220a  ata_dir.    """.
+00001370: 0a20 2020 2069 6620 636f 6e76 6572 745f  .    if convert_
+00001380: 7472 6169 6e3a 0a20 2020 2020 2020 205f  train:.        _
+00001390: 636f 6e76 6572 745f 6461 7461 280a 2020  convert_data(.  
+000013a0: 2020 2020 2020 2020 2020 7374 7228 6461            str(da
+000013b0: 7461 5f64 6972 292c 0a20 2020 2020 2020  ta_dir),.       
+000013c0: 2020 2020 2066 696c 655f 7369 7a65 2c0a       file_size,.
+000013d0: 2020 2020 2020 2020 2020 2020 6973 5f74              is_t
+000013e0: 7261 696e 3d54 7275 652c 0a20 2020 2020  rain=True,.     
+000013f0: 2020 2020 2020 206d 6178 5f6e 756d 5f72         max_num_r
+00001400: 6f77 733d 6d61 785f 6e75 6d5f 726f 7773  ows=max_num_rows
+00001410: 2c0a 2020 2020 2020 2020 2020 2020 7069  ,.            pi
+00001420: 636b 6c65 5f63 6f6d 6d6f 6e5f 6665 6174  ckle_common_feat
+00001430: 7572 6573 3d70 6963 6b6c 655f 636f 6d6d  ures=pickle_comm
+00001440: 6f6e 5f66 6561 7475 7265 732c 0a20 2020  on_features,.   
+00001450: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+00001460: 6469 723d 6f75 7470 7574 5f64 6972 2c0a  dir=output_dir,.
+00001470: 2020 2020 2020 2020 290a 2020 2020 6966          ).    if
+00001480: 2063 6f6e 7665 7274 5f74 6573 743a 0a20   convert_test:. 
+00001490: 2020 2020 2020 205f 636f 6e76 6572 745f         _convert_
+000014a0: 6461 7461 280a 2020 2020 2020 2020 2020  data(.          
+000014b0: 2020 7374 7228 6461 7461 5f64 6972 292c    str(data_dir),
+000014c0: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+000014d0: 655f 7369 7a65 2c0a 2020 2020 2020 2020  e_size,.        
+000014e0: 2020 2020 6973 5f74 7261 696e 3d46 616c      is_train=Fal
+000014f0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+00001500: 6d61 785f 6e75 6d5f 726f 7773 3d6d 6178  max_num_rows=max
+00001510: 5f6e 756d 5f72 6f77 732c 0a20 2020 2020  _num_rows,.     
+00001520: 2020 2020 2020 2070 6963 6b6c 655f 636f         pickle_co
+00001530: 6d6d 6f6e 5f66 6561 7475 7265 733d 7069  mmon_features=pi
+00001540: 636b 6c65 5f63 6f6d 6d6f 6e5f 6665 6174  ckle_common_feat
+00001550: 7572 6573 2c0a 2020 2020 2020 2020 2020  ures,.          
+00001560: 2020 6f75 7470 7574 5f64 6972 3d6f 7574    output_dir=out
+00001570: 7075 745f 6469 722c 0a20 2020 2020 2020  put_dir,.       
+00001580: 2029 0a0a 2020 2020 7265 7475 726e 2064   )..    return d
+00001590: 6174 615f 6469 720a 0a0a 6465 6620 6465  ata_dir...def de
+000015a0: 6661 756c 745f 616c 6963 6370 5f74 7261  fault_aliccp_tra
+000015b0: 6e73 666f 726d 6174 696f 6e28 6164 645f  nsformation(add_
+000015c0: 7461 7267 6574 5f65 6e63 6f64 696e 673d  target_encoding=
+000015d0: 5472 7565 2c20 2a2a 6b77 6172 6773 293a  True, **kwargs):
+000015e0: 0a20 2020 2069 6d70 6f72 7420 6e76 7461  .    import nvta
+000015f0: 6275 6c61 7220 6173 206e 7674 0a20 2020  bular as nvt.   
+00001600: 2066 726f 6d20 6e76 7461 6275 6c61 7220   from nvtabular 
+00001610: 696d 706f 7274 206f 7073 2061 7320 6e76  import ops as nv
+00001620: 745f 6f70 730a 0a20 2020 2063 6174 203d  t_ops..    cat =
+00001630: 206c 616d 6264 613a 206e 7674 5f6f 7073   lambda: nvt_ops
+00001640: 2e43 6174 6567 6f72 6966 7928 6474 7970  .Categorify(dtyp
+00001650: 653d 2269 6e74 3332 2229 2020 2320 6e6f  e="int32")  # no
+00001660: 7161 3a20 4537 3331 0a0a 2020 2020 7573  qa: E731..    us
+00001670: 6572 5f69 6420 3d20 5b22 7573 6572 5f69  er_id = ["user_i
+00001680: 6422 5d20 3e3e 2063 6174 2829 203e 3e20  d"] >> cat() >> 
+00001690: 6e76 745f 6f70 732e 5461 6741 7355 7365  nvt_ops.TagAsUse
+000016a0: 7249 4428 290a 2020 2020 6974 656d 5f69  rID().    item_i
+000016b0: 6420 3d20 5b22 6974 656d 5f69 6422 5d20  d = ["item_id"] 
+000016c0: 3e3e 2063 6174 2829 203e 3e20 6e76 745f  >> cat() >> nvt_
+000016d0: 6f70 732e 5461 6741 7349 7465 6d49 4428  ops.TagAsItemID(
+000016e0: 290a 0a20 2020 2069 7465 6d5f 6665 6174  )..    item_feat
+000016f0: 7572 6573 203d 2028 0a20 2020 2020 2020  ures = (.       
+00001700: 205b 2269 7465 6d5f 6361 7465 676f 7279   ["item_category
+00001710: 222c 2022 6974 656d 5f73 686f 7022 2c20  ", "item_shop", 
+00001720: 2269 7465 6d5f 6272 616e 6422 2c20 2269  "item_brand", "i
+00001730: 7465 6d5f 696e 7465 6e74 696f 6e22 5d0a  tem_intention"].
+00001740: 2020 2020 2020 2020 3e3e 2063 6174 2829          >> cat()
+00001750: 0a20 2020 2020 2020 203e 3e20 6e76 745f  .        >> nvt_
+00001760: 6f70 732e 5461 6741 7349 7465 6d46 6561  ops.TagAsItemFea
+00001770: 7475 7265 7328 290a 2020 2020 290a 0a20  tures().    ).. 
+00001780: 2020 2075 7365 725f 6665 6174 7572 6573     user_features
+00001790: 203d 2028 0a20 2020 2020 2020 205b 0a20   = (.        [. 
+000017a0: 2020 2020 2020 2020 2020 2022 7573 6572             "user
+000017b0: 5f73 686f 7073 222c 0a20 2020 2020 2020  _shops",.       
+000017c0: 2020 2020 2022 7573 6572 5f70 726f 6669       "user_profi
+000017d0: 6c65 222c 0a20 2020 2020 2020 2020 2020  le",.           
+000017e0: 2022 7573 6572 5f67 726f 7570 222c 0a20   "user_group",. 
+000017f0: 2020 2020 2020 2020 2020 2022 7573 6572             "user
+00001800: 5f67 656e 6465 7222 2c0a 2020 2020 2020  _gender",.      
+00001810: 2020 2020 2020 2275 7365 725f 6167 6522        "user_age"
+00001820: 2c0a 2020 2020 2020 2020 2020 2020 2275  ,.            "u
+00001830: 7365 725f 636f 6e73 756d 7074 696f 6e5f  ser_consumption_
+00001840: 3122 2c0a 2020 2020 2020 2020 2020 2020  1",.            
+00001850: 2275 7365 725f 636f 6e73 756d 7074 696f  "user_consumptio
+00001860: 6e5f 3222 2c0a 2020 2020 2020 2020 2020  n_2",.          
+00001870: 2020 2275 7365 725f 6973 5f6f 6363 7570    "user_is_occup
+00001880: 6965 6422 2c0a 2020 2020 2020 2020 2020  ied",.          
+00001890: 2020 2275 7365 725f 6765 6f67 7261 7068    "user_geograph
+000018a0: 7922 2c0a 2020 2020 2020 2020 2020 2020  y",.            
+000018b0: 2275 7365 725f 696e 7465 6e74 696f 6e73  "user_intentions
+000018c0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000018d0: 7573 6572 5f62 7261 6e64 7322 2c0a 2020  user_brands",.  
+000018e0: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
+000018f0: 6361 7465 676f 7269 6573 222c 0a20 2020  categories",.   
+00001900: 2020 2020 205d 0a20 2020 2020 2020 203e       ].        >
+00001910: 3e20 6361 7428 290a 2020 2020 2020 2020  > cat().        
+00001920: 3e3e 206e 7674 5f6f 7073 2e54 6167 4173  >> nvt_ops.TagAs
+00001930: 5573 6572 4665 6174 7572 6573 2829 0a20  UserFeatures(). 
+00001940: 2020 2029 0a0a 2020 2020 7573 6572 5f69     )..    user_i
+00001950: 7465 6d5f 6665 6174 7572 6573 203d 2028  tem_features = (
+00001960: 0a20 2020 2020 2020 205b 0a20 2020 2020  .        [.     
+00001970: 2020 2020 2020 2022 7573 6572 5f69 7465         "user_ite
+00001980: 6d5f 6361 7465 676f 7269 6573 222c 0a20  m_categories",. 
+00001990: 2020 2020 2020 2020 2020 2022 7573 6572             "user
+000019a0: 5f69 7465 6d5f 7368 6f70 7322 2c0a 2020  _item_shops",.  
+000019b0: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
+000019c0: 6974 656d 5f62 7261 6e64 7322 2c0a 2020  item_brands",.  
+000019d0: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
+000019e0: 6974 656d 5f69 6e74 656e 7469 6f6e 7322  item_intentions"
+000019f0: 2c0a 2020 2020 2020 2020 5d0a 2020 2020  ,.        ].    
+00001a00: 2020 2020 3e3e 2063 6174 2829 0a20 2020      >> cat().   
+00001a10: 2020 2020 203e 3e20 6e76 745f 6f70 732e       >> nvt_ops.
+00001a20: 4164 644d 6574 6164 6174 6128 7461 6773  AddMetadata(tags
+00001a30: 3d5b 2275 7365 725f 6974 656d 225d 290a  =["user_item"]).
+00001a40: 2020 2020 290a 0a20 2020 2063 6f6e 7465      )..    conte
+00001a50: 7874 5f66 6561 7475 7265 7320 3d20 5b22  xt_features = ["
+00001a60: 706f 7369 7469 6f6e 225d 203e 3e20 6361  position"] >> ca
+00001a70: 7428 2920 3e3e 206e 7674 5f6f 7073 2e41  t() >> nvt_ops.A
+00001a80: 6464 4d65 7461 6461 7461 2874 6167 733d  ddMetadata(tags=
+00001a90: 5b54 6167 732e 434f 4e54 4558 545d 290a  [Tags.CONTEXT]).
+00001aa0: 0a20 2020 2074 6172 6765 7473 203d 205b  .    targets = [
+00001ab0: 2263 6c69 636b 222c 2022 636f 6e76 6572  "click", "conver
+00001ac0: 7369 6f6e 225d 203e 3e20 6e76 745f 6f70  sion"] >> nvt_op
+00001ad0: 732e 4164 644d 6574 6164 6174 6128 0a20  s.AddMetadata(. 
+00001ae0: 2020 2020 2020 2074 6167 733d 5b54 6167         tags=[Tag
+00001af0: 732e 4249 4e41 5259 5f43 4c41 5353 4946  s.BINARY_CLASSIF
+00001b00: 4943 4154 494f 4e2c 2022 7461 7267 6574  ICATION, "target
+00001b10: 225d 0a20 2020 2029 0a20 2020 206f 7574  "].    ).    out
+00001b20: 7075 7473 203d 2028 0a20 2020 2020 2020  puts = (.       
+00001b30: 2075 7365 725f 6964 0a20 2020 2020 2020   user_id.       
+00001b40: 202b 2069 7465 6d5f 6964 0a20 2020 2020   + item_id.     
+00001b50: 2020 202b 2069 7465 6d5f 6665 6174 7572     + item_featur
+00001b60: 6573 0a20 2020 2020 2020 202b 2075 7365  es.        + use
+00001b70: 725f 6665 6174 7572 6573 0a20 2020 2020  r_features.     
+00001b80: 2020 202b 2075 7365 725f 6974 656d 5f66     + user_item_f
+00001b90: 6561 7475 7265 730a 2020 2020 2020 2020  eatures.        
+00001ba0: 2b20 636f 6e74 6578 745f 6665 6174 7572  + context_featur
+00001bb0: 6573 0a20 2020 2020 2020 202b 2074 6172  es.        + tar
+00001bc0: 6765 7473 0a20 2020 2029 0a0a 2020 2020  gets.    )..    
+00001bd0: 6966 2061 6464 5f74 6172 6765 745f 656e  if add_target_en
+00001be0: 636f 6469 6e67 3a0a 2020 2020 2020 2020  coding:.        
+00001bf0: 636f 6e74 696e 756f 7573 203d 2028 0a20  continuous = (. 
+00001c00: 2020 2020 2020 2020 2020 205b 2275 7365             ["use
+00001c10: 725f 6964 222c 2022 6974 656d 5f69 6422  r_id", "item_id"
+00001c20: 5d0a 2020 2020 2020 2020 2020 2020 3e3e  ].            >>
+00001c30: 206e 7674 5f6f 7073 2e54 6172 6765 7445   nvt_ops.TargetE
+00001c40: 6e63 6f64 696e 6728 5b22 636c 6963 6b22  ncoding(["click"
+00001c50: 5d2c 206b 666f 6c64 3d31 2c20 705f 736d  ], kfold=1, p_sm
+00001c60: 6f6f 7468 3d32 3029 0a20 2020 2020 2020  ooth=20).       
+00001c70: 2020 2020 203e 3e20 6e76 745f 6f70 732e       >> nvt_ops.
+00001c80: 4e6f 726d 616c 697a 6528 290a 2020 2020  Normalize().    
+00001c90: 2020 2020 290a 2020 2020 2020 2020 6f75      ).        ou
+00001ca0: 7470 7574 7320 2b3d 2063 6f6e 7469 6e75  tputs += continu
+00001cb0: 6f75 730a 0a20 2020 2072 6574 7572 6e20  ous..    return 
+00001cc0: 6e76 742e 576f 726b 666c 6f77 286f 7574  nvt.Workflow(out
+00001cd0: 7075 7473 290a 0a0a 6465 6620 7472 616e  puts)...def tran
+00001ce0: 7366 6f72 6d5f 616c 6963 6370 280a 2020  sform_aliccp(.  
+00001cf0: 2020 6461 7461 3a20 556e 696f 6e5b 7374    data: Union[st
+00001d00: 722c 2050 6174 682c 2054 7570 6c65 5b6d  r, Path, Tuple[m
+00001d10: 6572 6c69 6e2e 696f 2e44 6174 6173 6574  erlin.io.Dataset
+00001d20: 2c20 6d65 726c 696e 2e69 6f2e 4461 7461  , merlin.io.Data
+00001d30: 7365 745d 5d2c 0a20 2020 206f 7574 7075  set]],.    outpu
+00001d40: 745f 7061 7468 3a20 556e 696f 6e5b 7374  t_path: Union[st
+00001d50: 722c 2050 6174 685d 2c0a 2020 2020 6e76  r, Path],.    nv
+00001d60: 745f 776f 726b 666c 6f77 3d4e 6f6e 652c  t_workflow=None,
+00001d70: 0a20 2020 202a 2a6b 7761 7267 732c 0a29  .    **kwargs,.)
+00001d80: 3a0a 2020 2020 6e76 745f 776f 726b 666c  :.    nvt_workfl
+00001d90: 6f77 203d 206e 7674 5f77 6f72 6b66 6c6f  ow = nvt_workflo
+00001da0: 7720 6f72 2064 6566 6175 6c74 5f61 6c69  w or default_ali
+00001db0: 6363 705f 7472 616e 7366 6f72 6d61 7469  ccp_transformati
+00001dc0: 6f6e 282a 2a6c 6f63 616c 7328 2929 0a0a  on(**locals())..
+00001dd0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
+00001de0: 6528 6461 7461 2c20 2873 7472 2c20 5061  e(data, (str, Pa
+00001df0: 7468 2929 3a0a 2020 2020 2020 2020 5f74  th)):.        _t
+00001e00: 7261 696e 203d 2067 6c6f 6228 7374 7228  rain = glob(str(
+00001e10: 6461 7461 202f 2022 7472 6169 6e2f 2a2e  data / "train/*.
+00001e20: 7061 7271 7565 7422 2929 0a20 2020 2020  parquet")).     
+00001e30: 2020 205f 7661 6c69 6420 3d20 676c 6f62     _valid = glob
+00001e40: 2873 7472 2864 6174 6120 2f20 2274 6573  (str(data / "tes
+00001e50: 742f 2a2e 7061 7271 7565 7422 2929 0a20  t/*.parquet")). 
+00001e60: 2020 2065 6c69 6620 280a 2020 2020 2020     elif (.      
+00001e70: 2020 6973 696e 7374 616e 6365 2864 6174    isinstance(dat
+00001e80: 612c 2074 7570 6c65 290a 2020 2020 2020  a, tuple).      
+00001e90: 2020 616e 6420 6c65 6e28 6461 7461 2920    and len(data) 
+00001ea0: 3d3d 2032 0a20 2020 2020 2020 2061 6e64  == 2.        and
+00001eb0: 2061 6c6c 2869 7369 6e73 7461 6e63 6528   all(isinstance(
+00001ec0: 782c 206d 6572 6c69 6e2e 696f 2e44 6174  x, merlin.io.Dat
+00001ed0: 6173 6574 2920 666f 7220 7820 696e 2064  aset) for x in d
+00001ee0: 6174 6129 0a20 2020 2029 3a0a 2020 2020  ata).    ):.    
+00001ef0: 2020 2020 5f74 7261 696e 2c20 5f76 616c      _train, _val
+00001f00: 6964 203d 2064 6174 610a 2020 2020 656c  id = data.    el
+00001f10: 7365 3a0a 2020 2020 2020 2020 7261 6973  se:.        rais
+00001f20: 6520 5661 6c75 6545 7272 6f72 2822 6461  e ValueError("da
+00001f30: 7461 206d 7573 7420 6265 2061 2070 6174  ta must be a pat
+00001f40: 6820 6f72 2061 2074 7570 6c65 206f 6620  h or a tuple of 
+00001f50: 7472 6169 6e20 616e 6420 7661 6c69 6420  train and valid 
+00001f60: 6461 7461 7365 7473 2229 0a0a 2020 2020  datasets")..    
+00001f70: 776f 726b 666c 6f77 5f66 6974 5f74 7261  workflow_fit_tra
+00001f80: 6e73 666f 726d 286e 7674 5f77 6f72 6b66  nsform(nvt_workf
+00001f90: 6c6f 772c 205f 7472 6169 6e2c 205f 7661  low, _train, _va
+00001fa0: 6c69 642c 2073 7472 286f 7574 7075 745f  lid, str(output_
+00001fb0: 7061 7468 292c 202a 2a6b 7761 7267 7329  path), **kwargs)
+00001fc0: 0a0a 0a40 6461 7461 636c 6173 730a 636c  ...@dataclass.cl
+00001fd0: 6173 7320 5f46 6561 7475 7265 3a0a 2020  ass _Feature:.  
+00001fe0: 2020 6e61 6d65 3a20 7374 720a 2020 2020    name: str.    
+00001ff0: 6964 3a20 7374 720a 2020 2020 7461 6773  id: str.    tags
+00002000: 3a20 4c69 7374 5b55 6e69 6f6e 5b73 7472  : List[Union[str
+00002010: 2c20 5461 6773 5d5d 0a20 2020 2064 6573  , Tags]].    des
+00002020: 6372 6970 7469 6f6e 3a20 7374 720a 0a0a  cription: str...
+00002030: 636c 6173 7320 5f46 6561 7475 7265 733a  class _Features:
+00002040: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00002050: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00002060: 2073 656c 662e 6665 6174 7572 6573 3a20   self.features: 
+00002070: 4c69 7374 5b5f 4665 6174 7572 655d 203d  List[_Feature] =
+00002080: 205b 0a20 2020 2020 2020 2020 2020 2023   [.            #
+00002090: 2055 7365 720a 2020 2020 2020 2020 2020   User.          
+000020a0: 2020 5f46 6561 7475 7265 2822 7573 6572    _Feature("user
+000020b0: 5f69 6422 2c20 2231 3031 222c 205b 5461  _id", "101", [Ta
+000020c0: 6773 2e55 5345 525f 4944 2c20 5461 6773  gs.USER_ID, Tags
+000020d0: 2e55 5345 525d 2c20 2255 7365 7220 4944  .USER], "User ID
+000020e0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+000020f0: 5f46 6561 7475 7265 280a 2020 2020 2020  _Feature(.      
+00002100: 2020 2020 2020 2020 2020 2275 7365 725f            "user_
+00002110: 6361 7465 676f 7269 6573 222c 0a20 2020  categories",.   
+00002120: 2020 2020 2020 2020 2020 2020 2022 3130               "10
+00002130: 395f 3134 222c 0a20 2020 2020 2020 2020  9_14",.         
+00002140: 2020 2020 2020 205b 5461 6773 2e55 5345         [Tags.USE
+00002150: 525d 2c0a 2020 2020 2020 2020 2020 2020  R],.            
+00002160: 2020 2020 2255 7365 7220 6869 7374 6f72      "User histor
+00002170: 6963 616c 2062 6568 6176 696f 7273 206f  ical behaviors o
+00002180: 6620 6361 7465 676f 7279 2049 4420 616e  f category ID an
+00002190: 6420 636f 756e 7422 2c0a 2020 2020 2020  d count",.      
+000021a0: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+000021b0: 2020 2020 205f 4665 6174 7572 6528 0a20       _Feature(. 
+000021c0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+000021d0: 7573 6572 5f73 686f 7073 222c 0a20 2020  user_shops",.   
+000021e0: 2020 2020 2020 2020 2020 2020 2022 3131               "11
+000021f0: 305f 3134 222c 0a20 2020 2020 2020 2020  0_14",.         
+00002200: 2020 2020 2020 205b 5461 6773 2e55 5345         [Tags.USE
+00002210: 525d 2c0a 2020 2020 2020 2020 2020 2020  R],.            
+00002220: 2020 2020 2255 7365 7220 6869 7374 6f72      "User histor
+00002230: 6963 616c 2062 6568 6176 696f 7273 206f  ical behaviors o
+00002240: 6620 7368 6f70 2049 4420 616e 6420 636f  f shop ID and co
+00002250: 756e 7422 2c0a 2020 2020 2020 2020 2020  unt",.          
+00002260: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00002270: 205f 4665 6174 7572 6528 0a20 2020 2020   _Feature(.     
+00002280: 2020 2020 2020 2020 2020 2022 7573 6572             "user
+00002290: 5f62 7261 6e64 7322 2c0a 2020 2020 2020  _brands",.      
+000022a0: 2020 2020 2020 2020 2020 2231 3237 5f31            "127_1
+000022b0: 3422 2c0a 2020 2020 2020 2020 2020 2020  4",.            
+000022c0: 2020 2020 5b54 6167 732e 5553 4552 5d2c      [Tags.USER],
+000022d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000022e0: 2022 5573 6572 2068 6973 746f 7269 6361   "User historica
+000022f0: 6c20 6265 6861 7669 6f72 7320 6f66 2062  l behaviors of b
+00002300: 7261 6e64 2049 4420 616e 6420 636f 756e  rand ID and coun
+00002310: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
+00002320: 292c 0a20 2020 2020 2020 2020 2020 205f  ),.            _
+00002330: 4665 6174 7572 6528 0a20 2020 2020 2020  Feature(.       
+00002340: 2020 2020 2020 2020 2022 7573 6572 5f69           "user_i
+00002350: 6e74 656e 7469 6f6e 7322 2c0a 2020 2020  ntentions",.    
+00002360: 2020 2020 2020 2020 2020 2020 2231 3530              "150
+00002370: 5f31 3422 2c0a 2020 2020 2020 2020 2020  _14",.          
+00002380: 2020 2020 2020 5b54 6167 732e 5553 4552        [Tags.USER
+00002390: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+000023a0: 2020 2022 5573 6572 2068 6973 746f 7269     "User histori
+000023b0: 6361 6c20 6265 6861 7669 6f72 7320 6f66  cal behaviors of
+000023c0: 2069 6e74 656e 7469 6f6e 206e 6f64 6520   intention node 
+000023d0: 4944 2061 6e64 2063 6f75 6e74 222c 0a20  ID and count",. 
+000023e0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+000023f0: 2020 2020 2020 2020 2020 5f46 6561 7475            _Featu
+00002400: 7265 2822 7573 6572 5f70 726f 6669 6c65  re("user_profile
+00002410: 222c 2022 3132 3122 2c20 5b54 6167 732e  ", "121", [Tags.
+00002420: 5553 4552 5d2c 2022 4361 7465 676f 7269  USER], "Categori
+00002430: 6361 6c20 4944 206f 6620 5573 6572 2050  cal ID of User P
+00002440: 726f 6669 6c65 2229 2c0a 2020 2020 2020  rofile"),.      
+00002450: 2020 2020 2020 5f46 6561 7475 7265 2822        _Feature("
+00002460: 7573 6572 5f67 726f 7570 222c 2022 3132  user_group", "12
+00002470: 3222 2c20 5b54 6167 732e 5553 4552 5d2c  2", [Tags.USER],
+00002480: 2022 4361 7465 676f 7269 6361 6c20 6772   "Categorical gr
+00002490: 6f75 7020 4944 206f 6620 5573 6572 2050  oup ID of User P
+000024a0: 726f 6669 6c65 2229 2c0a 2020 2020 2020  rofile"),.      
+000024b0: 2020 2020 2020 5f46 6561 7475 7265 2822        _Feature("
+000024c0: 7573 6572 5f67 656e 6465 7222 2c20 2231  user_gender", "1
+000024d0: 3234 222c 205b 5461 6773 2e55 5345 525d  24", [Tags.USER]
+000024e0: 2c20 2255 7365 7273 2047 656e 6465 7220  , "Users Gender 
+000024f0: 4944 2229 2c0a 2020 2020 2020 2020 2020  ID"),.          
+00002500: 2020 5f46 6561 7475 7265 2822 7573 6572    _Feature("user
+00002510: 5f61 6765 222c 2022 3132 3522 2c20 5b54  _age", "125", [T
+00002520: 6167 732e 5553 4552 5d2c 2022 5573 6572  ags.USER], "User
+00002530: 7320 4167 6520 4944 2229 2c0a 2020 2020  s Age ID"),.    
+00002540: 2020 2020 2020 2020 5f46 6561 7475 7265          _Feature
+00002550: 2822 7573 6572 5f63 6f6e 7375 6d70 7469  ("user_consumpti
+00002560: 6f6e 5f31 222c 2022 3132 3622 2c20 5b54  on_1", "126", [T
+00002570: 6167 732e 5553 4552 5d2c 2022 5573 6572  ags.USER], "User
+00002580: 7320 436f 6e73 756d 7074 696f 6e20 4c65  s Consumption Le
+00002590: 7665 6c20 5479 7065 2049 2229 2c0a 2020  vel Type I"),.  
+000025a0: 2020 2020 2020 2020 2020 5f46 6561 7475            _Featu
+000025b0: 7265 2822 7573 6572 5f63 6f6e 7375 6d70  re("user_consump
+000025c0: 7469 6f6e 5f32 222c 2022 3132 3722 2c20  tion_2", "127", 
+000025d0: 5b54 6167 732e 5553 4552 5d2c 2022 5573  [Tags.USER], "Us
+000025e0: 6572 7320 436f 6e73 756d 7074 696f 6e20  ers Consumption 
+000025f0: 4c65 7665 6c20 5479 7065 2049 4922 292c  Level Type II"),
+00002600: 0a20 2020 2020 2020 2020 2020 205f 4665  .            _Fe
+00002610: 6174 7572 6528 0a20 2020 2020 2020 2020  ature(.         
+00002620: 2020 2020 2020 2022 7573 6572 5f69 735f         "user_is_
+00002630: 6f63 6375 7069 6564 222c 2022 3132 3822  occupied", "128"
+00002640: 2c20 5b54 6167 732e 5553 4552 5d2c 2022  , [Tags.USER], "
+00002650: 5573 6572 7320 4f63 6375 7061 7469 6f6e  Users Occupation
+00002660: 3a20 7768 6574 6865 7220 6f72 206e 6f74  : whether or not
+00002670: 2074 6f20 776f 726b 220a 2020 2020 2020   to work".      
+00002680: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00002690: 2020 2020 205f 4665 6174 7572 6528 2275       _Feature("u
+000026a0: 7365 725f 6765 6f67 7261 7068 7922 2c20  ser_geography", 
+000026b0: 2231 3239 222c 205b 5461 6773 2e55 5345  "129", [Tags.USE
+000026c0: 525d 2c20 2255 7365 7273 2047 656f 6772  R], "Users Geogr
+000026d0: 6170 6879 2049 6e66 6f72 6d61 7469 6f6e  aphy Information
+000026e0: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+000026f0: 2320 4974 656d 0a20 2020 2020 2020 2020  # Item.         
+00002700: 2020 205f 4665 6174 7572 6528 2269 7465     _Feature("ite
+00002710: 6d5f 6964 222c 2022 3230 3522 2c20 5b54  m_id", "205", [T
+00002720: 6167 732e 4954 454d 2c20 5461 6773 2e49  ags.ITEM, Tags.I
+00002730: 5445 4d5f 4944 5d2c 2022 4974 656d 2049  TEM_ID], "Item I
+00002740: 4422 292c 0a20 2020 2020 2020 2020 2020  D"),.           
+00002750: 205f 4665 6174 7572 6528 0a20 2020 2020   _Feature(.     
+00002760: 2020 2020 2020 2020 2020 2022 6974 656d             "item
+00002770: 5f63 6174 6567 6f72 7922 2c20 2232 3036  _category", "206
+00002780: 222c 205b 5461 6773 2e49 5445 4d5d 2c20  ", [Tags.ITEM], 
+00002790: 2243 6174 6567 6f72 7920 4944 2074 6f20  "Category ID to 
+000027a0: 7768 6963 6820 7468 6520 6974 656d 2062  which the item b
+000027b0: 656c 6f6e 6773 2074 6f22 0a20 2020 2020  elongs to".     
+000027c0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+000027d0: 2020 2020 2020 5f46 6561 7475 7265 2822        _Feature("
+000027e0: 6974 656d 5f73 686f 7022 2c20 2232 3037  item_shop", "207
+000027f0: 222c 205b 5461 6773 2e49 5445 4d5d 2c20  ", [Tags.ITEM], 
+00002800: 2253 686f 7020 4944 2074 6f20 7768 6963  "Shop ID to whic
+00002810: 6820 6974 656d 2062 656c 6f6e 6773 2074  h item belongs t
+00002820: 6f22 292c 0a20 2020 2020 2020 2020 2020  o"),.           
+00002830: 205f 4665 6174 7572 6528 0a20 2020 2020   _Feature(.     
+00002840: 2020 2020 2020 2020 2020 2022 6974 656d             "item
+00002850: 5f69 6e74 656e 7469 6f6e 222c 2022 3231  _intention", "21
+00002860: 3022 2c20 5b54 6167 732e 4954 454d 5d2c  0", [Tags.ITEM],
+00002870: 2022 496e 7465 6e74 696f 6e20 6e6f 6465   "Intention node
+00002880: 2049 4420 7768 6963 6820 7468 6520 6974   ID which the it
+00002890: 656d 2062 656c 6f6e 6773 2074 6f22 0a20  em belongs to". 
+000028a0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+000028b0: 2020 2020 2020 2020 2020 5f46 6561 7475            _Featu
+000028c0: 7265 2822 6974 656d 5f62 7261 6e64 222c  re("item_brand",
+000028d0: 2022 3231 3622 2c20 5b54 6167 732e 4954   "216", [Tags.IT
+000028e0: 454d 5d2c 2022 4272 616e 6420 4944 206f  EM], "Brand ID o
+000028f0: 6620 7468 6520 6974 656d 2229 2c0a 2020  f the item"),.  
+00002900: 2020 2020 2020 2020 2020 2320 5573 6572            # User
+00002910: 2d49 7465 6d0a 2020 2020 2020 2020 2020  -Item.          
+00002920: 2020 5f46 6561 7475 7265 280a 2020 2020    _Feature(.    
+00002930: 2020 2020 2020 2020 2020 2020 2275 7365              "use
+00002940: 725f 6974 656d 5f63 6174 6567 6f72 6965  r_item_categorie
+00002950: 7322 2c0a 2020 2020 2020 2020 2020 2020  s",.            
+00002960: 2020 2020 2235 3038 222c 0a20 2020 2020      "508",.     
+00002970: 2020 2020 2020 2020 2020 205b 2275 7365             ["use
+00002980: 725f 6974 656d 225d 2c0a 2020 2020 2020  r_item"],.      
+00002990: 2020 2020 2020 2020 2020 2254 6865 2063            "The c
+000029a0: 6f6d 6269 6e61 7469 6f6e 206f 6620 6665  ombination of fe
+000029b0: 6174 7572 6573 2077 6974 6820 3130 395f  atures with 109_
+000029c0: 3134 2061 6e64 2032 3036 222c 0a20 2020  14 and 206",.   
+000029d0: 2020 2020 2020 2020 2029 2c0a 2020 2020           ),.    
+000029e0: 2020 2020 2020 2020 5f46 6561 7475 7265          _Feature
+000029f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00002a00: 2020 2275 7365 725f 6974 656d 5f73 686f    "user_item_sho
+00002a10: 7073 222c 0a20 2020 2020 2020 2020 2020  ps",.           
+00002a20: 2020 2020 2022 3530 3922 2c0a 2020 2020       "509",.    
+00002a30: 2020 2020 2020 2020 2020 2020 5b22 7573              ["us
+00002a40: 6572 5f69 7465 6d22 5d2c 0a20 2020 2020  er_item"],.     
+00002a50: 2020 2020 2020 2020 2020 2022 5468 6520             "The 
+00002a60: 636f 6d62 696e 6174 696f 6e20 6f66 2066  combination of f
+00002a70: 6561 7475 7265 7320 7769 7468 2031 3130  eatures with 110
+00002a80: 5f31 3420 616e 6420 3230 3722 2c0a 2020  _14 and 207",.  
+00002a90: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00002aa0: 2020 2020 2020 2020 205f 4665 6174 7572           _Featur
+00002ab0: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
+00002ac0: 2020 2022 7573 6572 5f69 7465 6d5f 6272     "user_item_br
+00002ad0: 616e 6473 222c 0a20 2020 2020 2020 2020  ands",.         
+00002ae0: 2020 2020 2020 2022 3730 3222 2c0a 2020         "702",.  
+00002af0: 2020 2020 2020 2020 2020 2020 2020 5b22                ["
+00002b00: 7573 6572 5f69 7465 6d22 5d2c 0a20 2020  user_item"],.   
+00002b10: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
+00002b20: 6520 636f 6d62 696e 6174 696f 6e20 6f66  e combination of
+00002b30: 2066 6561 7475 7265 7320 7769 7468 2031   features with 1
+00002b40: 3237 5f31 3420 616e 6420 3231 3622 2c0a  27_14 and 216",.
+00002b50: 2020 2020 2020 2020 2020 2020 292c 0a20              ),. 
+00002b60: 2020 2020 2020 2020 2020 205f 4665 6174             _Feat
+00002b70: 7572 6528 0a20 2020 2020 2020 2020 2020  ure(.           
+00002b80: 2020 2020 2022 7573 6572 5f69 7465 6d5f       "user_item_
+00002b90: 696e 7465 6e74 696f 6e73 222c 0a20 2020  intentions",.   
+00002ba0: 2020 2020 2020 2020 2020 2020 2022 3835               "85
+00002bb0: 3322 2c0a 2020 2020 2020 2020 2020 2020  3",.            
+00002bc0: 2020 2020 5b22 7573 6572 5f69 7465 6d22      ["user_item"
+00002bd0: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00002be0: 2020 2022 5468 6520 636f 6d62 696e 6174     "The combinat
+00002bf0: 696f 6e20 6f66 2066 6561 7475 7265 7320  ion of features 
+00002c00: 7769 7468 2031 3530 5f31 3420 616e 6420  with 150_14 and 
+00002c10: 3231 3022 2c0a 2020 2020 2020 2020 2020  210",.          
+00002c20: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+00002c30: 2023 2043 6f6e 7465 7874 0a20 2020 2020   # Context.     
+00002c40: 2020 2020 2020 205f 4665 6174 7572 6528         _Feature(
+00002c50: 2270 6f73 6974 696f 6e22 2c20 2233 3031  "position", "301
+00002c60: 222c 205b 5461 6773 2e43 4f4e 5445 5854  ", [Tags.CONTEXT
+00002c70: 5d2c 2022 4120 6361 7465 676f 7269 6361  ], "A categorica
+00002c80: 6c20 6578 7072 6573 7369 6f6e 206f 6620  l expression of 
+00002c90: 706f 7369 7469 6f6e 2229 2c0a 2020 2020  position"),.    
+00002ca0: 2020 2020 5d0a 0a20 2020 2040 7072 6f70      ]..    @prop
+00002cb0: 6572 7479 0a20 2020 2064 6566 2062 795f  erty.    def by_
+00002cc0: 6964 2873 656c 6629 3a0a 2020 2020 2020  id(self):.      
+00002cd0: 2020 7265 7475 726e 207b 6665 6174 7572    return {featur
+00002ce0: 652e 6964 3a20 6665 6174 7572 652e 6e61  e.id: feature.na
+00002cf0: 6d65 2066 6f72 2066 6561 7475 7265 2069  me for feature i
+00002d00: 6e20 7365 6c66 2e66 6561 7475 7265 737d  n self.features}
+00002d10: 0a0a 0a64 6566 205f 636f 6e76 6572 745f  ...def _convert_
+00002d20: 636f 6d6d 6f6e 5f66 6561 7475 7265 7328  common_features(
+00002d30: 636f 6d6d 6f6e 5f70 6174 682c 2070 6963  common_path, pic
+00002d40: 6b6c 655f 7061 7468 3d4e 6f6e 6529 3a0a  kle_path=None):.
+00002d50: 2020 2020 636f 6d6d 6f6e 203d 207b 7d0a      common = {}.
+00002d60: 0a20 2020 2077 6974 6820 6f70 656e 2863  .    with open(c
+00002d70: 6f6d 6d6f 6e5f 7061 7468 2c20 2272 2229  ommon_path, "r")
+00002d80: 2061 7320 636f 6d6d 6f6e 5f66 6561 7475   as common_featu
+00002d90: 7265 733a 0a20 2020 2020 2020 2066 6f72  res:.        for
+00002da0: 2063 7376 5f6c 696e 6520 696e 2074 7164   csv_line in tqd
+00002db0: 6d28 636f 6d6d 6f6e 5f66 6561 7475 7265  m(common_feature
+00002dc0: 732c 2064 6573 633d 2252 6561 6469 6e67  s, desc="Reading
+00002dd0: 2063 6f6d 6d6f 6e20 6665 6174 7572 6573   common features
+00002de0: 2e2e 2e22 293a 0a20 2020 2020 2020 2020  ..."):.         
+00002df0: 2020 206c 696e 6520 3d20 6373 765f 6c69     line = csv_li
+00002e00: 6e65 2e73 7472 6970 2829 2e73 706c 6974  ne.strip().split
+00002e10: 2822 2c22 290a 2020 2020 2020 2020 2020  (",").          
+00002e20: 2020 6b76 203d 206e 702e 6172 7261 7928    kv = np.array(
+00002e30: 7265 2e73 706c 6974 2822 5b01 0203 5d22  re.split("[...]"
+00002e40: 2c20 6c69 6e65 5b32 5d29 290a 2020 2020  , line[2])).    
+00002e50: 2020 2020 2020 2020 6b65 7973 203d 206b          keys = k
+00002e60: 765b 7261 6e67 6528 302c 206c 656e 286b  v[range(0, len(k
+00002e70: 7629 2c20 3329 5d0a 2020 2020 2020 2020  v), 3)].        
+00002e80: 2020 2020 7661 6c75 6573 203d 206b 765b      values = kv[
+00002e90: 7261 6e67 6528 312c 206c 656e 286b 7629  range(1, len(kv)
+00002ea0: 2c20 3329 5d0a 2020 2020 2020 2020 2020  , 3)].          
+00002eb0: 2020 636f 6d6d 6f6e 5b6c 696e 655b 305d    common[line[0]
+00002ec0: 5d20 3d20 6469 6374 287a 6970 286b 6579  ] = dict(zip(key
+00002ed0: 732c 2076 616c 7565 7329 290a 0a20 2020  s, values))..   
+00002ee0: 2020 2020 2069 6620 7069 636b 6c65 5f70       if pickle_p
+00002ef0: 6174 683a 0a20 2020 2020 2020 2020 2020  ath:.           
+00002f00: 2077 6974 6820 6f70 656e 2870 6963 6b6c   with open(pickl
+00002f10: 655f 7061 7468 2c20 2277 6222 2920 6173  e_path, "wb") as
+00002f20: 2068 616e 646c 653a 0a20 2020 2020 2020   handle:.       
+00002f30: 2020 2020 2020 2020 2070 6963 6b6c 652e           pickle.
+00002f40: 6475 6d70 2863 6f6d 6d6f 6e2c 2068 616e  dump(common, han
+00002f50: 646c 652c 2070 726f 746f 636f 6c3d 7069  dle, protocol=pi
+00002f60: 636b 6c65 2e48 4947 4845 5354 5f50 524f  ckle.HIGHEST_PRO
+00002f70: 544f 434f 4c29 0a0a 2020 2020 7265 7475  TOCOL)..    retu
+00002f80: 726e 2063 6f6d 6d6f 6e0a 0a0a 2320 544f  rn common...# TO
+00002f90: 444f 3a20 4f70 7469 6d69 7a65 2074 6869  DO: Optimize thi
+00002fa0: 7320 6675 6e63 7469 6f6e 2c20 7269 6768  s function, righ
+00002fb0: 7420 6e6f 7720 6974 2773 2074 6f6f 2073  t now it's too s
+00002fc0: 6c6f 772e 0a64 6566 205f 636f 6e76 6572  low..def _conver
+00002fd0: 745f 6461 7461 280a 2020 2020 6461 7461  t_data(.    data
+00002fe0: 5f64 6972 2c0a 2020 2020 6669 6c65 5f73  _dir,.    file_s
+00002ff0: 697a 652c 0a20 2020 2069 735f 7472 6169  ize,.    is_trai
+00003000: 6e3d 5472 7565 2c0a 2020 2020 7069 636b  n=True,.    pick
+00003010: 6c65 5f63 6f6d 6d6f 6e5f 6665 6174 7572  le_common_featur
+00003020: 6573 3d54 7275 652c 0a20 2020 206d 6178  es=True,.    max
+00003030: 5f6e 756d 5f72 6f77 733d 4e6f 6e65 2c0a  _num_rows=None,.
+00003040: 2020 2020 6f75 7470 7574 5f64 6972 3d4e      output_dir=N
+00003050: 6f6e 652c 0a29 3a0a 2020 2020 6461 7461  one,.):.    data
+00003060: 5f74 7970 6520 3d20 2274 7261 696e 2220  _type = "train" 
+00003070: 6966 2069 735f 7472 6169 6e20 656c 7365  if is_train else
+00003080: 2022 7465 7374 220a 2020 2020 6f75 7470   "test".    outp
+00003090: 7574 5f64 6972 203d 206f 7574 7075 745f  ut_dir = output_
+000030a0: 6469 7220 6f72 2064 6174 615f 6469 720a  dir or data_dir.
+000030b0: 0a20 2020 2063 6f6d 6d6f 6e5f 7061 7468  .    common_path
+000030c0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+000030d0: 6461 7461 5f64 6972 2c20 6461 7461 5f74  data_dir, data_t
+000030e0: 7970 652c 2066 2263 6f6d 6d6f 6e5f 6665  ype, f"common_fe
+000030f0: 6174 7572 6573 5f7b 6461 7461 5f74 7970  atures_{data_typ
+00003100: 657d 2e63 7376 2229 0a20 2020 2070 6174  e}.csv").    pat
+00003110: 6820 3d20 6f73 2e70 6174 682e 6a6f 696e  h = os.path.join
+00003120: 2864 6174 615f 6469 722c 2064 6174 615f  (data_dir, data_
+00003130: 7479 7065 2c20 6622 7361 6d70 6c65 5f73  type, f"sample_s
+00003140: 6b65 6c65 746f 6e5f 7b64 6174 615f 7479  keleton_{data_ty
+00003150: 7065 7d2e 6373 7622 290a 2020 2020 636f  pe}.csv").    co
+00003160: 6d6d 6f6e 5f66 6561 7475 7265 735f 7061  mmon_features_pa
+00003170: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
+00003180: 6e28 6461 7461 5f64 6972 2c20 6461 7461  n(data_dir, data
+00003190: 5f74 7970 652c 2022 636f 6d6d 6f6e 5f66  _type, "common_f
+000031a0: 6561 7475 7265 732e 7069 636b 6c65 2229  eatures.pickle")
+000031b0: 0a0a 2020 2020 636f 6d6d 6f6e 203d 207b  ..    common = {
+000031c0: 7d0a 2020 2020 6966 2070 6963 6b6c 655f  }.    if pickle_
+000031d0: 636f 6d6d 6f6e 5f66 6561 7475 7265 733a  common_features:
+000031e0: 0a20 2020 2020 2020 2069 6620 6f73 2e70  .        if os.p
+000031f0: 6174 682e 6578 6973 7473 2863 6f6d 6d6f  ath.exists(commo
+00003200: 6e5f 6665 6174 7572 6573 5f70 6174 6829  n_features_path)
+00003210: 3a0a 2020 2020 2020 2020 2020 2020 7769  :.            wi
+00003220: 7468 206f 7065 6e28 636f 6d6d 6f6e 5f66  th open(common_f
+00003230: 6561 7475 7265 735f 7061 7468 2c20 2272  eatures_path, "r
+00003240: 6222 2920 6173 2066 3a0a 2020 2020 2020  b") as f:.      
+00003250: 2020 2020 2020 2020 2020 636f 6d6d 6f6e            common
+00003260: 203d 2070 6963 6b6c 652e 6c6f 6164 2866   = pickle.load(f
+00003270: 290a 0a20 2020 2069 6620 6e6f 7420 636f  )..    if not co
+00003280: 6d6d 6f6e 3a0a 2020 2020 2020 2020 7069  mmon:.        pi
+00003290: 636b 6c65 5f70 6174 6820 3d20 636f 6d6d  ckle_path = comm
+000032a0: 6f6e 5f66 6561 7475 7265 735f 7061 7468  on_features_path
+000032b0: 2069 6620 7069 636b 6c65 5f63 6f6d 6d6f   if pickle_commo
+000032c0: 6e5f 6665 6174 7572 6573 2065 6c73 6520  n_features else 
+000032d0: 4e6f 6e65 0a20 2020 2020 2020 2063 6f6d  None.        com
+000032e0: 6d6f 6e20 3d20 5f63 6f6e 7665 7274 5f63  mon = _convert_c
+000032f0: 6f6d 6d6f 6e5f 6665 6174 7572 6573 2863  ommon_features(c
+00003300: 6f6d 6d6f 6e5f 7061 7468 2c20 7069 636b  ommon_path, pick
+00003310: 6c65 5f70 6174 6829 0a0a 2020 2020 6375  le_path)..    cu
+00003320: 7272 656e 7420 3d20 5b5d 0a20 2020 2062  rrent = [].    b
+00003330: 795f 6964 203d 205f 4665 6174 7572 6573  y_id = _Features
+00003340: 2829 2e62 795f 6964 0a0a 2020 2020 6f75  ().by_id..    ou
+00003350: 745f 6469 7220 3d20 6f73 2e70 6174 682e  t_dir = os.path.
+00003360: 6a6f 696e 2873 7472 286f 7574 7075 745f  join(str(output_
+00003370: 6469 7229 2c20 6461 7461 5f74 7970 6529  dir), data_type)
+00003380: 0a20 2020 2074 6d70 5f64 6972 203d 206f  .    tmp_dir = o
+00003390: 732e 7061 7468 2e6a 6f69 6e28 6f75 745f  s.path.join(out_
+000033a0: 6469 722c 2022 746d 7022 290a 2020 2020  dir, "tmp").    
+000033b0: 6966 206e 6f74 206f 732e 7061 7468 2e65  if not os.path.e
+000033c0: 7869 7374 7328 746d 705f 6469 7229 3a0a  xists(tmp_dir):.
+000033d0: 2020 2020 2020 2020 6f73 2e6d 616b 6564          os.maked
+000033e0: 6972 7328 746d 705f 6469 7229 0a0a 2020  irs(tmp_dir)..  
+000033f0: 2020 7769 7468 206f 7065 6e28 7061 7468    with open(path
+00003400: 2c20 2272 2229 2061 7320 736b 656c 6574  , "r") as skelet
+00003410: 6f6e 3a0a 2020 2020 2020 2020 666f 7220  on:.        for 
+00003420: 692c 2063 7376 5f6c 696e 6520 696e 2074  i, csv_line in t
+00003430: 7164 6d28 656e 756d 6572 6174 6528 736b  qdm(enumerate(sk
+00003440: 656c 6574 6f6e 292c 2064 6573 633d 2250  eleton), desc="P
+00003450: 726f 6365 7373 696e 6720 6461 7461 2e2e  rocessing data..
+00003460: 2e22 293a 0a20 2020 2020 2020 2020 2020  ."):.           
+00003470: 2069 6620 6d61 785f 6e75 6d5f 726f 7773   if max_num_rows
+00003480: 2061 6e64 2069 203e 3d20 6d61 785f 6e75   and i >= max_nu
+00003490: 6d5f 726f 7773 3a0a 2020 2020 2020 2020  m_rows:.        
+000034a0: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
+000034b0: 2020 2020 2020 2020 2020 206c 696e 6520             line 
+000034c0: 3d20 6373 765f 6c69 6e65 2e73 7472 6970  = csv_line.strip
+000034d0: 2829 2e73 706c 6974 2822 2c22 290a 2020  ().split(",").  
+000034e0: 2020 2020 2020 2020 2020 6966 206c 696e            if lin
+000034f0: 655b 315d 203d 3d20 2230 2220 616e 6420  e[1] == "0" and 
+00003500: 6c69 6e65 5b32 5d20 3d3d 2022 3122 3a0a  line[2] == "1":.
+00003510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003520: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
+00003530: 2020 2020 206b 7620 3d20 6e70 2e61 7272       kv = np.arr
+00003540: 6179 2872 652e 7370 6c69 7428 225b 0102  ay(re.split("[..
+00003550: 035d 222c 206c 696e 655b 355d 2929 0a20  .]", line[5])). 
+00003560: 2020 2020 2020 2020 2020 206b 6579 203d             key =
+00003570: 206b 765b 7261 6e67 6528 302c 206c 656e   kv[range(0, len
+00003580: 286b 7629 2c20 3329 5d0a 2020 2020 2020  (kv), 3)].      
+00003590: 2020 2020 2020 7661 6c75 6520 3d20 6b76        value = kv
+000035a0: 5b72 616e 6765 2831 2c20 6c65 6e28 6b76  [range(1, len(kv
+000035b0: 292c 2033 295d 0a20 2020 2020 2020 2020  ), 3)].         
+000035c0: 2020 2066 6561 745f 6469 6374 203d 2064     feat_dict = d
+000035d0: 6963 7428 7a69 7028 6b65 792c 2076 616c  ict(zip(key, val
+000035e0: 7565 2929 0a20 2020 2020 2020 2020 2020  ue)).           
+000035f0: 2066 6561 745f 6469 6374 2e75 7064 6174   feat_dict.updat
+00003600: 6528 636f 6d6d 6f6e 5b6c 696e 655b 335d  e(common[line[3]
+00003610: 5d29 0a20 2020 2020 2020 2020 2020 2066  ]).            f
+00003620: 6561 745f 6469 6374 5b22 636c 6963 6b22  eat_dict["click"
+00003630: 5d20 3d20 696e 7428 6c69 6e65 5b31 5d29  ] = int(line[1])
+00003640: 0a20 2020 2020 2020 2020 2020 2066 6561  .            fea
+00003650: 745f 6469 6374 5b22 636f 6e76 6572 7369  t_dict["conversi
+00003660: 6f6e 225d 203d 2069 6e74 286c 696e 655b  on"] = int(line[
+00003670: 325d 290a 0a20 2020 2020 2020 2020 2020  2])..           
+00003680: 2063 7572 7265 6e74 2e61 7070 656e 6428   current.append(
+00003690: 6665 6174 5f64 6963 7429 0a0a 2020 2020  feat_dict)..    
+000036a0: 2020 2020 2020 2020 6966 2069 203e 2030          if i > 0
+000036b0: 2061 6e64 2069 2025 2066 696c 655f 7369   and i % file_si
+000036c0: 7a65 203d 3d20 303a 0a20 2020 2020 2020  ze == 0:.       
+000036d0: 2020 2020 2020 2020 2064 6620 3d20 6765           df = ge
+000036e0: 745f 6c69 6228 292e 4461 7461 4672 616d  t_lib().DataFram
+000036f0: 6528 6375 7272 656e 7429 0a20 2020 2020  e(current).     
+00003700: 2020 2020 2020 2020 2020 2063 6f6c 7320             cols 
+00003710: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00003720: 2020 2020 2066 6f72 2063 6f6c 2069 6e20       for col in 
+00003730: 6c69 7374 2864 662e 636f 6c75 6d6e 7329  list(df.columns)
+00003740: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00003750: 2020 2020 2020 6966 2063 6f6c 203d 3d20        if col == 
+00003760: 2263 6c69 636b 2220 6f72 2063 6f6c 203d  "click" or col =
+00003770: 3d20 2263 6f6e 7665 7273 696f 6e22 3a0a  = "conversion":.
+00003780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003790: 2020 2020 2020 2020 636f 6c73 2e61 7070          cols.app
+000037a0: 656e 6428 636f 6c29 0a20 2020 2020 2020  end(col).       
+000037b0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+000037c0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+000037d0: 2020 2020 2020 2020 2020 2063 6f6c 732e             cols.
+000037e0: 6170 7065 6e64 2862 795f 6964 5b63 6f6c  append(by_id[col
+000037f0: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
+00003800: 2020 2020 6466 2e63 6f6c 756d 6e73 203d      df.columns =
+00003810: 2063 6f6c 730a 2020 2020 2020 2020 2020   cols.          
+00003820: 2020 2020 2020 696e 6465 7820 3d20 696e        index = in
+00003830: 7428 2869 202f 2066 696c 655f 7369 7a65  t((i / file_size
+00003840: 2920 2d20 3129 0a20 2020 2020 2020 2020  ) - 1).         
+00003850: 2020 2020 2020 2064 662e 746f 5f70 6172         df.to_par
+00003860: 7175 6574 280a 2020 2020 2020 2020 2020  quet(.          
+00003870: 2020 2020 2020 2020 2020 6f73 2e70 6174            os.pat
+00003880: 682e 6a6f 696e 2874 6d70 5f64 6972 2c20  h.join(tmp_dir, 
+00003890: 6622 7b64 6174 615f 7479 7065 7d5f 7b69  f"{data_type}_{i
+000038a0: 6e64 6578 7d2e 7061 7271 7565 7422 292c  ndex}.parquet"),
+000038b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000038c0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
+000038d0: 2020 2063 7572 7265 6e74 203d 205b 5d0a     current = [].
+000038e0: 0a20 2020 2074 6d70 5f66 696c 6573 203d  .    tmp_files =
+000038f0: 2067 6c6f 6228 6f73 2e70 6174 682e 6a6f   glob(os.path.jo
+00003900: 696e 2874 6d70 5f64 6972 2c20 6622 7b64  in(tmp_dir, f"{d
+00003910: 6174 615f 7479 7065 7d5f 2a2e 7061 7271  ata_type}_*.parq
+00003920: 7565 7422 2929 0a20 2020 2064 7479 7065  uet")).    dtype
+00003930: 7320 3d20 7b66 2e6e 616d 653a 2022 696e  s = {f.name: "in
+00003940: 7433 3222 2066 6f72 2066 2069 6e20 5f46  t32" for f in _F
+00003950: 6561 7475 7265 7328 292e 6665 6174 7572  eatures().featur
+00003960: 6573 7d0a 2020 2020 6d65 726c 696e 2e69  es}.    merlin.i
+00003970: 6f2e 4461 7461 7365 7428 746d 705f 6669  o.Dataset(tmp_fi
+00003980: 6c65 732c 2064 7479 7065 733d 6474 7970  les, dtypes=dtyp
+00003990: 6573 292e 746f 5f70 6172 7175 6574 286f  es).to_parquet(o
+000039a0: 7574 5f64 6972 290a 2020 2020 7368 7574  ut_dir).    shut
+000039b0: 696c 2e72 6d74 7265 6528 746d 705f 6469  il.rmtree(tmp_di
+000039c0: 7229 0a                                  r).
```

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/raw/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/raw/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/transformed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/ecommerce/aliccp/transformed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/booking/dataset.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/booking/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 
 def default_booking_transformation(**kwargs):
     """Default transformation for the booking dataset.
 
     Returns:
         Workflow: NVTabular workflow
     """
-    cat = lambda: nvt.ops.Categorify(start_index=1)  # noqa: E731
+    cat = lambda: nvt.ops.Categorify()  # noqa: E731
 
     df_season = get_lib().DataFrame(
         {"month": range(1, 13), "season": ([0] * 3) + ([1] * 3) + ([2] * 3) + ([3] * 3)}
     )
 
     month = (
         ["checkin"]
```

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/ecommerce/booking/raw/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/ecommerce/booking/transformed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/dataset.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         from merlin.datasets.synthetic import generate_data
         train, valid = generate_data("dressipi2022-preprocessed")
 
     Parameters
     ----------
     path: Union[str, Path]
         Directory to load the raw data from.
+
     Returns
     -------
     train: merlin.io.Dataset
         Training dataset.
     valid: merlin.io.Dataset
         Test dataset.
     """
```

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/preprocessed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/ecommerce/dressipi/preprocessed/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/large/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/large/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/large/schema.json` & `merlin-models-23.6.0/merlin/datasets/ecommerce/large/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/small/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/small/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/small/schema.json` & `merlin-models-23.6.0/merlin/datasets/ecommerce/small/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/__init__.py` & `merlin-models-23.6.0/merlin/datasets/ecommerce/transactions/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/ecommerce/transactions/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/ecommerce/transactions/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/__init__.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/__init__.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/100k/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/100k/schema.json` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/100k/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/__init__.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m-raw/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/1m-raw/ratings/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/__init__.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/25m/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/25m/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/movielens/dataset.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/movielens/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/__init__.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/music_streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/music_streaming/schema.json` & `merlin-models-23.6.0/merlin/datasets/entertainment/music_streaming/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/__init__.py` & `merlin-models-23.6.0/merlin/datasets/entertainment/tenrec_video/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt` & `merlin-models-23.6.0/merlin/datasets/entertainment/tenrec_video/schema.pbtxt`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/social/__init__.py` & `merlin-models-23.6.0/merlin/datasets/social/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/social/schema.json` & `merlin-models-23.6.0/merlin/datasets/social/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/synthetic.py` & `merlin-models-23.6.0/merlin/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/testing/__init__.py` & `merlin-models-23.6.0/merlin/datasets/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/testing/schema.json` & `merlin-models-23.6.0/merlin/datasets/testing/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/__init__.py` & `merlin-models-23.6.0/merlin/datasets/testing/sequence_testing/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/datasets/testing/sequence_testing/schema.json` & `merlin-models-23.6.0/merlin/datasets/testing/sequence_testing/schema.json`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/__init__.py` & `merlin-models-23.6.0/merlin/models/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/api.py` & `merlin-models-23.6.0/merlin/models/api.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/config/__init__.py` & `merlin-models-23.6.0/merlin/models/config/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/config/schema.py` & `merlin-models-23.6.0/merlin/models/config/schema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/implicit/__init__.py` & `merlin-models-23.6.0/merlin/models/implicit/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/io.py` & `merlin-models-23.6.0/merlin/models/io.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/lightfm/__init__.py` & `merlin-models-23.6.0/merlin/models/lightfm/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/loader/__init__.py` & `merlin-models-23.6.0/merlin/models/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/loader/backend.py` & `merlin-models-23.6.0/merlin/models/loader/backend.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,15 @@
 )
 from merlin.models.tf.prediction_tasks.multi import PredictionTasks
 from merlin.models.tf.prediction_tasks.regression import RegressionTask
 from merlin.models.tf.prediction_tasks.retrieval import ItemRetrievalTask
 from merlin.models.utils.dependencies import is_transformers_available
 
 if is_transformers_available():
+    import transformers
     from merlin.models.tf.transformers.block import (
         AlbertBlock,
         BertBlock,
         GPT2Block,
         RobertaBlock,
         TransformerBlock,
         XLNetBlock,
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/cross.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/cross.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/dlrm.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/dlrm.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,60 +30,63 @@
 
 
 def DLRMBlock(
     schema: Schema,
     *,
     embedding_dim: int = None,
     embedding_options: EmbeddingOptions = None,
+    embeddings: Optional[Block] = None,
     bottom_block: Optional[Block] = None,
     top_block: Optional[Block] = None,
-    embeddings: Optional[Block] = None,
 ) -> SequentialBlock:
     """Builds the DLRM architecture, as proposed in the following
-    `paper https://arxiv.org/pdf/1906.00091.pdf`_ [1]_.
+     `paper https://arxiv.org/pdf/1906.00091.pdf`_ [1]_.
 
-    References
-    ----------
-    .. [1] Naumov, Maxim, et al. "Deep learning recommendation model for
-       personalization and recommendation systems." arXiv preprint arXiv:1906.00091 (2019).
-
-    Parameters
-    ----------
-    schema : Schema
-        The `Schema` with the input features
-    bottom_block : Block
-        The `Block` that combines the continuous features (typically a `MLPBlock`)
-    top_block : Optional[Block], optional
-        The optional `Block` that combines the outputs of bottom layer and of
-        the factorization machine layer, by default None
-    embedding_dim : Optional[int], optional
-        Dimension of the embeddings, by default None
-    embedding_options : EmbeddingOptions
-        Options for the input embeddings.
-        - embedding_dim_default: int - Default dimension of the embedding
-        table, when the feature is not found in ``embedding_dims``, by default 64
-        - infer_embedding_sizes : bool, Automatically defines the embedding
-        dimension from the feature cardinality in the schema, by default False,
-        which needs to be kept False for the DLRM architecture.
-
-    Returns
-    -------
-    SequentialBlock
-        The DLRM block
-
-    Raises
-    ------
-    ValueError
-        The schema is required by DLRM
-    ValueError
-        The bottom_block is required by DLRM
-    ValueError
-        The embedding_dim (X) needs to match the last layer of bottom MLP (Y).
-    ValueError
-        Only one-of `embeddings` or `embedding_options` can be used.
+     References
+     ----------
+     .. [1] Naumov, Maxim, et al. "Deep learning recommendation model for
+        personalization and recommendation systems." arXiv preprint arXiv:1906.00091 (2019).
+
+     Parameters
+     ----------
+     schema : Schema
+         The `Schema` with the input features
+     embedding_dim : Optional[int], optional
+         Dimension of the embeddings, by default None
+     embedding_options : EmbeddingOptions
+         Options for the input embeddings.
+         - embedding_dim_default: int - Default dimension of the embedding
+         table, when the feature is not found in ``embedding_dims``, by default 64
+         - infer_embedding_sizes : bool, Automatically defines the embedding
+         dimension from the feature cardinality in the schema, by default False,
+         which needs to be kept False for the DLRM architecture.
+    embeddings: Optional[Block]
+         If provided creates a ParallelBlock with an EmbeddingTable for each
+         categorical feature in the schema.
+     bottom_block : Block
+         The `Block` that combines the continuous features (typically a `MLPBlock`)
+     top_block : Optional[Block], optional
+         The optional `Block` that combines the outputs of bottom layer and of
+         the factorization machine layer, by default None
+
+     Returns
+     -------
+     SequentialBlock
+         The DLRM block
+
+     Raises
+     ------
+     ValueError
+         The schema is required by DLRM
+     ValueError
+         The bottom_block is required by DLRM
+     ValueError
+         The embedding_dim (X) needs to match the last layer of bottom MLP (Y).
+     ValueError
+         Only one-of `embeddings` or `embedding_options` can be used.
     """
     if schema is None:
         raise ValueError("The schema is required by DLRM")
 
     con_schema = schema.select_by_tag(Tags.CONTINUOUS).excluding_by_tag(Tags.TARGET)
     cat_schema = schema.select_by_tag(Tags.CATEGORICAL).excluding_by_tag(Tags.TARGET)
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/experts.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/experts.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/interaction.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/interaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,26 @@
         # square_sum part
         squared_sum = tf.reduce_sum(tf.square(inputs), 1)
 
         # second order
         return 0.5 * tf.subtract(summed_square, squared_sum)
 
     def compute_output_shape(self, input_shapes):
+        """Computes the output shape based on the input shapes
+
+        Parameters
+        ----------
+        input_shapes : tf.TensorShape
+            The input shapes
+
+        Returns
+        -------
+        tf.TensorShape
+            The output shape
+        """
         if len(input_shapes) != 3:
             raise ValueError("Found shape {} without 3 dimensions".format(input_shapes))
         return (input_shapes[0], input_shapes[2])
 
 
 def FMBlock(
     schema: Schema,
@@ -277,14 +289,15 @@
     wide_logit_block: Optional[Block], by default None
         The output layer of the wide input. The last dimension needs to be 1.
         You might want to provide your own output logit block if you want to add
         dropout or kernel regularization to the wide block.
     factors_dim : Optional[int], optional
         If fm_input_block is not provided, the factors_dim is used to define the
         embeddings dim to instantiate InputBlockV2, by default None
+
     Returns
     -------
     tf.Tensor
         Returns a 2D tensor (batch size, 1) with the sum of the wide component
         and 2nd-order interaction component of FM
     """
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/mlp.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/mlp.py`

 * *Files 7% similar despite different names*

```diff
@@ -220,14 +220,45 @@
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
         pre_aggregation="concat",
         dense=None,
         **kwargs,
     ):
+        """A Dense layer that aggregates features before projection
+        Parameters
+        ----------
+        units : _type_
+            _description_
+        activation : Optional[Union[str,tf.keras.layers.Layer]], optional
+            The activation function to use. By default None
+        use_bias : bool, optional
+            Whether to use a bias in the MLP, by default True
+        kernel_initializer: InitializerType
+            Initializer for the kernel weights matrix. Defaults to "glorot_uniform".
+        bias_initializer: InitializerType
+            Initializer for the bias vector. Default to "zeros".
+        kernel_regularizer: Optional[RegularizerType]
+            Regularizer function applied to the kernel weights matrix. Default to None.
+        bias_regularizer: Optional[RegularizerType]
+            Regularizer function applied to the bias vector.  Default to None.
+        activity_regularizer : optional
+            Regularizer function applied to the output of the layer (its "activation"),
+            by default None
+        kernel_constraint : optional
+            Constraint function applied to the kernel weights matrix, by default None
+        bias_constraint : optional
+            Constraint function applied to the bias vector, by default None
+        pre_aggregation : str, optional
+            If provided, aggregates inputs before the dense projection, by default "concat"
+        dense : _type_, optional
+            A tf.keras.layers.Layer that can be used to project the inputs.
+            Typically used when deserializing the layer. By default None
+        """
+
         super(_Dense, self).__init__(**kwargs)
         self.dense = dense or tf.keras.layers.Dense(
             units,
             activation,
             use_bias,
             kernel_initializer,
             bias_initializer,
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/optimizer.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/optimizer.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/base.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/retrieval/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,22 +131,23 @@
 
 @Block.registry.register_with_multiple_names("item_retrieval_scorer")
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class ItemRetrievalScorer(Block):
     """Block for ItemRetrieval, which expects query/user and item embeddings as input and
     uses dot product to score the positive item (inputs["item"]) and also sampled negative
     items (during training).
+
     Parameters
     ----------
-    samplers : List[ItemSampler], optional
+    samplers: List[ItemSampler], optional
         List of item samplers that provide negative samples when `training=True`
-    sampling_downscore_false_negatives : bool, optional
+    sampling_downscore_false_negatives: bool, optional
         Identify false negatives (sampled item ids equal to the positive item and downscore them
         to the `sampling_downscore_false_negatives_value`), by default True
-    sampling_downscore_false_negatives_value : int, optional
+    sampling_downscore_false_negatives_value: int, optional
         Value to be used to downscore false negatives when
         `sampling_downscore_false_negatives=True`, by default `np.finfo(np.float32).min / 100.0`
     item_id_feature_name: str
         Name of the column containing the item ids
         Defaults to `item_id`
     query_name: str
         Identify query tower for query/user embeddings, by default 'query'
@@ -170,14 +171,15 @@
         query_name: str = "query",
         item_name: str = "item",
         cache_query: bool = False,
         sampled_softmax_mode: bool = False,
         store_negative_ids: bool = False,
         **kwargs,
     ):
+        """Initializes the `ItemRetrievalScorer` class."""
         super().__init__(**kwargs)
 
         self.downscore_false_negatives = sampling_downscore_false_negatives
         self.false_negatives_score = sampling_downscore_false_negatives_value
         self.item_id_feature_name = item_id_feature_name
         self.item_domain = item_domain
         self.query_name = query_name
@@ -189,27 +191,41 @@
             samplers = (samplers,)  # type: ignore
         self.samplers = samplers
         self.sampled_softmax_mode = sampled_softmax_mode
 
         self.set_required_features()
 
     def build(self, input_shapes):
+        """Builds the block.
+
+        Parameters
+        ----------
+        input_shapes: tuple or dict
+            Shape of the input tensor.
+        """
         if isinstance(input_shapes, dict):
             query_shape = input_shapes[self.query_name]
             self.context.add_weight(
                 name="query",
                 shape=query_shape,
                 dtype=tf.float32,
                 trainable=False,
                 initializer=tf.keras.initializers.Zeros(),
             )
 
         super().build(input_shapes)
 
     def _check_input_from_two_tower(self, inputs):
+        """Checks if the inputs from the two towers (query and item) are correctly provided.
+
+        Parameters
+        ----------
+        inputs: dict
+            Dictionary of inputs.
+        """
         if set(inputs.keys()) != set([self.query_name, self.item_name]):
             raise ValueError(
                 f"Wrong input-names, expected: {[self.query_name, self.item_name]} "
                 f"but got: {inputs.keys()}"
             )
 
     def call(
@@ -219,21 +235,23 @@
         testing: bool = False,
         **kwargs,
     ) -> Union[tf.Tensor, TabularData]:
         """Based on the user/query embedding (inputs[self.query_name]), uses dot product to score
             the positive item (inputs["item"]).
             For the sampled-softmax mode, logits are computed by multiplying the query vector
             and the item embeddings matrix (self.context.get_embedding(self.item_domain))
+
         Parameters
         ----------
         inputs : Union[tf.Tensor, TabularData]
             Dict with the query and item embeddings (e.g. `{"query": <emb>}, "item": <emb>}`),
             where embeddings are 2D tensors (batch size, embedding size)
         training : bool, optional
             Flag that indicates whether in training mode, by default True
+
         Returns
         -------
         tf.Tensor
             2D Tensor with the scores for the positive items,
             If `training=True`, return the original inputs
         """
         if self.cache_query:
@@ -269,21 +287,23 @@
         features: Dict[str, tf.Tensor] = None,
         training=True,
         testing=False,
         **kwargs,
     ) -> "PredictionOutput":
         """Based on the user/query embedding (inputs[self.query_name]), uses dot product to score
             the positive item and also sampled negative items (during training).
+
         Parameters
         ----------
         inputs : TabularData
             Dict with the query and item embeddings (e.g. `{"query": <emb>}, "item": <emb>}`),
             where embeddings are 2D tensors (batch size, embedding size)
         training : bool, optional
             Flag that indicates whether in training mode, by default True
+
         Returns
         -------
         [tf.Tensor,tf.Tensor]
             all_scores: 2D Tensor with the scores for the positive items and, if `training=True`,
             for the negative sampled items too.
             Return tensor is 2D (batch size, 1 + #negatives)
         """
@@ -427,25 +447,33 @@
             )
         embedding_table = self.context.get_embedding(self.item_domain)
         batch_items_embeddings = embedding_ops.embedding_lookup(embedding_table, targets)
         predictions = {self.query_name: predictions, self.item_name: batch_items_embeddings}
         return predictions
 
     def set_required_features(self):
+        """Sets the required features for the samplers."""
         required_features = set()
         if self.downscore_false_negatives:
             required_features.add(self.item_id_feature_name)
 
         required_features.update(
             [feature for sampler in self.samplers for feature in sampler.required_features]
         )
 
         self._required_features = list(required_features)
 
     def get_config(self):
+        """Returns the configuration of the model as a dictionary.
+
+        Returns
+        -------
+        dict
+            The configuration of the model.
+        """
         config = super().get_config()
         config = maybe_serialize_keras_objects(self, config, ["samplers"])
         config["sampling_downscore_false_negatives"] = self.downscore_false_negatives
         config["sampling_downscore_false_negatives_value"] = self.false_negatives_score
         config["item_id_feature_name"] = self.item_id_feature_name
         config["item_domain"] = self.item_domain
         config["query_name"] = self.query_name
@@ -454,10 +482,21 @@
         config["sampled_softmax_mode"] = self.sampled_softmax_mode
         config["store_negative_ids"] = self.store_negative_ids
 
         return config
 
     @classmethod
     def from_config(cls, config):
+        """Creates a new instance of the class from its config.
+
+        Parameters
+        ----------
+        config: dict
+            A dictionary, typically the output of get_config.
+
+        Returns
+        -------
+        A new instance of the `ItemRetrievalScorer` class.
+        """
         config = maybe_deserialize_keras_objects(config, ["samplers"])
 
         return super().from_config(config)
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/retrieval/matrix_factorization.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/retrieval/two_tower.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/retrieval/two_tower.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/sampling/base.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/sampling/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/sampling/cross_batch.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/sampling/cross_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/sampling/in_batch.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/sampling/in_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/blocks/sampling/queue.py` & `merlin-models-23.6.0/merlin/models/tf/blocks/sampling/queue.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/core/aggregation.py` & `merlin-models-23.6.0/merlin/models/tf/core/aggregation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/core/base.py` & `merlin-models-23.6.0/merlin/models/tf/core/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/core/combinators.py` & `merlin-models-23.6.0/merlin/models/tf/core/combinators.py`

 * *Files 2% similar despite different names*

```diff
@@ -698,14 +698,19 @@
         output.__class__ = cls
 
         return output
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class ResidualBlock(WithShortcut):
+    """
+    Creates a shortcut connection where the residuals are
+    summed to the output of the block
+    """
+
     def __init__(
         self,
         block: Union[tf.keras.layers.Layer, Block],
         activation=None,
         post: Optional[BlockType] = None,
         schema: Optional[Schema] = None,
         name: Optional[str] = None,
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/core/encoder.py` & `merlin-models-23.6.0/merlin/models/tf/core/encoder.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2021, NVIDIA CORPORATION.
+# Copyright (c) 2023, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -84,14 +84,30 @@
     def encode(
         self,
         dataset: merlin.io.Dataset,
         index: Union[str, ColumnSchema, Schema, Tags],
         batch_size: int,
         **kwargs,
     ) -> merlin.io.Dataset:
+        """Encodes the given dataset and index.
+
+        Parameters
+        ----------
+        dataset: merlin.io.Dataset
+            The dataset to encode.
+        index: Union[str, ColumnSchema, Schema, Tags]
+            The index to use for encoding.
+        batch_size: int
+            The batch size for encoding.
+
+        Returns
+        -------
+        merlin.io.Dataset
+            The encoded dataset.
+        """
         if isinstance(index, Schema):
             output_schema = index
         elif isinstance(index, ColumnSchema):
             output_schema = Schema([index])
         elif isinstance(index, str):
             output_schema = Schema([self.schema[index]])
         elif isinstance(index, Tags):
@@ -113,20 +129,22 @@
         dataset: merlin.io.Dataset,
         batch_size: int,
         output_schema: Optional[Schema] = None,
         index: Optional[Union[str, ColumnSchema, Schema, Tags]] = None,
         **kwargs,
     ) -> merlin.io.Dataset:
         """Batched prediction using Dask.
+
         Parameters
         ----------
         dataset: merlin.io.Dataset
             Dataset to predict on.
         batch_size: int
             Batch size to use for prediction.
+
         Returns
         -------
         merlin.io.Dataset
         """
 
         if index:
             if isinstance(index, ColumnSchema):
@@ -162,56 +180,113 @@
         predictions = dataset.map_partitions(model_encode, **encode_kwargs)
         if index:
             predictions = predictions.set_index(index)
 
         return merlin.io.Dataset(predictions)
 
     def call(self, inputs, *, targets=None, training=False, testing=False, **kwargs):
+        """Calls the model on new inputs and returns the outputs as tensors.
+
+        Parameters
+        ----------
+        inputs : tensor-like or dict/tuple of tensors.
+            Tensors or dict/tuple of tensors representing the input batch.
+        targets : tensor-like, optional
+            Tensors representing the target data.
+        training : bool, optional
+            Whether the model is in training mode.
+        testing : bool, optional
+            Whether the model is in testing mode.
+
+        Returns
+        -------
+        A tensor or dict of tensors corresponding to the result of calling the layer.
+        """
         inputs = self._prepare_features(inputs, targets=targets)
         if isinstance(inputs, tuple):
             inputs, targets = inputs
         return combinators.call_sequentially(
             list(self.to_call),
             inputs=inputs,
             features=inputs,
             targets=targets,
             training=training,
             testing=testing,
             **kwargs,
         )
 
     def __call__(self, inputs, **kwargs):
+        """Overrides the default __call__ method to remove "features" from inputs.
+
+        Parameters
+        ----------
+        inputs : tensor-like or dict/tuple of tensors.
+            Tensors or dict/tuple of tensors representing the input batch.
+
+        Returns
+        -------
+        A tensor or dict of tensors corresponding to the result of calling the layer.
+        """
         # We remove features here since we don't expect them at inference time
         # Inside the `call` method, we will add them back by assuming inputs=features
         if "features" in kwargs:
             kwargs.pop("features")
 
         return super().__call__(inputs, **kwargs)
 
     def build(self, input_shape):
+        """Creates the variables of the layer.
+
+        Parameters
+        ----------
+        input_shape: Tuple[int]
+            The shape of the input data.
+        """
         self._prepare_features.build(input_shape)
         input_shape = self._prepare_features.compute_output_shape(input_shape)
 
         combinators.build_sequentially(self, list(self.to_call), input_shape=input_shape)
         if not hasattr(self.build, "_is_default"):
             self._build_input_shape = input_shape
 
     def compute_output_shape(self, input_shape):
+        """Computes the output shape of the layer.
+
+        Parameters
+        ----------
+        input_shape: Tuple[int]
+            The shape of the input data.
+
+        Returns
+        -------
+        Tuple[int]
+            The output shape of the layer.
+        """
         input_shape = self._prepare_features.compute_output_shape(input_shape)
         return combinators.compute_output_shape_sequentially(list(self.to_call), input_shape)
 
     def train_step(self, data):
-        """Train step"""
+        """Performs a training step.
+
+        Train step method is not implemented and Raises an error as the
+        Encoder block is not meant to be trained by itself and can only be
+        trained as part of a model.
+        """
         raise NotImplementedError(
             "This block is not meant to be trained by itself. ",
             "It can only be trained as part of a model.",
         )
 
     def fit(self, *args, **kwargs):
-        """Fit model"""
+        """Fits the model.
+
+        Fit method is not implemented and Raises an error as the Encoder block
+        is not meant to be trained by itself and can only be trained as part
+        of a model.
+        """
         raise NotImplementedError(
             "This block is not meant to be trained by itself. ",
             "It can only be trained as part of a model.",
         )
 
     def save(
         self,
@@ -241,41 +316,60 @@
         )
         input_schema = self.schema
         output_schema = get_output_schema(export_path)
         save_merlin_metadata(export_path, input_schema, output_schema)
 
     @property
     def to_call(self):
+        """Provides the list of blocks to be called during the execution of the model."""
         if self.pre:
             yield self.pre
 
         for block in self.blocks:
             yield block
 
         if self.post:
             yield self.post
 
     @property
     def has_schema(self) -> bool:
+        """Returns True as this class does contain a schema."""
         return True
 
     @property
     def schema(self) -> Schema:
+        """Returns the schema of the model."""
         return self._schema
 
     @property
     def first(self):
+        """Returns the first block of the model."""
         return self.blocks[0]
 
     @property
     def last(self):
+        """Returns the last block of the model."""
         return self.blocks[-1]
 
     @classmethod
     def from_config(cls, config, custom_objects=None):
+        """Creates a new instance of the class by deserializing.
+
+        Parameters
+        ----------
+        config: dict
+            A dictionary, typically the output of get_config.
+        custom_objects: dict, optional
+            A dictionary mapping the names of layers to the corresponding
+            functions and classes.
+
+        Returns
+        -------
+        A new instance of Encoder.
+        """
         pre = config.pop("pre", None)
         post = config.pop("post", None)
         layers = [
             tf.keras.layers.deserialize(conf, custom_objects=custom_objects)
             for conf in config.values()
         ]
 
@@ -287,14 +381,21 @@
 
         output = Encoder(*layers, pre=pre, post=post)
         output.__class__ = cls
 
         return output
 
     def get_config(self):
+        """Returns the configuration of the model as a dictionary.
+
+        Returns
+        -------
+        dict
+            The configuration of the model.
+        """
         config = tf_utils.maybe_serialize_keras_objects(self, {}, ["pre", "post"])
         for i, layer in enumerate(self.blocks):
             config[i] = tf.keras.utils.serialize_keras_object(layer)
 
         return config
 
 
@@ -522,31 +623,99 @@
             "This block is not meant to be trained by itself. ",
             "It can only be trained as part of a model.",
         )
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class EmbeddingEncoder(Encoder):
+    """Creates an Encoder from an EmbeddingTable.
+    Typically used with RetrievalModelV2.
+
+    Parameters
+    ----------
+    schema : Union[ColumnSchema, Schema]
+        The ColumnSchema of the column for which the
+        embedding table needs to be created.
+        If a Schema is passed, only the first column
+        is considered
+    dim : int
+        Dimension of the embeddings
+    embeddings_initializer : Union[str, tf.keras.layers.Layer], optional
+        Initializer for the `embeddings`
+        matrix (see `keras.initializers`). By default "uniform"
+    embeddings_regularizer : Union[str, tf.keras.layers.Layer], optional
+        Regularizer function applied to
+        the `embeddings` matrix (see `keras.regularizers`)., by default None
+    activity_regularizer : Union[str, tf.keras.layers.Layer], optional
+        Sets a layer that applies an update to the cost function based
+        input activity, by default None
+    embeddings_constraint : Union[str, tf.keras.layers.Layer], optional
+        Constraint function applied to
+        the `embeddings` matrix (see `keras.constraints`), by default None
+    mask_zero : bool, optional
+        Whether or not the input value 0 is a special "padding"
+        value that should be masked out.
+        This is useful when using recurrent layers
+        which may take variable length input.
+        If this is `True`, then all subsequent layers
+        in the model need to support masking or an exception will be raised.
+        If mask_zero is set to True, as a consequence, index 0 cannot be
+        used in the vocabulary (input_dim should equal size of
+        vocabulary + 1), by default False
+    input_length : int, optional
+        This argument is required if you are going to connect
+        `Flatten` then `Dense` layers upstream
+        (without it, the shape of the dense outputs cannot be computed),
+        by default None
+    sequence_combiner : Optional[CombinerType], optional
+        A string specifying how to combine embedding results for each
+        entry ("mean", "sqrtn" and "sum" are supported) or a layer.
+        Default is None (no combiner used), by default None
+    trainable : bool, optional
+        Whether the layer's variables should be trainable, by default True
+    name : str, optional
+        String name of the layer, by default None
+    dtype : optional
+        The dtype of the layer's computations and weights. Can also be a
+        `tf.keras.mixed_precision.Policy`, which allows the computation and weight
+        dtype to differ. Default of `None` means to use
+        `tf.keras.mixed_precision.global_policy()`, which is a float32 policy
+        unless set to different value., by default None
+    dynamic : bool, optional
+        Set this to `True` if your layer should only be run eagerly, and
+        should not be used to generate a static computation graph.
+        This would be the case for a Tree-RNN or a recursive network,
+        for example, or generally for any layer that manipulates tensors
+        using Python control flow. If `False`, we assume that the layer can
+        safely be used to generate a static computation graph., by default False
+    embeddings_l2_batch_regularization : Optional[Union[float, Dict[str, float]]], optional
+        Factor for L2 regularization of the embeddings vectors (from the current batch only)
+        by default 0.0, by default 0.0
+    post : Optional[tf.keras.layers.Layer], optional
+        _description_, by default None
+    **kwargs: Forwarded Encoder parameters
+    """
+
     def __init__(
         self,
         schema: Union[ColumnSchema, Schema],
         dim: int,
-        embeddings_initializer="uniform",
-        embeddings_regularizer=None,
-        activity_regularizer=None,
-        embeddings_constraint=None,
-        mask_zero=False,
-        input_length=None,
+        embeddings_initializer: Optional[Union[str, tf.keras.layers.Layer]] = "uniform",
+        embeddings_regularizer: Optional[Union[str, tf.keras.layers.Layer]] = None,
+        activity_regularizer: Optional[Union[str, tf.keras.layers.Layer]] = None,
+        embeddings_constraint: Optional[Union[str, tf.keras.layers.Layer]] = None,
+        mask_zero: bool = False,
+        input_length: int = None,
         sequence_combiner: Optional[CombinerType] = None,
-        trainable=True,
-        name=None,
+        trainable: bool = True,
+        name: str = None,
         dtype=None,
-        dynamic=False,
-        post: Optional[tf.keras.layers.Layer] = None,
+        dynamic: bool = False,
         embeddings_l2_batch_regularization: Optional[Union[float, Dict[str, float]]] = 0.0,
+        post: Optional[tf.keras.layers.Layer] = None,
         **kwargs,
     ):
         if isinstance(schema, ColumnSchema):
             col = schema
         else:
             col = schema.first
         col_name = col.name
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/core/index.py` & `merlin-models-23.6.0/merlin/models/tf/core/index.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/core/prediction.py` & `merlin-models-23.6.0/merlin/models/tf/core/prediction.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/core/tabular.py` & `merlin-models-23.6.0/merlin/models/tf/core/tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/distributed/backend.py` & `merlin-models-23.6.0/merlin/models/tf/distributed/backend.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/distributed/embedding.py` & `merlin-models-23.6.0/merlin/models/tf/distributed/embedding.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/experimental/sample_weight.py` & `merlin-models-23.6.0/merlin/models/tf/experimental/sample_weight.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/inputs/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/inputs/base.py` & `merlin-models-23.6.0/merlin/models/tf/inputs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 def InputBlock(
     schema: Schema,
     branches: Optional[Dict[str, Block]] = None,
     pre: Optional[BlockType] = None,
     post: Optional[BlockType] = None,
     aggregation: Optional[TabularAggregationType] = None,
     seq: bool = False,
-    max_seq_length: Optional[int] = None,
     add_continuous_branch: bool = True,
     continuous_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CONTINUOUS,),
     continuous_projection: Optional[Block] = None,
     add_embedding_branch: bool = True,
     embedding_options: EmbeddingOptions = EmbeddingOptions(),
     categorical_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.CATEGORICAL,),
     sequential_tags: Optional[Union[TagsType, Tuple[Tags]]] = (Tags.SEQUENCE,),
@@ -67,18 +66,21 @@
 
         mlp = ml.InputBlock(schema).connect(ml.MLPBlock([64, 32]))
 
     Parameters:
     ----------
     schema: Schema
         Schema of the input data. This Schema object will be automatically generated using
-        [NVTabular](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html).
+        [NVTabular](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html).
         Next to this, it's also possible to construct it manually.
     branches: Dict[str, Block], optional
         Dictionary of branches to use inside the InputBlock.
+    pre: Optional[BlockType]
+        Transformations to apply on the inputs before the module is
+        called (before 'forward'). Default is None.
     post: Optional[BlockType]
         Transformations to apply on the inputs after the module is
         called (so **after** `forward`).
         Defaults to None
     aggregation: Optional[TabularAggregationType]
         Aggregation to apply after processing the  `forward`-method to output a single Tensor.
         Defaults to None
@@ -256,15 +258,15 @@
         )
 
 
     Parameters
     ----------
     schema : Schema
         Schema of the input data. This Schema object will be automatically generated using
-        [NVTabular](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html).
+        [NVTabular](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html).
         Next to this, it's also possible to construct it manually.
     categorical : Union[Tags, Layer], defaults to `Tags.CATEGORICAL`
         A block or column-selector to use for categorical-features.
         If a column-selector is provided (either a schema or tags), the selector
         will be passed to `Embeddings()` to infer the embedding tables from the column-selector.
     continuous : Union[Tags, Layer], defaults to `Tags.CONTINUOUS`
         A block to use for continuous-features.
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/inputs/embedding.py` & `merlin-models-23.6.0/merlin/models/tf/inputs/embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -152,58 +152,54 @@
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class EmbeddingTable(EmbeddingTableBase):
     """Embedding table that is backed by a standard Keras Embedding Layer.
     It accepts as input features for lookup tf.Tensor, tf.RaggedTensor,
     and tf.SparseTensor which might be 2D (batch_size, 1) for scalars
     or 3d (batch_size, seq_length, 1) for sequential features
 
-     Parameters
-     ----------
-     dim: Dimension of the dense embedding.
-     col_schema: ColumnSchema
-         Schema of the column. This is used to infer the cardinality.
-     embeddings_initializer: Initializer for the `embeddings`
-       matrix (see `keras.initializers`).
-     embeddings_regularizer: Regularizer function applied to
-       the `embeddings` matrix (see `keras.regularizers`).
-     embeddings_constraint: Constraint function applied to
-       the `embeddings` matrix (see `keras.constraints`).
-     mask_zero: Boolean, whether or not the input value 0 is a special "padding"
-       value that should be masked out.
-       This is useful when using recurrent layers
-       which may take variable length input.
-       If this is `True`, then all subsequent layers
-       in the model need to support masking or an exception will be raised.
-       If mask_zero is set to True, as a consequence, index 0 cannot be
-       used in the vocabulary (input_dim should equal size of
-       vocabulary + 1).
-     input_length: Length of input sequences, when it is constant.
-       This argument is required if you are going to connect
-       `Flatten` then `Dense` layers upstream
-       (without it, the shape of the dense outputs cannot be computed).
-    combiner: A string specifying how to combine embedding results for each
-       entry ("mean", "sqrtn" and "sum" are supported) or a layer.
-       Default is None (no combiner used)
-    trainable: Boolean, whether the layer's variables should be trainable.
-    name: String name of the layer.
-    dtype: The dtype of the layer's computations and weights. Can also be a
-       `tf.keras.mixed_precision.Policy`, which allows the computation and weight
-       dtype to differ. Default of `None` means to use
-       `tf.keras.mixed_precision.global_policy()`, which is a float32 policy
-       unless set to different value.
-    dynamic: Set this to `True` if your layer should only be run eagerly, and
-       should not be used to generate a static computation graph.
-       This would be the case for a Tree-RNN or a recursive network,
-       for example, or generally for any layer that manipulates tensors
-       using Python control flow. If `False`, we assume that the layer can
-       safely be used to generate a static computation graph.
-    l2_batch_regularization_factor: float, optional
-        Factor for L2 regularization of the embeddings vectors (from the current batch only)
-        by default 0.0
-    **kwargs: Forwarded Keras Layer parameters
+    Parameters
+    ----------
+    dim : int
+        The dimension of the dense embedding.
+    col_schemas : ColumnSchema
+        The schema of the column(s) used to infer the cardinality.
+    embeddings_initializer : str, optional
+        The initializer for the `embeddings` matrix (see `keras.initializers`),
+        by default "uniform".
+    embeddings_regularizer : str, optional
+        The regularizer function applied to the `embeddings` matrix (see `keras.regularizers`),
+        by default None.
+    embeddings_constraint : str, optional
+        The constraint function applied to the `embeddings` matrix (see `keras.constraints`),
+        by default None.
+    mask_zero : bool, optional
+        Whether or not the input value 0 is a special "padding" value that should be masked out.
+        This is useful when using recurrent layers which may take variable length input,
+        by default False.
+    input_length : int, optional
+        The length of input sequences when it is constant, by default None.
+    sequence_combiner : CombinerType, optional
+        A string specifying how to combine embedding results for each entry ("mean", "sqrtn"
+        and "sum" are supported) or a layer. Default is None (no combiner used).
+    trainable : bool, optional
+        Whether the layer's variables should be trainable, by default True.
+    name : str, optional
+        The name of the layer, by default None.
+    dtype : str, optional
+        The data type of the layer's computations and weights. It can also be a
+        `tf.keras.mixed_precision.Policy`, which allows the computation and weight
+        dtype to differ, by default None.
+    dynamic : bool, optional
+        Set this to `True` if the layer should only be run eagerly and should not be used
+        to generate a static computation graph, by default False.
+    l2_batch_regularization_factor : float, optional
+        The factor for L2 regularization of the embeddings vectors (from the current batch only),
+        by default 0.0.
+    **kwargs:
+        Other keyword arguments forwarded to the Keras Layer.
     """
 
     def __init__(
         self,
         dim: int,
         *col_schemas: ColumnSchema,
         embeddings_initializer="uniform",
@@ -349,28 +345,59 @@
             The name of the layer.
         """
         return cls.from_pretrained(
             data, trainable=trainable, name=name, col_schema=col_schema, **kwargs
         )
 
     def to_dataset(self, gpu=None) -> merlin.io.Dataset:
+        """Converts the EmbeddingTable to a merlin.io.Dataset.
+
+        Parameters
+        ----------
+        gpu: bool
+            Whether to use gpu.
+
+        Returns
+        -------
+        merlin.io.Dataset
+            The dataset representation of the EmbeddingTable.
+        """
         return merlin.io.Dataset(self.to_df(gpu=gpu))
 
     def to_df(self, gpu=None):
+        """Converts the EmbeddingTable to a DataFrame.
+
+        Parameters
+        ----------
+        gpu: bool
+            Whether to use gpu.
+
+        Returns
+        -------
+        cudf or pandas DataFrame
+            The DataFrame representation of the EmbeddingTable.
+        """
         return tensor_to_df(self.table.embeddings, gpu=gpu)
 
     def _maybe_build(self, inputs):
         """Creates state between layer instantiation and layer call.
         Invoked automatically before the first execution of `call()`.
         """
         self.table._maybe_build(inputs)
 
         return super(EmbeddingTable, self)._maybe_build(inputs)
 
     def build(self, input_shapes):
+        """Builds the EmbeddingTable based on the input shapes.
+
+        Parameters
+        ----------
+        input_shapes: tf.TensorShape or dictionary of shapes.
+            The shapes of the input tensors.
+        """
         if not self.table.built:
             self.table.build(input_shapes)
         return super(EmbeddingTable, self).build(input_shapes)
 
     def call(
         self, inputs: Union[tf.Tensor, TabularData], **kwargs
     ) -> Union[tf.Tensor, TabularData]:
@@ -391,14 +418,21 @@
                     out[feature_name] = self._call_table(inputs[feature_name], **kwargs)
         else:
             out = self._call_table(inputs, **kwargs)
 
         return out
 
     def _call_table(self, inputs, **kwargs):
+        """Performs the lookup operation for the inputs in the embedding table.
+
+        Parameters
+        ----------
+        inputs : tf.Tensor, tf.RaggedTensor, or tf.SparseTensor
+            The input tensors for the lookup operation.
+        """
         if isinstance(inputs, (tf.RaggedTensor, tf.SparseTensor)):
             if self.sequence_combiner and isinstance(self.sequence_combiner, str):
                 if isinstance(inputs, tf.RaggedTensor):
                     inputs = inputs.to_sparse()
 
                 inputs = tf.sparse.reshape(inputs, tf.shape(inputs)[:-1])
 
@@ -435,14 +469,26 @@
             out = tf.cast(out, self._dtype_policy.compute_dtype)
 
         return out
 
     def compute_output_shape(
         self, input_shape: Union[tf.TensorShape, Dict[str, tf.TensorShape]]
     ) -> Union[tf.TensorShape, Dict[str, tf.TensorShape]]:
+        """Computes the shape of the output tensors.
+
+        Parameters
+        ----------
+        input_shape : Union[tf.TensorShape, Dict[str, tf.TensorShape]]
+            The shape of the input tensors.
+
+        Returns
+        -------
+        Union[tf.TensorShape, Dict[str, tf.TensorShape]]
+            The shape of the output tensors.
+        """
         if isinstance(input_shape, dict):
             output_shapes = {}
             for feature_name in self.schema.column_names:
                 if feature_name in input_shape:
                     output_shapes[feature_name] = self._compute_output_shape_table(
                         input_shape[feature_name]
                     )
@@ -450,42 +496,87 @@
             output_shapes = self._compute_output_shape_table(input_shape)
 
         return output_shapes
 
     def _compute_output_shape_table(
         self, input_shape: Union[tf.TensorShape, tuple]
     ) -> tf.TensorShape:
+        """Helper method to compute the output shape of a single input tensor.
+
+        Parameters
+        ----------
+        input_shape : tf.TensorShape
+            The shape of the input tensor.
+
+        Returns
+        -------
+        tf.TensorShape
+            The shape of the output tensor.
+        """
         first_dims = input_shape
 
         if input_shape.rank > 1:
             if self.sequence_combiner is not None:
                 first_dims = [input_shape[0]]
 
             elif input_shape[-1] == 1:
                 first_dims = input_shape[:-1]
 
         output_shapes = tf.TensorShape(list(first_dims) + [self.dim])
 
         return output_shapes
 
     def compute_call_output_shape(self, input_shapes):
+        """Computes the shape of the output of a call to this layer.
+
+        Parameters
+        ----------
+        input_shapes: tf.TensorShape or dictionary of shapes.
+            The shapes of the input tensors.
+
+        Returns
+        -------
+        Union[tf.TensorShape, Dict[str, tf.TensorShape]]
+            The shape of the output of a call to this layer.
+        """
         return self.compute_output_shape(input_shapes)
 
     @classmethod
     def from_config(cls, config, table=None):
+        """Creates an EmbeddingTable from its configuration.
+
+        Parameters
+        ----------
+        config : dict
+            Configuration dictionary.
+        table : tf.keras.layers.Embedding, optional
+            An optional embedding layer.
+
+        Returns
+        -------
+        EmbeddingTable
+            A newly created EmbeddingTable.
+        """
         if table:
             config["table"] = table
         else:
             config["table"] = tf.keras.layers.deserialize(config["table"])
         if "combiner-layer" in config:
             config["sequence_combiner"] = tf.keras.layers.deserialize(config.pop("combiner-layer"))
 
         return super().from_config(config)
 
     def get_config(self):
+        """Returns the configuration of this EmbeddingTable.
+
+        Returns
+        -------
+        dict
+            Configuration dictionary.
+        """
         config = super().get_config()
         config["table"] = tf.keras.layers.serialize(self.table)
         if isinstance(self.sequence_combiner, tf.keras.layers.Layer):
             config["combiner-layer"] = tf.keras.layers.serialize(self.sequence_combiner)
         else:
             config["sequence_combiner"] = self.sequence_combiner
         return config
@@ -511,15 +602,15 @@
     """Creates a ParallelBlock with an EmbeddingTable for each categorical feature
     in the schema.
 
     Parameters
     ----------
     schema: Schema
         Schema of the input data. This Schema object will be automatically generated using
-        [NVTabular](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html).
+        [NVTabular](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html).
         Next to this, it's also possible to construct it manually.
     dim: Optional[Union[Dict[str, int], int]], optional
         A dim to use for all features, or a
         Dict like {"feature_name": embedding size, ...}, by default None
     infer_dim_fn: Callable[[ColumnSchema], int], defaults to infer_embedding_dim
         The function to use to infer the embedding dimension, by default infer_embedding_dim
     sequence_combiner: Optional[Union[str, tf.keras.layers.Layer]], optional
@@ -549,14 +640,15 @@
         Transformation block to apply for aggregating the inputs, by default None
     block_name: str, optional
         Name of the block, by default "embeddings"
     l2_batch_regularization_factor: Optional[float, Dict[str, float]] = 0.0
         Factor for L2 regularization of the embeddings vectors (from the current batch only)
         If a dictionary is provided, the keys are feature names and the values are
         regularization factors
+
     Returns
     -------
     ParallelBlock
         Returns a parallel block with an embedding table for each categorical features
     """
     if trainable:
         kwargs["trainable"] = trainable
@@ -728,14 +820,33 @@
             the sequence length)
         """
         super(AverageEmbeddingsByWeightFeature, self).__init__(**kwargs)
         self.axis = axis
         self.weight_feature_name = weight_feature_name
 
     def call(self, inputs, features):
+        """Performs the weighted average calculation.
+
+        Parameters
+        ----------
+        inputs: tf.Tensor
+            Input tensor.
+        features: dict
+            Dictionary of features, must include the weight feature.
+
+        Returns
+        -------
+        Tensor
+            Output tensor after applying the weighted average calculation.
+
+        Raises
+        ------
+        ValueError
+            If the inputs is a tf.RaggedTensor, the weight feature should also be a tf.RaggedTensor.
+        """
         weight_feature = features[self.weight_feature_name]
         if isinstance(inputs, tf.RaggedTensor) and not isinstance(weight_feature, tf.RaggedTensor):
             raise ValueError(
                 f"If inputs is a tf.RaggedTensor, the weight feature ({self.weight_feature_name}) "
                 f"should also be a tf.RaggedTensor (and not a {type(weight_feature)}), "
                 "so that the list length can vary per example for both input embedding "
                 "and weight features."
@@ -747,14 +858,26 @@
         output = tf.divide(
             tf.reduce_sum(tf.multiply(inputs, weights), axis=self.axis),
             tf.reduce_sum(weights, axis=self.axis),
         )
         return output
 
     def compute_output_shape(self, input_shape):
+        """Computes the output shape.
+
+        Parameters
+        ----------
+        input_shape : tf.TensorShape
+            Shape of the input.
+
+        Returns
+        -------
+        tf.TensorShape
+            Shape of the output, which is the same as the input shape in this case.
+        """
         return input_shape
 
     @staticmethod
     def from_schema_convention(schema: Schema, weight_features_name_suffix: str = "_weight"):
         """Infers the weight features corresponding to sequential embedding
         features based on the feature name suffix. For example, if a
         sequential categorical feature is called `item_id_seq`, if there is another
@@ -787,14 +910,21 @@
                 else:
                     combiner = tf.keras.layers.Lambda(lambda x: tf.reduce_mean(x, axis=1))
                 seq_combiners[cat_col.name] = combiner
 
         return seq_combiners
 
     def get_config(self):
+        """Returns the configuration of the layer.
+
+        Returns
+        -------
+        dict
+            A dictionary containing the configuration of the layer.
+        """
         config = super().get_config()
         config["axis"] = self.axis
         config["weight_feature_name"] = self.weight_feature_name
 
         return config
 
 
@@ -1175,20 +1305,27 @@
     tabular_module_parameters=TABULAR_MODULE_PARAMS_DOCSTRING,
     embedding_features_parameters=EMBEDDING_FEATURES_PARAMS_DOCSTRING,
 )
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class SequenceEmbeddingFeatures(EmbeddingFeatures):
     """Input block for embedding-lookups for categorical features. This module produces 3-D tensors,
     this is useful for sequential models like transformers.
+
     Parameters
     ----------
-    {embedding_features_parameters}
+    feature_config: Dict[str, FeatureConfig]
+        This specifies what TableConfig to use for each feature. For shared embeddings, the same
+        TableConfig can be used for multiple features.
+    mask_zero: bool
+       Whether or not the input value 0 is a special "padding" value that should be masked out.
     padding_idx: int
         The symbol to use for padding.
     {tabular_module_parameters}
+    add_default_pre: bool, default True
+        Whether or not to add a default preprocessing block.
     """
 
     def __init__(
         self,
         feature_config: Dict[str, FeatureConfig],
         mask_zero: bool = True,
         padding_idx: int = 0,
@@ -1196,14 +1333,15 @@
         post: Optional[BlockType] = None,
         aggregation: Optional[TabularAggregationType] = None,
         schema: Optional[Schema] = None,
         name: Optional[str] = None,
         add_default_pre=True,
         **kwargs,
     ):
+        """Initializes the block."""
         if add_default_pre:
             embedding_pre = [Filter(list(feature_config.keys()))]
             pre = [embedding_pre, pre] if pre else embedding_pre  # type: ignore
 
         super().__init__(
             feature_config=feature_config,
             pre=pre,
@@ -1214,40 +1352,87 @@
             add_default_pre=False,
             **kwargs,
         )
         self.padding_idx = padding_idx
         self.mask_zero = mask_zero
 
     def lookup_feature(self, name, val, **kwargs):
+        """Looks up the embedding for a specific feature from the pre-trained embedding tables.
+
+        Parameters
+        ----------
+        name: str
+            The name of the feature to lookup.
+        val: tf.Tensor
+            The tensor of feature values to look up in the embedding tables.
+
+        Returns
+        -------
+        tf.Tensor
+            The corresponding embedding tensor.
+        """
         return super(SequenceEmbeddingFeatures, self).lookup_feature(
             name, val, output_sequence=True
         )
 
     def compute_call_output_shape(self, input_shapes):
+        """Computes the output shapes given the input shapes.
+
+        Parameters
+        ----------
+        input_shapes: dict
+            Dictionary mapping input names to their shapes.
+
+        Returns
+        -------
+        dict
+            Dictionary mapping output names to their shapes.
+        """
         batch_size = self.calculate_batch_size_from_input_shapes(input_shapes)
         sequence_length = input_shapes[list(self.feature_config.keys())[0]][1]
 
         output_shapes = {}
         for name, val in input_shapes.items():
             output_shapes[name] = tf.TensorShape(
                 [batch_size, sequence_length, self.feature_config[name].table.dim]
             )
 
         return output_shapes
 
     def compute_mask(self, inputs, mask=None):
+        """Computes a mask tensor from the inputs.
+
+        Parameters
+        ----------
+        inputs: dict
+            Dictionary mapping input names to their values.
+        mask: tf.Tensor, optional
+            An optional mask to apply to the inputs.
+
+        Returns
+        -------
+        dict or None
+            A mask tensor, or None if `mask_zero` is False.
+        """
         if not self.mask_zero:
             return None
         outputs = {}
         for key, val in inputs.items():
             outputs[key] = tf.not_equal(val, self.padding_idx)
 
         return outputs
 
     def get_config(self):
+        """Gets the configuration dictionary for this block.
+
+        Returns
+        -------
+        dict
+            The configuration dictionary.
+        """
         config = super().get_config()
         config["mask_zero"] = self.mask_zero
         config["padding_idx"] = self.padding_idx
 
         return config
 
 
@@ -1255,46 +1440,102 @@
     inputs: Block,
     embedding_block: Block,
     aggregation=None,
     continuous_aggregation="concat",
     name: str = "continuous",
     **kwargs,
 ) -> SequentialBlock:
+    """Concatenates all numerical features and project then using the
+        specified Block.
+
+    Parameters
+    ----------
+    inputs : Block
+        Expects a ParallelBlock with a number of features
+    embedding_block : Block
+        Block to project the continuous features
+    aggregation : optional
+        Aggregation combining continuous feature switch the other features, by default None
+    continuous_aggregation : str, optional
+        Aggregation for continuous features, by default "concat"
+    name : str, optional
+        Name of the projected continuous block, by default "continuous"
+    Returns
+    -------
+    SequentialBlock
+        A block that contains the projected continuous features along with the other features
+    """
     continuous_embedding = Filter(Tags.CONTINUOUS, aggregation=continuous_aggregation).connect(
         embedding_block
     )
 
     outputs = inputs.connect_branch(
         continuous_embedding.as_tabular(name), add_rest=True, aggregation=aggregation, **kwargs
     )
 
     return outputs
 
 
 def serialize_table_config(table_config: TableConfig) -> Dict[str, Any]:
+    """Serializes a TableConfig instance
+
+    Parameters
+    ----------
+    table_config : TableConfig
+        Configuration data for one embedding table
+
+    Returns
+    -------
+    Dict[str, Any]
+        A dict with the serialized embedding "initializer" and "optimizer"
+    """
     table = deepcopy(table_config.__dict__)
     if "initializer" in table:
         table["initializer"] = tf.keras.initializers.serialize(table["initializer"])
     if "optimizer" in table:
         table["optimizer"] = tf.keras.optimizers.serialize(table["optimizer"])
 
     return table
 
 
 def deserialize_table_config(table_params: Dict[str, Any]) -> TableConfig:
+    """Deserializes a TableConfig from the serialized
+    embedding "initializer" and "optimizer"
+    Parameters
+    ----------
+    table_params : Dict[str, Any]
+        Dict with the serialized values
+
+    Returns
+    -------
+    TableConfig
+        An instance of the TableConfig
+    """
     if "initializer" in table_params and table_params["initializer"]:
         table_params["initializer"] = tf.keras.initializers.deserialize(table_params["initializer"])
     if "optimizer" in table_params and table_params["optimizer"]:
         table_params["optimizer"] = tf.keras.optimizers.deserialize(table_params["optimizer"])
     table = TableConfig(**table_params)
 
     return table
 
 
 def serialize_feature_config(feature_config: FeatureConfig) -> Dict[str, Any]:
+    """Serializes a FeatureConfig instance
+
+    Parameters
+    ----------
+    feature_config : FeatureConfig
+        Configuration data for one embedding feature
+
+    Returns
+    -------
+    Dict[str, Any]
+        Dict with FeatureConfig properties set
+    """
     outputs = {}
 
     for key, val in feature_config.items():
         feature_config_dict = dict(name=val.name, max_sequence_length=val.max_sequence_length)
         feature_config_dict["table"] = serialize_table_config(feature_config_dict["table"])
         outputs[key] = feature_config_dict
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/loader.py` & `merlin-models-23.6.0/merlin/models/tf/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,16 @@
     include_targets: bool
         Whether to include the targets in the returned batch, by default True.
     prepare_features: bool
         Whether to prepare features from dataloader for the model, by default False.
         If enabled, it converts multi-hot/list features to dense or ragged based on the schema.
         It also ensures that scalar features are converted to 2D (batch size, 1).
         P.s. The features are automatically prepared by InputBlockV2 if it is used
-    Returns:
+
+    Returns
     -------
     batch: Dict[tf.tensor]
         dictionary of input tensors.
     """
 
     from merlin.models.tf.transforms.features import PrepareFeatures
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/logging/callbacks.py` & `merlin-models-23.6.0/merlin/models/tf/logging/callbacks.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/losses/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/losses/base.py` & `merlin-models-23.6.0/merlin/models/tf/losses/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/losses/listwise.py` & `merlin-models-23.6.0/merlin/models/tf/losses/listwise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/losses/pairwise.py` & `merlin-models-23.6.0/merlin/models/tf/losses/pairwise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/metrics/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/metrics/evaluation.py` & `merlin-models-23.6.0/merlin/models/tf/metrics/evaluation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/metrics/topk.py` & `merlin-models-23.6.0/merlin/models/tf/metrics/topk.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     y_true: tf.Tensor,
     y_pred: tf.Tensor,
     label_relevant_counts: Optional[tf.Tensor] = None,
     k: int = 5,
 ) -> tf.Tensor:
     """
     Computes Precision@K metric
+
     Parameters
     ----------
     {METRIC_PARAMETERS_DOCSTRING}
     """
     results = tf.cast(tf.reduce_mean(y_true[:, : int(k)], axis=-1), backend.floatx())
     return results
 
@@ -86,14 +87,15 @@
     y_true: tf.Tensor,
     y_pred: tf.Tensor,
     label_relevant_counts: Optional[tf.Tensor] = None,
     k: int = 5,
 ) -> tf.Tensor:
     """
     Computes Mean Average Precision (MAP) @K
+
     Parameters
     ----------
     {METRIC_PARAMETERS_DOCSTRING}
     """
     # Computing the precision from 1 to k range
     precisions = tf.stack([precision_at(y_true, y_pred, k=_k) for _k in range(1, k + 1)], axis=-1)
     # Keeping only the precision at the position of relevant items
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/models/base.py` & `merlin-models-23.6.0/merlin/models/tf/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,25 @@
 import collections
 import inspect
 import os
 import sys
 import warnings
 from collections.abc import Sequence as SequenceCollection
 from functools import partial
-from typing import TYPE_CHECKING, Dict, List, Optional, Protocol, Sequence, Union, runtime_checkable
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    List,
+    Optional,
+    Protocol,
+    Sequence,
+    Union,
+    runtime_checkable,
+)
 
 import six
 import tensorflow as tf
 from keras.engine.compile_utils import MetricsContainer
 from keras.utils.losses_utils import cast_losses_to_common_dtype
 from packaging import version
 from tensorflow.keras.losses import Loss
@@ -53,14 +63,15 @@
 from merlin.models.tf.loader import Loader
 from merlin.models.tf.losses.base import loss_registry
 from merlin.models.tf.metrics import metrics_registry
 from merlin.models.tf.metrics.evaluation import MetricType
 from merlin.models.tf.metrics.topk import TopKMetricsAggregator, filter_topk_metrics, split_metrics
 from merlin.models.tf.models.utils import parse_prediction_blocks
 from merlin.models.tf.outputs.base import ModelOutput, ModelOutputType
+from merlin.models.tf.outputs.classification import CategoricalOutput
 from merlin.models.tf.outputs.contrastive import ContrastiveOutput
 from merlin.models.tf.prediction_tasks.base import ParallelPredictionBlock, PredictionTask
 from merlin.models.tf.transforms.features import PrepareFeatures, expected_input_cols_from_schema
 from merlin.models.tf.transforms.sequence import SequenceTransform
 from merlin.models.tf.typing import TabularData
 from merlin.models.tf.utils.search_utils import find_all_instances_in_layers
 from merlin.models.tf.utils.tf_utils import (
@@ -101,15 +112,20 @@
             be like "click/binary_classification_task", "rating/regression_task".
             If OutputBlock (V2) is used, the task names should be like
             "click/binary_output", "rating/regression_output"
 """
 
 
 class MetricsComputeCallback(tf.keras.callbacks.Callback):
-    """Callback that handles when to compute metrics."""
+    """Callback that handles when to compute metrics."
+    Parameters
+    ----------
+    train_metrics_steps : int, optional
+        Frequency (number of steps) to compute train metrics, by default 1
+    """
 
     def __init__(self, train_metrics_steps=1, **kwargs):
         self.train_metrics_steps = train_metrics_steps
         self._is_fitting = False
         self._is_first_batch = True
         super().__init__(**kwargs)
 
@@ -162,15 +178,23 @@
         output_schema.column_schemas[output_name] = col_schema
 
     return output_schema
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class ModelBlock(Block, tf.keras.Model):
-    """Block that extends `tf.keras.Model` to make it saveable."""
+    """Block that extends `tf.keras.Model` to make it saveable.
+
+    Parameters
+    ----------
+    block : Block
+        Block to be turned into a model
+    prep_features : Optional[bool], optional
+        Whether features need to be prepared or not, by default True
+    """
 
     def __init__(self, block: Block, prep_features: Optional[bool] = True, **kwargs):
         super().__init__(**kwargs)
         self.block = block
         if hasattr(self, "set_schema"):
             block_schema = getattr(block, "schema", None)
             self.set_schema(block_schema)
@@ -280,14 +304,18 @@
         return cls(block, **config)
 
     def get_config(self):
         return {"block": tf.keras.utils.serialize_keras_object(self.block)}
 
 
 class BaseModel(tf.keras.Model):
+    """Base model, that overrides Keras model methods
+    to compile, compute metrics and loss and also
+    to compute the train, eval, predict steps"""
+
     def __init__(self, **kwargs):
         super(BaseModel, self).__init__(**kwargs)
 
         # Initializing model control flags controlled by MetricsComputeCallback()
         self._should_compute_train_metrics_for_batch = tf.Variable(
             dtype=tf.bool,
             name="should_compute_train_metrics_for_batch",
@@ -656,14 +684,18 @@
             if isinstance(out[key], str) and out[key] in loss_registry:
                 out[key] = loss_registry.parse(out[key])
 
         return out
 
     @property
     def prediction_tasks(self) -> List[PredictionTask]:
+        """Returns the Prediction tasks in the model.
+        Going to be deprecated in favor of model_outputs()
+        """
+
         from merlin.models.tf.prediction_tasks.base import PredictionTask
 
         results = find_all_instances_in_layers(self, PredictionTask)
         # Ensures tasks are sorted by name, so that they match the metrics
         # which are sorted the same way by Keras
         results = list(sorted(results, key=lambda x: x.task_name))
 
@@ -689,22 +721,24 @@
                     outputs[task.target_name] = [outputs[task.target_name], task]
             outputs[task.target] = task
 
         return outputs
 
     @property
     def model_outputs(self) -> List[ModelOutput]:
+        """Returns a list with the ModelOutput in the model"""
         results = find_all_instances_in_layers(self, ModelOutput)
         # Ensures tasks are sorted by name, so that they match the metrics
         # which are sorted the same way by Keras
         results = list(sorted(results, key=lambda x: x.full_name))
 
         return results
 
     def outputs_by_name(self) -> Dict[str, ModelOutput]:
+        """Returns the task names from the model outputs"""
         return {task.full_name: task for task in self.model_outputs}
 
     def outputs_by_target(self) -> Dict[str, List[ModelOutput]]:
         """Method to index the model's prediction blocks by target names.
 
         Returns
         -------
@@ -1171,14 +1205,15 @@
         # Batch loss (the default loss metric from Keras is the incremental average per epoch,
         # not the actual batch loss)
         metrics["loss_batch"] = loss
 
         return metrics
 
     def predict_step(self, data):
+        """Custom predict step to obtain the outputs"""
         x, _, _ = unpack_x_y_sample_weight(data)
 
         if getattr(self, "predict_pre", None):
             out = call_layer(self.predict_pre, x, features=x, training=False)
             if isinstance(out, Prediction):
                 x = out.outputs
             elif isinstance(out, tuple):
@@ -1554,16 +1589,21 @@
         super().save(*args, **kwargs)
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class Model(BaseModel):
     """Merlin Model class
 
+    `Model` is the main base class that represents a model in Merlin Models.
+    It can be configured with a number of pre and post processing blocks and can manage a context.
+
     Parameters
     ----------
+    blocks : list
+        List of `Block` instances in the model
     context : Optional[ModelContext], optional
         ModelContext is used to store/retrieve public variables across blocks,
         by default None.
     pre : Optional[BlockType], optional
         Optional `Block` instance to apply before the `call` method of the Two-Tower block
     post : Optional[BlockType], optional
         Optional `Block` instance to apply on both outputs of Two-tower model
@@ -1581,14 +1621,15 @@
         context: Optional[ModelContext] = None,
         pre: Optional[tf.keras.layers.Layer] = None,
         post: Optional[tf.keras.layers.Layer] = None,
         schema: Optional[Schema] = None,
         prep_features: Optional[bool] = True,
         **kwargs,
     ):
+        """Creates a new `Model` instance."""
         super(Model, self).__init__(**kwargs)
 
         context = context or ModelContext()
         if len(blocks) == 1 and isinstance(blocks[0], SequentialBlock):
             blocks = blocks[0].layers
 
         self.blocks = blocks
@@ -1730,14 +1771,35 @@
 
         if self.post is not None:
             self.post.build(input_shape)
 
         self.built = True
 
     def call(self, inputs, targets=None, training=False, testing=False, output_context=False):
+        """
+        Method for forward pass of the model.
+
+        Parameters
+        ----------
+        inputs : Tensor or dict of Tensor
+            Input Tensor(s) for the model
+        targets : Tensor or dict of Tensor, optional
+            Target Tensor(s) for the model
+        training : bool, optional
+            Flag to indicate whether the model is in training phase
+        testing : bool, optional
+            Flag to indicate whether the model is in testing phase
+        output_context : bool, optional
+            Flag to indicate whether to return the context along with the output
+
+        Returns
+        -------
+        Tensor or tuple of Tensor and ModelContext
+            Output of the model, and optionally the context
+        """
         outputs = inputs
         features = self._prepare_features(inputs, targets=targets)
         if isinstance(features, tuple):
             features, targets = features
         if self.prep_features:
             outputs = features
         context = self._create_context(
@@ -1790,18 +1852,40 @@
                 outputs = outputs[0]
             context = context.with_updates(targets=targets, features=features)
 
         return outputs, context
 
     @property
     def first(self):
+        """
+        The first `Block` in the model.
+
+        This property provides a simple way to quickly access the first `Block` in the model's
+        sequence of blocks.
+
+        Returns
+        -------
+        Block
+            The first `Block` in the model.
+        """
         return self.blocks[0]
 
     @property
     def last(self):
+        """
+        The last `Block` in the model.
+
+        This property provides a simple way to quickly access the last `Block` in the model's
+        sequence of blocks.
+
+        Returns
+        -------
+        Block
+            The last `Block` in the model.
+        """
         return self.blocks[-1]
 
     @classmethod
     def from_block(
         cls,
         block: Block,
         schema: Schema,
@@ -1842,14 +1926,33 @@
 
         prediction_tasks = parse_prediction_blocks(schema, prediction_tasks)
 
         return cls(_input_block, block, prediction_tasks)
 
     @classmethod
     def from_config(cls, config, custom_objects=None):
+        """
+        Creates a model from its config.
+
+        This method recreates a model instance from a configuration dictionary and
+        optional custom objects.
+
+        Parameters
+        ----------
+        config : dict
+            The configuration dictionary representing the model.
+        custom_objects : dict, optional
+            Dictionary mapping names to custom classes or functions to be considered
+            during deserialization.
+
+        Returns
+        -------
+        Model
+            The created `Model` instance.
+        """
         pre = config.pop("pre", None)
         post = config.pop("post", None)
         schema = config.pop("schema", None)
         batch_size = config.pop("batch_size", None)
 
         layers = [
             tf.keras.layers.deserialize(conf, custom_objects=custom_objects)
@@ -1878,14 +1981,30 @@
             inputs = model.get_sample_inputs(batch_size=batch_size)
             if inputs:
                 model(inputs)
 
         return model
 
     def get_sample_inputs(self, batch_size=None):
+        """
+        Generates sample inputs for the model.
+
+        This method creates a dictionary of sample inputs for each input feature, useful for
+        testing or initializing the model.
+
+        Parameters
+        ----------
+        batch_size : int, optional
+            The batch size for the sample inputs. If not specified, defaults to 2.
+
+        Returns
+        -------
+        dict
+            A dictionary mapping feature names to sample input tensors.
+        """
         batch_size = batch_size or 2
         if self.input_schema is not None:
             inputs = {}
             for column in self.input_schema:
                 shape = [batch_size]
                 try:
                     dtype = column.dtype.to("tensorflow")
@@ -1923,14 +2042,26 @@
                         shape + [row_length], dtype=dtype, maxval=maxval
                     )
                 else:
                     inputs[column.name] = tf.random.uniform(shape, dtype=dtype, maxval=maxval)
             return inputs
 
     def get_config(self):
+        """
+        Returns the model configuration as a dictionary.
+
+        This method returns a dictionary containing the configuration of the model.
+        The dictionary includes the configuration of each block in the model,
+        as well as additional properties such as `pre` and `post` layers, and the `schema`.
+
+        Returns
+        -------
+        dict
+            The configuration of the model.
+        """
         config = maybe_serialize_keras_objects(self, {}, ["pre", "post"])
         config["schema"] = schema_utils.schema_to_tensorflow_metadata_json(self.schema)
         for i, layer in enumerate(self.blocks):
             config[i] = tf.keras.utils.serialize_keras_object(layer)
         config["batch_size"] = self._batch_size
 
         return config
@@ -2080,14 +2211,16 @@
             if len(block_names) > 0:
                 raise ValueError(f"Cannot find block with the name of {block_names}")
         return list(result_blocks)
 
 
 @runtime_checkable
 class RetrievalBlock(Protocol):
+    """Protocol class for a RetrievalBlock"""
+
     def query_block(self) -> Block:
         ...
 
     def item_block(self) -> Block:
         ...
 
 
@@ -2370,15 +2503,15 @@
                 return candidate.encode(dataset, index=index, **kwargs)
 
             if hasattr(candidate, "to_dataset"):
                 return candidate.to_dataset(**kwargs)
 
             return candidate.encode(dataset, index=index, **kwargs)
 
-        if isinstance(self.last, ContrastiveOutput):
+        if isinstance(self.last, (ContrastiveOutput, CategoricalOutput)):
             return self.last.to_dataset()
 
         raise Exception(...)
 
     @property
     def encoder(self):
         return self._encoder
@@ -2483,15 +2616,34 @@
             k=k,
             candidates=candidates_embeddings,
             target=self.encoder._schema.select_by_tag(candidate_id).first.name,
         )
         return topk_model
 
 
-def _maybe_convert_merlin_dataset(data, batch_size, shuffle=True, **kwargs):
+def _maybe_convert_merlin_dataset(
+    data: Any, batch_size: int, shuffle: bool = True, **kwargs
+) -> Any:
+    """Converts the Dataset to a Loader with the given
+    batch_size and shuffle options
+
+    Parameters
+    ----------
+    data
+        Dataset instance
+    batch_size : int
+        Batch size
+    shuffle : bool, optional
+        Enables data shuffling during loading, by default True
+
+    Returns
+    -------
+    Any
+        Returns a Loader instance if a Dataset, otherwise returns the data
+    """
     # Check if merlin-dataset is passed
     if hasattr(data, "to_ddf"):
         if not batch_size:
             raise ValueError("batch_size must be specified when using merlin-dataset.")
 
         data = Loader(data, batch_size=batch_size, shuffle=shuffle, **kwargs)
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/models/benchmark.py` & `merlin-models-23.6.0/merlin/models/tf/models/benchmark.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/models/ranking.py` & `merlin-models-23.6.0/merlin/models/tf/models/ranking.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,14 +234,15 @@
         dropout or kernel regularization to the wide block.
 
     prediction_tasks: Optional[Union[PredictionTask,List[PredictionTask],
                                 ParallelPredictionBlock,ModelOutputType]
         The prediction tasks to be used, by default this will be inferred from the Schema.
         For custom prediction tasks we recommending using OutputBlock and blocks based
         on ModelOutput than the ones based in PredictionTask (that will be deprecated).
+
     Returns
     -------
     Model
 
     """
 
     input_block = input_block or InputBlockV2(
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/models/retrieval.py` & `merlin-models-23.6.0/merlin/models/tf/models/retrieval.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,17 +66,14 @@
     post: Optional[Block], optional
         The optional `Block` to apply on both outputs of Two-tower model
     prediction_tasks: optional
         The optional `PredictionTask` or list of `PredictionTask` to apply on the model.
     logits_temperature: float
         Parameter used to reduce model overconfidence, so that logits / T.
         Defaults to 1.
-    loss: Optional[LossType]
-        Loss function.
-        Defaults to `bpr`.
     samplers: List[ItemSampler]
         List of samplers for negative sampling, by default `[InBatchSampler()]`
 
     Returns
     -------
     RetrievalModel
     """
@@ -539,27 +536,34 @@
         vector.
     inputs: tf.keras.layers.Layer, optional
         The input layer to encode input features (sparse and context features)
         If not specified, the input layer is inferred from the schema
         By default None
     post: Optional[tf.keras.layers.Layer], optional
         The optional layer to apply on top of the query encoder.
+    outputs : Union[ModelOutput, List[ModelOutput]], optional
+        Specifies the model's outputs. If not specified, the outputs will be inferred.
     logits_temperature: float, optional
         Parameter used to reduce model overconfidence, so that logits / T.
         Defaults to 1.
     num_sampled: int, optional
         When sampled_softmax is enabled, specify the number of
         negative candidates to generate for each batch.
         By default 100
     min_sampled_id: int, optional
         The minimum id value to be sampled with sampled softmax.
         Useful to ignore the first categorical
         encoded ids, which are usually reserved for <nulls>,
         out-of-vocabulary or padding.
         By default 0.
+
+    Returns
+    --------
+    RetrievalModelV2
+        The constructed Youtube-DNN based retrieval model
     """
     if not inputs:
         inputs = schema
 
     candidate = schema.select_by_tag(candidate_id_tag)
     if not candidate:
         raise ValueError(f"The schema should contain a feature tagged as `{candidate_id_tag}`")
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/models/utils.py` & `merlin-models-23.6.0/merlin/models/tf/models/utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/base.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
     Parameters
     ----------
     to_call : Layer
         The layer to call in the forward-pass of the model
     default_loss: Union[str, tf.keras.losses.Loss]
         Default loss to set if the user does not specify one
-    get_default_metrics: Callable
+    default_metrics_fn: Callable
         A function returning the list of default metrics to set
         if the user does not specify any
     name: Optional[Text], optional
         Task name, by default None
     target: Optional[str], optional
         Label name, by default None
     pre: Optional[Block], optional
@@ -249,15 +249,25 @@
             objects.append("default_loss")
 
         config = tf_utils.maybe_serialize_keras_objects(self, config, objects)
 
         return config
 
     @classmethod
-    def get_task_name(cls, target_name):
+    def get_task_name(cls, target_name: str) -> str:
+        """Returns the name of the task
+        Parameters
+        ----------
+        target_name : str
+            Name of the target
+        Returns
+        -------
+        str
+            Returns the task name, which includes the target name
+        """
         base_name = to_snake_case(cls.__name__)
         return name_fn(target_name, base_name) if target_name else base_name
 
     @classmethod
     def from_config(cls, config):
         config["default_metrics_fn"] = cls._parse_function_from_config(
             config, "default_metrics_fn", "module", "function_type"
@@ -276,14 +286,15 @@
 
         return super().from_config(config)
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class DotProduct(Layer):
     """Dot-product between queries & items.
+
     Parameters:
     -----------
     query_name : str, optional
         Identify query tower for query/user embeddings, by default 'query'
     item_name : str, optional
         Identify item tower for item embeddings, by default 'item'
     """
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/block.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     Simple Usage::
         outputs = OutputBlock(schema)
 
     Parameters
     ----------
     schema : Schema
         Schema of the input data. This Schema object will be automatically generated using
-        [NVTabular](https://nvidia-merlin.github.io/NVTabular/main/Introduction.html).
+        [NVTabular](https://nvidia-merlin.github.io/NVTabular/stable/Introduction.html).
         Next to this, it's also possible to construct it manually.
     model_outputs: Optional[Union[Sequence[ModelOutput], Dict[str, ModelOutput]]]
         Optional dict or list of ModelOutput. If a dict, the keys must be the
         <target_name>/output_type (e.g. "click/binary_output", "rating/regression_output"))
         This method will create ModelOutput only for the tasks not provided in model_outputs.
     pre : Optional[Layer], optional
         Transformation block to apply before the embeddings lookup, by default None
@@ -127,22 +127,52 @@
     if len(outputs) == 1:
         return list(outputs.values())[0]
 
     return ParallelBlock(outputs, pre=pre, post=post, schema=Schema(cols))
 
 
 def _get_col_set_by_tags(schema: Schema, tags) -> Set[str]:
+    """Returns a set with the schema column names
+
+    Parameters
+    ----------
+    schema : Schema
+        Schema
+    tags :
+        Tags to filter
+
+    Returns
+    -------
+    Set[str]
+        A set with the schema column names
+    """
     return set(schema.select_by_tag(tags).column_names)
 
 
 def _set_task_block(
     output_block: OutputBlock,
     col_name: str,
     task_blocks: Optional[Union[Layer, Dict[str, Layer]]] = None,
 ):
+    """Creates a tower (task_block) for each task (output).
+
+    Parameters
+    ----------
+    output_block : OutputBlock
+        The output block with the tasks
+    col_name : str
+        Specify the task name
+    task_blocks : Optional[Union[Layer, Dict[str, Layer]]], optional
+        Task blocks to be used as task towers. If a single Layer, it is copied to all
+        tasks. If a dict, the keys must match the task names
+        (e.g. "click/binary_output", rating/regression_output", "item_id/categorical_output").
+        You might want to use the task_blocks to create a task-specific tower
+        (e.g. MLPBLock([32])) or to customize inputs, targets or sample_weights for a
+        given task. By default None
+    """
     task_block = None
     if task_blocks is not None:
         if isinstance(task_blocks, dict):
             if output_block.name in task_blocks:
                 task_block = task_blocks[output_block.name]
             elif col_name in task_blocks:
                 task_block = task_blocks[col_name]
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/classification.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/classification.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import logging
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 import tensorflow as tf
 from tensorflow.keras.layers import Layer
 from tensorflow.python.ops import embedding_ops
 
 import merlin.io
 from merlin.models.tf.inputs.embedding import EmbeddingTable
@@ -30,24 +30,39 @@
     tensor_to_df,
 )
 from merlin.schema import ColumnSchema, Schema
 
 LOG = logging.getLogger("merlin_models")
 
 
-def default_binary_metrics():
+def default_binary_metrics() -> List[tf.keras.metrics.Metric]:
+    """Returns the default binary metrics
+
+    Returns
+    -------
+    List[tf.keras.metrics.Metric]
+        List with metrics for binary classification
+    """
     return (
         tf.keras.metrics.Precision(name="precision"),
         tf.keras.metrics.Recall(name="recall"),
         tf.keras.metrics.BinaryAccuracy(name="binary_accuracy"),
         tf.keras.metrics.AUC(name="auc"),
     )
 
 
 def default_categorical_prediction_metrics(k=10):
+    """Returns the default top-k metrics for
+    categorical classification
+
+    Returns
+    -------
+    List[tf.keras.metrics.Metric]
+        List with top-k metrics for categorical classification
+    """
     return (
         RecallAt(k),
         MRRAt(k),
         NDCGAt(k),
         AvgPrecisionAt(k),
         PrecisionAt(k),
     )
@@ -66,16 +81,14 @@
         Optional block to transform predictions before computing the binary logits,
         by default None
     post: Optional[Block], optional
         Optional block to transform the binary logits,
         by default None
     name: str, optional
         The name of the task.
-    task_block: Block, optional
-        The block to use for the task.
     logits_temperature: float, optional
         Parameter used to reduce model overconfidence, so that logits / T.
         by default 1.
     default_loss: Union[str, tf.keras.losses.Loss], optional
         Default loss to use for binary-classification
         by 'binary_crossentropy'
     default_metrics_fn: Callable
@@ -300,44 +313,49 @@
 
     Parameters
     ----------
     table : EmbeddingTable
         The embedding table to use as the weight matrix
     bias_initializer : str, optional
         Initializer for the bias vector, by default "zeros"
+    use_bias: bool, optional
+        Whether to add a bias term to weight-tying, by default False
 
     References:
     ----------
     [1] Hakan Inan, Khashayar Khosravi, and Richard Socher. 2016. Tying word vectors
     and word classifiers: A loss framework for language modeling. arXiv preprint
     arXiv:1611.01462 (2016).
     """
 
-    def __init__(self, table: EmbeddingTable, bias_initializer="zeros", **kwargs):
+    def __init__(self, table: EmbeddingTable, bias_initializer="zeros", use_bias=False, **kwargs):
         self.table = table
         self.num_classes = table.input_dim
         self.bias_initializer = bias_initializer
+        self.use_bias = use_bias
         super().__init__(**kwargs)
 
     def build(self, input_shape):
-        self.bias = self.add_weight(
-            name="output_layer_bias",
-            shape=(self.num_classes,),
-            initializer=self.bias_initializer,
-        )
+        if self.use_bias:
+            self.bias = self.add_weight(
+                name="output_layer_bias",
+                shape=(self.num_classes,),
+                initializer=self.bias_initializer,
+            )
         self.table.build(input_shape)
         return super().build(input_shape)
 
     def call(self, inputs, training=False, **kwargs) -> tf.Tensor:
         is_ragged = isinstance(inputs, tf.RaggedTensor)
         if is_ragged:
             original_inputs = inputs
             inputs = inputs.flat_values
         logits = tf.matmul(inputs, self.table.table.embeddings, transpose_b=True)
-        logits = tf.nn.bias_add(logits, self.bias)
+        if self.use_bias:
+            logits = tf.nn.bias_add(logits, self.bias)
         if is_ragged:
             logits = original_inputs.with_flat_values(logits)
         return logits
 
     @property
     def embeddings(self):
         return self.table.table.embeddings
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/contrastive.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/contrastive.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/regression.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/sampling/base.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/sampling/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/sampling/in_batch.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/sampling/in_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     in training batches.
     P.s. Ignoring the false negatives (negative items equal to the positive ones) is
     managed by `ItemRetrievalScorer(..., sampling_downscore_false_negatives=True)`
     References
     ----------
     .. [1] Yi, Xinyang, et al. "Sampling-bias-corrected neural modeling for large corpus item
        recommendations." Proceedings of the 13th ACM Conference on Recommender Systems. 2019.
+
     Parameters
     ----------
     batch_size : int, optional
         The batch size. If not set it is inferred when the layer is built (first call())
     """
 
     def __init__(self, batch_size: Optional[int] = None, **kwargs):
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/sampling/popularity.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/sampling/popularity.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/outputs/topk.py` & `merlin-models-23.6.0/merlin/models/tf/outputs/topk.py`

 * *Files 4% similar despite different names*

```diff
@@ -202,28 +202,38 @@
         """
         k = k if k is not None else self._k
         if self._candidates is None:
             raise ValueError(
                 "You should call the `index` method first to " "set the _candidates index."
             )
 
+        if isinstance(inputs, tf.RaggedTensor):
+            # Evaluates on last session's item only
+            # (which is the default mode during inference too).
+            # TODO extend top-k generation to other items in the input session.
+            inputs = tf.squeeze(inputs.to_tensor(), axis=1)
         tf.assert_equal(
             tf.shape(inputs)[1],
             tf.shape(self._candidates)[1],
             "Query and candidates vectors must have the same embedding size "
             f"(got query dimension of {tf.shape(inputs)[1]} and candidates"
             f" dimension of {tf.shape(self._candidates)[1]} ",
         )
         scores = self._score(inputs, self._candidates)
         top_scores, top_idx = tf.math.top_k(scores, k=k)
         top_ids = tf.gather(self._ids, top_idx)
         if testing:
             assert targets is not None, ValueError(
                 "Targets should be provided during the evaluation mode"
             )
+            if isinstance(targets, tf.RaggedTensor):
+                targets = tf.ragged.boolean_mask(
+                    targets, targets._keras_mask.with_row_splits_dtype(targets.row_splits.dtype)
+                )
+                targets = targets.to_tensor()
             targets = tf.cast(tf.squeeze(targets), tf.int32)
             targets = tf.cast(tf.expand_dims(targets, -1) == top_ids, tf.float32)
             targets = tf.reshape(targets, tf.shape(top_scores))
             return Prediction(top_scores, targets)
         return TopKPrediction(top_scores, top_ids)
 
     def compute_output_shape(self, input_shape):
@@ -232,14 +242,15 @@
             tf.TensorShape((input_shape[0], self._k)),
         )
 
 
 @tf.keras.utils.register_keras_serializable(package="merlin.models")
 class TopKOutput(ModelOutput):
     """Prediction block for top-k evaluation
+
     Parameters
     ----------
     to_call:  Union[str, TopKLayer]
        The top-k layer to use for retrieving top-k candidates ids and scores
     item_dataset:  merlin.io.Dataset,
         Dataset of the pretrained candidates embeddings to use for the top-k index.
     k: int, optional
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/prediction_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/base.py` & `merlin-models-23.6.0/merlin/models/tf/prediction_tasks/base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/classification.py` & `merlin-models-23.6.0/merlin/models/tf/prediction_tasks/classification.py`

 * *Files 18% similar despite different names*

```diff
@@ -95,20 +95,47 @@
         # To ensure that the output is always fp32, avoiding numerical
         # instabilities with mixed_float16 (fp16) policy
         self.output_activation = tf.keras.layers.Activation(
             "sigmoid", dtype="float32", name="prediction"
         )
 
     def call(self, inputs, training=False, **kwargs):
+        """Projects the input with the output layer to a single logit
+
+        Parameters
+        ----------
+        inputs : tf.Tensor
+            Input tensor
+        training : bool, optional
+            Flag that indicates whether it is training or not, by default False
+
+        Returns
+        -------
+        tf.Tensor
+            Tensor with the classification probabilities
+        """
         return self.output_activation(self.output_layer(inputs))
 
     def compute_output_shape(self, input_shape):
+        """Computes the output shape based on the input shape
+
+        Parameters
+        ----------
+        input_shape : tf.TensorShape
+            The input shape
+
+        Returns
+        -------
+        tf.TensorShape
+            The output shape
+        """
         return self.output_layer.compute_output_shape(input_shape)
 
     def get_config(self):
+        """Return a Python dict containing the configuration of the model."""
         config = super().get_config()
         config = maybe_serialize_keras_objects(
             self,
             config,
             {"output_layer": tf.keras.layers.serialize},
         )
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/multi.py` & `merlin-models-23.6.0/merlin/models/tf/prediction_tasks/multi.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/next_item.py` & `merlin-models-23.6.0/merlin/models/tf/prediction_tasks/next_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 @Block.registry.register_with_multiple_names("weight-tying")
 @tf.keras.utils.register_keras_serializable(package="merlin_models")
 class ItemsPredictionWeightTying(Block):
     """Tying the item embedding weights with the output projection layer matrix [1]
     The output logits are obtained by multiplying the output vector by the item-ids embeddings.
+
     Parameters
     ----------
         schema : Schema
             The `Schema` with the input features
         bias_initializer : str, optional
             Initializer to use on the bias vector, by default "zeros"
     References:
@@ -97,31 +98,34 @@
     Compute the items logits on a subset of sampled candidates to optimize
     training. During inference, the scores are computed over the whole
     catalog of items.
     The PopularityBasedSampler is used for sampled softmax [1]_ [2]_ [3]_.
     That implementation does not require the actual item frequencies/probabilities
     if the item ids are sorted by frequency. The PopularityBasedSampler
     approximates the item probabilities using the log_uniform (zipfian) distribution.
+
     Parameters:
     -----------
         schema: Schema
             The schema object including features to use and their properties.
         num_sampled: int
             The number of candidates to sample during training
         min_id: int
             The minimum id value to be sampled as negative. Useful to ignore the first categorical
             encoded ids, which are usually reserved for <nulls>, out-of-vocabulary or padding.
             Defaults to 0.
         ignore_false_negatives: bool
             Ignore sampled items that are equal to the target classes
             Defaults to True
-    Returns:
+
+    Returns
     -------
         A SequenceBlock that performs popularity-based sampling of negatives, scores
         the items and applies the logQ correction for sampled softmax
+
     References
     ----------
     .. [1] Yoshua Bengio and Jean-Sébastien Sénécal. 2003. Quick Training of Probabilistic
        Neural Nets by Importance Sampling. In Proceedings of the conference on Artificial
        Intelligence and Statistics (AISTATS).
     .. [2 Y. Bengio and J. S. Senecal. 2008. Adaptive Importance Sampling to Accelerate
        Training of a Neural Probabilistic Language Model. Trans. Neur. Netw. 19, 4 (April
@@ -165,14 +169,15 @@
     sampled_softmax: bool = False,
     num_sampled: int = 100,
     min_sampled_id: int = 0,
     post_logits: Optional[Block] = None,
 ) -> MultiClassClassificationTask:
     """
     Function to create the NextItemPrediction task with the right parameters.
+
     Parameters
     ----------
         schema: Schema
             The schema object including features to use and their properties.
         weight_tying: bool
             The item_id embedding weights are shared with the prediction network layer.
             Defaults to True
@@ -205,14 +210,15 @@
             The minimum id value to be sampled. Useful to ignore the first categorical
             encoded ids, which are usually reserved for <nulls>, out-of-vocabulary or padding.
             Defaults to 0.
         post_logits: Optional[PredictionBlock]
             Optional extra pre-call block for post-processing the logits, by default None.
             You can for example use `post_logits = mm.PopularitySamplingBlock(item_fequency)`
             for populariy sampling correction.
+
     Returns
     -------
         PredictionTask
             The next item prediction task
     """
     if sampled_softmax:
         prediction_call = ItemsPredictionPopSampled(
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/regression.py` & `merlin-models-23.6.0/merlin/models/tf/prediction_tasks/regression.py`

 * *Files 14% similar despite different names*

```diff
@@ -101,17 +101,30 @@
         -------
         tf.Tensor
             Tensor with the regression logit
         """
         return self.output_activation(self.output_layer(inputs))
 
     def compute_output_shape(self, input_shape):
+        """Computes the output shape based on the input shape
+
+        Parameters
+        ----------
+        input_shape : tf.TensorShape
+            The input shape
+
+        Returns
+        -------
+        tf.TensorShape
+            The output shape
+        """
         return self.output_layer.compute_output_shape(input_shape)
 
     def get_config(self):
+        """Return a Python dict containing the configuration of the model."""
         config = super().get_config()
         config = maybe_serialize_keras_objects(
             self, config, {"output_layer": tf.keras.layers.serialize}
         )
 
         return config
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/prediction_tasks/retrieval.py` & `merlin-models-23.6.0/merlin/models/tf/prediction_tasks/retrieval.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,30 +35,35 @@
 
     Parameters
     ----------
         schema: Schema
             The schema object including features to use and their properties.
         samplers: List[ItemSampler]
             List of samplers for negative sampling, by default `[InBatchSampler()]`
-        post_logits: Optional[PredictionBlock]
-            Optional extra pre-call block for post-processing the logits, by default None.
-            You can for example use `post_logits = mm.PopularitySamplingBlock(item_fequency)`
-            for populariy sampling correction.
         target_name: Optional[str]
             If specified, name of the target tensor to retrieve from dataloader.
             Defaults to None.
         task_name: Optional[str]
             name of the task.
             Defaults to None.
         task_block: Block
             The `Block` that applies additional layers op to inputs.
             Defaults to None.
+        post_logits: Optional[PredictionBlock]
+            Optional extra pre-call block for post-processing the logits, by default None.
+            You can for example use `post_logits = mm.PopularitySamplingBlock(item_fequency)`
+            for populariy sampling correction.
         logits_temperature: float
             Parameter used to reduce the model overconfidence, so that logits / T.
             Defaults to 1.
+        cache_query: bool
+            Add query embeddings to the context block, by default False
+        store_negative_ids: bool
+            Returns negative items ids as part of the output, by default False
+
     Returns
     -------
         PredictionTask
             The item retrieval prediction task
     """
 
     DEFAULT_LOSS = "categorical_crossentropy"
@@ -108,14 +113,15 @@
         self,
         samplers: Sequence[ItemSampler],
         logits_temperature: float,
         post_logits: Optional[Block] = None,
         store_negative_ids: bool = False,
         **kwargs,
     ):
+        """Returns a SequentialBlock of ItemRetrievalScorer() and LogitsTemperatureScaler()"""
         if samplers is None or len(samplers) == 0:
             samplers = (InBatchSampler(),)
 
         prediction_call = ItemRetrievalScorer(
             samplers=samplers,
             item_id_feature_name=self.item_id_feature_name,
             item_domain=self.item_domain,
@@ -130,14 +136,15 @@
             prediction_call = prediction_call.connect(LogitsTemperatureScaler(logits_temperature))
 
         return prediction_call
 
     @property
     def retrieval_scorer(self):
         def find_retrieval_scorer_block(block):
+            """Returns the ItemRetrievalScorer layer"""
             if isinstance(block, ItemRetrievalScorer):
                 return block
 
             if getattr(block, "layers", None):
                 for subblock in block.layers:
                     result = find_retrieval_scorer_block(subblock)
                     if result:
@@ -152,14 +159,15 @@
 
         return result
 
     def set_retrieval_cache_query(self, value: bool):
         self.retrieval_scorer.cache_query = value
 
     def get_config(self):
+        """Return a Python dict containing the configuration of the model."""
         config = super(ItemRetrievalTask, self).get_config()
         del config["pre"]
         if self.samplers:
             config["samplers"] = [tf.keras.layers.serialize(sampler) for sampler in self.samplers]
         if self.post_logits is not None:
             config["post_logits"] = self.post_logits
         config.update(
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/transformers/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/transformers/block.py` & `merlin-models-23.6.0/merlin/models/tf/transformers/block.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/transformers/transforms.py` & `merlin-models-23.6.0/merlin/models/tf/transformers/transforms.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/transforms/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/transforms/bias.py` & `merlin-models-23.6.0/merlin/models/tf/transforms/bias.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/transforms/features.py` & `merlin-models-23.6.0/merlin/models/tf/transforms/features.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/transforms/negative_sampling.py` & `merlin-models-23.6.0/merlin/models/tf/transforms/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/transforms/noise.py` & `merlin-models-23.6.0/merlin/models/tf/transforms/noise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/transforms/sequence.py` & `merlin-models-23.6.0/merlin/models/tf/transforms/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     Flatten the sequence of labels and filter out non-targets positions
 
     Parameters
     ----------
         padding_idx: int
             The padding index value.
             Defaults to 0.
+
     Returns
     -------
         targets: tf.Tensor
             The flattened vector of true targets positions
         flatten_predictions: tf.Tensor
             If the predictions are 3-D vectors (sequential task),
             flatten the predictions vectors to keep only the ones related to target positions.
@@ -969,18 +970,37 @@
     To support masked training approach in Transformer-based model,
     SequenceMaskRandom and SequenceLastRandom implements `configure_for_train` method
     that sets `ReplaceMaskedEmbeddings` as part of the `masking_pre` of
     the transformer block.
     """
 
     def __init__(self, **kwargs):
+        """Initializes the block."""
         super().__init__(**kwargs)
         self.supports_masking = True
 
     def build(self, input_shape):
+        """Builds the block's internal variables.
+
+        This method creates a trainable embedding to replace masked interactions in the input.
+
+        Parameters
+        ----------
+        input_shape : tf.TensorShape
+            Shape of the input tensor.
+
+        Returns
+        -------
+        None
+
+        Raises
+        ------
+        ValueError
+            If the last dimension of the input shape is None.
+        """
         self.hidden_size = input_shape[-1]
         if self.hidden_size is None:
             raise ValueError("The last dim of inputs cannot be None")
         # Create a trainable embedding to replace masked interactions
         initializer = tf.random_normal_initializer(mean=0.0, stddev=0.001)
         self.masked_embedding = tf.Variable(initializer(shape=[self.hidden_size], dtype=tf.float32))
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/transforms/tensor.py` & `merlin-models-23.6.0/merlin/models/tf/transforms/tensor.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/typing.py` & `merlin-models-23.6.0/merlin/models/tf/typing.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/utils/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/utils/batch_utils.py` & `merlin-models-23.6.0/merlin/models/tf/utils/batch_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/utils/repr_utils.py` & `merlin-models-23.6.0/merlin/models/tf/utils/repr_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/utils/search_utils.py` & `merlin-models-23.6.0/merlin/models/tf/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/tf/utils/testing_utils.py` & `merlin-models-23.6.0/merlin/models/tf/utils/testing_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,14 +209,15 @@
         be tested for this layer. This is only relevant for PreprocessingLayers.
       custom_objects: Optional dictionary mapping name strings to custom objects
         in the layer class. This is helpful for testing custom layers.
       test_harness: The Tensorflow test, if any, that this function is being
         called in.
       supports_masking: Optional boolean to check the `supports_masking`
         property of the layer. If None, the check will not be performed.
+
     Returns:
       The output data (Numpy array) returned by the layer, for additional
       checks to be done by the calling code.
     Raises:
       ValueError: if `input_shape is None`.
     """
     if input_data is None:
```

### Comparing `merlin-models-23.5.0/merlin/models/tf/utils/tf_utils.py` & `merlin-models-23.6.0/merlin/models/tf/utils/tf_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,15 @@
     shuffle_ties : bool, optional
         Adds a small random value to predictions to break ties if any, by default False
     shuffle_ties_epsilon : float, optional
         The maximum random value to be added to break ties (used only if shuffle_ties=True),
         by default 1e-6
     seed : int, optional
         Random seed to use for tie breaking
+
     Returns
     -------
     Tuple(tf.Tensor,tf.Tensor,tf.Tensor)
         Returns a triple with the following tensors
         (topk_predictions,topk_labels,label_relevant_counts).
         The label_relevant_counts holds the total number of positive values per example,
         as some metrics (e.g. recall) need that information, which is lost when we
@@ -356,14 +357,15 @@
     ----------
     item_freq_probs : Union[tf.Tensor, Sequence]
         A Tensor or list with item frequencies (if is_prob_distribution=False)
         or with item probabilities (if is_prob_distribution=True)
     is_prob_distribution: bool, optional
         If True, the item_freq_probs should be a probability distribution of the items.
         If False, the item frequencies is converted to probabilities
+
     Returns
     -------
         A tensor with the item probability distributon
     """
     item_freq_probs = tf.convert_to_tensor(item_freq_probs)
 
     if is_prob_distribution:
@@ -479,14 +481,15 @@
     return tf.RaggedTensor.from_row_splits(values, offsets)
 
 
 def check_inputs_mask_compatible_shape(
     inputs: Union[tf.Tensor, tf.RaggedTensor], mask: Union[tf.Tensor, tf.RaggedTensor]
 ):
     """Check if the shape and the type of the input and mask tensors are compatible.
+
     Parameters
     ----------
     inputs : Union[tf.Tensor, tf.RaggedTensor]
         The input tensor, which can be either a dense or ragged tensor.
     mask : Union[tf.Tensor, tf.RaggedTensor]
         The mask tensor, which can be either a dense or ragged tensor.
```

### Comparing `merlin-models-23.5.0/merlin/models/torch/__init__.py` & `merlin-models-23.6.0/tests/integration/tf/retrieval/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #
-# Copyright (c) 2023, NVIDIA CORPORATION.
+# Copyright (c) 2021, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from merlin.models.torch.batch import Batch, Sequence
-from merlin.models.torch.block import Block, ParallelBlock
+import pytest
 
-__all__ = ["Batch", "Block", "ParallelBlock", "Sequence"]
+pytest.importorskip("wandb")
+pytest.importorskip("fiddle")
```

### Comparing `merlin-models-23.5.0/merlin/models/torch/block.py` & `merlin-models-23.6.0/merlin/models/torch/block.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,29 +18,39 @@
 from typing import Dict, Optional, Union
 
 import torch
 from torch import nn
 
 from merlin.models.torch.batch import Batch
 from merlin.models.torch.container import BlockContainer, BlockContainerDict
+from merlin.models.torch.link import Link, LinkType
+from merlin.models.torch.registry import registry
+from merlin.models.torch.utils.schema_utils import SchemaTrackingMixin
+from merlin.models.utils.registry import RegistryMixin
 
 
-class Block(BlockContainer):
-    """A base-class that calls it's modules sequentially.
+class Block(BlockContainer, SchemaTrackingMixin, RegistryMixin):
+    """A base-class that calls its modules sequentially.
 
     Parameters
     ----------
     *module : nn.Module
         Variable length argument list of PyTorch modules to be contained in the block.
     name : Optional[str], default = None
         The name of the block. If None, no name is assigned.
+    track_schema : bool, default = True
+        If True, the schema of the output tensors are tracked.
     """
 
-    def __init__(self, *module: nn.Module, name: Optional[str] = None):
+    registry = registry
+
+    def __init__(self, *module: nn.Module, name: Optional[str] = None, track_schema: bool = True):
         super().__init__(*module, name=name)
+        if track_schema:
+            self._register_schema_tracking_hook()
 
     def forward(
         self, inputs: Union[torch.Tensor, Dict[str, torch.Tensor]], batch: Optional[Batch] = None
     ):
         """
         Forward pass through the block. Applies each contained module sequentially on the input.
 
@@ -57,15 +67,15 @@
             The output of the block after processing the input.
         """
         for module in self.values:
             inputs = module(inputs, batch=batch)
 
         return inputs
 
-    def repeat(self, n: int = 1, name=None) -> "Block":
+    def repeat(self, n: int = 1, link: Optional[LinkType] = None, name=None) -> "Block":
         """
         Creates a new block by repeating the current block `n` times.
         Each repetition is a deep copy of the current block.
 
         Parameters
         ----------
         n : int
@@ -81,14 +91,17 @@
         if not isinstance(n, int):
             raise TypeError("n must be an integer")
 
         if n < 1:
             raise ValueError("n must be greater than 0")
 
         repeats = [self.copy() for _ in range(n - 1)]
+        if link:
+            parsed_link = Link.parse(link)
+            repeats = [parsed_link.copy().setup_link(repeat) for repeat in repeats]
 
         return Block(self, *repeats, name=name)
 
     def copy(self) -> "Block":
         """
         Creates a deep copy of the current block.
 
@@ -97,15 +110,15 @@
         Block
             The copy of the current block.
         """
         return deepcopy(self)
 
 
 class ParallelBlock(Block):
-    """A base-class that calls it's modules in parallel.
+    """A base-class that calls its modules in parallel.
 
     A ParallelBlock contains multiple branches that will be executed
     in parallel. Each branch can contain multiple modules, and
     the outputs of all branches are collected into a dictionary.
 
     If a branch returns a dictionary of tensors instead of a single tensor,
     it will be flattened into the output dictionary. This ensures the output-type
@@ -126,25 +139,24 @@
 
     Parameters
     ----------
     *module : nn.Module
         Variable length argument list of PyTorch modules to be contained in the block.
     name : Optional[str], default = None
         The name of the block. If None, no name is assigned.
+    track_schema : bool, default = True
+        If True, the schema of the output tensors are tracked.
     """
 
-    def __init__(
-        self,
-        *inputs: Union[nn.Module, Dict[str, nn.Module]],
-    ):
+    def __init__(self, *inputs: Union[nn.Module, Dict[str, nn.Module]], track_schema: bool = True):
         pre = BlockContainer(name="pre")
         branches = BlockContainerDict(*inputs)
         post = BlockContainer(name="post")
 
-        super().__init__()
+        super().__init__(track_schema=track_schema)
 
         self.pre = pre
         self.branches = branches
         self.post = post
 
     def forward(
         self, inputs: Union[torch.Tensor, Dict[str, torch.Tensor]], batch: Optional[Batch] = None
@@ -174,16 +186,20 @@
         """
         for module in self.pre.values:
             inputs = module(inputs, batch=batch)
 
         outputs = {}
         for name, branch_container in self.branches.items():
             branch = inputs
-            for module in branch_container.values:
-                branch = module(branch, batch=batch)
+
+            if hasattr(branch_container, "branches"):
+                branch = branch_container(branch, batch=batch)
+            else:
+                for module in branch_container.values:
+                    branch = module(branch, batch=batch)
 
             if isinstance(branch, torch.Tensor):
                 branch_dict = {name: branch}
             elif torch.jit.isinstance(branch, Dict[str, torch.Tensor]):
                 branch_dict = branch
             else:
                 raise TypeError(
@@ -197,51 +213,38 @@
             outputs.update(branch_dict)
 
         for module in self.post.values:
             outputs = module(outputs, batch=batch)
 
         return outputs
 
-    def append(self, module: nn.Module):
+    def append(self, module: nn.Module, link: Optional[LinkType] = None):
         """Appends a module to the post-processing stage.
 
         Parameters
         ----------
         module : nn.Module
             The module to append.
 
         Returns
         -------
         ParallelBlock
             The current object itself.
         """
 
-        self.post.append(module)
+        self.post.append(module, link=link)
 
         return self
 
     def prepend(self, module: nn.Module):
-        """Prepends a module to the pre-processing stage.
-
-        Parameters
-        ----------
-        module : nn.Module
-            The module to prepend.
-
-        Returns
-        -------
-        ParallelBlock
-            The current object itself.
-        """
-
         self.pre.prepend(module)
 
         return self
 
-    def append_to(self, name: str, module: nn.Module):
+    def append_to(self, name: str, module: nn.Module, link: Optional[LinkType] = None):
         """Appends a module to a specified branch.
 
         Parameters
         ----------
         name : str
             The name of the branch.
         module : nn.Module
@@ -249,38 +252,38 @@
 
         Returns
         -------
         ParallelBlock
             The current object itself.
         """
 
-        self.branches[name].append(module)
+        self.branches[name].append(module, link=link)
 
         return self
 
-    def prepend_to(self, name: str, module: nn.Module):
+    def prepend_to(self, name: str, module: nn.Module, link: Optional[LinkType] = None):
         """Prepends a module to a specified branch.
 
         Parameters
         ----------
         name : str
             The name of the branch.
         module : nn.Module
             The module to prepend.
 
         Returns
         -------
         ParallelBlock
             The current object itself.
         """
-        self.branches[name].prepend(module)
+        self.branches[name].prepend(module, link=link)
 
         return self
 
-    def append_for_each(self, module: nn.Module, shared=False):
+    def append_for_each(self, module: nn.Module, shared=False, link: Optional[LinkType] = None):
         """Appends a module to each branch.
 
         Parameters
         ----------
         module : nn.Module
             The module to append.
         shared : bool, default=False
@@ -289,19 +292,19 @@
 
         Returns
         -------
         ParallelBlock
             The current object itself.
         """
 
-        self.branches.append_for_each(module, shared=shared)
+        self.branches.append_for_each(module, shared=shared, link=link)
 
         return self
 
-    def prepend_for_each(self, module: nn.Module, shared=False):
+    def prepend_for_each(self, module: nn.Module, shared=False, link: Optional[LinkType] = None):
         """Prepends a module to each branch.
 
         Parameters
         ----------
         module : nn.Module
             The module to prepend.
         shared : bool, default=False
@@ -310,15 +313,15 @@
 
         Returns
         -------
         ParallelBlock
             The current object itself.
         """
 
-        self.branches.prepend_for_each(module, shared=shared)
+        self.branches.prepend_for_each(module, shared=shared, link=link)
 
         return self
 
     def __getitem__(self, idx: Union[slice, int, str]):
         if isinstance(idx, str) and idx in self.branches:
             return self.branches[idx]
```

### Comparing `merlin-models-23.5.0/merlin/models/torch/utils/__init__.py` & `merlin-models-23.6.0/merlin/models/tf/distributed/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/torch/utils/torchscript_utils.py` & `merlin-models-23.6.0/merlin/models/torch/utils/torchscript_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         self.to_wrap = to_wrap
         self.accepts_batch, self.requires_batch = module_utils.check_batch_arg(to_wrap)
         self.accepts_dict = module_utils.is_tabular(to_wrap)
 
     def forward(
         self, inputs: Union[torch.Tensor, Dict[str, torch.Tensor]], batch: Optional[Batch] = None
     ):
-        """
+        """Forward pass through the wrapped module with appropriate torchscript type-checking.
 
         Parameters
         ----------
         inputs : Union[torch.Tensor, Dict[str, torch.Tensor]]
             The input tensor(s) for the model.
         batch : Optional[Batch]
             An optional batch object.
```

### Comparing `merlin-models-23.5.0/merlin/models/utils/__init__.py` & `merlin-models-23.6.0/merlin/models/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/constants.py` & `merlin-models-23.6.0/merlin/models/utils/constants.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/dataset.py` & `merlin-models-23.6.0/merlin/models/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/dependencies.py` & `merlin-models-23.6.0/merlin/models/utils/dependencies.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/doc_utils.py` & `merlin-models-23.6.0/merlin/models/utils/doc_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/example_utils.py` & `merlin-models-23.6.0/merlin/models/utils/example_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/misc_utils.py` & `merlin-models-23.6.0/merlin/models/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/nvt_utils.py` & `merlin-models-23.6.0/merlin/models/utils/nvt_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/registry.py` & `merlin-models-23.6.0/merlin/models/utils/registry.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/utils/schema_utils.py` & `merlin-models-23.6.0/merlin/models/utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/merlin/models/xgb/__init__.py` & `merlin-models-23.6.0/merlin/models/xgb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2022, NVIDIA CORPORATION.
+# Copyright (c) 2023, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `merlin-models-23.5.0/merlin_models.egg-info/PKG-INFO` & `merlin-models-23.6.0/merlin_models.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merlin-models
-Version: 23.5.0
+Version: 23.6.0
 Summary: Merlin recommender system models
 Home-page: https://github.com/NVIDIA-Merlin/models
 Author: NVIDIA Corporation
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -33,53 +33,53 @@
 Provides-Extra: all
 License-File: LICENSE
 
 ## Merlin Models
 
 [![PyPI version shields.io](https://img.shields.io/pypi/v/merlin-models.svg)](https://pypi.python.org/pypi/merlin-models/)
 ![GitHub License](https://img.shields.io/github/license/NVIDIA-Merlin/models)
-[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/main/)
+[![Documentation](https://img.shields.io/badge/documentation-blue.svg)](https://nvidia-merlin.github.io/models/)
 
 The Merlin Models library provides standard models for recommender systems with an aim for high-quality implementations
 that range from classic machine learning models to highly-advanced deep learning models.
 
 The goal of this library is to make it easy for users in the industry to train and deploy recommender models with the best
 practices that are already baked into the library. The library simplifies how users in the industry can train standard models against their dataset and put high-performance, GPU-accelerated models into production. The library also enables researchers to build custom
 models by incorporating standard components of deep learning recommender models and then researchers can benchmark the new models on
 example offline
 datasets.
 
 In our initial releases, Merlin Models features a TensorFlow API. The PyTorch API is initiated, but incomplete. We have PyTorch support for transformer-based, session-based recommender systems in the [Transformer4Rec](https://github.com/NVIDIA-Merlin/Transformers4Rec/) library.
 
 ### Benefits of Merlin Models
 
-**[RecSys model implementations](https://nvidia-merlin.github.io/models/main/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
+**[RecSys model implementations](https://nvidia-merlin.github.io/models/stable/models_overview.html)** - The library provides a high-level API for classic and state-of-the-art deep learning architectures for recommender models.
 These models include both retrieval (e.g. Matrix Factorization, Two tower, YouTube DNN, ..) and ranking (e.g. DLRM, DCN-v2, DeepFM, ...) models.
 
 **Building blocks** - Within Merlin Models, recommender models are built on reusable building blocks.
 The design makes it easy to combine the blocks to define new architectures.
 The library provides model definition blocks (MLP layers, factorization layers, input blocks, negative samplers, loss functions), training models (data loaders from Parquet files), and evaluation (e.g. ranking metrics).
 
 **Integration with Merlin platform** - Merlin Models is deeply integrated with the other Merlin components.
 For example, models depend on NVTabular for pre-processing and integrate easily with Merlin Systems for inference.
 The thoughtfully-designed integration makes it straightforward to build performant end-to-end RecSys pipelines.
 
-**[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/main/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
+**[Merlin Models DataLoaders](https://nvidia-merlin.github.io/models/stable/api.html#loader-utility-functions)** - Merlin provides seamless integration with common deep learning frameworks, such as TensorFlow, PyTorch, and HugeCTR.
 When training deep learning recommender system models, data loading can be a bottleneck.
 To address the challenge, Merlin has custom, highly-optimized dataloaders to accelerate existing TensorFlow and PyTorch training pipelines.
 The Merlin dataloaders can lead to a speedup that is nine times faster than the same training pipeline used with the GPU.
 
 With the Merlin dataloaders, you can:
 
 - Remove bottlenecks from data loading by processing large chunks of data at a time instead of item by item.
 - Process datasets that don't fit within the GPU or CPU memory by streaming from the disk.
 - Prepare batches asynchronously into the GPU to avoid CPU-to-GPU communication.
 - Integrate easily into existing TensorFlow or PyTorch training pipelines by using a similar API.
 
-To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/main/models_overview.html) page.
+To learn about the core features of Merlin Models, see the [Models Overview](https://nvidia-merlin.github.io/models/stable/models_overview.html) page.
 
 ### Installation
 
 #### Installing Merlin Models Using Pip
 
 Merlin Models can be installed with `pip` by running the following command:
 
@@ -90,15 +90,15 @@
 > Installing Merlin Models with `pip` does not install some additional GPU dependencies, such as the CUDA Toolkit.
 > When you run Merlin Models in one of our Docker containers, the dependencies are already installed.
 
 #### Docker Containers that include Merlin Models
 
 Merlin Models is included in the Merlin Containers.
 
-Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/main/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
+Refer to the [Merlin Containers](https://nvidia-merlin.github.io/Merlin/stable/containers.html) documentation page for information about the Merlin container names, URLs to the container images on the NVIDIA GPU Cloud catalog, and key Merlin components.
 
 #### Installing Merlin Models from Source
 
 Merlin Models can be installed from source by running the following commands:
 
 ```shell
 git clone https://github.com/NVIDIA-Merlin/models
@@ -106,15 +106,15 @@
 ```
 
 ### Getting Started
 
 Merlin Models makes it straightforward to define architectures that adapt to different input features.
 This adaptability is provided by building on a core feature of the NVTabular library.
 When you use NVTabular for feature engineering, NVTabular creates a schema that identifies the input features.
-You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/main/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
+You can see the `Schema` object in action by looking at the [From ETL to Training RecSys models - NVTabular and Merlin Models integrated example](https://nvidia-merlin.github.io/models/stable/examples/02-Merlin-Models-and-NVTabular-integration.html) example notebook.
 
 You can easily build popular RecSys architectures like [DLRM](http://arxiv.org/abs/1906.00091), as shown in the following code sample.
 After you define the model, you can train and evaluate it with a typical Keras model.
 
 ```python
 import merlin.models.tf as mm
 from merlin.io.dataset import Dataset
@@ -138,19 +138,19 @@
 1.  To build the internal input layer, the model identifies them from the schema object.
     The schema identifies the continuous features and categorical features, for which embedding tables are created.
 2.  To define the body of the architecture, MLP layers are used with configurable dimensions.
 3.  The head of the architecture is created from the chosen task, `BinaryClassificationTask` in this example.
     The target binary feature is also inferred from the schema (i.e., tagged as 'TARGET').
 
 You can find more details and information about a low-level API in our overview of the
-[Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/main/models_overview.html#deep-learning-recommender-model).
+[Deep Learning Recommender Model](https://nvidia-merlin.github.io/models/stable/models_overview.html#deep-learning-recommender-model).
 
 ### Notebook Examples and Tutorials
 
-View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/main/examples/README.html) to help you become familiar with Merlin Models.
+View the example notebooks in the [documentation](https://nvidia-merlin.github.io/models/stable/examples/README.html) to help you become familiar with Merlin Models.
 
 The same notebooks are available in the `examples` directory from the [Merlin Models](https://github.com/NVIDIA-Merlin/models) GitHub repository.
 
 ### Feedback and Support
 
 If you'd like to contribute to the library directly, see the [CONTRIBUTING.md](CONTRIBUTING.md) file.
 We're particularly interested in contributions or feature requests for our feature engineering and preprocessing operations.
```

### Comparing `merlin-models-23.5.0/merlin_models.egg-info/SOURCES.txt` & `merlin-models-23.6.0/merlin_models.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -159,18 +159,34 @@
 merlin/models/tf/utils/search_utils.py
 merlin/models/tf/utils/testing_utils.py
 merlin/models/tf/utils/tf_utils.py
 merlin/models/torch/__init__.py
 merlin/models/torch/batch.py
 merlin/models/torch/block.py
 merlin/models/torch/container.py
+merlin/models/torch/link.py
+merlin/models/torch/registry.py
+merlin/models/torch/router.py
+merlin/models/torch/blocks/__init__.py
+merlin/models/torch/blocks/mlp.py
+merlin/models/torch/models/__init__.py
+merlin/models/torch/models/base.py
+merlin/models/torch/outputs/__init__.py
+merlin/models/torch/outputs/base.py
+merlin/models/torch/outputs/classification.py
+merlin/models/torch/outputs/regression.py
+merlin/models/torch/transforms/__init__.py
+merlin/models/torch/transforms/agg.py
 merlin/models/torch/utils/__init__.py
 merlin/models/torch/utils/module_utils.py
+merlin/models/torch/utils/schema_utils.py
+merlin/models/torch/utils/selection_utils.py
 merlin/models/torch/utils/torchscript_utils.py
 merlin/models/utils/__init__.py
+merlin/models/utils/ci_utils.py
 merlin/models/utils/constants.py
 merlin/models/utils/dataset.py
 merlin/models/utils/dependencies.py
 merlin/models/utils/doc_utils.py
 merlin/models/utils/example_utils.py
 merlin/models/utils/misc_utils.py
 merlin/models/utils/nvt_utils.py
@@ -193,14 +209,15 @@
 requirements/pytorch.txt
 requirements/tensorflow.txt
 requirements/test.txt
 requirements/transformers.txt
 requirements/xgboost.txt
 tests/__init__.py
 tests/conftest.py
+tests/benchmark/test_asvdb_transformers_next_item_prediction.py
 tests/common/__init__.py
 tests/common/tf/__init__.py
 tests/common/tf/tests_utils.py
 tests/common/tf/retrieval/__init__.py
 tests/common/tf/retrieval/retrieval_config.py
 tests/common/tf/retrieval/retrieval_tests_common.py
 tests/common/tf/retrieval/retrieval_utils.py
@@ -320,13 +337,27 @@
 tests/unit/tf/utils/test_batch.py
 tests/unit/tf/utils/test_dataset.py
 tests/unit/tf/utils/test_tf_utils.py
 tests/unit/torch/__init__.py
 tests/unit/torch/test_batch.py
 tests/unit/torch/test_block.py
 tests/unit/torch/test_container.py
+tests/unit/torch/test_link.py
+tests/unit/torch/test_router.py
+tests/unit/torch/blocks/__init__.py
+tests/unit/torch/blocks/test_mlp.py
+tests/unit/torch/models/__init__.py
+tests/unit/torch/models/test_base.py
+tests/unit/torch/outputs/__init__.py
+tests/unit/torch/outputs/test_base.py
+tests/unit/torch/outputs/test_classification.py
+tests/unit/torch/outputs/test_regression.py
+tests/unit/torch/transforms/__init__.py
+tests/unit/torch/transforms/test_agg.py
 tests/unit/torch/utils/__init__.py
 tests/unit/torch/utils/test_module_utils.py
+tests/unit/torch/utils/test_schema_utils.py
+tests/unit/torch/utils/test_selection_utils.py
 tests/unit/torch/utils/test_torchscript_utils.py
 tests/unit/utils/test_schema_utils.py
 tests/unit/xgb/__init__.py
 tests/unit/xgb/test_xgboost.py
```

### Comparing `merlin-models-23.5.0/pyproject.toml` & `merlin-models-23.6.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -57,8 +57,10 @@
     "implicit",
     "xgboost",
     "transformers",
     "horovod",
     "example",
     "integration",
     "unit",
+    "changed",
+    "unchanged"
 ]
```

### Comparing `merlin-models-23.5.0/pytest.ini` & `merlin-models-23.6.0/pytest.ini`

 * *Files 14% similar despite different names*

```diff
@@ -9,7 +9,9 @@
     tensorflow: mark as requiring tensorflow
     torch: mark as requiring torch
     implicit: mark as requiring implicit
     lightfm: mark as requiring lightfm
     xgboost: mark as requiring xgboost
     transformers: mark as requiring transformers
     horovod: mark as requiring horovod
+    changed: mark as requiring changed files
+    always: mark as always running
```

### Comparing `merlin-models-23.5.0/setup.cfg` & `merlin-models-23.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/setup.py` & `merlin-models-23.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/__init__.py` & `merlin-models-23.6.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/common/__init__.py` & `merlin-models-23.6.0/tests/common/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/common/tf/__init__.py` & `merlin-models-23.6.0/tests/common/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/common/tf/retrieval/__init__.py` & `merlin-models-23.6.0/tests/common/tf/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_config.py` & `merlin-models-23.6.0/tests/common/tf/retrieval/retrieval_config.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_tests_common.py` & `merlin-models-23.6.0/tests/common/tf/retrieval/retrieval_tests_common.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/common/tf/retrieval/retrieval_utils.py` & `merlin-models-23.6.0/tests/common/tf/retrieval/retrieval_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/common/tf/tests_utils.py` & `merlin-models-23.6.0/tests/common/tf/tests_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/integration/tf/__init__.py` & `merlin-models-23.6.0/tests/integration/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/integration/tf/retrieval/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/horovod/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #
-# Copyright (c) 2021, NVIDIA CORPORATION.
+# Copyright (c) 2022, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import pytest
 
-pytest.importorskip("wandb")
-pytest.importorskip("fiddle")
+pytest.importorskip("horovod.tensorflow")
```

### Comparing `merlin-models-23.5.0/tests/integration/tf/retrieval/test_integration_retrieval.py` & `merlin-models-23.6.0/tests/integration/tf/retrieval/test_integration_retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/integration/tf/test_ci_01_getting_started.py` & `merlin-models-23.6.0/tests/integration/tf/test_ci_01_getting_started.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/integration/tf/test_ci_02_dataschema.py` & `merlin-models-23.6.0/tests/integration/tf/test_ci_02_dataschema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/integration/tf/test_ci_03_exploring_different_models.py` & `merlin-models-23.6.0/tests/integration/tf/test_ci_03_exploring_different_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/integration/tf/test_ci_04_export_ranking_models.py` & `merlin-models-23.6.0/tests/integration/tf/test_ci_04_export_ranking_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/integration/tf/test_ci_05_export_retrieval_model.py` & `merlin-models-23.6.0/tests/integration/tf/test_ci_05_export_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py` & `merlin-models-23.6.0/tests/integration/tf/test_ci_06_advanced_own_architecture.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/config/test_schema.py` & `merlin-models-23.6.0/tests/unit/config/test_schema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/datasets/test_advertising.py` & `merlin-models-23.6.0/tests/unit/datasets/test_advertising.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/datasets/test_ecommerce.py` & `merlin-models-23.6.0/tests/unit/datasets/test_ecommerce.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     ]
 
 
 @pytest.mark.skipif(
     MAYBE_ALICCP_DATA is None,
     reason="ALI-CCP data is not available, pass it through env variable $DATA_PATH_ALICCP",
 )
-def test_get_alliccp():
+def test_get_aliccp():
     data_path = MAYBE_ALICCP_DATA
 
     nvt_workflow = ecommerce.default_aliccp_transformation(add_target_encoding=False)
     train, valid = ecommerce.get_aliccp(
         data_path, nvt_workflow=nvt_workflow, transformed_name="raw_transform", overwrite=True
     )
 
@@ -100,29 +100,29 @@
     assert isinstance(valid, merlin.io.Dataset)
 
 
 @pytest.mark.skipif(
     MAYBE_ALICCP_DATA is None,
     reason="ALI-CCP data is not available, pass it through env variable $DATA_PATH_ALICCP",
 )
-def test_prepare_alliccp(tmp_path):
+def test_prepare_aliccp(tmp_path):
     data_path = MAYBE_ALICCP_DATA
 
-    ecommerce.prepare_alliccp(data_path, file_size=50, max_num_rows=100, output_dir=tmp_path)
+    ecommerce.prepare_aliccp(data_path, file_size=50, max_num_rows=100, output_dir=tmp_path)
     output_files = list(tmp_path.glob("*/*"))
 
     assert len(output_files) == 2
     assert all(f.name.endswith(".parquet") for f in output_files)
 
 
 @pytest.mark.skipif(
     MAYBE_ALICCP_DATA is None,
     reason="ALI-CCP data is not available, pass it through env variable $DATA_PATH_ALICCP",
 )
-def test_transform_alliccp(tmp_path):
+def test_transform_aliccp(tmp_path):
     data_path = MAYBE_ALICCP_DATA
 
     ecommerce.transform_aliccp(data_path, tmp_path)
     output_files = list(tmp_path.glob("*/*"))
 
     assert len(output_files) == 10
```

### Comparing `merlin-models-23.5.0/tests/unit/datasets/test_entertainment.py` & `merlin-models-23.6.0/tests/unit/datasets/test_entertainment.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/datasets/test_synthetic.py` & `merlin-models-23.6.0/tests/unit/datasets/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/implicit/__init__.py` & `merlin-models-23.6.0/tests/unit/implicit/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/implicit/test_implicit.py` & `merlin-models-23.6.0/tests/unit/implicit/test_implicit.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/lightfm/__init__.py` & `merlin-models-23.6.0/tests/unit/lightfm/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/lightfm/test_lightfm.py` & `merlin-models-23.6.0/tests/unit/lightfm/test_lightfm.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/_conftest.py` & `merlin-models-23.6.0/tests/unit/tf/_conftest.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_base.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/retrieval/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/retrieval/test_matrix_factorization.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/retrieval/test_two_tower.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/retrieval/test_two_tower.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/sampling/test_cross_batch.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/sampling/test_cross_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/sampling/test_in_batch.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/sampling/test_in_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/test_cross.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/test_cross.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/test_dlrm.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/test_dlrm.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/test_interactions.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/test_interactions.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/test_mlp.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/test_mlp.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/blocks/test_optimizer.py` & `merlin-models-23.6.0/tests/unit/tf/blocks/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/core/test_aggregation.py` & `merlin-models-23.6.0/tests/unit/tf/core/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/core/test_base.py` & `merlin-models-23.6.0/tests/unit/tf/core/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/core/test_combinators.py` & `merlin-models-23.6.0/tests/unit/tf/core/test_combinators.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/core/test_encoder.py` & `merlin-models-23.6.0/tests/unit/tf/core/test_encoder.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/core/test_index.py` & `merlin-models-23.6.0/tests/unit/tf/core/test_index.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/core/test_prediction.py` & `merlin-models-23.6.0/tests/unit/tf/core/test_prediction.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/core/test_tabular.py` & `merlin-models-23.6.0/tests/unit/tf/core/test_tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_01_getting_started.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_01_getting_started.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_02_dataschema.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_02_dataschema.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_03_exploring_different_models.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_03_exploring_different_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_04_export_ranking_models.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_04_export_ranking_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_05_export_retrieval_model.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_05_export_retrieval_model.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_06_advanced_own_architecture.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_07_train_traditional_models.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_07_train_traditional_models.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_accelerate_training_by_lazyadam.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_ecommerce_session_based.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_incremental_training_layer_freezing.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_incremental_training_layer_freezing.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_pretrained_embeddings.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_pretrained_embeddings.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_ranking_with_multitask_learning.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_retrieval_with_hpo.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py` & `merlin-models-23.6.0/tests/unit/tf/examples/test_usecase_transformers_next_item_prediction.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,34 +18,32 @@
     execute=False,
 )
 @pytest.mark.notebook
 def test_next_item_prediction(tb, tmpdir):
     tb.inject(
         f"""
         import os, random
+        os.environ["INPUT_DATA_DIR"] = "{tmpdir}"
+        os.environ["OUTPUT_DATA_DIR"] = "{tmpdir}"
         from datetime import datetime, timedelta
         from merlin.datasets.synthetic import generate_data
         ds = generate_data('booking.com-raw', 10000)
         df = ds.compute()
         def generate_date():
             date = datetime.today()
             if random.randint(0, 1):
                 date -= timedelta(days=7)
             return date
         df['checkin'] = [generate_date() for _ in range(df.shape[0])]
         df['checkout'] = [generate_date() for _ in range(df.shape[0])]
         df.to_csv('{tmpdir}/train_set.csv')
         """
     )
-    tb.cells[4].source = tb.cells[4].source.replace("get_booking('/workspace/data')", "")
-    tb.cells[4].source = tb.cells[4].source.replace(
-        "read_csv('/workspace/data/train_set.csv'", f"read_csv('{tmpdir}/train_set.csv'"
-    )
-    tb.cells[31].source = tb.cells[31].source.replace("epochs=5", "epochs=1")
-    tb.cells[37].source = tb.cells[37].source.replace("/workspace/ensemble", f"{tmpdir}/ensemble")
+    tb.cells.pop(6)
+    tb.cells[29].source = tb.cells[29].source.replace("epochs=5", "epochs=1")
     tb.execute_cell(list(range(0, 38)))
 
     with utils.run_triton_server(f"{tmpdir}/ensemble", grpc_port=8001):
         tb.execute_cell(list(range(38, len(tb.cells))))
 
     tb.inject(
         """
```

### Comparing `merlin-models-23.5.0/tests/unit/tf/experimental/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/experimental/test_sample_weight.py` & `merlin-models-23.6.0/tests/unit/tf/experimental/test_sample_weight.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/horovod/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/test_public_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 #
-# Copyright (c) 2022, NVIDIA CORPORATION.
+# Copyright (c) 2021, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
 import pytest
 
-pytest.importorskip("horovod.tensorflow")
+import merlin.models.tf as ml
+
+
+def test_tf_import():
+    pytest.importorskip("tensorflow")
+
+    assert ml is not None
+    assert ml.Model is not None
```

### Comparing `merlin-models-23.5.0/tests/unit/tf/horovod/test_embedding.py` & `merlin-models-23.6.0/tests/unit/tf/horovod/test_embedding.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/horovod/test_horovod.py` & `merlin-models-23.6.0/tests/unit/tf/horovod/test_horovod.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/inputs/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/inputs/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/inputs/test_base.py` & `merlin-models-23.6.0/tests/unit/tf/inputs/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/inputs/test_block.py` & `merlin-models-23.6.0/tests/unit/tf/inputs/test_block.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/inputs/test_continuous.py` & `merlin-models-23.6.0/tests/unit/tf/inputs/test_continuous.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/inputs/test_embedding.py` & `merlin-models-23.6.0/tests/unit/tf/inputs/test_embedding.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/inputs/test_tabular.py` & `merlin-models-23.6.0/tests/unit/tf/inputs/test_tabular.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/layers/test_queue.py` & `merlin-models-23.6.0/tests/unit/tf/layers/test_queue.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/losses/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/losses/test_losses.py` & `merlin-models-23.6.0/tests/unit/tf/losses/test_losses.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/metrics/test_metrics.py` & `merlin-models-23.6.0/tests/unit/tf/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/metrics/test_metrics_topk.py` & `merlin-models-23.6.0/tests/unit/tf/metrics/test_metrics_topk.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/models/test_base.py` & `merlin-models-23.6.0/tests/unit/tf/models/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/models/test_benchmark.py` & `merlin-models-23.6.0/tests/unit/tf/models/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/models/test_ranking.py` & `merlin-models-23.6.0/tests/unit/tf/models/test_ranking.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/models/test_retrieval.py` & `merlin-models-23.6.0/tests/unit/tf/models/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/outputs/test_base.py` & `merlin-models-23.6.0/tests/unit/tf/outputs/test_base.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/outputs/test_block.py` & `merlin-models-23.6.0/tests/unit/tf/outputs/test_block.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/outputs/test_classification.py` & `merlin-models-23.6.0/tests/unit/tf/outputs/test_classification.py`

 * *Files 17% similar despite different names*

```diff
@@ -94,27 +94,28 @@
         "mrr_at_10",
         "recall_at_10",
         "regularization_loss",
     }
 
 
 @pytest.mark.parametrize("run_eagerly", [True, False])
-def test_last_item_prediction(sequence_testing_data: Dataset, run_eagerly):
+@pytest.mark.parametrize("use_bias", [True, False])
+def test_last_item_prediction(sequence_testing_data: Dataset, run_eagerly, use_bias):
     dataloader, schema = testing_utils.loader_for_last_item_prediction(sequence_testing_data)
     embeddings = mm.Embeddings(
         schema,
         sequence_combiner=tf.keras.layers.Lambda(lambda x: tf.reduce_mean(x, axis=1)),
     )
 
     predictions = [
         schema.select_by_name("item_id_seq"),
         schema["item_id_seq"],
         CategoricalTarget(schema["item_id_seq"]),
         embeddings["item_id_seq"],
-        EmbeddingTablePrediction(embeddings["item_id_seq"]),
+        EmbeddingTablePrediction(embeddings["item_id_seq"], use_bias=use_bias),
     ]
 
     for target in predictions:
         model = mm.Model(
             mm.InputBlockV2(schema, categorical=embeddings),
             mm.MLPBlock([8]),
             mm.CategoricalOutput(target),
```

### Comparing `merlin-models-23.5.0/tests/unit/tf/outputs/test_contrastive.py` & `merlin-models-23.6.0/tests/unit/tf/outputs/test_contrastive.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/outputs/test_regression.py` & `merlin-models-23.6.0/tests/unit/tf/outputs/test_regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/outputs/test_sampling.py` & `merlin-models-23.6.0/tests/unit/tf/outputs/test_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/outputs/test_topk.py` & `merlin-models-23.6.0/tests/unit/tf/outputs/test_topk.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import numpy as np
 import pytest
 import tensorflow as tf
 
 
 def test_brute_force_layer():
     from merlin.models.tf.core.prediction import TopKPrediction
     from merlin.models.tf.outputs.topk import BruteForce
@@ -24,14 +25,18 @@
     num_candidates = 1000
     num_queries = 100
     top_k = 5
 
     candidates = tf.random.uniform(shape=(num_candidates, 4), dtype=tf.float32)
     query = tf.random.uniform(shape=(num_queries, 4), dtype=tf.float32)
 
+    # Create a ragged query
+    elements = np.random.rand(num_queries, 1, 4)
+    ragged_query = tf.ragged.constant(elements)
+
     wrong_candidates_rank = tf.random.uniform(shape=(num_candidates,), dtype=tf.float32)
     wrong_query_dim = tf.random.uniform(shape=(num_queries, 8), dtype=tf.float32)
     wrong_identifiers_shape = tf.range(num_candidates + 1, dtype=tf.int32)
 
     brute_force = BruteForce(k=top_k)
 
     with pytest.raises(Exception) as excinfo:
@@ -56,14 +61,17 @@
         brute_force(wrong_query_dim)
     assert "Query and candidates vectors must have the same embedding size" in str(excinfo.value)
 
     topk_output = brute_force(query)
     assert list(topk_output.scores.shape) == [num_queries, top_k]
     assert list(topk_output.identifiers.shape) == [num_queries, top_k]
     assert isinstance(topk_output, TopKPrediction)
+    assert list(topk_output.scores.shape) == [num_queries, top_k]
+    ragged_topk_output = brute_force(ragged_query)
+    assert list(ragged_topk_output.scores.shape) == [num_queries, top_k]
 
     with pytest.raises(Exception) as excinfo:
         brute_force(query, targets=None, testing=True)
     assert "Targets should be provided during the evaluation mode" in str(excinfo.value)
 
     new_candidates = tf.random.uniform(shape=(num_candidates, 4), dtype=tf.float32)
     brute_force.index(candidates=new_candidates)
```

### Comparing `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_classification.py` & `merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_classification.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_multi_task.py` & `merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_multi_task.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_next_item.py` & `merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_next_item.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_regression.py` & `merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_regression.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_retrieval.py` & `merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_retrieval.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/prediction_tasks/test_sampling.py` & `merlin-models-23.6.0/tests/unit/tf/prediction_tasks/test_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/test_core.py` & `merlin-models-23.6.0/tests/unit/tf/test_core.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/test_loader.py` & `merlin-models-23.6.0/tests/unit/tf/test_loader.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/test_public_api.py` & `merlin-models-23.6.0/tests/unit/torch/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,18 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
 import pytest
 
-import merlin.models.tf as ml
-
-
-def test_tf_import():
-    pytest.importorskip("tensorflow")
-
-    assert ml is not None
-    assert ml.Model is not None
+pytest.importorskip("torch")
```

### Comparing `merlin-models-23.5.0/tests/unit/tf/transformers/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/transformers/test_block.py` & `merlin-models-23.6.0/tests/unit/tf/transformers/test_block.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,17 +75,17 @@
 
     query_embeddings = query_encoder.predict(loader)
     assert list(query_embeddings.shape) == [100, d_model]
 
     item_embeddings = model.candidate_embeddings().compute().to_numpy()
 
     assert list(item_embeddings.shape) == [101, d_model]
-    predicitons_2 = np.dot(query_embeddings, item_embeddings.T)
+    predictions_2 = tf.matmul(query_embeddings, tf.transpose(item_embeddings)).numpy()
 
-    np.testing.assert_allclose(predictions, predicitons_2, atol=1e-3)
+    np.testing.assert_allclose(predictions, predictions_2, atol=1e-4)
 
 
 def test_transformer_encoder():
     NUM_ROWS = 100
     SEQ_LENGTH = 10
     EMBED_DIM = 128
```

### Comparing `merlin-models-23.5.0/tests/unit/tf/transformers/test_transforms.py` & `merlin-models-23.6.0/tests/unit/tf/transformers/test_transforms.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/transforms/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/transforms/test_bias.py` & `merlin-models-23.6.0/tests/unit/tf/transforms/test_bias.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/transforms/test_features.py` & `merlin-models-23.6.0/tests/unit/tf/transforms/test_features.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/transforms/test_negative_sampling.py` & `merlin-models-23.6.0/tests/unit/tf/transforms/test_negative_sampling.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/transforms/test_noise.py` & `merlin-models-23.6.0/tests/unit/tf/transforms/test_noise.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/transforms/test_sequence.py` & `merlin-models-23.6.0/tests/unit/tf/transforms/test_sequence.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/transforms/test_tensor.py` & `merlin-models-23.6.0/tests/unit/tf/transforms/test_tensor.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/utils/__init__.py` & `merlin-models-23.6.0/tests/unit/tf/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/utils/test_batch.py` & `merlin-models-23.6.0/tests/unit/tf/utils/test_batch.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/utils/test_dataset.py` & `merlin-models-23.6.0/tests/unit/tf/utils/test_dataset.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/tf/utils/test_tf_utils.py` & `merlin-models-23.6.0/tests/unit/tf/utils/test_tf_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/torch/__init__.py` & `merlin-models-23.6.0/tests/unit/xgb/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+
 import pytest
 
-pytest.importorskip("torch")
+pytest.importorskip("xgboost")
```

### Comparing `merlin-models-23.5.0/tests/unit/torch/test_batch.py` & `merlin-models-23.6.0/tests/unit/torch/test_batch.py`

 * *Files 24% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
 import torch
 
-from merlin.models.torch.batch import Batch, Sequence
+from merlin.dataloader.torch import Loader
+from merlin.models.torch.batch import Batch, Sequence, sample_batch, sample_features
 
 
 class TestSequence:
     @pytest.fixture
     def sequence(self):
         lengths = {"feature1": torch.tensor([4, 5]), "feature2": torch.tensor([3, 7])}
         masks = {
@@ -52,14 +53,15 @@
         # Test when lengths is a tensor
         lengths = torch.tensor([1.0])
         sequence = Sequence(lengths)
 
         assert isinstance(sequence.lengths, dict)
         assert "default" in sequence.lengths
         assert torch.equal(sequence.lengths["default"], lengths)
+        assert sequence.device() == lengths.device
 
     def test_init_tensor_masks(self):
         # Test when masks is a tensor
         lengths = torch.tensor([1.0])
         masks = torch.tensor([2.0])
         sequence = Sequence(lengths, masks)
 
@@ -86,14 +88,20 @@
         # Test when masks is not a tensor nor a dictionary of tensors
         lengths = torch.tensor([1.0])
         masks = "invalid_masks"
 
         with pytest.raises(ValueError, match="Masks must be a tensor or a dictionary of tensors"):
             Sequence(lengths, masks)
 
+    def test_device(self):
+        empty_seq = Sequence({})
+
+        with pytest.raises(ValueError, match="Sequence is empty"):
+            empty_seq.device()
+
 
 class TestBatch:
     @pytest.fixture
     def batch(self):
         features = {"feature1": torch.tensor([1, 2]), "feature2": torch.tensor([3, 4])}
         targets = {"target1": torch.tensor([0, 1])}
         lengths = {"feature1": torch.tensor([4, 5]), "feature2": torch.tensor([3, 7])}
@@ -124,14 +132,15 @@
         features = torch.tensor([1.0])
         targets = torch.tensor([2.0])
         batch = Batch(features, targets)
 
         assert isinstance(batch.targets, dict)
         assert "default" in batch.targets
         assert torch.equal(batch.targets["default"], targets)
+        assert batch.device() == features.device
 
     def test_batch_init_invalid_targets(self):
         # Test when targets is not a tensor nor a dictionary of tensors
         features = torch.tensor([1.0])
         targets = "invalid_target"
 
         with pytest.raises(ValueError, match="Targets must be a tensor or a dictionary of tensors"):
@@ -151,7 +160,78 @@
         assert bool(batch)
         empty_batch = Batch({}, {})
         assert not bool(empty_batch)
 
     def test_with_incorrect_types(self):
         with pytest.raises(ValueError):
             Batch("not a tensor or dict", "not a tensor or dict", "not a sequence")
+
+    def test_sample(self, music_streaming_data):
+        batch = Batch.sample_from(music_streaming_data)
+        assert isinstance(batch, Batch)
+
+        assert isinstance(batch.features, dict)
+        assert len(list(batch.features.keys())) == 12
+        for key, val in batch.features.items():
+            if not key.endswith("__values") and not key.endswith("__offsets"):
+                assert val.shape[0] == 32
+
+        assert isinstance(batch.targets, dict)
+        assert list(batch.targets.keys()) == ["click", "play_percentage", "like"]
+        for val in batch.targets.values():
+            assert val.shape[0] == 32
+
+    def test_device(self):
+        empty_batch = Batch({}, {})
+
+        with pytest.raises(ValueError, match="Batch is empty"):
+            empty_batch.device()
+
+
+class Test_sample_batch:
+    def test_loader(self, music_streaming_data):
+        loader = Loader(music_streaming_data, batch_size=2)
+
+        batch = sample_batch(loader)
+
+        assert isinstance(batch.features, dict)
+        assert len(list(batch.features.keys())) == 12
+        for key, val in batch.features.items():
+            if not key.endswith("__values") and not key.endswith("__offsets"):
+                assert val.shape[0] == 2
+
+        assert isinstance(batch.targets, dict)
+        assert list(batch.targets.keys()) == ["click", "play_percentage", "like"]
+        for val in batch.targets.values():
+            assert val.shape[0] == 2
+
+    def test_dataset(self, music_streaming_data):
+        batch = sample_batch(music_streaming_data, batch_size=2)
+
+        assert isinstance(batch.features, dict)
+        assert len(list(batch.features.keys())) == 12
+        for key, val in batch.features.items():
+            if not key.endswith("__values") and not key.endswith("__offsets"):
+                assert val.shape[0] == 2
+
+        assert isinstance(batch.targets, dict)
+        assert list(batch.targets.keys()) == ["click", "play_percentage", "like"]
+        for val in batch.targets.values():
+            assert val.shape[0] == 2
+
+    def test_exceptions(self, music_streaming_data):
+        with pytest.raises(ValueError, match="specify 'batch_size'"):
+            sample_batch(music_streaming_data)
+
+        with pytest.raises(ValueError, match="Expected Dataset or Loader instance"):
+            sample_batch(torch.tensor([1, 2, 3]))
+
+
+class Test_sample_features:
+    def test_no_targets(self, music_streaming_data):
+        features = sample_features(music_streaming_data, batch_size=2)
+
+        assert isinstance(features, dict)
+        assert len(list(features.keys())) == 12
+        for key, val in features.items():
+            if not key.endswith("__values") and not key.endswith("__offsets"):
+                assert val.shape[0] == 2
```

### Comparing `merlin-models-23.5.0/tests/unit/torch/test_block.py` & `merlin-models-23.6.0/tests/unit/torch/test_block.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,18 +15,20 @@
 #
 from typing import Dict, Tuple
 
 import pytest
 import torch
 from torch import nn
 
+from merlin.models.torch import link
 from merlin.models.torch.batch import Batch
 from merlin.models.torch.block import Block, ParallelBlock
 from merlin.models.torch.container import BlockContainer, BlockContainerDict
 from merlin.models.torch.utils import module_utils
+from merlin.schema import Tags
 
 
 class PlusOne(nn.Module):
     def forward(self, inputs: torch.Tensor) -> torch.Tensor:
         return inputs + 1
 
 
@@ -45,24 +47,35 @@
         block = Block()
 
         inputs = torch.tensor([[1.0, 2.0], [3.0, 4.0]])
         outputs = module_utils.module_test(block, inputs, batch=Batch(inputs))
 
         assert torch.equal(inputs, outputs)
 
+        schema = block.output_schema()
+        assert schema.first.dtype.name == str(outputs.dtype).split(".")[-1]
+
+    def test_no_schema_tracking(self):
+        block = Block(track_schema=False)
+        with pytest.raises(RuntimeError, match="Schema-tracking hook not registered"):
+            block.output_schema()
+
     def test_insertion(self):
         block = Block()
         block.prepend(PlusOne())
         block.append(PlusOne())
 
         inputs = torch.tensor([[1.0, 2.0], [3.0, 4.0]])
         outputs = module_utils.module_test(block, inputs, batch=Batch(inputs))
 
         assert torch.equal(outputs, inputs + 2)
 
+        block.append(PlusOne(), link="residual")
+        assert isinstance(block[-1], link.Residual)
+
     def test_copy(self):
         block = Block(PlusOne())
 
         copied = block.copy()
         assert isinstance(copied, Block)
         assert isinstance(copied[0], PlusOne)
         assert copied != block
@@ -78,14 +91,41 @@
 
         with pytest.raises(TypeError, match="n must be an integer"):
             block.repeat("invalid_input")
 
         with pytest.raises(ValueError, match="n must be greater than 0"):
             block.repeat(0)
 
+    def test_repeat_with_link(self):
+        block = Block(PlusOne())
+
+        repeated = block.repeat(2, link="residual")
+        assert isinstance(repeated, Block)
+        assert len(repeated) == 2
+        assert isinstance(repeated[-1], link.Residual)
+
+        inputs = torch.tensor([[1.0, 2.0], [3.0, 4.0]])
+        outputs = module_utils.module_test(repeated, inputs)
+
+        assert torch.equal(outputs, (inputs + 1) + (inputs + 1) + 1)
+
+    def test_from_registry(self):
+        @Block.registry.register("my_block")
+        class MyBlock(Block):
+            def forward(self, inputs):
+                _inputs = inputs + 1
+
+                return super().forward(_inputs)
+
+        block = Block.parse("my_block")
+        assert block.__class__ == MyBlock
+
+        inputs = torch.randn(1, 3)
+        assert torch.equal(block(inputs), inputs + 1)
+
 
 class TestParallelBlock:
     def test_init(self):
         pb = ParallelBlock({"test": PlusOne()})
         assert isinstance(pb, ParallelBlock)
         assert isinstance(pb.pre, BlockContainer)
         assert isinstance(pb.branches, BlockContainerDict)
@@ -113,14 +153,28 @@
     def test_forward_dict_duplicate(self):
         inputs = {"a": torch.randn(1, 3)}
         pb = ParallelBlock({"1": PlusOneDict(), "2": PlusOneDict()})
 
         with pytest.raises(RuntimeError):
             pb(inputs)
 
+    def test_schema_tracking(self):
+        pb = ParallelBlock({"a": PlusOne(), "b": PlusOne()})
+
+        inputs = torch.randn(1, 3)
+        outputs = pb(inputs)
+
+        schema = pb.output_schema()
+
+        for name in outputs:
+            assert name in schema.column_names
+            assert schema[name].dtype.name == str(outputs[name].dtype).split(".")[-1]
+
+        assert len(schema.select_by_tag(Tags.EMBEDDING)) == 2
+
     def test_forward_tuple(self):
         inputs = torch.randn(1, 3)
         pb = ParallelBlock({"test": PlusOneTuple()})
         with pytest.raises(RuntimeError):
             module_utils.module_test(pb, inputs)
 
     def test_append(self):
```

### Comparing `merlin-models-23.5.0/tests/unit/torch/test_container.py` & `merlin-models-23.6.0/tests/unit/torch/test_container.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,18 +11,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 import pytest
+import torch
 import torch.nn as nn
 
+from merlin.models.torch import link
 from merlin.models.torch.container import BlockContainer, BlockContainerDict
-from merlin.models.torch.utils import torchscript_utils
+from merlin.models.torch.utils import module_utils, torchscript_utils
 
 
 class TestBlockContainer:
     def setup_method(self):
         self.block_container = BlockContainer(name="test_container")
 
     def test_init(self):
@@ -30,30 +32,60 @@
         assert self.block_container._name == "test_container"
 
     def test_append(self):
         module = nn.Linear(20, 30)
         self.block_container.append(module)
         assert len(self.block_container) == 1
 
+    def test_append_link(self):
+        module = nn.Linear(20, 20)
+        self.block_container.append(module, link="residual")
+        assert len(self.block_container) == 1
+
+        inputs = torch.randn(1, 20)
+        outputs = module_utils.module_test(self.block_container[0], inputs)
+
+        assert torch.equal(inputs + module(inputs), outputs)
+
     def test_prepend(self):
         module1 = nn.Linear(20, 30)
         module2 = nn.Linear(30, 40)
         self.block_container.append(module1)
         self.block_container.prepend(module2)
         assert len(self.block_container) == 2
         assert isinstance(self.block_container[0], nn.Linear)
 
+    def test_prepend_link(self):
+        module = nn.Linear(20, 20)
+        self.block_container.prepend(module, link="residual")
+        assert len(self.block_container) == 1
+
+        inputs = torch.randn(1, 20)
+        outputs = module_utils.module_test(self.block_container[0], inputs)
+
+        assert torch.equal(inputs + module(inputs), outputs)
+
     def test_insert(self):
         module1 = nn.Linear(20, 30)
         module2 = nn.Linear(30, 40)
         self.block_container.append(module1)
         self.block_container.insert(0, module2)
         assert len(self.block_container) == 2
         assert isinstance(self.block_container[0], nn.Linear)
 
+    def test_insert_link(self):
+        module = nn.Linear(20, 20)
+        self.block_container.insert(0, module, link="residual")
+        assert len(self.block_container) == 1
+
+        inputs = torch.randn(1, 20)
+        outputs = module_utils.module_test(self.block_container[0], inputs)
+
+        assert torch.equal(inputs + module(inputs), outputs)
+
     def test_len(self):
         module = nn.Linear(20, 30)
         self.block_container.append(module)
         assert len(self.block_container) == 1
 
     def test_getitem(self):
         module = nn.Linear(20, 30)
@@ -150,38 +182,52 @@
         with pytest.raises(ValueError):
             BlockContainerDict({"test": "not a module"})
 
     def test_append_to(self):
         self.container.append_to("test", self.module)
         assert "test" in self.container._modules
 
+        self.container.append_to("test", self.module, link="residual")
+        assert isinstance(self.container["test"][-1], link.Residual)
+
     def test_prepend_to(self):
         self.container.prepend_to("test", self.module)
         assert "test" in self.container._modules
 
+        self.container.prepend_to("test", self.module, link="residual")
+        assert isinstance(self.container["test"][0], link.Residual)
+
     def test_append_for_each(self):
         container = BlockContainerDict({"a": nn.Module(), "b": nn.Module()})
 
         to_add = nn.Module()
         container.append_for_each(to_add)
         assert len(container["a"]) == 2
         assert len(container["b"]) == 2
         assert container["a"][-1] != container["b"][-1]
 
         container.append_for_each(to_add, shared=True)
         assert len(container["a"]) == 3
         assert len(container["b"]) == 3
         assert container["a"][-1] == container["b"][-1]
 
+        container.append_for_each(to_add, link="residual")
+        assert isinstance(container["a"][-1], link.Residual)
+        assert isinstance(container["b"][-1], link.Residual)
+
     def test_prepend_for_each(self):
         container = BlockContainerDict({"a": nn.Module(), "b": nn.Module()})
 
         to_add = nn.Module()
         container.prepend_for_each(to_add)
         assert len(container["a"]) == 2
         assert len(container["b"]) == 2
         assert container["a"][0] != container["b"][0]
 
         container.prepend_for_each(to_add, shared=True)
         assert len(container["a"]) == 3
         assert len(container["b"]) == 3
         assert container["a"][0] == container["b"][0]
+
+        container.prepend_for_each(to_add, link="residual")
+        assert isinstance(container["a"][0], link.Residual)
+        assert isinstance(container["b"][0], link.Residual)
```

### Comparing `merlin-models-23.5.0/tests/unit/torch/utils/test_module_utils.py` & `merlin-models-23.6.0/tests/unit/torch/utils/test_module_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,34 +10,46 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-from typing import Dict
+from typing import Dict, Union
 
 import pytest
 import torch
 from torch import nn
 
 from merlin.models.torch.batch import Batch, Sequence
+from merlin.models.torch.block import ParallelBlock
 from merlin.models.torch.utils.module_utils import (
     _all_close_dict,
     check_batch_arg,
+    find_all_instances,
     is_tabular,
     module_test,
 )
 
 
 class ModuleWithDict(nn.Module):
     def forward(self, x: Dict[str, torch.Tensor]):
         pass
 
 
+class ModuleWithDictUnion(nn.Module):
+    def forward(self, x: Union[Dict[str, torch.Tensor], torch.Tensor]):
+        pass
+
+
+class ModuleWithDictUnion2(nn.Module):
+    def forward(self, x: Union[torch.Tensor, Dict[str, torch.Tensor]]):
+        pass
+
+
 class ModuleWithBatch(nn.Module):
     def forward(self, x, batch=None):
         pass
 
 
 class ModuleWithBatchRequired(nn.Module):
     def forward(self, x, batch):
@@ -53,14 +65,21 @@
     def test_basic(self):
         module_with_dict = ModuleWithDict()
         module_without_dict = ModuleWithoutDict()
 
         assert is_tabular(module_with_dict)
         assert not is_tabular(module_without_dict)
 
+    def test_union(self):
+        module_with_dict_union = ModuleWithDictUnion()
+        module_with_dict_union2 = ModuleWithDictUnion2()
+
+        assert is_tabular(module_with_dict_union)
+        assert is_tabular(module_with_dict_union2)
+
 
 class Test_check_batch_arg:
     def test_basic(self):
         module_with_batch = ModuleWithBatch()
         module_without_batch = ModuleWithoutDict()
         module_with_batch_required = ModuleWithBatchRequired()
 
@@ -204,7 +223,69 @@
         module = TupleOutput()
         input_data = torch.tensor([1.0])
 
         with pytest.raises(
             ValueError, match="The outputs of the original and scripted modules are not the same"
         ):
             module_test(module, input_data, method="script")
+
+
+class TestFindAllInstances:
+    def test_find_all_instances_base(self):
+        class SomeBlock(nn.Module):
+            ...
+
+        class OtherBlock(nn.Module):
+            ...
+
+        some_block = SomeBlock()
+        other_block = OtherBlock()
+
+        assert len(find_all_instances(SomeBlock, SomeBlock)) == 1
+        assert len(find_all_instances(some_block, SomeBlock)) == 1
+        assert len(find_all_instances(some_block, some_block)) == 1
+        assert len(find_all_instances(some_block, OtherBlock)) == 0
+        assert len(find_all_instances(some_block, other_block)) == 0
+
+    def test_find_all_instances_module_list(self):
+        class ToFind(nn.Module):
+            ...
+
+        class NotToFind(nn.Module):
+            ...
+
+        block = torch.nn.ModuleList(
+            [
+                ToFind(),
+                NotToFind(),
+                ToFind(),
+                NotToFind(),
+                ToFind(),
+            ]
+        )
+        assert len(find_all_instances(block, ToFind)) == 3
+
+    def test_find_all_instances_nested(self):
+        class ToFind(nn.Module):
+            ...
+
+        class NotToFind(nn.Module):
+            ...
+
+        block = ParallelBlock(
+            {
+                "a": NotToFind(),
+                "b": ParallelBlock(
+                    {
+                        "c": NotToFind(),
+                        "d": ToFind(),
+                        "e": ParallelBlock(
+                            {
+                                "f": ToFind(),
+                            }
+                        ),
+                    }
+                ),
+                "g": ToFind(),
+            }
+        )
+        assert len(find_all_instances(block, ToFind)) == 3
```

### Comparing `merlin-models-23.5.0/tests/unit/torch/utils/test_torchscript_utils.py` & `merlin-models-23.6.0/tests/unit/torch/utils/test_torchscript_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/utils/test_schema_utils.py` & `merlin-models-23.6.0/tests/unit/utils/test_schema_utils.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tests/unit/xgb/__init__.py` & `merlin-models-23.6.0/merlin/models/torch/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,15 @@
 #
-# Copyright (c) 2021, NVIDIA CORPORATION.
+# Copyright (c) 2023, NVIDIA CORPORATION.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-
-import pytest
-
-pytest.importorskip("xgboost")
```

### Comparing `merlin-models-23.5.0/tests/unit/xgb/test_xgboost.py` & `merlin-models-23.6.0/tests/unit/xgb/test_xgboost.py`

 * *Files identical despite different names*

### Comparing `merlin-models-23.5.0/tox.ini` & `merlin-models-23.6.0/tox.ini`

 * *Files 17% similar despite different names*

```diff
@@ -8,112 +8,112 @@
 commands =
     pip install --upgrade pip
     pip install -e .[all]
 
 [testenv:py38-gpu]
 ; Runs in: Github Actions
 ; Runs GPU-based tests.
+allowlist_externals =
+    bash
 deps =
     --no-deps -rrequirements/test.txt
+passenv =
+    OPAL_PREFIX
 setenv =
     TF_GPU_ALLOCATOR=cuda_malloc_async
 sitepackages=true
 commands =
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/systems.git@{posargs:main}
-    python -m pytest --cov-report term --cov merlin -rxs tests/unit/
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/systems.git@{env:MERLIN_BRANCH:main}
+    bash -c 'python -m pytest --cov-report term --cov merlin -m "{env:PYTEST_MARKERS}" -rxs tests/ || ([ $? = 5 ] && exit 0 || exit $?)'
 
 [testenv:py38-multi-gpu]
 ; Runs in: Github Actions
 ; Runs GPU-based tests.
 allowlist_externals =
     horovodrun
     sh
-#deps =
-#    -rrequirements/test.txt
+    bash
 passenv =
     OPAL_PREFIX
 setenv =
     TF_GPU_ALLOCATOR=cuda_malloc_async
     CPATH={env:CPATH}{:}{envdir}/hugectr/include
     LD_LIBRARY_PATH=${envdir}/hugectr/include/lib{:}/usr/local/lib/python3.8/dist-packages/tensorflow{:}{env:LD_LIBRARY_PATH}
     LIBRARY_PATH=${envdir}/hugectr/lib{:}{env:LIBRARY_PATH}
 sitepackages=true
 commands =
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git@{posargs:main}
-    # TODO: Move SOK installation to ci-runner dockerfile
-    # Install SOK
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git@{env:MERLIN_BRANCH:main}
     sh examples/usecases/multi-gpu/install_sparse_operation_kit.sh {envdir}
-    # Run multi-gpu tests marked with `horovod` marker
-    horovodrun -np 2 sh examples/usecases/multi-gpu/hvd_wrapper.sh python -m pytest -m horovod -rxs tests/unit
+    bash -c 'horovodrun -np 2 sh examples/usecases/multi-gpu/hvd_wrapper.sh python -m pytest -m "horovod {env:EXTRA_PYTEST_MARKERS}" -rxs tests/unit || ([ $? = 5 ] && exit 0 || exit $?)'
 
 [testenv:py38-horovod-cpu]
 setenv =
     HOROVOD_WITH_MPI=1
     HOROVOD_WITH_TENSORFLOW=1
     PATH={env:PATH}{:}{envdir}/env/bin
     LD_LIBRARY_PATH={env:LD_LIBRARY_PATH}{:}{envdir}/env/lib
 commands =
     conda update --yes --name base --channel defaults conda
     conda env create --prefix {envdir}/env --file requirements/horovod-cpu-environment.yml --force
     {envdir}/env/bin/python -m pip install 'horovod==0.27.0' --no-cache-dir
     {envdir}/env/bin/horovodrun --check-build
-    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git
-    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git    
-    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git    
-    {envdir}/env/bin/horovodrun -np 2 sh examples/usecases/multi-gpu/hvd_wrapper.sh pytest -m horovod -rxs tests/unit
+    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{env:MERLIN_BRANCH:main}
+    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{env:MERLIN_BRANCH:main}
+    {envdir}/env/bin/python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/nvtabular.git@{env:MERLIN_BRANCH:main}
+    {envdir}/env/bin/horovodrun -np 2 sh examples/usecases/multi-gpu/hvd_wrapper.sh pytest -m "horovod {env:EXTRA_PYTEST_MARKERS}" -rxs tests/unit
 
 [testenv:py38-nvtabular-cpu]
 passenv=GIT_COMMIT
 allowlist_externals = git
 deps =
     -rrequirements/base.txt
     -rrequirements/dev.txt
 commands =
     ; the GIT_COMMIT env is the current commit of the models repo
-    git clone --depth 1 --branch {posargs:main} https://github.com/NVIDIA-Merlin/NVTabular.git nvtabular-{env:GIT_COMMIT}
+    git clone --depth 1 --branch {env:MERLIN_BRANCH:main} https://github.com/NVIDIA-Merlin/NVTabular.git nvtabular-{env:GIT_COMMIT}
     python -m pip install --upgrade "./nvtabular-{env:GIT_COMMIT}"
     python -m pip install --upgrade -r "./nvtabular-{env:GIT_COMMIT}/requirements/test.txt"
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}    
-    python -m pip install .    
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{env:MERLIN_BRANCH:main}
+    python -m pip install .
     python -m pytest nvtabular-{env:GIT_COMMIT}/tests/unit
 
 [testenv:py38-systems-cpu]
 passenv=GIT_COMMIT
 allowlist_externals = git
 deps =
     -rrequirements/base.txt
     -rrequirements/dev.txt
 commands =
     ; the GIT_COMMIT env is the current commit of the models repo
-    git clone --depth 1 --branch {posargs:main} https://github.com/NVIDIA-Merlin/systems.git systems-{env:GIT_COMMIT}
+    git clone --depth 1 --branch {env:MERLIN_BRANCH:main} https://github.com/NVIDIA-Merlin/systems.git systems-{env:GIT_COMMIT}
     python -m pip install --upgrade "./systems-{env:GIT_COMMIT}"
     python -m pip install --upgrade -r "./systems-{env:GIT_COMMIT}/requirements/test-cpu.txt"
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
-    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/NVTabular.git@{posargs:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/NVTabular.git@{env:MERLIN_BRANCH:main}
     python -m pip install .
     python -m pytest -m "not notebook" systems-{env:GIT_COMMIT}/tests/unit
 
 [testenv:py38-transformers4rec-cpu]
 passenv=GIT_COMMIT
 allowlist_externals = git
 commands =
     ; the GIT_COMMIT env is the current commit of the models repo
-    git clone --depth 1 --branch {posargs:main} https://github.com/NVIDIA-Merlin/Transformers4Rec.git Transformers4Rec-{env:GIT_COMMIT}
+    git clone --depth 1 --branch {env:MERLIN_BRANCH:main} https://github.com/NVIDIA-Merlin/Transformers4Rec.git Transformers4Rec-{env:GIT_COMMIT}
     python -m pip install --upgrade -r "./Transformers4Rec-{env:GIT_COMMIT}/requirements/test.txt"
     python -m pip install --upgrade "./Transformers4Rec-{env:GIT_COMMIT}"
-    python -m pip install --no-deps git+https://github.com/NVIDIA-Merlin/core.git@{posargs:main}
-    python -m pip install --no-deps git+https://github.com/NVIDIA-Merlin/dataloader.git@{posargs:main}
-    python -m pip install --no-deps .
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/core.git@{env:MERLIN_BRANCH:main}
+    python -m pip install --upgrade git+https://github.com/NVIDIA-Merlin/dataloader.git@{env:MERLIN_BRANCH:main}
+    python -m pip install .
     python -m pytest Transformers4Rec-{env:GIT_COMMIT}/tests/unit
 
 [testenv:docs]
 ; Runs in: Github Actions
 ; Generates documentation with sphinx. There are other steps in the Github Actions workflow
 ; to publish the documentation on release.
 changedir = {toxinidir}
```

### Comparing `merlin-models-23.5.0/versioneer.py` & `merlin-models-23.6.0/versioneer.py`

 * *Files identical despite different names*

