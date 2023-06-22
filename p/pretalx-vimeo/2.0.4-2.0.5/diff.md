# Comparing `tmp/pretalx-vimeo-2.0.4.tar.gz` & `tmp/pretalx-vimeo-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretalx-vimeo-2.0.4.tar", last modified: Mon Oct 31 23:18:41 2022, max compression
+gzip compressed data, was "pretalx-vimeo-2.0.5.tar", last modified: Thu Jun 22 16:20:34 2023, max compression
```

## Comparing `pretalx-vimeo-2.0.4.tar` & `pretalx-vimeo-2.0.5.tar`

### file list

```diff
@@ -1,94 +1,98 @@
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.734150 pretalx-vimeo-2.0.4/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.4/LICENSE
--rw-r--r--   0 rixx      (1000) rixx      (1000)      220 2022-01-28 01:46:33.000000 pretalx-vimeo-2.0.4/MANIFEST.in
--rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.4/Makefile
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1474 2022-10-31 23:18:41.734150 pretalx-vimeo-2.0.4/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1194 2021-12-15 00:49:20.000000 pretalx-vimeo-2.0.4/README.rst
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.720817 pretalx-vimeo-2.0.4/pretalx_vimeo/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:17:57.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/__init__.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      532 2022-10-31 23:18:24.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/apps.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1334 2022-07-11 16:29:55.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/forms.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.724150 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ar/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.724150 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ar/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1533 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ca/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.724150 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ca/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/cs/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.724150 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/cs/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      460 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1530 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_DE/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.724150 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_DE/LC_MESSAGES/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_DE/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_Formal/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.727483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_Formal/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_Formal/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_Formal/LC_MESSAGES/django.po
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2022-10-31 00:08:25.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/django.pot
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/el/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.727483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/el/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/en_Mozilla/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.727483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/en_Mozilla/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2021-12-14 00:10:24.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/en_Mozilla/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1373 2021-10-26 13:05:59.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/en_Mozilla/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.727483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es_MX/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.727483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es_MX/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es_MX/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es_MX/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/fr_FR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.727483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/it/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.730817 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/it/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ja_JP/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.730817 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/pt_BR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.730817 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1446 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.707483 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/zh_TW/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.730817 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2022-10-31 00:02:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2022-10-31 23:17:50.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.730817 pretalx-vimeo-2.0.4/pretalx_vimeo/migrations/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      969 2021-12-15 00:16:42.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/migrations/0001_initial.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1335 2021-12-15 00:19:09.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/migrations/0002_data.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 00:07:31.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/migrations/__init__.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      781 2021-12-15 00:40:46.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/models.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      306 2021-12-15 00:28:00.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/recording.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      827 2021-12-14 12:06:28.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/signals.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.710816 pretalx-vimeo-2.0.4/pretalx_vimeo/static/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.730817 pretalx-vimeo-2.0.4/pretalx_vimeo/static/pretalx_vimeo/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/static/pretalx_vimeo/.gitkeep
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.710816 pretalx-vimeo-2.0.4/pretalx_vimeo/templates/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.730817 pretalx-vimeo-2.0.4/pretalx_vimeo/templates/pretalx_vimeo/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/templates/pretalx_vimeo/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)      817 2021-08-29 21:27:39.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/templates/pretalx_vimeo/settings.html
--rw-r--r--   0 rixx      (1000) rixx      (1000)      592 2022-07-11 16:29:33.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/urls.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2569 2021-12-15 00:53:56.000000 pretalx-vimeo-2.0.4/pretalx_vimeo/views.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:18:41.724150 pretalx-vimeo-2.0.4/pretalx_vimeo.egg-info/
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1474 2022-10-31 23:18:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo.egg-info/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2179 2022-10-31 23:18:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo.egg-info/SOURCES.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2022-10-31 23:18:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo.egg-info/dependency_links.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       64 2022-10-31 23:18:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo.egg-info/entry_points.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       14 2022-10-31 23:18:41.000000 pretalx-vimeo-2.0.4/pretalx_vimeo.egg-info/top_level.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2022-10-31 23:18:41.734150 pretalx-vimeo-2.0.4/setup.cfg
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1035 2022-10-31 23:18:10.000000 pretalx-vimeo-2.0.4/setup.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.5/LICENSE
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      220 2022-01-28 01:46:33.000000 pretalx-vimeo-2.0.5/MANIFEST.in
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.5/Makefile
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1454 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1194 2021-12-15 00:49:20.000000 pretalx-vimeo-2.0.5/README.rst
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:17:57.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/__init__.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      532 2023-06-22 16:19:40.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/apps.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1333 2022-12-19 14:09:09.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/forms.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.263714 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ar/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1533 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.263714 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ca/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.263714 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/cs/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      460 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1530 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_DE/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_DE/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-07 09:14:31.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_DE/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_Formal/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_Formal/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_Formal/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_Formal/LC_MESSAGES/django.po
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2023-06-07 09:15:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/django.pot
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/el/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/el/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/en_Mozilla/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/en_Mozilla/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/en_Mozilla/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1373 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/en_Mozilla/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es_MX/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es_MX/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es_MX/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es_MX/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/fr_FR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/it/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.270380 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/it/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1447 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ja_JP/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_BR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1446 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_PT/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2023-02-19 15:38:17.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/zh_TW/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1400 2023-06-22 16:19:52.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/pretalx_vimeo/migrations/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      968 2022-12-19 14:09:09.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/migrations/0001_initial.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1334 2022-12-19 14:09:09.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/migrations/0002_data.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 00:07:31.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/migrations/__init__.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      781 2021-12-15 00:40:46.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/models.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      306 2021-12-15 00:28:00.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/recording.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      827 2021-12-14 12:06:28.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/signals.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/static/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/pretalx_vimeo/static/pretalx_vimeo/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/static/pretalx_vimeo/.gitkeep
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo/templates/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/pretalx_vimeo/templates/pretalx_vimeo/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-08-24 22:32:08.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/templates/pretalx_vimeo/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      817 2021-08-29 21:27:39.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/templates/pretalx_vimeo/settings.html
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      592 2022-07-11 16:29:33.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/urls.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2669 2023-06-22 16:18:12.000000 pretalx-vimeo-2.0.5/pretalx_vimeo/views.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:20:34.267047 pretalx-vimeo-2.0.5/pretalx_vimeo.egg-info/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1454 2023-06-22 16:20:34.000000 pretalx-vimeo-2.0.5/pretalx_vimeo.egg-info/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2277 2023-06-22 16:20:34.000000 pretalx-vimeo-2.0.5/pretalx_vimeo.egg-info/SOURCES.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2023-06-22 16:20:34.000000 pretalx-vimeo-2.0.5/pretalx_vimeo.egg-info/dependency_links.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       65 2023-06-22 16:20:34.000000 pretalx-vimeo-2.0.5/pretalx_vimeo.egg-info/entry_points.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       14 2023-06-22 16:20:34.000000 pretalx-vimeo-2.0.5/pretalx_vimeo.egg-info/top_level.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2023-06-22 16:20:34.273714 pretalx-vimeo-2.0.5/setup.cfg
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1035 2023-06-22 16:19:30.000000 pretalx-vimeo-2.0.5/setup.py
```

### Comparing `pretalx-vimeo-2.0.4/LICENSE` & `pretalx-vimeo-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/PKG-INFO` & `pretalx-vimeo-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pretalx-vimeo
-Version: 2.0.4
+Version: 2.0.5
 Summary: Embed Vimeo videos as session recordings
 Home-page: https://github.com/pretalx/pretalx-vimeo
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
-Platform: UNKNOWN
 License-File: LICENSE
 
 Vimeo integration
 =================
 
 This is a plugin for `pretalx`_ that provides an integration with Vimeo, allowing you to embed recordings on talk pages.
 
@@ -40,9 +39,7 @@
 Copyright 2021 Tobias Kunze
 
 Released under the terms of the Apache License 2.0
 
 
 .. _pretalx: https://github.com/pretalx/pretalx
 .. _pretalx development setup: https://docs.pretalx.org/en/latest/developer/setup.html
-
-
```

### Comparing `pretalx-vimeo-2.0.4/README.rst` & `pretalx-vimeo-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/apps.py` & `pretalx-vimeo-2.0.5/pretalx_vimeo/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     class PretalxPluginMeta:
         name = gettext_lazy("Vimeo integration")
         author = "Tobias Kunze"
         description = gettext_lazy(
             "Embed Vimeo videos as session recordings, and retrieve them via an API."
         )
         visible = True
-        version = "2.0.4"
+        version = "2.0.5"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/forms.py` & `pretalx-vimeo-2.0.5/pretalx_vimeo/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from django import forms
 from django.utils.translation import gettext_lazy as _
 
 from .models import VimeoLink
 
 
 class VimeoUrlForm(forms.Form):
-
     video_id = forms.URLField(required=False)
 
     def __init__(self, *args, **kwargs):
         self.submission = kwargs.pop("submission")
 
         vimeo = getattr(self.submission, "vimeo_link", None)
         if vimeo:
```

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ar/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ca/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/cs/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_DE/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/de_Formal/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/de_Formal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/django.pot` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-10-31 00:08+0000\n"
+"POT-Creation-Date: 2023-02-19 15:38+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -21,15 +21,15 @@
 msgid "Vimeo integration"
 msgstr ""
 
 #: local/pretalx-vimeo/pretalx_vimeo/apps.py:13
 msgid "Embed Vimeo videos as session recordings, and retrieve them via an API."
 msgstr ""
 
-#: local/pretalx-vimeo/pretalx_vimeo/forms.py:27
+#: local/pretalx-vimeo/pretalx_vimeo/forms.py:26
 msgid "Please provide a Vimeo URL!"
 msgstr ""
 
 #: local/pretalx-vimeo/pretalx_vimeo/templates/pretalx_vimeo/settings.html:7
 msgid "Set up Vimeo embeds"
 msgstr ""
```

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/el/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/en_Mozilla/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/en_Mozilla/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/es_MX/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/es_MX/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/it/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/ja_JP/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/pt_BR/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/locale/zh_TW/LC_MESSAGES/django.po` & `pretalx-vimeo-2.0.5/pretalx_vimeo/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/migrations/0001_initial.py` & `pretalx-vimeo-2.0.5/pretalx_vimeo/migrations/0001_initial.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # Generated by Django 3.2.4 on 2021-12-15 00:07
 
 from django.db import migrations, models
 import django.db.models.deletion
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = [
         ("submission", "0062_cfp_settings_data"),
     ]
 
     operations = [
```

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/migrations/0002_data.py` & `pretalx-vimeo-2.0.5/pretalx_vimeo/migrations/0002_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,13 +30,12 @@
 
 def delete_all_links(apps, schema_editor):
     VimeoLink = apps.get_model("pretalx_vimeo", "VimeoLink")
     VimeoLink.objects.all().delete()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("pretalx_vimeo", "0001_initial"),
     ]
 
     operations = [migrations.RunPython(migrate_data, migrations.RunPython.noop)]
```

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/models.py` & `pretalx-vimeo-2.0.5/pretalx_vimeo/models.py`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/signals.py` & `pretalx-vimeo-2.0.5/pretalx_vimeo/signals.py`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/templates/pretalx_vimeo/settings.html` & `pretalx-vimeo-2.0.5/pretalx_vimeo/templates/pretalx_vimeo/settings.html`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/urls.py` & `pretalx-vimeo-2.0.5/pretalx_vimeo/urls.py`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo/views.py` & `pretalx-vimeo-2.0.5/pretalx_vimeo/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,17 @@
 
         return super().post(request, *args, **kwargs)
 
     def get_context_data(self, *args, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         kwargs["url_forms"] = [
             VimeoUrlForm(submission=submission)
-            for submission in self.request.event.talks
+            for submission in self.request.event.talks.all()
+            .filter(is_visible=True, submission__isnull=False)
+            .order_by("start")
         ]
         return kwargs
 
 
 def check_api_access(request):
     if "pretalx_vimeo" not in request.event.plugin_list:
         raise Http404()
```

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo.egg-info/PKG-INFO` & `pretalx-vimeo-2.0.5/pretalx_vimeo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pretalx-vimeo
-Version: 2.0.4
+Version: 2.0.5
 Summary: Embed Vimeo videos as session recordings
 Home-page: https://github.com/pretalx/pretalx-vimeo
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
-Platform: UNKNOWN
 License-File: LICENSE
 
 Vimeo integration
 =================
 
 This is a plugin for `pretalx`_ that provides an integration with Vimeo, allowing you to embed recordings on talk pages.
 
@@ -40,9 +39,7 @@
 Copyright 2021 Tobias Kunze
 
 Released under the terms of the Apache License 2.0
 
 
 .. _pretalx: https://github.com/pretalx/pretalx
 .. _pretalx development setup: https://docs.pretalx.org/en/latest/developer/setup.html
-
-
```

### Comparing `pretalx-vimeo-2.0.4/pretalx_vimeo.egg-info/SOURCES.txt` & `pretalx-vimeo-2.0.5/pretalx_vimeo.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 pretalx_vimeo/locale/fr_FR/LC_MESSAGES/django.po
 pretalx_vimeo/locale/it/LC_MESSAGES/django.mo
 pretalx_vimeo/locale/it/LC_MESSAGES/django.po
 pretalx_vimeo/locale/ja_JP/LC_MESSAGES/django.mo
 pretalx_vimeo/locale/ja_JP/LC_MESSAGES/django.po
 pretalx_vimeo/locale/pt_BR/LC_MESSAGES/django.mo
 pretalx_vimeo/locale/pt_BR/LC_MESSAGES/django.po
+pretalx_vimeo/locale/pt_PT/LC_MESSAGES/django.mo
+pretalx_vimeo/locale/pt_PT/LC_MESSAGES/django.po
 pretalx_vimeo/locale/zh_TW/LC_MESSAGES/django.mo
 pretalx_vimeo/locale/zh_TW/LC_MESSAGES/django.po
 pretalx_vimeo/migrations/0001_initial.py
 pretalx_vimeo/migrations/0002_data.py
 pretalx_vimeo/migrations/__init__.py
 pretalx_vimeo/static/pretalx_vimeo/.gitkeep
 pretalx_vimeo/templates/pretalx_vimeo/.gitkeep
```

### Comparing `pretalx-vimeo-2.0.4/setup.cfg` & `pretalx-vimeo-2.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretalx-vimeo-2.0.4/setup.py` & `pretalx-vimeo-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 cmdclass = {"build": CustomBuild}
 
 
 setup(
     name="pretalx-vimeo",
-    version="2.0.4",
+    version="2.0.5",
     description="Embed Vimeo videos as session recordings",
     long_description=long_description,
     url="https://github.com/pretalx/pretalx-vimeo",
     author="Tobias Kunze",
     author_email="r@rixx.de",
     license="Apache Software License",
     install_requires=[],
```

