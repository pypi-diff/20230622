# Comparing `tmp/pretalx-media-ccc-de-1.1.0.tar.gz` & `tmp/pretalx-media-ccc-de-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretalx-media-ccc-de-1.1.0.tar", last modified: Fri Jun  9 13:20:33 2023, max compression
+gzip compressed data, was "pretalx-media-ccc-de-1.1.1.tar", last modified: Thu Jun 22 16:21:49 2023, max compression
```

## Comparing `pretalx-media-ccc-de-1.1.0.tar` & `pretalx-media-ccc-de-1.1.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.0/LICENSE
--rw-r--r--   0 rixx      (1000) rixx      (1000)      256 2022-01-27 19:06:49.000000 pretalx-media-ccc-de-1.1.0/MANIFEST.in
--rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.0/Makefile
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1212 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)      912 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.0/README.rst
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:09:26.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/__init__.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      578 2023-06-09 13:20:14.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/apps.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1370 2022-12-19 14:09:09.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/forms.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2129 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      460 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2126 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      893 2023-06-07 09:14:31.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2640 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/de/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      625 2021-07-02 10:27:24.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.po
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-07 09:15:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/django.pot
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2042 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-02-19 15:38:17.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      373 2021-07-28 19:29:04.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2021-07-02 10:27:24.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0 rixx      (1000) rixx      (1000)      691 2021-12-14 11:47:59.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/recording.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1776 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/signals.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/static/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/static/pretalx_media_ccc_de/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2019-07-10 20:57:32.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/static/pretalx_media_ccc_de/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2074 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/tasks.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.524108 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2019-07-10 20:57:32.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1443 2021-08-24 22:55:04.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html
--rw-r--r--   0 rixx      (1000) rixx      (1000)      300 2022-07-11 16:34:44.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/urls.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2625 2023-06-09 13:18:43.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/views.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:20:33.527441 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1212 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2589 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/SOURCES.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/dependency_links.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       79 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/entry_points.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       21 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/top_level.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2023-06-09 13:20:33.530774 pretalx-media-ccc-de-1.1.0/setup.cfg
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1081 2023-06-09 13:20:20.000000 pretalx-media-ccc-de-1.1.0/setup.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.1/LICENSE
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      256 2022-01-27 19:06:49.000000 pretalx-media-ccc-de-1.1.1/MANIFEST.in
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.1/Makefile
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1212 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      912 2019-07-10 20:57:31.000000 pretalx-media-ccc-de-1.1.1/README.rst
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:09:26.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/__init__.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      578 2023-06-22 16:21:36.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/apps.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1370 2022-12-19 14:09:09.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/forms.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ar/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2129 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ca/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/cs/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      460 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2126 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      893 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2640 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/de/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      625 2021-07-02 10:27:24.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_Formal/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.po
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-07 09:15:13.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/django.pot
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/el/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/el/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/en_Mozilla/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es_MX/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/fr_FR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/it/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/it/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ja_JP/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_BR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2042 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_PT/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-02-19 15:38:17.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_Hant/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      373 2021-07-28 19:29:04.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2043 2021-07-02 10:27:24.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_TW/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:20:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1996 2023-06-09 13:19:33.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      691 2021-12-14 11:47:59.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/recording.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1776 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/signals.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/static/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/static/pretalx_media_ccc_de/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2019-07-10 20:57:32.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/static/pretalx_media_ccc_de/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2074 2021-12-14 11:48:01.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/tasks.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.503301 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/templates/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.509968 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2019-07-10 20:57:32.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1443 2021-08-24 22:55:04.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      300 2022-07-11 16:34:44.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/urls.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2651 2023-06-22 16:17:44.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/views.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:21:49.506634 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de.egg-info/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1212 2023-06-22 16:21:49.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de.egg-info/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2589 2023-06-22 16:21:49.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de.egg-info/SOURCES.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2023-06-22 16:21:49.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de.egg-info/dependency_links.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       79 2023-06-22 16:21:49.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de.egg-info/entry_points.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       21 2023-06-22 16:21:49.000000 pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de.egg-info/top_level.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2023-06-22 16:21:49.513301 pretalx-media-ccc-de-1.1.1/setup.cfg
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1081 2023-06-22 16:21:29.000000 pretalx-media-ccc-de-1.1.1/setup.py
```

### Comparing `pretalx-media-ccc-de-1.1.0/LICENSE` & `pretalx-media-ccc-de-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/PKG-INFO` & `pretalx-media-ccc-de-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretalx-media-ccc-de
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pull recordings from media.ccc.de and embed them in talk pages
 Home-page: https://github.com/pretalx/pretalx-media-ccc-de.git
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
 License-File: LICENSE
```

### Comparing `pretalx-media-ccc-de-1.1.0/README.rst` & `pretalx-media-ccc-de-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/apps.py` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/apps.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,12 +9,12 @@
     class PretalxPluginMeta:
         name = gettext_lazy("media.ccc.de recordings")
         author = "Tobias Kunze"
         description = gettext_lazy(
             "Pull recordings from media.ccc.de and embed them in talk pages"
         )
         visible = True
-        version = "1.1.0"
+        version = "1.1.1"
 
     def ready(self):
         from . import signals  # NOQA
         from . import tasks  # NOQA
```

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/forms.py` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/forms.py`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.mo` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_DE/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/de_Formal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/django.pot` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/en_Mozilla/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/es_MX/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_Hant/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/recording.py` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/recording.py`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/signals.py` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/signals.py`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/tasks.py` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/tasks.py`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/templates/pretalx_media_ccc_de/settings.html`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de/views.py` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,11 +59,11 @@
         return {"obj": self.request.event, "attribute_name": "settings", **kwargs}
 
     def get_context_data(self, *args, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         kwargs["url_forms"] = [
             MediaCCCDeUrlForm(submission=slot.submission)
             for slot in self.request.event.current_schedule.talks.all()
-            .filter(is_visible=True)
+            .filter(is_visible=True, submission__isnull=False)
             .order_by("start")
         ]
         return kwargs
```

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/PKG-INFO` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretalx-media-ccc-de
-Version: 1.1.0
+Version: 1.1.1
 Summary: Pull recordings from media.ccc.de and embed them in talk pages
 Home-page: https://github.com/pretalx/pretalx-media-ccc-de.git
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
 License-File: LICENSE
```

### Comparing `pretalx-media-ccc-de-1.1.0/pretalx_media_ccc_de.egg-info/SOURCES.txt` & `pretalx-media-ccc-de-1.1.1/pretalx_media_ccc_de.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/setup.cfg` & `pretalx-media-ccc-de-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretalx-media-ccc-de-1.1.0/setup.py` & `pretalx-media-ccc-de-1.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 cmdclass = {"build": CustomBuild}
 
 
 setup(
     name="pretalx-media-ccc-de",
-    version="1.1.0",
+    version="1.1.1",
     description="Pull recordings from media.ccc.de and embed them in talk pages",
     long_description=long_description,
     url="https://github.com/pretalx/pretalx-media-ccc-de.git",
     author="Tobias Kunze",
     author_email="r@rixx.de",
     license="Apache Software License",
     install_requires=[],
```

