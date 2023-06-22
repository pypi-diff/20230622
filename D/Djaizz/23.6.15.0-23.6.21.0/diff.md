# Comparing `tmp/Djaizz-23.6.15.0.tar.gz` & `tmp/Djaizz-23.6.21.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Djaizz-23.6.15.0.tar", last modified: Thu Jun 15 17:48:56 2023, max compression
+gzip compressed data, was "Djaizz-23.6.21.0.tar", last modified: Thu Jun 22 00:52:38 2023, max compression
```

## Comparing `Djaizz-23.6.15.0.tar` & `Djaizz-23.6.21.0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.640157 Djaizz-23.6.15.0/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1092 2023-02-09 04:49:59.000000 Djaizz-23.6.15.0/LICENSE
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-15 17:48:56.639834 Djaizz-23.6.15.0/PKG-INFO
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      187 2023-02-28 01:51:17.000000 Djaizz-23.6.15.0/README.md
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.495182 Djaizz-23.6.15.0/metadata/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2584 2023-03-09 04:40:50.000000 Djaizz-23.6.15.0/metadata/classifiers
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       52 2023-02-28 04:56:41.000000 Djaizz-23.6.15.0/metadata/description
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       65 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/metadata/entry-points
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.496548 Djaizz-23.6.15.0/metadata/requirements/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     6496 2023-06-15 17:26:24.000000 Djaizz-23.6.15.0/metadata/requirements/base.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       16 2023-02-28 04:56:41.000000 Djaizz-23.6.15.0/metadata/requirements/build.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       40 2023-06-14 20:47:00.000000 Djaizz-23.6.15.0/metadata/requirements/dev.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      215 2023-06-14 21:42:52.000000 Djaizz-23.6.15.0/metadata/requirements/doc.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      225 2023-06-14 19:57:11.000000 Djaizz-23.6.15.0/metadata/requirements/lint.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       15 2023-02-28 04:56:41.000000 Djaizz-23.6.15.0/metadata/requirements/publish.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       85 2023-06-13 01:17:31.000000 Djaizz-23.6.15.0/metadata/requirements/test.txt
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)      150 2023-06-13 01:17:55.000000 Djaizz-23.6.15.0/metadata/requirements/viz.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       10 2023-06-15 17:26:33.000000 Djaizz-23.6.15.0/metadata/version
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3129 2023-06-14 20:38:47.000000 Djaizz-23.6.15.0/pyproject.toml
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-06-15 17:48:56.640246 Djaizz-23.6.15.0/setup.cfg
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.487714 Djaizz-23.6.15.0/src/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.497726 Djaizz-23.6.15.0/src/Djaizz.egg-info/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/PKG-INFO
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5814 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/SOURCES.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/dependency_links.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       50 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/entry_points.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     3924 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/requires.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        7 2023-06-15 17:48:56.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/top_level.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-03-01 01:27:25.000000 Djaizz-23.6.15.0/src/Djaizz.egg-info/zip-safe
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.500050 Djaizz-23.6.15.0/src/djaizz/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      300 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.500618 Djaizz-23.6.15.0/src/djaizz/client/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      270 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/client/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.502615 Djaizz-23.6.15.0/src/djaizz/data/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      873 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/admin.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.503120 Djaizz-23.6.15.0/src/djaizz/data/api/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      816 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/api/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.503618 Djaizz-23.6.15.0/src/djaizz/data/api/gql/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/api/gql/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.503771 Djaizz-23.6.15.0/src/djaizz/data/api/json/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/api/json/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.503898 Djaizz-23.6.15.0/src/djaizz/data/api/rest/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/api/rest/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2703 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.505876 Djaizz-23.6.15.0/src/djaizz/data/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     6026 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1730 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1537 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/migrations/0003_Django4.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.540875 Djaizz-23.6.15.0/src/djaizz/data/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1005 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/audio.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8019 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/models/base.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/csv.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/hdf.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/image.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2596 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/data/models/json.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      528 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/live_api.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      585 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/numpy.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/orc.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      595 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/pandas.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      550 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/parquet.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.554483 Djaizz-23.6.15.0/src/djaizz/data/models/public/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/gov.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/hugging_face.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       50 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/intl_dev.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       31 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/kaggle.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/tf.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       30 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/torch.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       51 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/public/weather.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      538 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/text.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/tfrecord.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/models/video.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      294 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/data/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.557150 Djaizz-23.6.15.0/src/djaizz/model/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2559 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/admin.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.558199 Djaizz-23.6.15.0/src/djaizz/model/api/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1821 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/api/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.558791 Djaizz-23.6.15.0/src/djaizz/model/api/gql/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/api/gql/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.558961 Djaizz-23.6.15.0/src/djaizz/model/api/json/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/api/json/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.559109 Djaizz-23.6.15.0/src/djaizz/model/api/rest/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/api/rest/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3259 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.583880 Djaizz-23.6.15.0/src/djaizz/model/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3211 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0001_AIModel.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2941 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    18732 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1226 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0004_CloudAIService.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1237 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0005_GoogleTranslate.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8705 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/0006_Django4.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.584626 Djaizz-23.6.15.0/src/djaizz/model/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1867 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    22789 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.586207 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      340 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.586665 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/amazon/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/amazon/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1021 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.587585 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/google/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      286 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/google/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8461 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.587995 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       58 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.588364 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.590230 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/meta/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       72 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/meta/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.590844 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/microsoft/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/microsoft/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.591227 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       59 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.593007 Djaizz-23.6.15.0/src/djaizz/model/models/ml/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1769 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1849 2023-06-06 18:00:24.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.604649 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1905 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9221 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1205 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/base.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8955 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9778 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9748 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/object_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10400 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/question_answering.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8633 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9303 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9572 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8648 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10268 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_generation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     9509 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8748 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/token_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10158 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/translation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    10300 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.606225 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      386 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2127 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.607055 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      322 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.608014 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/vision/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      343 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/vision/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    12235 2023-06-06 18:00:24.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1446 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/skl.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.610072 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      265 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      814 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/base.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.610708 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       46 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.612701 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/audio/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/audio/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       74 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/audio/text_to_speech.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.630737 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       53 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/image_classification.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       71 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/instance_segmentation.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       69 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/keypoint_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       67 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/object_detection.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       70 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/semantic_segmentation.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/pre_trained/vision/video_classification.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.633707 Djaizz-23.6.15.0/src/djaizz/model/scripts/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      401 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_google_cloud_ai_svcs.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)    19753 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     8394 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      705 2023-02-28 22:45:23.000000 Djaizz-23.6.15.0/src/djaizz/model/urls.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     5267 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/model/views.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      838 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.635117 Djaizz-23.6.15.0/src/djaizz/util/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1018 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.636557 Djaizz-23.6.15.0/src/djaizz/util/cli/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      735 2023-05-26 21:52:35.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.638372 Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/asgi.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      426 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/manage.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      553 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/wsgi.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-15 17:48:56.639070 Djaizz-23.6.15.0/src/djaizz/util/cli/aws_eb/
--rwxr-xr-x   0 thevinhluong102   (501) staff       (20)    11074 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/aws_eb/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1065 2023-06-15 17:20:24.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/deps.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     4374 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/cli/run_cmd.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1310 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/git.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1261 2023-06-06 18:00:20.000000 Djaizz-23.6.15.0/src/djaizz/util/pip.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1740 2023-02-28 00:21:53.000000 Djaizz-23.6.15.0/src/djaizz/util/views.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.570618 Djaizz-23.6.21.0/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1092 2023-02-09 04:49:59.000000 Djaizz-23.6.21.0/LICENSE
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-22 00:52:38.570256 Djaizz-23.6.21.0/PKG-INFO
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      187 2023-02-28 01:51:17.000000 Djaizz-23.6.21.0/README.md
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.511612 Djaizz-23.6.21.0/metadata/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2584 2023-03-09 04:40:50.000000 Djaizz-23.6.21.0/metadata/classifiers
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       52 2023-02-28 04:56:41.000000 Djaizz-23.6.21.0/metadata/description
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       65 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/metadata/entry-points
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.513439 Djaizz-23.6.21.0/metadata/requirements/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     6681 2023-06-21 20:14:13.000000 Djaizz-23.6.21.0/metadata/requirements/base.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       16 2023-02-28 04:56:41.000000 Djaizz-23.6.21.0/metadata/requirements/build.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       60 2023-06-21 03:38:10.000000 Djaizz-23.6.21.0/metadata/requirements/dev.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      215 2023-06-20 20:43:34.000000 Djaizz-23.6.21.0/metadata/requirements/doc.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      225 2023-06-21 03:38:28.000000 Djaizz-23.6.21.0/metadata/requirements/lint.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       15 2023-02-28 04:56:41.000000 Djaizz-23.6.21.0/metadata/requirements/publish.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       85 2023-06-20 20:43:34.000000 Djaizz-23.6.21.0/metadata/requirements/test.txt
+-rwxr-xr-x   0 thevinhluong102   (501) staff       (20)      150 2023-06-20 20:43:34.000000 Djaizz-23.6.21.0/metadata/requirements/viz.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       10 2023-06-21 16:52:01.000000 Djaizz-23.6.21.0/metadata/version
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3129 2023-06-21 03:26:52.000000 Djaizz-23.6.21.0/pyproject.toml
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-06-22 00:52:38.570727 Djaizz-23.6.21.0/setup.cfg
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.503610 Djaizz-23.6.21.0/src/
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.514784 Djaizz-23.6.21.0/src/Djaizz.egg-info/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5702 2023-06-22 00:52:38.000000 Djaizz-23.6.21.0/src/Djaizz.egg-info/PKG-INFO
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5814 2023-06-22 00:52:38.000000 Djaizz-23.6.21.0/src/Djaizz.egg-info/SOURCES.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-22 00:52:38.000000 Djaizz-23.6.21.0/src/Djaizz.egg-info/dependency_links.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       50 2023-06-22 00:52:38.000000 Djaizz-23.6.21.0/src/Djaizz.egg-info/entry_points.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     3988 2023-06-22 00:52:38.000000 Djaizz-23.6.21.0/src/Djaizz.egg-info/requires.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        7 2023-06-22 00:52:38.000000 Djaizz-23.6.21.0/src/Djaizz.egg-info/top_level.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-03-01 01:27:25.000000 Djaizz-23.6.21.0/src/Djaizz.egg-info/zip-safe
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.515536 Djaizz-23.6.21.0/src/djaizz/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      300 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.515915 Djaizz-23.6.21.0/src/djaizz/client/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      270 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/client/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.517321 Djaizz-23.6.21.0/src/djaizz/data/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      873 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/data/admin.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.517788 Djaizz-23.6.21.0/src/djaizz/data/api/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      816 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/data/api/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.518362 Djaizz-23.6.21.0/src/djaizz/data/api/gql/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/api/gql/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.518544 Djaizz-23.6.21.0/src/djaizz/data/api/json/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/api/json/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.518901 Djaizz-23.6.21.0/src/djaizz/data/api/rest/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/api/rest/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2703 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/data/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.521781 Djaizz-23.6.21.0/src/djaizz/data/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     6026 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1730 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1537 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/migrations/0003_Django4.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.530309 Djaizz-23.6.21.0/src/djaizz/data/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1005 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/audio.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8019 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/data/models/base.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/csv.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/hdf.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/image.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2596 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/data/models/json.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      528 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/live_api.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      585 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/numpy.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      534 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/orc.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      595 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/pandas.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      550 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/parquet.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.532877 Djaizz-23.6.21.0/src/djaizz/data/models/public/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/public/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/public/gov.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       37 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/public/hugging_face.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       50 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/public/intl_dev.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       31 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/public/kaggle.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       35 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/public/tf.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       30 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/public/torch.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       51 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/public/weather.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      538 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/text.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/tfrecord.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      542 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/models/video.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      294 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/data/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.534676 Djaizz-23.6.21.0/src/djaizz/model/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2559 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/admin.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.535079 Djaizz-23.6.21.0/src/djaizz/model/api/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1821 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/api/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.536162 Djaizz-23.6.21.0/src/djaizz/model/api/gql/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/api/gql/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.536319 Djaizz-23.6.21.0/src/djaizz/model/api/json/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/api/json/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.536470 Djaizz-23.6.21.0/src/djaizz/model/api/rest/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/api/rest/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3259 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.540040 Djaizz-23.6.21.0/src/djaizz/model/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3211 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/migrations/0001_AIModel.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2941 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    18732 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1226 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/migrations/0004_CloudAIService.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1237 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/migrations/0005_GoogleTranslate.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8705 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/migrations/0006_Django4.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        0 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.541300 Djaizz-23.6.21.0/src/djaizz/model/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1867 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    22789 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.542521 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      340 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.544879 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/amazon/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/amazon/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1021 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.545803 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/google/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      286 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/google/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8461 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.546290 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       58 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/hugging_face/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.546873 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/ibm_watson/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.547325 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/meta/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       72 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/meta/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.547724 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/microsoft/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/microsoft/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.548065 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       59 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/wolfram_alpha/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.549162 Djaizz-23.6.21.0/src/djaizz/model/models/ml/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1769 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1849 2023-06-06 18:00:24.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.556836 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1905 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9221 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1205 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/base.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8955 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9778 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9748 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/object_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10400 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/question_answering.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8633 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9303 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9572 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8648 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/text_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10268 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/text_generation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     9509 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8748 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/token_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10158 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/translation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    10300 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.557623 Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      386 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2127 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.558056 Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/pre_trained/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      322 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/pre_trained/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.558891 Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/pre_trained/vision/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      343 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/pre_trained/vision/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    12235 2023-06-06 18:00:24.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1446 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/skl.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.559712 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      265 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      814 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/base.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.560136 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       46 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.560886 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/audio/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/audio/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       74 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/audio/text_to_speech.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.563534 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/vision/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       53 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/vision/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/vision/image_classification.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       71 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/vision/instance_segmentation.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       69 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/vision/keypoint_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       67 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/vision/object_detection.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       70 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/vision/semantic_segmentation.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       68 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/pre_trained/vision/video_classification.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.564969 Djaizz-23.6.21.0/src/djaizz/model/scripts/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      401 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/scripts/setup_google_cloud_ai_svcs.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)    19753 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     8394 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      705 2023-02-28 22:45:23.000000 Djaizz-23.6.21.0/src/djaizz/model/urls.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     5267 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/model/views.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      838 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.566693 Djaizz-23.6.21.0/src/djaizz/util/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1018 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/util/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.567908 Djaizz-23.6.21.0/src/djaizz/util/cli/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      735 2023-05-26 21:52:35.000000 Djaizz-23.6.21.0/src/djaizz/util/cli/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.569343 Djaizz-23.6.21.0/src/djaizz/util/cli/_server_files/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      554 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/util/cli/_server_files/asgi.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      426 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/util/cli/_server_files/manage.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      553 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/util/cli/_server_files/wsgi.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 00:52:38.569799 Djaizz-23.6.21.0/src/djaizz/util/cli/aws_eb/
+-rwxr-xr-x   0 thevinhluong102   (501) staff       (20)    11074 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/util/cli/aws_eb/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1065 2023-06-20 20:43:34.000000 Djaizz-23.6.21.0/src/djaizz/util/cli/deps.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     4374 2023-06-21 23:57:05.000000 Djaizz-23.6.21.0/src/djaizz/util/cli/run_cmd.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1310 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/util/git.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1261 2023-06-06 18:00:20.000000 Djaizz-23.6.21.0/src/djaizz/util/pip.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1740 2023-02-28 00:21:53.000000 Djaizz-23.6.21.0/src/djaizz/util/views.py
```

### Comparing `Djaizz-23.6.15.0/LICENSE` & `Djaizz-23.6.21.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/PKG-INFO` & `Djaizz-23.6.21.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Djaizz
-Version: 23.6.15.0
+Version: 23.6.21.0
 Summary: Artificial Intelligence (AI) in Django Applications
 Author-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 Maintainer-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 License: MIT License
         
         Copyright (c) 2021 The Vinh LUONG (LƯƠNG Thế Vinh)
```

### Comparing `Djaizz-23.6.15.0/metadata/classifiers` & `Djaizz-23.6.21.0/metadata/classifiers`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/metadata/requirements/base.txt` & `Djaizz-23.6.21.0/metadata/requirements/base.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # DATA MANAGEMENT & PROCESSING
 # ============================
 
 Dask >= 2023.6.0
 Distributed >= 2023.6.0
 Kedro >= 0.18.10; python_version < '3.11'
-MetaFlow >= 2.9.4
+MetaFlow >= 2.9.5
 NumBa >= 0.57.0
 NumPy >= 1.23
   # let higher dependencies figure
 Pandas >= 1.5
   # let higher dependencies figure
 Pandarallel >= 1.6.5
 PyArrow >= 12.0.1
 PySpark >= 3.4.0
-Ray >= 2.5.0; python_version < '3.11'
+Ray >= 2.5.1; python_version < '3.11'
 SciPy >= 1.10.1
 
 Pillow >= 9.5.0
 # Pillow-SIMD >= 9.0.0
   # complex to install
 PyCOCOTools >= 2.0.6
 SciKit-Image >= 0.21.0
@@ -34,16 +34,16 @@
 # SciKit-Learn & related
 # Auto-SKLearn >= 0.15.0
   # depends on SciKit-Learn < 0.25
 SciKit-Learn >= 1.2.2
 
 # TensorFlow & related
 TensorFlow >= 2.12.0; sys_platform != 'darwin'
-TensorFlow-MacOS >= 2.12.0; sys_platform == 'darwin'
-TensorFlow-Metal >= 1.0.1; sys_platform == 'darwin'
+TensorFlow-MacOS >= 2.12.0; (sys_platform == 'darwin') and (platform_release > '20.6.0')
+TensorFlow-Metal >= 1.0.0; (sys_platform == 'darwin') and (platform_release > '20.6.0')
 TensorFlow-DataSets >= 4.9.2
 TensorFlow-Hub >= 0.13.0
 
 # Torch & related
 Torch >= 2.0.1
 Torch-Model-Archiver >= 0.8.1
 TorchServe >= 0.8.1
@@ -101,17 +101,17 @@
 SciKit-Fuzzy >= 0.4.2
 
 
 # LARGE FOUNDATIONAL MODELS & related
 # ===================================
 
 AutoGPT >= 0.0.1.dev0
-LangChain >= 0.0.200
+LangChain >= 0.0.208
 OpenAI >= 0.27.8
-PandasAI >= 0.5.2
+PandasAI >= 0.6.2
 
 
 # FILE SYSTEMS
 # ============
 FSSpec >= 2023.6.0
 
 
@@ -142,20 +142,20 @@
 Django-Generic-M2M >= 0.3.1
 Django-GM2M >= 1.1.1
 Django-QuerySetSequence >= 0.16
 Django-Tagging >= 0.5.0
 Django-Taggit >= 4.0.0
 
 # GraphQL
-Ariadne >= 0.19.1
+Ariadne >= 0.20.0
 Django-GraphQL-Extensions >= 0.1.0
 Django-RESTQL >= 0.15.3
 GQL >= 3.4.1
 Graphene >= 3.2.2
-Graphene-Django >= 3.1.1
+Graphene-Django >= 3.1.2
 # Graphene-Django-Extras >= 0.5.2
   # conflicting/slow-resolving dependencies
 Graphene-Django-Optimizer >= 0.9.1
 # Graphene-Django-Subscriptions >= 0.0.9
   # conflicting/slow-resolving dependencies
 # Graphene-Django-Tools >= 0.21.0
   # conflicting/slow-resolving dependencies
@@ -164,15 +164,15 @@
 # Graphene-SQLAlchemy >= 2.3.0
   # conflicting/slow-resolving dependencies
 GraphQLClient >= 0.2.4
 GraphQL-Core >= 3.2.3
 GraphQL-Relay >= 3.2.0
 Py-GQL >= 0.6.1
 SGQLC >= 16.2
-Strawberry-GraphQL >= 0.185.1
+Strawberry-GraphQL >= 0.187.3
 
 # Django REST Framework & other API-related
 DjangoRESTFramework >= 3.14.0
 DRFPasswordless >= 1.5.8
 DRF-Writable-Nested >= 0.7.0
 CoreAPI >= 2.3.3
   # closely related to Django REST Framework
@@ -187,14 +187,15 @@
 Django-Typed-Models >= 0.13.0
 
 HAL-Codec >= 1.0.2
 JSONHyperSchema-Codec >= 1.0.3
 OpenAPI-Codec >= 1.3.2
 
 JSONSchema >= 4.17.3
+Pyrsistent >= 0.19.3  # required by JSONSchema
 Pydantic >= 1.10.9
 
 HTTPie >= 3.2.2
 
 # Django Filtering
 Django-Filter >= 23.2
 DjangoRESTFramework-Filters >= 1.0.0.dev2
@@ -203,15 +204,15 @@
 Django-Guardian >= 2.4.0
 Rules >= 3.3
 
 # Django Debugging & Query Profiling
 Django-Debug-Toolbar >= 4.1.0
 Django-Query-Profiler >= 0.9
 Django-Silk >= 5.0.3
-Kolo >= 2.9.4
+Kolo >= 2.10.0
 
 # Django Extensions & Utilities
 Django-Annoying >= 0.10.6
 Django-Choices >= 1.7.2
 Django-Compressor >= 4.3.1
 Django-Configurations >= 2.4.1
 Django-Crispy-Forms >= 2.0
@@ -231,25 +232,25 @@
 # Application UIs
 Django-HTMX >= 1.15.0
 
 Django-Plotly-Dash >= 2.2.1
 Dash-Bootstrap-Components >= 1.4.1
 DPD-Static-Support >= 0.0.5
 Django-Bootstrap4 >= 23.1
-WhiteNoise >= 6.4.0
+WhiteNoise >= 6.5.0
 
-Gradio >= 3.34.0
+Gradio >= 3.35.2
 Gradio-Tools >= 0.0.9
 
 Streamlit >= 1.23.1
 Watchdog >= 3.0.0
 
 # Database Adapters/Backends/Connectors/Drivers
 MariaDB-DynCol >= 3.6.1
-Django-MySQL >= 4.9.0
+Django-MySQL >= 4.10.0
 MySQLClient >= 2.1.1
 MySQL-Connector-Python >= 8.0.33
 PsycoPG >= 3.1.9
 PsycoPG2-binary >= 2.9.6
 
 # ASGI Web Servers & related
 ASGIRef >= 3.7.2
@@ -264,15 +265,15 @@
   # let higher dependencies figure
 Uvicorn >= 0.22.0
 
 
 # COMMAND-LINE INTERFACE (CLI)
 # ============================
 CLICK >= 8.1.3
-Colored >= 1.4.4
+Colored >= 2.1.1
 
 
 # JUPYTER
 # =======
 Jupyter >= 1.0.0
 
 
@@ -291,29 +292,31 @@
 
 # Dropbox
 DropboxDriveFS >= 1.3.1
 
 
 # REACT JAVASCRIPT
 # ================
-ReactPy >= 1.0.0
+ReactPy >= 1.0.1
 ReactPy-Django >= 3.1.0
-ReactPy-Jupyter >= 0.9.5
+# ReactPy-Jupyter >= 0.9.5
+  # very buggy
+Packaging >= 23.1  # required by React-Jupyter
 
 
 # MISC / OTHER
 # ============
 GitPython >= 3.1.31
 Loguru >= 0.7.0
 PSUtil >= 5.9.5
 Python-DateUtil >= 2.8.2
 Python-DotEnv >= 1.0.0
 PyTZ >= 2023.3
 Requests >= 2.31.0
-Ruamel.YAML >= 0.17.31
+Ruamel.YAML >= 0.17.32
 Tqdm >= 4.65.0
 
 
 # INDIRECT DEPENDENCIES: explicitly specify to avoid outdated versions
 # ====================================================================
 FastAPI >= 0.97.0
 Pydantic >= 1.10.9
```

### Comparing `Djaizz-23.6.15.0/pyproject.toml` & `Djaizz-23.6.21.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -145,11 +145,11 @@
 
 # BUILD SYSTEM
 # (SetUpTools)
 # ============
 
 [build-system]
 requires = [
-  'SetUpTools >= 67.8.0',
+  'SetUpTools >= 68.0.0',
   'Wheel >= 0.40.0',
 ]
 build-backend = 'setuptools.build_meta'
```

### Comparing `Djaizz-23.6.15.0/src/Djaizz.egg-info/PKG-INFO` & `Djaizz-23.6.21.0/src/Djaizz.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Djaizz
-Version: 23.6.15.0
+Version: 23.6.21.0
 Summary: Artificial Intelligence (AI) in Django Applications
 Author-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 Maintainer-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 License: MIT License
         
         Copyright (c) 2021 The Vinh LUONG (LƯƠNG Thế Vinh)
```

### Comparing `Djaizz-23.6.15.0/src/Djaizz.egg-info/SOURCES.txt` & `Djaizz-23.6.21.0/src/Djaizz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/Djaizz.egg-info/requires.txt` & `Djaizz-23.6.21.0/src/Djaizz.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Dask>=2023.6.0
 Distributed>=2023.6.0
-MetaFlow>=2.9.4
+MetaFlow>=2.9.5
 NumBa>=0.57.0
 NumPy>=1.23
 Pandas>=1.5
 Pandarallel>=1.6.5
 PyArrow>=12.0.1
 PySpark>=3.4.0
 SciPy>=1.10.1
@@ -36,17 +36,17 @@
 ConfigSpace>=0.7.1
 Hpbandster>=0.7.4
 Tabulate>=0.9.0
 LIME>=0.2.0.1
 SHAP>=0.41.0
 SciKit-Fuzzy>=0.4.2
 AutoGPT>=0.0.1.dev0
-LangChain>=0.0.200
+LangChain>=0.0.208
 OpenAI>=0.27.8
-PandasAI>=0.5.2
+PandasAI>=0.6.2
 FSSpec>=2023.6.0
 CloudPickle>=2.2.1
 JobLib>=1.2.0
 Django>=4.2.2
 Django-Polymorphic>=3.1.0
 Django-Admin-HStore-Widget>=1.2.1
 Django-Admin-Relation-Links>=0.2.5
@@ -54,50 +54,51 @@
 Django-Jazzmin>=2.6.0
 Django-Autocomplete-Light>=3.9.7
 Django-Generic-M2M>=0.3.1
 Django-GM2M>=1.1.1
 Django-QuerySetSequence>=0.16
 Django-Tagging>=0.5.0
 Django-Taggit>=4.0.0
-Ariadne>=0.19.1
+Ariadne>=0.20.0
 Django-GraphQL-Extensions>=0.1.0
 Django-RESTQL>=0.15.3
 GQL>=3.4.1
 Graphene>=3.2.2
-Graphene-Django>=3.1.1
+Graphene-Django>=3.1.2
 Graphene-Django-Optimizer>=0.9.1
 GraphQLClient>=0.2.4
 GraphQL-Core>=3.2.3
 GraphQL-Relay>=3.2.0
 Py-GQL>=0.6.1
 SGQLC>=16.2
-Strawberry-GraphQL>=0.185.1
+Strawberry-GraphQL>=0.187.3
 DjangoRESTFramework>=3.14.0
 DRFPasswordless>=1.5.8
 DRF-Writable-Nested>=0.7.0
 CoreAPI>=2.3.3
 CoreAPI-CLI>=1.0.9
 Markdown>=3.4.3
 DRF-Nested-Routers>=0.93.4
 Django-PolyModels>=1.8.0
 Django-Typed-Models>=0.13.0
 HAL-Codec>=1.0.2
 JSONHyperSchema-Codec>=1.0.3
 OpenAPI-Codec>=1.3.2
 JSONSchema>=4.17.3
+Pyrsistent>=0.19.3
 Pydantic>=1.10.9
 HTTPie>=3.2.2
 Django-Filter>=23.2
 DjangoRESTFramework-Filters>=1.0.0.dev2
 Django-Guardian>=2.4.0
 Rules>=3.3
 Django-Debug-Toolbar>=4.1.0
 Django-Query-Profiler>=0.9
 Django-Silk>=5.0.3
-Kolo>=2.9.4
+Kolo>=2.10.0
 Django-Annoying>=0.10.6
 Django-Choices>=1.7.2
 Django-Compressor>=4.3.1
 Django-Configurations>=2.4.1
 Django-Crispy-Forms>=2.0
 Django-Environ>=0.10.0
 Django-Extensions>=3.2.3
@@ -109,89 +110,90 @@
 Dju>=23.6.14
 Django-CORS-Headers>=4.1.0
 Django-HTMX>=1.15.0
 Django-Plotly-Dash>=2.2.1
 Dash-Bootstrap-Components>=1.4.1
 DPD-Static-Support>=0.0.5
 Django-Bootstrap4>=23.1
-WhiteNoise>=6.4.0
-Gradio>=3.34.0
+WhiteNoise>=6.5.0
+Gradio>=3.35.2
 Gradio-Tools>=0.0.9
 Streamlit>=1.23.1
 Watchdog>=3.0.0
 MariaDB-DynCol>=3.6.1
-Django-MySQL>=4.9.0
+Django-MySQL>=4.10.0
 MySQLClient>=2.1.1
 MySQL-Connector-Python>=8.0.33
 PsycoPG>=3.1.9
 PsycoPG2-binary>=2.9.6
 ASGIRef>=3.7.2
 Channels>=4.0.0
 Daphne>=4.0.0
 GUnicorn>=20.1.0
 H11>=0.9
 Hypercorn>=0.14.3
 Quart>=0.18.4
 Starlette>=0.27
 Uvicorn>=0.22.0
 CLICK>=8.1.3
-Colored>=1.4.4
+Colored>=2.1.1
 Jupyter>=1.0.0
 S3FS>=2023.6.0
 ADLFS>=2023.4.0
 GCSFS>=2023.6.0
 GDriveFS>=0.14.13
 DropboxDriveFS>=1.3.1
-ReactPy>=1.0.0
+ReactPy>=1.0.1
 ReactPy-Django>=3.1.0
-ReactPy-Jupyter>=0.9.5
+Packaging>=23.1
 GitPython>=3.1.31
 Loguru>=0.7.0
 PSUtil>=5.9.5
 Python-DateUtil>=2.8.2
 Python-DotEnv>=1.0.0
 PyTZ>=2023.3
 Requests>=2.31.0
-Ruamel.YAML>=0.17.31
+Ruamel.YAML>=0.17.32
 Tqdm>=4.65.0
 FastAPI>=0.97.0
 Pydantic>=1.10.9
 
 [:python_version < "3.11"]
 Kedro>=0.18.10
-Ray>=2.5.0
+Ray>=2.5.1
 Giotto-TDA>=0.6.0
 CausalNex>=0.12.0
 Django-ForestAdmin>=1.5.0
 
 [:sys_platform != "darwin"]
 TensorFlow>=2.12.0
 
-[:sys_platform == "darwin"]
+[:sys_platform == "darwin" and platform_release > "20.6.0"]
 TensorFlow-MacOS>=2.12.0
-TensorFlow-Metal>=1.0.1
+TensorFlow-Metal>=1.0.0
 
 [build]
 Build>=0.10.0
 
 [dev]
-Commitizen>=3.3.0
+Commitizen>=3.4.0
 Pre-Commit>=3.3.3
+PyWatchman>=1.4.1
 
 [doc]
 Sphinx>=7.0.1
 Sphinx-AutoBuild>=2021.3.14
 SphinxContrib-JSMath>=1.0.1
 CommonMark>=0.9.1
 ReCommonMark>=0.7.1
 
 [lint]
 Bandit>=1.7.5
 Flake8>=6.0.0
-MyPy>=1.3.0
+MyPy>=1.4.0
 PyCodeStyle>=2.10.0
 PyDocStyle>=6.3.0
 PyLama>=8.4.1
 PyLint>=2.17.4
 ReactPy-Flake8>=0.7.0
 
 [publish]
```

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/admin.py` & `Djaizz-23.6.21.0/src/djaizz/data/admin.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/api/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/data/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/apps.py` & `Djaizz-23.6.21.0/src/djaizz/data/apps.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py` & `Djaizz-23.6.21.0/src/djaizz/data/migrations/0001_DataSchema_DataSet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py` & `Djaizz-23.6.21.0/src/djaizz/data/migrations/0002_InDBJSONDataSet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/migrations/0003_Django4.py` & `Djaizz-23.6.21.0/src/djaizz/data/migrations/0003_Django4.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/audio.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/audio.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/base.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/csv.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/csv.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/hdf.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/hdf.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/image.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/image.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/json.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/json.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/live_api.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/live_api.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/numpy.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/numpy.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/orc.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/orc.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/pandas.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/pandas.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/parquet.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/parquet.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/text.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/text.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/tfrecord.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/tfrecord.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/data/models/video.py` & `Djaizz-23.6.21.0/src/djaizz/data/models/video.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/admin.py` & `Djaizz-23.6.21.0/src/djaizz/model/admin.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/api/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/model/api/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/apps.py` & `Djaizz-23.6.21.0/src/djaizz/model/apps.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/migrations/0001_AIModel.py` & `Djaizz-23.6.21.0/src/djaizz/model/migrations/0001_AIModel.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py` & `Djaizz-23.6.21.0/src/djaizz/model/migrations/0002_PreTrainedKerasImageNetClassifier.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py` & `Djaizz-23.6.21.0/src/djaizz/model/migrations/0003_PreTrainedHuggingFaceTransformers.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/migrations/0004_CloudAIService.py` & `Djaizz-23.6.21.0/src/djaizz/model/migrations/0004_CloudAIService.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/migrations/0005_GoogleTranslate.py` & `Djaizz-23.6.21.0/src/djaizz/model/migrations/0005_GoogleTranslate.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/migrations/0006_Django4.py` & `Djaizz-23.6.21.0/src/djaizz/model/migrations/0006_Django4.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/base.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/base.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/cloud_ai_svc/google/translation.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/base.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/audio_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/base.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/image_classification.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/image_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/mask_filling.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/object_detection.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/object_detection.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/question_answering.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/question_answering.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/speech_recognition.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/table_question_answering.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/text2text_generation.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_classification.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/text_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_generation.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/text_generation.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/text_summarization.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/token_classification.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/token_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/translation.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/translation.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/hugging_face/zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/base.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/keras/pre_trained/vision/image_classification.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/skl.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/skl.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/models/ml/torch/base.py` & `Djaizz-23.6.21.0/src/djaizz/model/models/ml/torch/base.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py` & `Djaizz-23.6.21.0/src/djaizz/model/scripts/setup_pretrained_huggingface_models.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py` & `Djaizz-23.6.21.0/src/djaizz/model/scripts/setup_pretrained_keras_models.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/urls.py` & `Djaizz-23.6.21.0/src/djaizz/model/urls.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/model/views.py` & `Djaizz-23.6.21.0/src/djaizz/model/views.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/urls.py` & `Djaizz-23.6.21.0/src/djaizz/urls.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/util/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/cli/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/asgi.py` & `Djaizz-23.6.21.0/src/djaizz/util/cli/_server_files/asgi.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/cli/_server_files/wsgi.py` & `Djaizz-23.6.21.0/src/djaizz/util/cli/_server_files/wsgi.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/cli/aws_eb/__init__.py` & `Djaizz-23.6.21.0/src/djaizz/util/cli/aws_eb/__init__.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/cli/deps.py` & `Djaizz-23.6.21.0/src/djaizz/util/cli/deps.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/cli/run_cmd.py` & `Djaizz-23.6.21.0/src/djaizz/util/cli/run_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,24 +49,24 @@
     PROCFILE_NAME: str = 'Procfile'
 
     def __init__(self, asgi: Optional[str] = None):
         """Initialize context manager."""
         self.asgi: Optional[str] = asgi
 
         if self.asgi:
-            self.agsi_py_missing: bool = not Path(self.ASGI_PY_FILE_NAME).exists()   # noqa: E501
+            self.asgi_py_missing: bool = not Path(self.ASGI_PY_FILE_NAME).exists()   # noqa: E501
             self.procfile_missing: bool = not Path(self.PROCFILE_NAME).exists()
 
         else:
             self.wsgi_py_missing: bool = not Path(self.WSGI_PY_FILE_NAME).exists()   # noqa: E501
 
     def __enter__(self):
         """Add `asgi.py`/`wsgi.py` file & Procfile, if applicable."""
         if self.asgi:
-            if self.agsi_py_missing:
+            if self.asgi_py_missing:
                 shutil.copyfile(src=self.ASGI_PY_FILE_SRC_PATH,
                                 dst=self.ASGI_PY_FILE_NAME,
                                 follow_symlinks=False)
 
             if self.procfile_missing:
                 shutil.copyfile(
                     src=(_SERVER_FILES_DIR_PATH /
```

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/git.py` & `Djaizz-23.6.21.0/src/djaizz/util/git.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/pip.py` & `Djaizz-23.6.21.0/src/djaizz/util/pip.py`

 * *Files identical despite different names*

### Comparing `Djaizz-23.6.15.0/src/djaizz/util/views.py` & `Djaizz-23.6.21.0/src/djaizz/util/views.py`

 * *Files identical despite different names*

