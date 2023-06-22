# Comparing `tmp/DjAIoT-23.6.14.0.tar.gz` & `tmp/DjAIoT-23.6.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DjAIoT-23.6.14.0.tar", last modified: Wed Jun 14 23:00:44 2023, max compression
+gzip compressed data, was "DjAIoT-23.6.21.1.tar", last modified: Thu Jun 22 04:36:01 2023, max compression
```

## Comparing `DjAIoT-23.6.14.0.tar` & `DjAIoT-23.6.21.1.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.738059 DjAIoT-23.6.14.0/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      189 2023-02-09 04:50:50.000000 DjAIoT-23.6.14.0/.gitignore
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       45 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/.prospector.yaml
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.676849 DjAIoT-23.6.14.0/.vscode/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1020 2023-02-09 04:50:43.000000 DjAIoT-23.6.14.0/.vscode/settings.json
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1092 2023-02-09 04:50:50.000000 DjAIoT-23.6.14.0/LICENSE
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     5578 2023-06-14 23:00:44.737777 DjAIoT-23.6.14.0/PKG-INFO
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       98 2023-03-03 02:29:36.000000 DjAIoT-23.6.14.0/README.md
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.677842 DjAIoT-23.6.14.0/metadata/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2500 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/metadata/classifiers
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       96 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/metadata/description
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.679055 DjAIoT-23.6.14.0/metadata/requirements/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       20 2023-06-14 22:59:12.000000 DjAIoT-23.6.14.0/metadata/requirements/base.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       16 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/metadata/requirements/build.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       41 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/metadata/requirements/dev.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      199 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/metadata/requirements/doc.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      189 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/metadata/requirements/lint.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       15 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/metadata/requirements/publish.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       85 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/metadata/requirements/test.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       10 2023-06-14 22:59:22.000000 DjAIoT-23.6.14.0/metadata/version
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     3152 2023-06-14 21:54:18.000000 DjAIoT-23.6.14.0/pyproject.toml
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-06-14 23:00:44.738127 DjAIoT-23.6.14.0/setup.cfg
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.670159 DjAIoT-23.6.14.0/src/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.680271 DjAIoT-23.6.14.0/src/DjAIoT.egg-info/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5578 2023-06-14 23:00:44.000000 DjAIoT-23.6.14.0/src/DjAIoT.egg-info/PKG-INFO
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5633 2023-06-14 23:00:44.000000 DjAIoT-23.6.14.0/src/DjAIoT.egg-info/SOURCES.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-14 23:00:44.000000 DjAIoT-23.6.14.0/src/DjAIoT.egg-info/dependency_links.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      422 2023-06-14 23:00:44.000000 DjAIoT-23.6.14.0/src/DjAIoT.egg-info/requires.txt
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        7 2023-06-14 23:00:44.000000 DjAIoT-23.6.14.0/src/DjAIoT.egg-info/top_level.txt
--rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-14 22:53:26.000000 DjAIoT-23.6.14.0/src/DjAIoT.egg-info/zip-safe
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.681684 DjAIoT-23.6.14.0/src/djaiot/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      300 2023-03-03 02:23:30.000000 DjAIoT-23.6.14.0/src/djaiot/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.682991 DjAIoT-23.6.14.0/src/djaiot/device_data/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.685608 DjAIoT-23.6.14.0/src/djaiot/device_data/admin/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      209 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/admin/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    59933 2022-11-06 17:51:40.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/admin/admin copy.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     2822 2022-11-06 17:52:04.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/admin/install_data.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     8503 2022-11-06 17:51:43.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/admin/instance_types.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.686342 DjAIoT-23.6.14.0/src/djaiot/device_data/api/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     3279 2022-11-06 17:51:43.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/field_names.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.686910 DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 23:31:40.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.688335 DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/schema/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:24:27.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/schema/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      742 2022-11-07 00:31:09.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/schema/mutations.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     3287 2022-11-07 00:31:08.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/schema/queries.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     3296 2022-11-07 00:31:08.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/schema/types.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.689831 DjAIoT-23.6.14.0/src/djaiot/device_data/api/python/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)   211423 2022-11-06 23:38:26.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/python/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     1433 2023-05-26 22:13:59.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/python/util.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.690268 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 23:31:40.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.690429 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:18:14.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.690912 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/serializers/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:41:29.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/serializers/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     9566 2022-11-07 00:41:53.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/serializers/serializers.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.691637 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/views/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:41:53.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/views/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    26606 2022-11-07 00:41:53.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/views/views.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.692228 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:24:29.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.692886 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/serializers/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       75 2022-11-07 00:41:53.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/serializers/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    21201 2022-11-07 00:41:53.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/serializers/serializers.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.693875 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/views/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:42:09.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/views/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    26934 2022-11-07 00:42:09.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/views/views.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.695861 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/queries/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       74 2022-11-07 00:20:24.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/queries/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      229 2022-11-07 00:20:24.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/queries/device_class.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     8543 2022-11-07 00:20:24.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/queries/queries.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      377 2022-11-07 00:20:24.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/queries/wsgi.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      685 2023-03-03 02:26:00.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.697056 DjAIoT-23.6.14.0/src/djaiot/device_data/autocompletes/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      217 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/autocompletes/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     2861 2022-11-06 17:51:43.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/autocompletes/autocompletes.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.697973 DjAIoT-23.6.14.0/src/djaiot/device_data/filters/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      211 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/filters/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    31431 2022-11-06 17:52:04.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/filters/filters.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.698824 DjAIoT-23.6.14.0/src/djaiot/device_data/forms/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      209 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/forms/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    15398 2021-09-16 20:59:02.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/forms/forms.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.700600 DjAIoT-23.6.14.0/src/djaiot/device_data/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1858 2023-02-09 04:51:09.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/migrations/0001_JSONInfo.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     2388 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/migrations/0002_DeviceClass.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       54 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.708573 DjAIoT-23.6.14.0/src/djaiot/device_data/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      323 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     4678 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/_abc.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)   167062 2022-11-06 17:51:04.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1591 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_class.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:07.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_data_stream.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:04.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_data_stream_daily_agg.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      447 2022-11-06 17:51:07.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_data_stream_type.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:04.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_family.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:05.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_family_data_stream_pairwise_correlation.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:05.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_family_data_stream_profile.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:07.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_parquet_data_set.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:07.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_site.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:26.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_sku.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)     1717 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/json_info.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      206 2022-11-06 17:51:05.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/logical_data_type.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     3097 2022-11-06 17:51:07.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/measurement_unit.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     6674 2022-11-06 17:51:04.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/physical_data_type.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.709045 DjAIoT-23.6.14.0/src/djaiot/device_data/models/signals/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      235 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/models/signals/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.709896 DjAIoT-23.6.14.0/src/djaiot/device_data/queries/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      228 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/queries/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    42044 2022-11-06 17:52:19.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/queries/queries.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.710913 DjAIoT-23.6.14.0/src/djaiot/device_data/scripts/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      157 2023-02-09 04:51:25.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/scripts/profile_device_data_streams.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     6126 2022-11-05 15:22:20.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/urls copy.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       53 2023-03-03 02:24:23.000000 DjAIoT-23.6.14.0/src/djaiot/device_data/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.712787 DjAIoT-23.6.14.0/src/djaiot/device_health/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.715121 DjAIoT-23.6.14.0/src/djaiot/device_health/admin/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      211 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/admin/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    11252 2022-11-06 17:43:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/admin/admin copy 2.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    40753 2022-11-06 17:43:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/admin/admin copy.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       44 2023-02-28 00:14:45.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/admin/admin.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.715464 DjAIoT-23.6.14.0/src/djaiot/device_health/api/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.715906 DjAIoT-23.6.14.0/src/djaiot/device_health/api/cli/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    76279 2022-11-06 23:37:52.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/cli/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     2176 2022-11-06 17:43:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/field_names.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.716760 DjAIoT-23.6.14.0/src/djaiot/device_health/api/graphql/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 23:31:40.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/graphql/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.718417 DjAIoT-23.6.14.0/src/djaiot/device_health/api/graphql/schema/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:20:24.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/graphql/schema/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)       98 2022-11-07 00:20:24.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/graphql/schema/mutations.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:20:24.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/graphql/schema/queries.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:20:24.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/graphql/schema/types.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.718581 DjAIoT-23.6.14.0/src/djaiot/device_health/api/python/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)   150720 2021-09-16 20:59:02.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/python/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.720603 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2021-09-16 20:59:02.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.722302 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/core/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:19:57.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/core/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     6050 2022-11-07 00:19:57.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/core/serializers.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    15965 2022-11-07 00:19:57.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/core/views.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.723539 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/json/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:19:58.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/json/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    15458 2022-11-07 00:19:57.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/json/serializers.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    16710 2022-11-07 00:19:57.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/json/views.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     5131 2021-09-16 20:59:02.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/queries.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      699 2023-03-03 02:28:20.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.724610 DjAIoT-23.6.14.0/src/djaiot/device_health/autocompletes/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      219 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/autocompletes/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      591 2022-11-06 17:47:37.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/autocompletes/autocompletes.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.725528 DjAIoT-23.6.14.0/src/djaiot/device_health/filters/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      213 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/filters/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    38821 2022-11-06 17:43:50.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/filters/filters.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.726775 DjAIoT-23.6.14.0/src/djaiot/device_health/forms/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      211 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/forms/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     8139 2022-11-06 17:47:40.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/forms/forms.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.727505 DjAIoT-23.6.14.0/src/djaiot/device_health/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.729169 DjAIoT-23.6.14.0/src/djaiot/device_health/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       50 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/models/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    18928 2022-11-06 17:43:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/models/models copy.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)   102757 2022-11-06 17:46:43.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/models/models.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.731084 DjAIoT-23.6.14.0/src/djaiot/device_health/queries/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      230 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/queries/__init__.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    33056 2022-11-06 17:47:39.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/queries/queries.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     4424 2022-11-05 15:22:20.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/urls copy.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       55 2023-03-03 02:28:08.000000 DjAIoT-23.6.14.0/src/djaiot/device_health/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.732689 DjAIoT-23.6.14.0/src/djaiot/device_perf/
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.733176 DjAIoT-23.6.14.0/src/djaiot/device_perf/admin/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      216 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/admin/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      720 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/apps.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.733706 DjAIoT-23.6.14.0/src/djaiot/device_perf/autocompletes/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      224 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/autocompletes/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.734180 DjAIoT-23.6.14.0/src/djaiot/device_perf/filters/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      218 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/filters/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.734551 DjAIoT-23.6.14.0/src/djaiot/device_perf/forms/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      216 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/forms/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.735002 DjAIoT-23.6.14.0/src/djaiot/device_perf/migrations/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/migrations/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.735460 DjAIoT-23.6.14.0/src/djaiot/device_perf/models/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      224 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/models/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.735780 DjAIoT-23.6.14.0/src/djaiot/device_perf/queries/
--rw-r--r--   0 thevinhluong102   (501) staff       (20)      235 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/queries/__init__.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       60 2023-03-03 04:41:49.000000 DjAIoT-23.6.14.0/src/djaiot/device_perf/urls.py
--rwxr--r--   0 thevinhluong102   (501) staff       (20)      670 2022-11-05 02:48:22.000000 DjAIoT-23.6.14.0/src/djaiot/graphql_schema.py
--rw-r--r--   0 thevinhluong102   (501) staff       (20)       34 2023-03-03 02:23:22.000000 DjAIoT-23.6.14.0/src/djaiot/urls.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.736125 DjAIoT-23.6.14.0/src/djaiot/util/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)     4154 2022-11-05 15:22:20.000000 DjAIoT-23.6.14.0/src/djaiot/util/__init__.py
-drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-14 23:00:44.736601 DjAIoT-23.6.14.0/src/djaiot/util/cli/
--rwxr--r--   0 thevinhluong102   (501) staff       (20)    95068 2021-09-16 20:59:02.000000 DjAIoT-23.6.14.0/src/djaiot/util/cli/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.075818 DjAIoT-23.6.21.1/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      189 2023-02-09 04:50:50.000000 DjAIoT-23.6.21.1/.gitignore
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       45 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/.prospector.yaml
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.017640 DjAIoT-23.6.21.1/.vscode/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1020 2023-02-09 04:50:43.000000 DjAIoT-23.6.21.1/.vscode/settings.json
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1092 2023-02-09 04:50:50.000000 DjAIoT-23.6.21.1/LICENSE
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     5578 2023-06-22 04:36:01.075608 DjAIoT-23.6.21.1/PKG-INFO
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       98 2023-03-03 02:29:36.000000 DjAIoT-23.6.21.1/README.md
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.018729 DjAIoT-23.6.21.1/metadata/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2500 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/metadata/classifiers
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       96 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/metadata/description
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.020235 DjAIoT-23.6.21.1/metadata/requirements/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       20 2023-06-22 04:21:07.000000 DjAIoT-23.6.21.1/metadata/requirements/base.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       16 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/metadata/requirements/build.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       40 2023-06-22 00:57:27.000000 DjAIoT-23.6.21.1/metadata/requirements/dev.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      198 2023-06-22 00:57:14.000000 DjAIoT-23.6.21.1/metadata/requirements/doc.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      190 2023-06-22 00:56:45.000000 DjAIoT-23.6.21.1/metadata/requirements/lint.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       15 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/metadata/requirements/publish.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       85 2023-06-22 00:55:59.000000 DjAIoT-23.6.21.1/metadata/requirements/test.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       10 2023-06-22 04:21:10.000000 DjAIoT-23.6.21.1/metadata/version
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     3152 2023-06-14 21:54:18.000000 DjAIoT-23.6.21.1/pyproject.toml
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       38 2023-06-22 04:36:01.075879 DjAIoT-23.6.21.1/setup.cfg
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.009649 DjAIoT-23.6.21.1/src/
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.021261 DjAIoT-23.6.21.1/src/DjAIoT.egg-info/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5578 2023-06-22 04:36:00.000000 DjAIoT-23.6.21.1/src/DjAIoT.egg-info/PKG-INFO
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5633 2023-06-22 04:36:01.000000 DjAIoT-23.6.21.1/src/DjAIoT.egg-info/SOURCES.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-22 04:36:00.000000 DjAIoT-23.6.21.1/src/DjAIoT.egg-info/dependency_links.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      421 2023-06-22 04:36:00.000000 DjAIoT-23.6.21.1/src/DjAIoT.egg-info/requires.txt
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        7 2023-06-22 04:36:00.000000 DjAIoT-23.6.21.1/src/DjAIoT.egg-info/top_level.txt
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)        1 2023-06-14 22:53:26.000000 DjAIoT-23.6.21.1/src/DjAIoT.egg-info/zip-safe
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.022455 DjAIoT-23.6.21.1/src/djaiot/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      300 2023-03-03 02:23:30.000000 DjAIoT-23.6.21.1/src/djaiot/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.024066 DjAIoT-23.6.21.1/src/djaiot/device_data/
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.026365 DjAIoT-23.6.21.1/src/djaiot/device_data/admin/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      209 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/admin/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    59933 2022-11-06 17:51:40.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/admin/admin copy.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     2822 2022-11-06 17:52:04.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/admin/install_data.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     8503 2022-11-06 17:51:43.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/admin/instance_types.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.026696 DjAIoT-23.6.21.1/src/djaiot/device_data/api/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     3279 2022-11-06 17:51:43.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/field_names.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.027044 DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 23:31:40.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.028058 DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/schema/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:24:27.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/schema/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      742 2022-11-07 00:31:09.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/schema/mutations.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     3287 2022-11-07 00:31:08.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/schema/queries.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     3296 2022-11-07 00:31:08.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/schema/types.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.029242 DjAIoT-23.6.21.1/src/djaiot/device_data/api/python/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)   211423 2022-11-06 23:38:26.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/python/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     1433 2023-05-26 22:13:59.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/python/util.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.029653 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 23:31:40.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.029843 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:18:14.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.030150 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/serializers/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:41:29.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/serializers/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     9566 2022-11-07 00:41:53.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/serializers/serializers.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.031660 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/views/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:41:53.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/views/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    26606 2022-11-07 00:41:53.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/views/views.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.032249 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:24:29.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.032833 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/serializers/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       75 2022-11-07 00:41:53.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/serializers/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    21201 2022-11-07 00:41:53.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/serializers/serializers.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.033633 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/views/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:42:09.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/views/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    26934 2022-11-07 00:42:09.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/views/views.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.035825 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/queries/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       74 2022-11-07 00:20:24.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/queries/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      229 2022-11-07 00:20:24.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/queries/device_class.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     8543 2022-11-07 00:20:24.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/queries/queries.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      377 2022-11-07 00:20:24.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/queries/wsgi.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      685 2023-03-03 02:26:00.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.036864 DjAIoT-23.6.21.1/src/djaiot/device_data/autocompletes/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      217 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/autocompletes/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     2861 2022-11-06 17:51:43.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/autocompletes/autocompletes.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.037653 DjAIoT-23.6.21.1/src/djaiot/device_data/filters/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      211 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/filters/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    31431 2022-11-06 17:52:04.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/filters/filters.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.038663 DjAIoT-23.6.21.1/src/djaiot/device_data/forms/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      209 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/forms/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    15398 2021-09-16 20:59:02.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/forms/forms.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.040108 DjAIoT-23.6.21.1/src/djaiot/device_data/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1858 2023-02-09 04:51:09.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/migrations/0001_JSONInfo.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     2388 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/migrations/0002_DeviceClass.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       54 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.046137 DjAIoT-23.6.21.1/src/djaiot/device_data/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      323 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     4678 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/_abc.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)   167062 2022-11-06 17:51:04.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1591 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_class.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:07.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_data_stream.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:04.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_data_stream_daily_agg.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      447 2022-11-06 17:51:07.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_data_stream_type.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:04.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_family.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:05.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_family_data_stream_pairwise_correlation.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:05.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_family_data_stream_profile.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:07.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_parquet_data_set.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:07.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_site.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 17:51:26.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_sku.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)     1717 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/json_info.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      206 2022-11-06 17:51:05.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/logical_data_type.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     3097 2022-11-06 17:51:07.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/measurement_unit.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     6674 2022-11-06 17:51:04.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/physical_data_type.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.046431 DjAIoT-23.6.21.1/src/djaiot/device_data/models/signals/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      235 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/models/signals/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.047539 DjAIoT-23.6.21.1/src/djaiot/device_data/queries/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      228 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/queries/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    42044 2022-11-06 17:52:19.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/queries/queries.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.048375 DjAIoT-23.6.21.1/src/djaiot/device_data/scripts/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      157 2023-02-09 04:51:25.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/scripts/profile_device_data_streams.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     6126 2022-11-05 15:22:20.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/urls copy.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       53 2023-03-03 02:24:23.000000 DjAIoT-23.6.21.1/src/djaiot/device_data/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.052789 DjAIoT-23.6.21.1/src/djaiot/device_health/
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.056197 DjAIoT-23.6.21.1/src/djaiot/device_health/admin/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      211 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/admin/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    11252 2022-11-06 17:43:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/admin/admin copy 2.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    40753 2022-11-06 17:43:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/admin/admin copy.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       44 2023-02-28 00:14:45.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/admin/admin.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.056591 DjAIoT-23.6.21.1/src/djaiot/device_health/api/
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.057056 DjAIoT-23.6.21.1/src/djaiot/device_health/api/cli/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    76279 2022-11-06 23:37:52.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/cli/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     2176 2022-11-06 17:43:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/field_names.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.057908 DjAIoT-23.6.21.1/src/djaiot/device_health/api/graphql/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-06 23:31:40.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/graphql/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.058908 DjAIoT-23.6.21.1/src/djaiot/device_health/api/graphql/schema/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:20:24.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/graphql/schema/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)       98 2022-11-07 00:20:24.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/graphql/schema/mutations.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:20:24.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/graphql/schema/queries.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:20:24.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/graphql/schema/types.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.059059 DjAIoT-23.6.21.1/src/djaiot/device_health/api/python/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)   150720 2021-09-16 20:59:02.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/python/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.060530 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2021-09-16 20:59:02.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.061670 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/core/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:19:57.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/core/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     6050 2022-11-07 00:19:57.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/core/serializers.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    15965 2022-11-07 00:19:57.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/core/views.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.062770 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/json/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)        0 2022-11-07 00:19:58.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/json/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    15458 2022-11-07 00:19:57.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/json/serializers.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    16710 2022-11-07 00:19:57.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/json/views.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     5131 2021-09-16 20:59:02.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/queries.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      699 2023-03-03 02:28:20.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.063682 DjAIoT-23.6.21.1/src/djaiot/device_health/autocompletes/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      219 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/autocompletes/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      591 2022-11-06 17:47:37.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/autocompletes/autocompletes.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.064563 DjAIoT-23.6.21.1/src/djaiot/device_health/filters/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      213 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/filters/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    38821 2022-11-06 17:43:50.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/filters/filters.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.065723 DjAIoT-23.6.21.1/src/djaiot/device_health/forms/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      211 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/forms/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     8139 2022-11-06 17:47:40.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/forms/forms.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.066428 DjAIoT-23.6.21.1/src/djaiot/device_health/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       56 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.067765 DjAIoT-23.6.21.1/src/djaiot/device_health/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       50 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/models/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    18928 2022-11-06 17:43:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/models/models copy.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)   102757 2022-11-06 17:46:43.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/models/models.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.069145 DjAIoT-23.6.21.1/src/djaiot/device_health/queries/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      230 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/queries/__init__.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    33056 2022-11-06 17:47:39.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/queries/queries.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     4424 2022-11-05 15:22:20.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/urls copy.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       55 2023-03-03 02:28:08.000000 DjAIoT-23.6.21.1/src/djaiot/device_health/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.070289 DjAIoT-23.6.21.1/src/djaiot/device_perf/
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.070726 DjAIoT-23.6.21.1/src/djaiot/device_perf/admin/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      216 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/admin/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      720 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/apps.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.071132 DjAIoT-23.6.21.1/src/djaiot/device_perf/autocompletes/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      224 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/autocompletes/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.071546 DjAIoT-23.6.21.1/src/djaiot/device_perf/filters/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      218 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/filters/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.071985 DjAIoT-23.6.21.1/src/djaiot/device_perf/forms/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      216 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/forms/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.072807 DjAIoT-23.6.21.1/src/djaiot/device_perf/migrations/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       61 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/migrations/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.073476 DjAIoT-23.6.21.1/src/djaiot/device_perf/models/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      224 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/models/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.073977 DjAIoT-23.6.21.1/src/djaiot/device_perf/queries/
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)      235 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/queries/__init__.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       60 2023-03-03 04:41:49.000000 DjAIoT-23.6.21.1/src/djaiot/device_perf/urls.py
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)      670 2022-11-05 02:48:22.000000 DjAIoT-23.6.21.1/src/djaiot/graphql_schema.py
+-rw-r--r--   0 thevinhluong102   (501) staff       (20)       34 2023-03-03 02:23:22.000000 DjAIoT-23.6.21.1/src/djaiot/urls.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.074433 DjAIoT-23.6.21.1/src/djaiot/util/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)     4154 2022-11-05 15:22:20.000000 DjAIoT-23.6.21.1/src/djaiot/util/__init__.py
+drwxr-xr-x   0 thevinhluong102   (501) staff       (20)        0 2023-06-22 04:36:01.074786 DjAIoT-23.6.21.1/src/djaiot/util/cli/
+-rwxr--r--   0 thevinhluong102   (501) staff       (20)    95068 2021-09-16 20:59:02.000000 DjAIoT-23.6.21.1/src/djaiot/util/cli/__init__.py
```

### Comparing `DjAIoT-23.6.14.0/.vscode/settings.json` & `DjAIoT-23.6.21.1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/LICENSE` & `DjAIoT-23.6.21.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/PKG-INFO` & `DjAIoT-23.6.21.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjAIoT
-Version: 23.6.14.0
+Version: 23.6.21.1
 Summary: `DjAIoT`: Artificial Intelligence (AI) in Internet-of-Things (IoT) Applications based on Django
 Author-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 Maintainer-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 License: MIT License
         
         Copyright (c) 2021 The Vinh LUONG (LƯƠNG Thế Vinh)
```

### Comparing `DjAIoT-23.6.14.0/metadata/classifiers` & `DjAIoT-23.6.21.1/metadata/classifiers`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/pyproject.toml` & `DjAIoT-23.6.21.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/DjAIoT.egg-info/PKG-INFO` & `DjAIoT-23.6.21.1/src/DjAIoT.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DjAIoT
-Version: 23.6.14.0
+Version: 23.6.21.1
 Summary: `DjAIoT`: Artificial Intelligence (AI) in Internet-of-Things (IoT) Applications based on Django
 Author-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 Maintainer-email: "STEAM for Vietnam Foundation: AI, IoT & Robotics Educational Initiative" <Edu.AI@STEAMforVietNam.org>
 License: MIT License
         
         Copyright (c) 2021 The Vinh LUONG (LƯƠNG Thế Vinh)
```

### Comparing `DjAIoT-23.6.14.0/src/DjAIoT.egg-info/SOURCES.txt` & `DjAIoT-23.6.21.1/src/DjAIoT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/admin/admin copy.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/admin/admin copy.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/admin/install_data.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/admin/install_data.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/admin/instance_types.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/admin/instance_types.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/field_names.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/field_names.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/schema/mutations.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/schema/mutations.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/schema/queries.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/schema/queries.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/gql/schema/types.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/gql/schema/types.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/python/__init__.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/python/__init__.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/python/util.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/python/util.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/serializers/serializers.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/core/views/views.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/core/views/views.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/serializers/serializers.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/serializers/serializers.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/json/views/views.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/json/views/views.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/api/rest/queries/queries.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/api/rest/queries/queries.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/apps.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/apps.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/autocompletes/autocompletes.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/autocompletes/autocompletes.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/filters/filters.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/filters/filters.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/forms/forms.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/forms/forms.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/migrations/0001_JSONInfo.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/migrations/0001_JSONInfo.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/migrations/0002_DeviceClass.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/migrations/0002_DeviceClass.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/models/_abc.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/models/_abc.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/models/device.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/models/device.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/models/device_class.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/models/device_class.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/models/json_info.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/models/json_info.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/models/measurement_unit.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/models/measurement_unit.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/models/physical_data_type.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/models/physical_data_type.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/queries/queries.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/queries/queries.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_data/urls copy.py` & `DjAIoT-23.6.21.1/src/djaiot/device_data/urls copy.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/admin/admin copy 2.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/admin/admin copy 2.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/admin/admin copy.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/admin/admin copy.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/api/cli/__init__.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/api/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/api/field_names.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/api/field_names.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/api/python/__init__.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/api/python/__init__.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/core/serializers.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/core/serializers.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/core/views.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/core/views.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/json/serializers.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/json/serializers.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/json/views.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/json/views.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/api/rest/queries.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/api/rest/queries.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/apps.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/apps.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/autocompletes/autocompletes.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/autocompletes/autocompletes.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/filters/filters.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/filters/filters.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/forms/forms.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/forms/forms.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/models/models copy.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/models/models copy.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/models/models.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/models/models.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/queries/queries.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/queries/queries.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_health/urls copy.py` & `DjAIoT-23.6.21.1/src/djaiot/device_health/urls copy.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/device_perf/apps.py` & `DjAIoT-23.6.21.1/src/djaiot/device_perf/apps.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/graphql_schema.py` & `DjAIoT-23.6.21.1/src/djaiot/graphql_schema.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/util/__init__.py` & `DjAIoT-23.6.21.1/src/djaiot/util/__init__.py`

 * *Files identical despite different names*

### Comparing `DjAIoT-23.6.14.0/src/djaiot/util/cli/__init__.py` & `DjAIoT-23.6.21.1/src/djaiot/util/cli/__init__.py`

 * *Files identical despite different names*

