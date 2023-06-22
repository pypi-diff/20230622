# Comparing `tmp/bpkio_python_sdk-1.4.0.tar.gz` & `tmp/bpkio_python_sdk-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpkio_python_sdk-1.4.0.tar", max compression
+gzip compressed data, was "bpkio_python_sdk-1.4.1.tar", max compression
```

## Comparing `bpkio_python_sdk-1.4.0.tar` & `bpkio_python_sdk-1.4.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.4.0/README.md
--rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.4.0/bpkio_api/__init__.py
--rw-r--r--   0        0        0     5794 2023-06-09 10:58:27.429762 bpkio_python_sdk-1.4.0/bpkio_api/api.py
--rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.4.0/bpkio_api/caching.py
--rw-r--r--   0        0        0      506 2023-06-09 11:08:00.617751 bpkio_python_sdk-1.4.0/bpkio_api/consumer.py
--rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.4.0/bpkio_api/credential_provider.py
--rw-r--r--   0        0        0      178 2023-06-09 11:21:14.279980 bpkio_python_sdk-1.4.0/bpkio_api/defaults.py
--rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/__init__.py
--rw-r--r--   0        0        0     4563 2023-06-09 11:03:02.185931 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/categories.py
--rw-r--r--   0        0        0      747 2023-06-09 11:03:16.109406 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/consumption.py
--rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/enums.py
--rw-r--r--   0        0        0    22070 2023-06-09 11:08:21.660390 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/services.py
--rw-r--r--   0        0        0    21704 2023-06-09 11:08:38.030315 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/sources.py
--rw-r--r--   0        0        0     2721 2023-06-09 11:05:03.964297 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/tenants.py
--rw-r--r--   0        0        0     6014 2023-06-09 11:05:16.807277 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/transcoding_profiles.py
--rw-r--r--   0        0        0     2673 2023-06-09 11:05:32.498036 bpkio_python_sdk-1.4.0/bpkio_api/endpoints/users.py
--rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.4.0/bpkio_api/exceptions.py
--rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.4.0/bpkio_api/helpers/codecstrings.py
--rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/__init__.py
--rw-r--r--   0        0        0     4582 2023-06-09 11:40:34.918187 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/dash.py
--rw-r--r--   0        0        0     3532 2023-06-09 12:34:36.766352 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/factory.py
--rw-r--r--   0        0        0     2949 2023-06-09 14:49:36.436548 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/generic.py
--rw-r--r--   0        0        0     4521 2023-06-09 11:38:49.325871 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/hls.py
--rw-r--r--   0        0        0      446 2023-06-09 11:39:02.452951 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/jpeg.py
--rw-r--r--   0        0        0      472 2023-06-09 11:40:16.383318 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/mp4.py
--rw-r--r--   0        0        0      434 2023-06-09 11:40:11.132158 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/png.py
--rw-r--r--   0        0        0     1976 2023-06-09 11:39:37.280020 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/vast.py
--rw-r--r--   0        0        0     2325 2023-06-09 11:39:46.049574 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/vmap.py
--rw-r--r--   0        0        0      580 2023-06-09 11:39:59.258206 bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/xml.py
--rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.4.0/bpkio_api/helpers/list.py
--rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.4.0/bpkio_api/helpers/objects.py
--rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/__init__.py
--rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/analyser.py
--rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/dash.py
--rw-r--r--   0        0        0     3360 2023-05-23 21:47:41.314435 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/hls.py
--rw-r--r--   0        0        0     1587 2023-05-23 22:08:22.519293 bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/profile_generator.py
--rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/__init__.py
--rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/curl.py
--rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/exporter.py
--rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/markdown.py
--rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/postman.py
--rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/session_items.py
--rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/session_recorder.py
--rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/text.py
--rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.4.0/bpkio_api/helpers/search.py
--rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.4.0/bpkio_api/helpers/source_type.py
--rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.4.0/bpkio_api/helpers/times.py
--rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.4.0/bpkio_api/mappings.py
--rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.4.0/bpkio_api/models/Categories.py
--rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.4.0/bpkio_api/models/Consumption.py
--rw-r--r--   0        0        0     5036 2023-05-20 07:16:01.794965 bpkio_python_sdk-1.4.0/bpkio_api/models/Services.py
--rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.4.0/bpkio_api/models/Slots.py
--rw-r--r--   0        0        0     3136 2023-05-01 20:17:25.667591 bpkio_python_sdk-1.4.0/bpkio_api/models/Sources.py
--rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.4.0/bpkio_api/models/Tenants.py
--rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.4.0/bpkio_api/models/TranscodingProfiles.py
--rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.4.0/bpkio_api/models/Users.py
--rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.4.0/bpkio_api/models/__init__.py
--rw-r--r--   0        0        0      911 2023-05-18 20:10:20.759170 bpkio_python_sdk-1.4.0/bpkio_api/models/common.py
--rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.4.0/bpkio_api/models/model_graph.py
--rw-r--r--   0        0        0     2152 2023-06-09 10:37:32.988041 bpkio_python_sdk-1.4.0/bpkio_api/response_handler.py
--rw-r--r--   0        0        0     1195 2023-06-09 15:44:56.748527 bpkio_python_sdk-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-26 15:21:53.748951 bpkio_python_sdk-1.4.1/README.md
+-rw-r--r--   0        0        0      203 2023-05-17 14:14:39.237826 bpkio_python_sdk-1.4.1/bpkio_api/__init__.py
+-rw-r--r--   0        0        0     5794 2023-06-09 10:58:27.429762 bpkio_python_sdk-1.4.1/bpkio_api/api.py
+-rw-r--r--   0        0        0     1846 2023-05-21 21:00:22.979671 bpkio_python_sdk-1.4.1/bpkio_api/caching.py
+-rw-r--r--   0        0        0      506 2023-06-09 11:08:00.617751 bpkio_python_sdk-1.4.1/bpkio_api/consumer.py
+-rw-r--r--   0        0        0     4038 2023-05-17 21:43:51.682208 bpkio_python_sdk-1.4.1/bpkio_api/credential_provider.py
+-rw-r--r--   0        0        0      178 2023-06-09 11:21:14.279980 bpkio_python_sdk-1.4.1/bpkio_api/defaults.py
+-rw-r--r--   0        0        0      393 2023-04-07 16:54:49.526444 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/__init__.py
+-rw-r--r--   0        0        0     4563 2023-06-09 11:03:02.185931 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/categories.py
+-rw-r--r--   0        0        0      747 2023-06-09 11:03:16.109406 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/consumption.py
+-rw-r--r--   0        0        0      122 2023-05-20 07:16:01.791125 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/enums.py
+-rw-r--r--   0        0        0    22070 2023-06-09 11:08:21.660390 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/services.py
+-rw-r--r--   0        0        0    21704 2023-06-09 11:08:38.030315 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/sources.py
+-rw-r--r--   0        0        0     2721 2023-06-09 11:05:03.964297 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/tenants.py
+-rw-r--r--   0        0        0     6014 2023-06-09 11:05:16.807277 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/transcoding_profiles.py
+-rw-r--r--   0        0        0     2673 2023-06-09 11:05:32.498036 bpkio_python_sdk-1.4.1/bpkio_api/endpoints/users.py
+-rw-r--r--   0        0        0     1046 2023-04-09 18:25:32.780569 bpkio_python_sdk-1.4.1/bpkio_api/exceptions.py
+-rw-r--r--   0        0        0     2449 2023-04-29 21:37:29.834823 bpkio_python_sdk-1.4.1/bpkio_api/helpers/codecstrings.py
+-rw-r--r--   0        0        0      290 2023-04-25 10:30:47.335772 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/__init__.py
+-rw-r--r--   0        0        0     4582 2023-06-09 11:40:34.918187 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/dash.py
+-rw-r--r--   0        0        0     3532 2023-06-09 12:34:36.766352 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/factory.py
+-rw-r--r--   0        0        0     2949 2023-06-09 14:49:36.436548 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/generic.py
+-rw-r--r--   0        0        0     4521 2023-06-14 13:48:46.586787 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/hls.py
+-rw-r--r--   0        0        0      446 2023-06-09 11:39:02.452951 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/jpeg.py
+-rw-r--r--   0        0        0      472 2023-06-09 11:40:16.383318 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/mp4.py
+-rw-r--r--   0        0        0      434 2023-06-09 11:40:11.132158 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/png.py
+-rw-r--r--   0        0        0     1976 2023-06-09 11:39:37.280020 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/vast.py
+-rw-r--r--   0        0        0     2325 2023-06-09 11:39:46.049574 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/vmap.py
+-rw-r--r--   0        0        0      580 2023-06-09 11:39:59.258206 bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/xml.py
+-rw-r--r--   0        0        0      829 2023-05-12 07:24:24.243818 bpkio_python_sdk-1.4.1/bpkio_api/helpers/list.py
+-rw-r--r--   0        0        0      442 2023-04-23 18:47:18.968034 bpkio_python_sdk-1.4.1/bpkio_api/helpers/objects.py
+-rw-r--r--   0        0        0      119 2023-04-29 21:53:41.608570 bpkio_python_sdk-1.4.1/bpkio_api/helpers/profile_generator/__init__.py
+-rw-r--r--   0        0        0      461 2023-04-30 19:12:24.858790 bpkio_python_sdk-1.4.1/bpkio_api/helpers/profile_generator/analyser.py
+-rw-r--r--   0        0        0     1713 2023-04-29 21:41:55.874476 bpkio_python_sdk-1.4.1/bpkio_api/helpers/profile_generator/dash.py
+-rw-r--r--   0        0        0     3360 2023-05-23 21:47:41.314435 bpkio_python_sdk-1.4.1/bpkio_api/helpers/profile_generator/hls.py
+-rw-r--r--   0        0        0     1728 2023-06-16 10:38:47.386661 bpkio_python_sdk-1.4.1/bpkio_api/helpers/profile_generator/profile_generator.py
+-rw-r--r--   0        0        0      127 2023-05-21 20:48:50.293128 bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/__init__.py
+-rw-r--r--   0        0        0     3600 2023-05-21 08:17:50.000601 bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/curl.py
+-rw-r--r--   0        0        0     1440 2023-05-21 08:26:30.294698 bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/exporter.py
+-rw-r--r--   0        0        0     2499 2023-05-21 21:03:14.891415 bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/markdown.py
+-rw-r--r--   0        0        0     6158 2023-05-21 21:04:23.629108 bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/postman.py
+-rw-r--r--   0        0        0      626 2023-05-20 15:13:58.838560 bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/session_items.py
+-rw-r--r--   0        0        0     4184 2023-05-24 07:02:25.413166 bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/session_recorder.py
+-rw-r--r--   0        0        0     1461 2023-05-21 21:01:55.655743 bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/text.py
+-rw-r--r--   0        0        0     1464 2023-03-27 20:12:34.222658 bpkio_python_sdk-1.4.1/bpkio_api/helpers/search.py
+-rw-r--r--   0        0        0     1075 2023-04-29 18:54:18.517631 bpkio_python_sdk-1.4.1/bpkio_api/helpers/source_type.py
+-rw-r--r--   0        0        0     2108 2023-05-20 07:16:01.794406 bpkio_python_sdk-1.4.1/bpkio_api/helpers/times.py
+-rw-r--r--   0        0        0     2621 2023-05-17 14:38:59.521244 bpkio_python_sdk-1.4.1/bpkio_api/mappings.py
+-rw-r--r--   0        0        0      305 2023-04-16 00:14:59.527618 bpkio_python_sdk-1.4.1/bpkio_api/models/Categories.py
+-rw-r--r--   0        0        0      338 2023-04-06 18:07:44.688798 bpkio_python_sdk-1.4.1/bpkio_api/models/Consumption.py
+-rw-r--r--   0        0        0     5036 2023-05-20 07:16:01.794965 bpkio_python_sdk-1.4.1/bpkio_api/models/Services.py
+-rw-r--r--   0        0        0     1655 2023-05-20 07:16:01.795523 bpkio_python_sdk-1.4.1/bpkio_api/models/Slots.py
+-rw-r--r--   0        0        0     3142 2023-06-16 19:27:48.570327 bpkio_python_sdk-1.4.1/bpkio_api/models/Sources.py
+-rw-r--r--   0        0        0      413 2023-04-16 00:16:26.848163 bpkio_python_sdk-1.4.1/bpkio_api/models/Tenants.py
+-rw-r--r--   0        0        0      490 2023-05-04 09:32:32.372844 bpkio_python_sdk-1.4.1/bpkio_api/models/TranscodingProfiles.py
+-rw-r--r--   0        0        0      365 2023-04-26 08:30:20.691048 bpkio_python_sdk-1.4.1/bpkio_api/models/Users.py
+-rw-r--r--   0        0        0     1423 2023-05-04 09:38:56.033293 bpkio_python_sdk-1.4.1/bpkio_api/models/__init__.py
+-rw-r--r--   0        0        0      911 2023-05-18 20:10:20.759170 bpkio_python_sdk-1.4.1/bpkio_api/models/common.py
+-rw-r--r--   0        0        0     2152 2023-04-24 18:28:45.561873 bpkio_python_sdk-1.4.1/bpkio_api/models/model_graph.py
+-rw-r--r--   0        0        0     2152 2023-06-09 10:37:32.988041 bpkio_python_sdk-1.4.1/bpkio_api/response_handler.py
+-rw-r--r--   0        0        0     1195 2023-06-22 10:40:37.616600 bpkio_python_sdk-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      778 1970-01-01 00:00:00.000000 bpkio_python_sdk-1.4.1/PKG-INFO
```

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/api.py` & `bpkio_python_sdk-1.4.1/bpkio_api/api.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/caching.py` & `bpkio_python_sdk-1.4.1/bpkio_api/caching.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/credential_provider.py` & `bpkio_python_sdk-1.4.1/bpkio_api/credential_provider.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/categories.py` & `bpkio_python_sdk-1.4.1/bpkio_api/endpoints/categories.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/consumption.py` & `bpkio_python_sdk-1.4.1/bpkio_api/endpoints/consumption.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/services.py` & `bpkio_python_sdk-1.4.1/bpkio_api/endpoints/services.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/sources.py` & `bpkio_python_sdk-1.4.1/bpkio_api/endpoints/sources.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/tenants.py` & `bpkio_python_sdk-1.4.1/bpkio_api/endpoints/tenants.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/transcoding_profiles.py` & `bpkio_python_sdk-1.4.1/bpkio_api/endpoints/transcoding_profiles.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/endpoints/users.py` & `bpkio_python_sdk-1.4.1/bpkio_api/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/exceptions.py` & `bpkio_python_sdk-1.4.1/bpkio_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/codecstrings.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/codecstrings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/dash.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/factory.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/factory.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/generic.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/generic.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/hls.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/hls.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/vast.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/vast.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/vmap.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/vmap.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/handlers/xml.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/handlers/xml.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/list.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/list.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/dash.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/profile_generator/dash.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/hls.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/profile_generator/hls.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/profile_generator/profile_generator.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/profile_generator/profile_generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,17 @@
 
         jobs = []
         for r in renditions:
             if r["type"] == "video":
                 jobs.append(
                     {
                         "level": str(r["level"]),
-                        "scale": f"-1:{r['resolution'][1]}",
+                        # -2 seems to ensure that the calculated width is divisible by 2, 
+                        # a constraint of libx264
+                        "scale": f"-2:{r['resolution'][1]}",
                         "bitratev": str(r["bitrate"]),
                         "profilev": r["profile"],
                         "frameratev": str(r["framerate"]),
                     }
                 )
 
             if r["type"] == "audio":
```

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/curl.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/curl.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/exporter.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/exporter.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/markdown.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/markdown.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/postman.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/postman.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/session_items.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/session_items.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/session_recorder.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/session_recorder.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/recorder/text.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/recorder/text.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/search.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/search.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/source_type.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/source_type.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/helpers/times.py` & `bpkio_python_sdk-1.4.1/bpkio_api/helpers/times.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/mappings.py` & `bpkio_python_sdk-1.4.1/bpkio_api/mappings.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/models/Services.py` & `bpkio_python_sdk-1.4.1/bpkio_api/models/Services.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/models/Slots.py` & `bpkio_python_sdk-1.4.1/bpkio_api/models/Slots.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/models/Sources.py` & `bpkio_python_sdk-1.4.1/bpkio_api/models/Sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         return str(self.value)
 
 
 # === SOURCES Models ===
 
 
 class SourceIn(NamedModel, PropertyMixin):
-    url: AnyHttpUrl
+    url: AnyHttpUrl | str
 
     @property
     def full_url(self):
         return self.make_full_url()
 
     def make_full_url(self, *args, **kwargs):
         return self.url
```

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/models/__init__.py` & `bpkio_python_sdk-1.4.1/bpkio_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/models/common.py` & `bpkio_python_sdk-1.4.1/bpkio_api/models/common.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/models/model_graph.py` & `bpkio_python_sdk-1.4.1/bpkio_api/models/model_graph.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/bpkio_api/response_handler.py` & `bpkio_python_sdk-1.4.1/bpkio_api/response_handler.py`

 * *Files identical despite different names*

### Comparing `bpkio_python_sdk-1.4.0/pyproject.toml` & `bpkio_python_sdk-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bpkio-python-sdk"
-version = "1.4.0"
+version = "1.4.1"
 description = "An (opinionated) Python SDK for the broadpeak.io REST APIs"
 authors = ["Fabre Lambeau <fabre.lambeau@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "bpkio_api" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bpkio_python_sdk-1.4.0/PKG-INFO` & `bpkio_python_sdk-1.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpkio-python-sdk
-Version: 1.4.0
+Version: 1.4.1
 Summary: An (opinionated) Python SDK for the broadpeak.io REST APIs
 Author: Fabre Lambeau
 Author-email: fabre.lambeau@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

