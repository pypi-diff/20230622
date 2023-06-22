# Comparing `tmp/pretalx-youtube-1.2.0.tar.gz` & `tmp/pretalx-youtube-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretalx-youtube-1.2.0.tar", last modified: Fri Jun  9 13:19:19 2023, max compression
+gzip compressed data, was "pretalx-youtube-1.2.1.tar", last modified: Thu Jun 22 16:19:16 2023, max compression
```

## Comparing `pretalx-youtube-1.2.0.tar` & `pretalx-youtube-1.2.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2021-12-15 01:11:11.000000 pretalx-youtube-1.2.0/LICENSE
--rw-r--r--   0 rixx      (1000) rixx      (1000)      230 2022-01-28 01:52:30.000000 pretalx-youtube-1.2.0/MANIFEST.in
--rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2021-12-15 01:09:31.000000 pretalx-youtube-1.2.0/Makefile
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1476 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1210 2021-12-15 01:28:25.000000 pretalx-youtube-1.2.0/README.rst
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:19:32.000000 pretalx-youtube-1.2.0/pretalx_youtube/__init__.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      540 2023-06-09 13:18:53.000000 pretalx-youtube-1.2.0/pretalx_youtube/apps.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1859 2023-06-09 13:06:24.000000 pretalx-youtube-1.2.0/pretalx_youtube/forms.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/ar/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/ar/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1675 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/ca/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/ca/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/cs/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/cs/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1308 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2030 2023-06-09 13:06:24.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/de_DE/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/de_Formal/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/de_Formal/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-07 09:15:13.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/django.pot
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/el/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/el/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/el/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/en_Mozilla/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-02-19 15:38:17.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/es/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/es/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/es_MX/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/locale/es_MX/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/fr_FR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/locale/fr_FR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/it/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/locale/it/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/ja_JP/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.907845 pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_BR/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1588 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_PT/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-02-19 15:38:17.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/locale/zh_TW/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.0/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/migrations/
--rw-r--r--   0 rixx      (1000) rixx      (1000)      972 2023-06-09 13:06:24.000000 pretalx-youtube-1.2.0/pretalx_youtube/migrations/0001_initial.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:19:02.000000 pretalx-youtube-1.2.0/pretalx_youtube/migrations/__init__.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      820 2021-12-15 01:24:02.000000 pretalx-youtube-1.2.0/pretalx_youtube/models.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      372 2021-12-15 01:24:02.000000 pretalx-youtube-1.2.0/pretalx_youtube/recording.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)      841 2021-12-15 01:21:10.000000 pretalx-youtube-1.2.0/pretalx_youtube/signals.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/static/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/static/pretalx_youtube/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:09:31.000000 pretalx-youtube-1.2.0/pretalx_youtube/static/pretalx_youtube/.gitkeep
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube/templates/
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/pretalx_youtube/templates/pretalx_youtube/
--rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:09:31.000000 pretalx-youtube-1.2.0/pretalx_youtube/templates/pretalx_youtube/.gitkeep
--rw-r--r--   0 rixx      (1000) rixx      (1000)      821 2021-12-15 01:23:22.000000 pretalx-youtube-1.2.0/pretalx_youtube/templates/pretalx_youtube/settings.html
--rw-r--r--   0 rixx      (1000) rixx      (1000)      602 2022-07-11 16:28:30.000000 pretalx-youtube-1.2.0/pretalx_youtube/urls.py
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2677 2023-06-09 13:18:43.000000 pretalx-youtube-1.2.0/pretalx_youtube/views.py
-drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-09 13:19:19.911178 pretalx-youtube-1.2.0/pretalx_youtube.egg-info/
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1476 2023-06-09 13:19:19.000000 pretalx-youtube-1.2.0/pretalx_youtube.egg-info/PKG-INFO
--rw-r--r--   0 rixx      (1000) rixx      (1000)     2247 2023-06-09 13:19:19.000000 pretalx-youtube-1.2.0/pretalx_youtube.egg-info/SOURCES.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2023-06-09 13:19:19.000000 pretalx-youtube-1.2.0/pretalx_youtube.egg-info/dependency_links.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       69 2023-06-09 13:19:19.000000 pretalx-youtube-1.2.0/pretalx_youtube.egg-info/entry_points.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)       16 2023-06-09 13:19:19.000000 pretalx-youtube-1.2.0/pretalx_youtube.egg-info/top_level.txt
--rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2023-06-09 13:19:19.914512 pretalx-youtube-1.2.0/setup.cfg
--rw-r--r--   0 rixx      (1000) rixx      (1000)     1045 2023-06-09 13:19:03.000000 pretalx-youtube-1.2.0/setup.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      553 2021-12-15 01:11:11.000000 pretalx-youtube-1.2.1/LICENSE
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      230 2022-01-28 01:52:30.000000 pretalx-youtube-1.2.1/MANIFEST.in
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      142 2021-12-15 01:09:31.000000 pretalx-youtube-1.2.1/Makefile
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1476 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1210 2021-12-15 01:28:25.000000 pretalx-youtube-1.2.1/README.rst
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2022-10-31 23:19:32.000000 pretalx-youtube-1.2.1/pretalx_youtube/__init__.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      540 2023-06-22 16:18:44.000000 pretalx-youtube-1.2.1/pretalx_youtube/apps.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1877 2023-06-13 13:57:53.000000 pretalx-youtube-1.2.1/pretalx_youtube/forms.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/locale/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/ar/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      463 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1675 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/ca/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/cs/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1308 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2030 2023-06-09 13:06:24.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/de_DE/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/de_Formal/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/locale/de_Formal/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-07 09:15:13.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/django.pot
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/el/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/locale/el/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/el/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/en_Mozilla/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-02-19 15:38:17.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/es/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/locale/es/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/es_MX/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/locale/es_MX/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/fr_FR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/locale/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/it/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/locale/it/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      380 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1589 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/ja_JP/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_BR/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      379 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1588 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_PT/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-05-13 03:03:13.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-02-19 15:38:17.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/locale/zh_TW/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      337 2023-06-09 13:06:52.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1542 2023-06-09 13:05:07.000000 pretalx-youtube-1.2.1/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/migrations/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      972 2023-06-09 13:06:24.000000 pretalx-youtube-1.2.1/pretalx_youtube/migrations/0001_initial.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:19:02.000000 pretalx-youtube-1.2.1/pretalx_youtube/migrations/__init__.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      820 2021-12-15 01:24:02.000000 pretalx-youtube-1.2.1/pretalx_youtube/models.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      372 2021-12-15 01:24:02.000000 pretalx-youtube-1.2.1/pretalx_youtube/recording.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      841 2021-12-15 01:21:10.000000 pretalx-youtube-1.2.1/pretalx_youtube/signals.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/static/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/static/pretalx_youtube/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:09:31.000000 pretalx-youtube-1.2.1/pretalx_youtube/static/pretalx_youtube/.gitkeep
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.140809 pretalx-youtube-1.2.1/pretalx_youtube/templates/
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/pretalx_youtube/templates/pretalx_youtube/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        0 2021-12-15 01:09:31.000000 pretalx-youtube-1.2.1/pretalx_youtube/templates/pretalx_youtube/.gitkeep
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      821 2021-12-15 01:23:22.000000 pretalx-youtube-1.2.1/pretalx_youtube/templates/pretalx_youtube/settings.html
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      602 2022-07-11 16:28:30.000000 pretalx-youtube-1.2.1/pretalx_youtube/urls.py
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2703 2023-06-22 16:18:12.000000 pretalx-youtube-1.2.1/pretalx_youtube/views.py
+drwxr-xr-x   0 rixx      (1000) rixx      (1000)        0 2023-06-22 16:19:16.144142 pretalx-youtube-1.2.1/pretalx_youtube.egg-info/
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1476 2023-06-22 16:19:16.000000 pretalx-youtube-1.2.1/pretalx_youtube.egg-info/PKG-INFO
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     2247 2023-06-22 16:19:16.000000 pretalx-youtube-1.2.1/pretalx_youtube.egg-info/SOURCES.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)        1 2023-06-22 16:19:16.000000 pretalx-youtube-1.2.1/pretalx_youtube.egg-info/dependency_links.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       69 2023-06-22 16:19:16.000000 pretalx-youtube-1.2.1/pretalx_youtube.egg-info/entry_points.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)       16 2023-06-22 16:19:16.000000 pretalx-youtube-1.2.1/pretalx_youtube.egg-info/top_level.txt
+-rw-r--r--   0 rixx      (1000) rixx      (1000)      530 2023-06-22 16:19:16.147476 pretalx-youtube-1.2.1/setup.cfg
+-rw-r--r--   0 rixx      (1000) rixx      (1000)     1045 2023-06-22 16:18:30.000000 pretalx-youtube-1.2.1/setup.py
```

### Comparing `pretalx-youtube-1.2.0/LICENSE` & `pretalx-youtube-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/PKG-INFO` & `pretalx-youtube-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretalx-youtube
-Version: 1.2.0
+Version: 1.2.1
 Summary: Embed YouTube videos as session recordings
 Home-page: https://github.com/pretalx/pretalx-youtube
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
 License-File: LICENSE
```

### Comparing `pretalx-youtube-1.2.0/README.rst` & `pretalx-youtube-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/apps.py` & `pretalx-youtube-1.2.1/pretalx_youtube/apps.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     class PretalxPluginMeta:
         name = gettext_lazy("YouTube integration")
         author = "Tobias Kunze"
         description = gettext_lazy(
             "Embed YouTube videos as session recordings, and retrieve them via an API."
         )
         visible = True
-        version = "1.2.0"
+        version = "1.2.1"
 
     def ready(self):
         from . import signals  # NOQA
```

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/forms.py` & `pretalx-youtube-1.2.1/pretalx_youtube/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
         youtube = getattr(self.submission, "youtube_link", None)
         if youtube:
             initial = kwargs.get("initial", dict())
             initial["video_id"] = f"https://youtube.com/watch?v={youtube.video_id}"
             kwargs["initial"] = initial
         super().__init__(*args, **kwargs)
-        self.fields["video_id"].label = self.submission.title
+        self.fields["video_id"].label = getattr(self.submission, "title", None)
 
     def clean_video_id(self):
         data = self.cleaned_data["video_id"]
         if not data:
             return data
         # Get ID from youtube.com and youtu.be URLs
         if "youtube.com" in data:
```

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/ar/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/ca/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/cs/LC_MESSAGES/django.mo` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/cs/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/de_Formal/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/django.pot` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/django.pot`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/el/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/en_Mozilla/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/es/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/es_MX/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/it/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po` & `pretalx-youtube-1.2.1/pretalx_youtube/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/migrations/0001_initial.py` & `pretalx-youtube-1.2.1/pretalx_youtube/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/models.py` & `pretalx-youtube-1.2.1/pretalx_youtube/models.py`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/signals.py` & `pretalx-youtube-1.2.1/pretalx_youtube/signals.py`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/templates/pretalx_youtube/settings.html` & `pretalx-youtube-1.2.1/pretalx_youtube/templates/pretalx_youtube/settings.html`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/urls.py` & `pretalx-youtube-1.2.1/pretalx_youtube/urls.py`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube/views.py` & `pretalx-youtube-1.2.1/pretalx_youtube/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         return super().post(request, *args, **kwargs)
 
     def get_context_data(self, *args, **kwargs):
         kwargs = super().get_context_data(**kwargs)
         kwargs["url_forms"] = [
             YouTubeUrlForm(submission=slot.submission)
             for slot in self.request.event.current_schedule.talks.all()
-            .filter(is_visible=True)
+            .filter(is_visible=True, submission__isnull=False)
             .order_by("start")
         ]
         return kwargs
 
 
 def check_api_access(request):
     if "pretalx_youtube" not in request.event.plugin_list:
```

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube.egg-info/PKG-INFO` & `pretalx-youtube-1.2.1/pretalx_youtube.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretalx-youtube
-Version: 1.2.0
+Version: 1.2.1
 Summary: Embed YouTube videos as session recordings
 Home-page: https://github.com/pretalx/pretalx-youtube
 Author: Tobias Kunze
 Author-email: r@rixx.de
 License: Apache Software License
 License-File: LICENSE
```

### Comparing `pretalx-youtube-1.2.0/pretalx_youtube.egg-info/SOURCES.txt` & `pretalx-youtube-1.2.1/pretalx_youtube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/setup.cfg` & `pretalx-youtube-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretalx-youtube-1.2.0/setup.py` & `pretalx-youtube-1.2.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 
 cmdclass = {"build": CustomBuild}
 
 
 setup(
     name="pretalx-youtube",
-    version="1.2.0",
+    version="1.2.1",
     description="Embed YouTube videos as session recordings",
     long_description=long_description,
     url="https://github.com/pretalx/pretalx-youtube",
     author="Tobias Kunze",
     author_email="r@rixx.de",
     license="Apache Software License",
     install_requires=[],
```

