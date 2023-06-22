# Comparing `tmp/liitos-2023.6.17.tar.gz` & `tmp/liitos-2023.6.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liitos-2023.6.17.tar", last modified: Sat Jun 17 21:20:40 2023, max compression
+gzip compressed data, was "liitos-2023.6.22.tar", last modified: Thu Jun 22 18:40:35 2023, max compression
```

## Comparing `liitos-2023.6.17.tar` & `liitos-2023.6.22.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 21:20:40.122604 liitos-2023.6.17/
--rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.6.17/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.6.17/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     3037 2023-06-17 21:20:40.122293 liitos-2023.6.17/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     2068 2023-03-14 22:27:04.000000 liitos-2023.6.17/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 21:20:39.984327 liitos-2023.6.17/liitos/
--rw-r--r--   0 ruth       (501) staff       (20)     5001 2023-06-17 21:17:10.000000 liitos-2023.6.17/liitos/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.6.17/liitos/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)     4998 2023-06-17 20:58:59.000000 liitos-2023.6.17/liitos/approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1825 2023-04-25 19:10:10.000000 liitos-2023.6.17/liitos/captions.py
--rw-r--r--   0 ruth       (501) staff       (20)     6777 2023-06-17 20:58:56.000000 liitos-2023.6.17/liitos/changes.py
--rw-r--r--   0 ruth       (501) staff       (20)    10260 2023-02-07 22:48:13.000000 liitos-2023.6.17/liitos/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)    31810 2023-02-04 14:18:21.000000 liitos-2023.6.17/liitos/concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.6.17/liitos/configure.py
--rw-r--r--   0 ruth       (501) staff       (20)     1818 2023-04-25 19:46:43.000000 liitos-2023.6.17/liitos/description_lists.py
--rw-r--r--   0 ruth       (501) staff       (20)     2018 2023-06-17 18:14:28.000000 liitos-2023.6.17/liitos/eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     1688 2023-04-25 19:10:05.000000 liitos-2023.6.17/liitos/figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    12884 2023-06-17 18:24:25.000000 liitos-2023.6.17/liitos/gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     4375 2023-04-25 19:50:27.000000 liitos-2023.6.17/liitos/labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.6.17/liitos/liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    41648 2023-02-04 14:18:21.000000 liitos-2023.6.17/liitos/meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.6.17/liitos/patch.py
--rw-r--r--   0 ruth       (501) staff       (20)    18808 2023-06-17 18:16:15.000000 liitos-2023.6.17/liitos/render.py
--rw-r--r--   0 ruth       (501) staff       (20)    25124 2023-05-10 23:10:37.000000 liitos-2023.6.17/liitos/tables.py
--rw-r--r--   0 ruth       (501) staff       (20)     1517 2023-06-17 18:13:28.000000 liitos-2023.6.17/liitos/template_loader.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 21:20:40.089529 liitos-2023.6.17/liitos/templates/
--rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.6.17/liitos/templates/approvals.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1283 2023-06-17 17:00:35.000000 liitos-2023.6.17/liitos/templates/bookmatter.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.6.17/liitos/templates/changes.yml
--rw-r--r--   0 ruth       (501) staff       (20)      889 2023-05-10 17:17:37.000000 liitos-2023.6.17/liitos/templates/driver.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)       90 2023-06-17 17:58:54.000000 liitos-2023.6.17/liitos/templates/layout.yml
--rw-r--r--   0 ruth       (501) staff       (20)       97 2023-06-17 17:49:55.000000 liitos-2023.6.17/liitos/templates/meta-patch.yml
--rw-r--r--   0 ruth       (501) staff       (20)     1516 2023-06-17 17:52:06.000000 liitos-2023.6.17/liitos/templates/meta.yml
--rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.6.17/liitos/templates/metadata.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.6.17/liitos/templates/mkdocs.yml.in
--rw-r--r--   0 ruth       (501) staff       (20)     1347 2023-06-17 17:32:59.000000 liitos-2023.6.17/liitos/templates/publisher.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     9727 2023-06-17 17:26:10.000000 liitos-2023.6.17/liitos/templates/setup.tex.in
--rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.6.17/liitos/templates/vocabulary.yml
--rw-r--r--   0 ruth       (501) staff       (20)     7497 2023-04-25 19:15:13.000000 liitos-2023.6.17/liitos/tools.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 21:20:39.987194 liitos-2023.6.17/liitos.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     3037 2023-06-17 21:20:39.000000 liitos-2023.6.17/liitos.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1292 2023-06-17 21:20:39.000000 liitos-2023.6.17/liitos.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-17 21:20:39.000000 liitos-2023.6.17/liitos.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       42 2023-06-17 21:20:39.000000 liitos-2023.6.17/liitos.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      179 2023-06-17 21:20:39.000000 liitos-2023.6.17/liitos.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       15 2023-06-17 21:20:39.000000 liitos-2023.6.17/liitos.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)     2692 2023-06-17 21:15:36.000000 liitos-2023.6.17/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-17 21:20:40.122690 liitos-2023.6.17/setup.cfg
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-17 21:20:40.121635 liitos-2023.6.17/test/
--rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.6.17/test/test_approvals.py
--rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.6.17/test/test_captions.py
--rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.6.17/test/test_changes.py
--rw-r--r--   0 ruth       (501) staff       (20)     3728 2023-06-17 18:29:21.000000 liitos-2023.6.17/test/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.6.17/test/test_concat.py
--rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.6.17/test/test_eject.py
--rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.6.17/test/test_figures.py
--rw-r--r--   0 ruth       (501) staff       (20)    10514 2023-06-17 18:30:26.000000 liitos-2023.6.17/test/test_gather.py
--rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.6.17/test/test_labels.py
--rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.6.17/test/test_liitos.py
--rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.6.17/test/test_meta.py
--rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.6.17/test/test_patch.py
--rw-r--r--   0 ruth       (501) staff       (20)      486 2023-01-31 21:27:46.000000 liitos-2023.6.17/test/test_render.py
--rw-r--r--   0 ruth       (501) staff       (20)     3608 2023-05-09 18:14:35.000000 liitos-2023.6.17/test/test_tables.py
--rw-r--r--   0 ruth       (501) staff       (20)      431 2023-06-17 18:28:31.000000 liitos-2023.6.17/test/test_template_loader.py
--rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.6.17/test/test_tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.450073 liitos-2023.6.22/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 liitos-2023.6.22/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       95 2023-01-11 18:32:01.000000 liitos-2023.6.22/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3086 2023-06-22 18:40:35.449924 liitos-2023.6.22/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2068 2023-03-14 22:27:04.000000 liitos-2023.6.22/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.433150 liitos-2023.6.22/liitos/
+-rw-r--r--   0 ruth       (501) staff       (20)     5016 2023-06-22 18:39:03.000000 liitos-2023.6.22/liitos/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      125 2022-11-23 21:28:47.000000 liitos-2023.6.22/liitos/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5052 2023-06-22 18:04:59.000000 liitos-2023.6.22/liitos/approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1856 2023-06-22 17:55:57.000000 liitos-2023.6.22/liitos/captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6830 2023-06-22 18:04:41.000000 liitos-2023.6.22/liitos/changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10347 2023-06-22 17:56:51.000000 liitos-2023.6.22/liitos/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)    31870 2023-06-22 18:05:37.000000 liitos-2023.6.22/liitos/concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1642 2023-01-02 19:46:21.000000 liitos-2023.6.22/liitos/configure.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1849 2023-06-22 17:57:21.000000 liitos-2023.6.22/liitos/description_lists.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2018 2023-06-17 18:14:28.000000 liitos-2023.6.22/liitos/eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1725 2023-06-22 17:58:10.000000 liitos-2023.6.22/liitos/figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    12919 2023-06-22 18:04:28.000000 liitos-2023.6.22/liitos/gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4406 2023-06-22 17:58:35.000000 liitos-2023.6.22/liitos/labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       55 2022-09-17 11:23:46.000000 liitos-2023.6.22/liitos/liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    41823 2023-06-22 17:54:03.000000 liitos-2023.6.22/liitos/meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      624 2023-01-31 19:15:44.000000 liitos-2023.6.22/liitos/patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)    19019 2023-06-22 18:05:07.000000 liitos-2023.6.22/liitos/render.py
+-rw-r--r--   0 ruth       (501) staff       (20)    25142 2023-06-22 17:59:43.000000 liitos-2023.6.22/liitos/tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1548 2023-06-22 18:00:40.000000 liitos-2023.6.22/liitos/template_loader.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.440016 liitos-2023.6.22/liitos/templates/
+-rw-r--r--   0 ruth       (501) staff       (20)      116 2022-12-01 18:05:38.000000 liitos-2023.6.22/liitos/templates/approvals.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1283 2023-06-17 17:00:35.000000 liitos-2023.6.22/liitos/templates/bookmatter.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)      109 2023-01-17 18:43:02.000000 liitos-2023.6.22/liitos/templates/changes.yml
+-rw-r--r--   0 ruth       (501) staff       (20)      889 2023-05-10 17:17:37.000000 liitos-2023.6.22/liitos/templates/driver.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)       90 2023-06-17 17:58:54.000000 liitos-2023.6.22/liitos/templates/layout.yml
+-rw-r--r--   0 ruth       (501) staff       (20)       97 2023-06-17 17:49:55.000000 liitos-2023.6.22/liitos/templates/meta-patch.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     1516 2023-06-17 17:52:06.000000 liitos-2023.6.22/liitos/templates/meta.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     2505 2023-01-17 20:37:22.000000 liitos-2023.6.22/liitos/templates/metadata.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1538 2022-12-14 16:45:30.000000 liitos-2023.6.22/liitos/templates/mkdocs.yml.in
+-rw-r--r--   0 ruth       (501) staff       (20)     1347 2023-06-17 17:32:59.000000 liitos-2023.6.22/liitos/templates/publisher.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     9727 2023-06-17 17:26:10.000000 liitos-2023.6.22/liitos/templates/setup.tex.in
+-rw-r--r--   0 ruth       (501) staff       (20)     7450 2023-01-17 20:39:19.000000 liitos-2023.6.22/liitos/templates/vocabulary.yml
+-rw-r--r--   0 ruth       (501) staff       (20)     7522 2023-06-22 18:01:41.000000 liitos-2023.6.22/liitos/tools.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.435203 liitos-2023.6.22/liitos.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3086 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1292 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       42 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      179 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       15 2023-06-22 18:40:35.000000 liitos-2023.6.22/liitos.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     2753 2023-06-22 17:39:51.000000 liitos-2023.6.22/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-06-22 18:40:35.450112 liitos-2023.6.22/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-06-22 18:40:35.449597 liitos-2023.6.22/test/
+-rw-r--r--   0 ruth       (501) staff       (20)      499 2022-12-06 21:07:15.000000 liitos-2023.6.22/test/test_approvals.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1708 2023-02-07 22:58:06.000000 liitos-2023.6.22/test/test_captions.py
+-rw-r--r--   0 ruth       (501) staff       (20)      433 2022-12-06 21:11:22.000000 liitos-2023.6.22/test/test_changes.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3728 2023-06-17 18:29:21.000000 liitos-2023.6.22/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)     6984 2022-12-09 17:00:57.000000 liitos-2023.6.22/test/test_concat.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1073 2022-12-05 16:28:35.000000 liitos-2023.6.22/test/test_eject.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2689 2022-12-07 18:21:39.000000 liitos-2023.6.22/test/test_figures.py
+-rw-r--r--   0 ruth       (501) staff       (20)    10514 2023-06-17 18:30:26.000000 liitos-2023.6.22/test/test_gather.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1410 2022-12-05 16:41:47.000000 liitos-2023.6.22/test/test_labels.py
+-rw-r--r--   0 ruth       (501) staff       (20)       89 2022-08-01 14:41:37.000000 liitos-2023.6.22/test/test_liitos.py
+-rw-r--r--   0 ruth       (501) staff       (20)    15742 2023-02-04 14:19:02.000000 liitos-2023.6.22/test/test_meta.py
+-rw-r--r--   0 ruth       (501) staff       (20)      669 2022-12-05 18:19:44.000000 liitos-2023.6.22/test/test_patch.py
+-rw-r--r--   0 ruth       (501) staff       (20)      575 2023-06-22 17:30:47.000000 liitos-2023.6.22/test/test_render.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3608 2023-05-09 18:14:35.000000 liitos-2023.6.22/test/test_tables.py
+-rw-r--r--   0 ruth       (501) staff       (20)      431 2023-06-17 18:28:31.000000 liitos-2023.6.22/test/test_template_loader.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1436 2023-01-31 21:28:22.000000 liitos-2023.6.22/test/test_tools.py
```

### Comparing `liitos-2023.6.17/LICENSE` & `liitos-2023.6.22/LICENSE`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/PKG-INFO` & `liitos-2023.6.22/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.6.17
+Version: 2023.6.22
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
@@ -12,15 +12,16 @@
 Keywords: developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Liitos
 
 Splice (Finnish: liitos) contributions.
```

### Comparing `liitos-2023.6.17/README.md` & `liitos-2023.6.22/README.md`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/__init__.py` & `liitos-2023.6.22/liitos/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import logging
 import os
 import pathlib
 import shellingham  # type: ignore
 from typing import List, no_type_check
 
 # [[[fill git_describe()]]]
-__version__ = '2023.6.17+parent.67670e79'
-# [[[end]]] (checksum: 0d631da18950a0902a57b46b309622bb)
+__version__ = '2023.6.22+parent.v2023.6.17-25-ga525df55'
+# [[[end]]] (checksum: e713b82096b77b208181225e7aa7082a)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 
 APP_NAME = 'Splice (Finnish liitos) contributions.'
 APP_ALIAS = 'liitos'
 APP_ENV = 'LIITOS'
```

### Comparing `liitos-2023.6.17/liitos/approvals.py` & `liitos-2023.6.22/liitos/approvals.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Weave the content of the approvals data file into the output structure (for now LaTeX)."""
 import os
 import pathlib
+from typing import Union
 
 import liitos.gather as gat
 import liitos.template_loader as template
 from liitos import ENCODING, LOG_SEPARATOR, log
 
 BOOKMATTER_TEMPLATE = os.getenv('LIITOS_BOOKMATTER_TEMPLATE', '')
 BOOKMATTER_TEMPLATE_IS_EXTERNAL = bool(BOOKMATTER_TEMPLATE)
@@ -22,15 +23,19 @@
 YAML_CHANNEL = 'yaml'
 COLUMNS_EXPECTED = ['name', 'role']
 CUT_MARKER_TOP = '% |-- approvals - cut - marker - top -->'
 CUT_MARKER_BOTTOM = '% <-- approvals - cut - marker - bottom --|'
 
 
 def weave(
-    doc_root: str | pathlib.Path, structure_name: str, target_key: str, facet_key: str, options: dict[str, bool | str]
+    doc_root: Union[str, pathlib.Path],
+    structure_name: str,
+    target_key: str,
+    facet_key: str,
+    options: dict[str, Union[bool, str]],
 ) -> int:
     """Later alligator."""
     log.info(LOG_SEPARATOR)
     log.info('entered signatures weave function ...')
     structure, asset_map = gat.prelude(
         doc_root=doc_root,
         structure_name=structure_name,
```

### Comparing `liitos-2023.6.17/liitos/captions.py` & `liitos-2023.6.22/liitos/captions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections.abc import Iterable
+from typing import Union
 
 from liitos import log
 
 
-def weave(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
+def weave(incoming: Iterable[str], lookup: Union[dict[str, str], None] = None) -> list[str]:
     """Later alligator."""
     outgoing = []
     modus = 'copy'
     table: list[str] = []
     caption: list[str] = []
     for slot, line in enumerate(incoming):
         if modus == 'copy':
```

### Comparing `liitos-2023.6.17/liitos/changes.py` & `liitos-2023.6.22/liitos/changes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Weave the content of the changes data file into the output structure (for now LaTeX)."""
 import os
 import pathlib
+from typing import Union
 
 import liitos.gather as gat
 import liitos.template_loader as template
 from liitos import ENCODING, LOG_SEPARATOR, log
 
 PUBLISHER_TEMPLATE = os.getenv('LIITOS_PUBLISHER_TEMPLATE', '')
 PUBLISHER_TEMPLATE_IS_EXTERNAL = bool(PUBLISHER_TEMPLATE)
@@ -25,15 +26,19 @@
 CUT_MARKER_NOTICES_TOP = '% |-- notices - cut - marker - top -->'
 CUT_MARKER_NOTICES_BOTTOM = '% <-- notices - cut - marker - bottom --|'
 TOKEN_ADJUSTED_PUSHDOWN = r'\AdustedPushdown'  # nosec B105
 DEFAULT_ADJUSTED_PUSHDOWN_VALUE = 14
 
 
 def weave(
-    doc_root: str | pathlib.Path, structure_name: str, target_key: str, facet_key: str, options: dict[str, bool | str]
+    doc_root: Union[str, pathlib.Path],
+    structure_name: str,
+    target_key: str,
+    facet_key: str,
+    options: dict[str, Union[bool, str]],
 ) -> int:
     """Later alligator."""
     log.info(LOG_SEPARATOR)
     log.info('entered changes weave function ...')
     structure, asset_map = gat.prelude(
         doc_root=doc_root, structure_name=structure_name, target_key=target_key, facet_key=facet_key, command='changes'
     )
@@ -112,15 +117,15 @@
 
     if not any(TOKEN_ADJUSTED_PUSHDOWN in line for line in lines):
         log.error(TOKEN_ADJUSTED_PUSHDOWN, 'not in lines of template?????')
     else:
         for n, line in enumerate(lines):
             if TOKEN_ADJUSTED_PUSHDOWN in line:
                 lines[n] = line.replace(TOKEN_ADJUSTED_PUSHDOWN, f'{pushdown}em')
-                log.error(f'set adjusted pushdown value {pushdown}em')
+                log.info(f'set adjusted pushdown value {pushdown}em')
                 break
 
     if not layout['layout']['global']['has_changes']:
         log.info('removing changes from document layout')
         in_section = False
         keep = []
         for line in lines:
```

### Comparing `liitos-2023.6.17/liitos/cli.py` & `liitos-2023.6.22/liitos/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Command line interface for splice (Finnish liitos) contributions."""
 import datetime as dti
 import logging
 import os
 import pathlib
 import sys
+from typing import Union
 
 import typer
 
 import liitos.approvals as sig
 import liitos.changes as chg
 import liitos.concat as cat
 import liitos.eject as eje
@@ -60,18 +61,18 @@
 FromFormatSpec = typer.Option(
     FROM_FORMAT_SPEC,
     '-s',
     '--from-format-spec',
     help='from format specification handed over to pandoc',
 )
 FilterCSList = typer.Option(
-    FILTER_CS_LIST,
+    'DEFAULT_FILTER',
     '-F',
     '--filters',
-    help='comma separated list of filters handed over to pandoc (in order)',
+    help='comma separated list of filters handed over to pandoc (in order) or empty to apply no filter',
 )
 Verbosity = typer.Option(
     False,
     '-v',
     '--verbose',
     help='Verbose output (default is False)',
 )
@@ -124,15 +125,15 @@
     doc_root_pos: str,
     verbose: bool,
     strict: bool,
     label: str = '',
     patch_tables: bool = False,
     from_format_spec: str = '',
     filter_cs_list: str = '',
-) -> tuple[int, str, str, dict[str, bool | str]]:
+) -> tuple[int, str, str, dict[str, Union[bool, str]]]:
     """DRY"""
     doc = doc_root.strip()
     if not doc and doc_root_pos:
         doc = doc_root_pos
     if not doc:
         print('Document tree root required', file=sys.stderr)
         return 2, 'Document tree root required', '', {}
@@ -142,22 +143,22 @@
         if not doc_root_path.is_dir():
             print(f'requested tree root at ({doc}) is not a folder', file=sys.stderr)
             return 2, f'requested tree root at ({doc}) is not a folder', '', {}
     else:
         print(f'requested tree root at ({doc}) does not exist', file=sys.stderr)
         return 2, f'requested tree root at ({doc}) does not exist', '', {}
 
-    options: dict[str, bool | str] = {
+    options: dict[str, Union[bool, str]] = {
         'quiet': QUIET and not verbose and not strict,
         'strict': strict,
         'verbose': verbose,
         'label': label,
         'patch_tables': patch_tables,
         'from_format_spec': from_format_spec if from_format_spec else FROM_FORMAT_SPEC,
-        'filter_cs_list': filter_cs_list if filter_cs_list else FILTER_CS_LIST,
+        'filter_cs_list': filter_cs_list if filter_cs_list != 'DEFAULT_FILTER' else FILTER_CS_LIST,
     }
     if verbose:
         logging.getLogger().setLevel(logging.DEBUG)
     return 0, '', doc, options
 
 
 @app.command('verify')
```

### Comparing `liitos-2023.6.17/liitos/concat.py` & `liitos-2023.6.22/liitos/concat.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import os
 import pathlib
 import re
 import shutil
 import sys
 from io import StringIO
-from typing import no_type_check
+from typing import Union, no_type_check
 
 import treelib  # type: ignore
 import yaml
 
 import liitos.gather as gat
 from liitos import ENCODING, LOG_SEPARATOR, log
 
@@ -67,15 +67,15 @@
 
     @no_type_check
     def __str__(self):
         return self._string_io.getvalue()
 
 
 @no_type_check
-def process_approvals(aspects: str) -> gat.Approvals | int:
+def process_approvals(aspects: str) -> Union[gat.Approvals, int]:
     """TODO."""
     approvals_path = DOC_BASE / aspects[gat.KEY_APPROVALS]
     if not approvals_path.is_file() or not approvals_path.stat().st_size:
         log.error(f'destructure failed to find non-empty approvals file at {approvals_path}')
         return 1
     if approvals_path.suffix.lower() not in ('.json', '.yaml', '.yml'):
         log.error(f'approvals file format per suffix ({approvals_path.suffix}) not supported')
@@ -92,15 +92,15 @@
     else:
         with open('approvals.json', 'wt', encoding=ENCODING) as handle:
             json.dump(approvals, handle, indent=2)
     return approvals
 
 
 @no_type_check
-def process_binder(aspects: str) -> gat.Binder | int:
+def process_binder(aspects: str) -> Union[gat.Binder, int]:
     """TODO."""
     bind_path = DOC_BASE / aspects[gat.KEY_BIND]
     if not bind_path.is_file() or not bind_path.stat().st_size:
         log.error(f'destructure failed to find non-empty bind file at {bind_path}')
         return 1
     if bind_path.suffix.lower() not in ('.txt',):
         log.error(f'bind file format per suffix ({bind_path.suffix}) not supported')
@@ -112,15 +112,15 @@
         return 1
     with open('bind.txt', 'wt', encoding=ENCODING) as handle:
         handle.write('\n'.join(binder) + '\n')
     return binder
 
 
 @no_type_check
-def process_changes(aspects: str) -> gat.Changes | int:
+def process_changes(aspects: str) -> Union[gat.Changes, int]:
     """TODO."""
     changes_path = DOC_BASE / aspects[gat.KEY_CHANGES]
     if not changes_path.is_file() or not changes_path.stat().st_size:
         log.error(f'destructure failed to find non-empty changes file at {changes_path}')
         return 1
     if changes_path.suffix.lower() not in ('.json', '.yaml', '.yml'):
         log.error(f'changes file format per suffix ({changes_path.suffix}) not supported')
@@ -137,15 +137,15 @@
     else:
         with open('changes.json', 'wt', encoding=ENCODING) as handle:
             json.dump(changes, handle, indent=2)
     return changes
 
 
 @no_type_check
-def process_meta(aspects: str) -> gat.Meta | int:
+def process_meta(aspects: str) -> Union[gat.Meta, int]:
     """TODO."""
     meta_path = DOC_BASE / aspects[gat.KEY_META]
     if not meta_path.is_file() or not meta_path.stat().st_size:
         log.error(f'destructure failed to find non-empty meta file at {meta_path}')
         return 1
     if meta_path.suffix.lower() not in ('.yaml', '.yml'):
         log.error(f'meta file format per suffix ({meta_path.suffix}) not supported')
@@ -365,15 +365,19 @@
             source_asset = DOC_BASE / img_path
             target_asset = diagrams / pathlib.Path(img_path).name
             shutil.copy(source_asset, target_asset)
 
 
 @no_type_check
 def concatenate(
-    doc_root: str | pathlib.Path, structure_name: str, target_key: str, facet_key: str, options: dict[str, bool | str]
+    doc_root: Union[str, pathlib.Path],
+    structure_name: str,
+    target_key: str,
+    facet_key: str,
+    options: dict[str, Union[bool, str]],
 ) -> int:
     """Later alligator."""
     log.info(LOG_SEPARATOR)
     log.info('entered concat function ...')
     target_code = target_key
     facet_code = facet_key
     if not facet_code.strip() or not target_code.strip():
```

### Comparing `liitos-2023.6.17/liitos/configure.py` & `liitos-2023.6.22/liitos/configure.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/description_lists.py` & `liitos-2023.6.22/liitos/description_lists.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from collections.abc import Iterable
+from typing import Union
 
 from liitos import log
 
 NO_OPTION: str = ''
 
 
 def parse_options_command(slot: int, text_line: str) -> tuple[bool, str, str]:
@@ -17,15 +18,15 @@
         except Exception as err:
             log.error(f'failed to parse option value from {text_line.strip()} with err: {err}')
             return False, text_line, ''
     else:
         return False, text_line, ''
 
 
-def options(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
+def options(incoming: Iterable[str], lookup: Union[dict[str, str], None] = None) -> list[str]:
     """Later alligator. \\option[style=multiline,leftmargin=6em]"""
     outgoing = []
     modus = 'copy'
     opt = NO_OPTION
     for slot, line in enumerate(incoming):
         if modus == 'copy':
             has_opt, text_line, opt = parse_options_command(slot, line)
```

### Comparing `liitos-2023.6.17/liitos/eject.py` & `liitos-2023.6.22/liitos/eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/figures.py` & `liitos-2023.6.22/liitos/figures.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from collections.abc import Iterable
+from typing import Union
 
 from liitos import log
 
-NO_RESCALE: float | int = 0
+NO_RESCALE: Union[float, int] = 0
 
 
-def scale(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
+def scale(incoming: Iterable[str], lookup: Union[dict[str, str], None] = None) -> list[str]:
     """Later alligator."""
     outgoing = []
     modus = 'copy'
     rescale = NO_RESCALE
     for slot, line in enumerate(incoming):
         if modus == 'copy':
             if line.startswith(r'\scale='):
```

### Comparing `liitos-2023.6.17/liitos/gather.py` & `liitos-2023.6.22/liitos/gather.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,15 +223,15 @@
         asset, message = action(facet, target, asset_struct)
         if not asset:
             return False, f'{key} asset for facet ({facet}) of target ({target}) is invalid'
     return True, ''
 
 
 def prelude(
-    doc_root: str | pathlib.Path, structure_name: str, target_key: str, facet_key: str, command: str
+    doc_root: Union[str, pathlib.Path], structure_name: str, target_key: str, facet_key: str, command: str
 ) -> tuple[Structure, Assets]:
     """DRY."""
     doc_root = pathlib.Path(doc_root)
     idem = os.getcwd()
     os.chdir(doc_root)
     job_description = (
         f'facet ({facet_key}) of target ({target_key}) with structure map ({structure_name})'
@@ -240,15 +240,19 @@
     log.info(f'executing prelude of command ({command}) for {job_description}')
     structure = load_structure(structure_name)
     asset_map = assets(structure)
     return structure, asset_map
 
 
 def verify(
-    doc_root: str | pathlib.Path, structure_name: str, target_key: str, facet_key: str, options: dict[str, bool | str]
+    doc_root: Union[str, pathlib.Path],
+    structure_name: str,
+    target_key: str,
+    facet_key: str,
+    options: dict[str, Union[bool, str]],
 ) -> int:
     """Drive the verification."""
     doc_root = pathlib.Path(doc_root)
     os.chdir(doc_root)
     facet = facet_key
     target = target_key
     structure_name = structure_name
```

### Comparing `liitos-2023.6.17/liitos/labels.py` & `liitos-2023.6.22/liitos/labels.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from collections.abc import Iterable
+from typing import Union
 
 from liitos import log
 
 NO_LABEL = 'no-label-found-ERROR'
 
 
-def inject(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
+def inject(incoming: Iterable[str], lookup: Union[dict[str, str], None] = None) -> list[str]:
     """Later alligator."""
     outgoing = []
     modus = 'copy'
     label = NO_LABEL
     figure: list[str] = []
     caption: list[str] = []
     precondition = r'\begin{figure}'
```

### Comparing `liitos-2023.6.17/liitos/meta.py` & `liitos-2023.6.22/liitos/meta.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Weave the content of the meta file(s) of metadata.tex.in into the output metadata.tex."""
 import datetime as dti
 import os
 import pathlib
-from typing import no_type_check
+from typing import Union, no_type_check
 
 import yaml
 
 import liitos.gather as gat
 import liitos.template_loader as template
 from liitos import ENCODING, LOG_SEPARATOR, log
 
@@ -51,15 +51,15 @@
 ACROSS = {
     'eff_font_folder': '',
     'eff_font_suffix': '',
 }
 
 
 @no_type_check
-def process_meta(aspects: str) -> gat.Meta | int:
+def process_meta(aspects: str) -> Union[gat.Meta, int]:
     """TODO."""
     meta_path = DOC_BASE / aspects[gat.KEY_META]
     if not meta_path.is_file() or not meta_path.stat().st_size:
         log.error(f'destructure failed to find non-empty meta file at {meta_path}')
         return 1
     if meta_path.suffix.lower() not in ('.yaml', '.yml'):
         log.error(f'meta file format per suffix ({meta_path.suffix}) not supported')
@@ -85,15 +85,15 @@
     with open('metadata.yml', 'wt', encoding=ENCODING) as handle:
         yaml.dump(metadata, handle, default_flow_style=False)
     return metadata
 
 
 @no_type_check
 def weave_setup_font_path(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the xxxx from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_FONT_%_PATH_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -107,15 +107,15 @@
         log.warning(f'font_path value missing ... setting default ({defaults["font_path"]})')
         ACROSS['eff_font_folder'] = defaults['font_path']
         return text.replace(VALUE_SLOT, defaults['font_path'])
 
 
 @no_type_check
 def weave_setup_font_suffix(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the font_suffix from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_FONT_%_SUFFIX_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -129,15 +129,15 @@
         log.warning(f'font_suffix value missing ... setting default ({defaults["font_suffix"]})')
         ACROSS['eff_font_suffix'] = defaults['font_suffix']
         return text.replace(VALUE_SLOT, defaults['font_suffix'])
 
 
 @no_type_check
 def weave_setup_bold_font(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the bold_font from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_BOLD_%_FONT_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -155,15 +155,15 @@
     else:
         log.warning(f'bold_font value missing ... setting default ({defaults["bold_font"]})')
         return text.replace(VALUE_SLOT, defaults['bold_font'])
 
 
 @no_type_check
 def weave_setup_italic_font(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the italic_font from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_ITALIC_%_FONT_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -181,15 +181,15 @@
     else:
         log.warning(f'italic_font value missing ... setting default ({defaults["italic_font"]})')
         return text.replace(VALUE_SLOT, defaults['italic_font'])
 
 
 @no_type_check
 def weave_setup_bold_italic_font(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the bold_italic_font from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_BOLDITALIC_%_FONT_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -207,15 +207,15 @@
     else:
         log.warning(f'bold_italic_font value missing ... setting default ({defaults["bold_italic_font"]})')
         return text.replace(VALUE_SLOT, defaults['bold_italic_font'])
 
 
 @no_type_check
 def weave_setup_main_font(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the main_font from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_MAIN_%_FONT_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -233,15 +233,15 @@
     else:
         log.warning(f'main_font value missing ... setting default ({defaults["main_font"]})')
         return text.replace(VALUE_SLOT, defaults['main_font'])
 
 
 @no_type_check
 def weave_setup_fixed_font_package(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the fixed_font_package from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_FIXED_%_FONT_%_PACKAGE_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -256,15 +256,15 @@
     else:
         log.warning(f'fixed_font_package value missing ... setting default ({defaults["fixed_font_package"]})')
         return text.replace(VALUE_SLOT, defaults['fixed_font_package'])
 
 
 @no_type_check
 def weave_setup_code_fontsize(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the code_fontsize from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_CODE_%_FONTSIZE_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -305,15 +305,15 @@
             f' - in config that would be {defaults["code_fontsize"]}'
         )
         return text.replace(VALUE_SLOT, defaults['code_fontsize'])
 
 
 @no_type_check
 def weave_setup_chosen_logo(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the chosen_logo from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_CHOSEN_%_LOGO_%%')
     """
     defaults = {**WEAVE_DEFAULTS}
@@ -329,15 +329,15 @@
     else:
         log.warning(f'chosen_logo value missing ... setting default ({defaults["chosen_logo"]})')
         return text.replace(VALUE_SLOT, defaults['chosen_logo'])
 
 
 @no_type_check
 def dispatch_setup_weaver(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Dispatch the driver weaver by mapping to handled groups per source marker."""
     dispatch = {
         '%%_PATCH_%_FONT_%_PATH_%%': weave_setup_font_path,
         '%%_PATCH_%_FONT_%_SUFFIX_%%': weave_setup_font_suffix,
         '%%_PATCH_%_BOLD_%_FONT_%%': weave_setup_bold_font,
@@ -362,15 +362,15 @@
     if completed and completed[-1]:
         completed.append('\n')
     return completed
 
 
 @no_type_check
 def weave_driver_toc_level(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the toc_level from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_TOC_%_LEVEL_%%')
     """
     toc_level = 2
@@ -389,15 +389,15 @@
     else:
         log.warning(f'toc_level value missing ... setting default ({toc_level})')
     return text.replace(VALUE_SLOT, str(toc_level))
 
 
 @no_type_check
 def weave_driver_list_of_figures(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the list_of_figures from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_LOF_%%')
     """
     if mapper.get('list_of_figures', None) is not None:
@@ -414,15 +414,15 @@
         log.warning('list_of_figures value missing ... setting default (comment out the lof per %)')
 
     return text.replace(VALUE_SLOT, '%')
 
 
 @no_type_check
 def weave_driver_list_of_tables(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the list_of_tables from mapper or default for driver.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_LOT_%%')
     """
     if mapper.get('list_of_tables', None) is not None:
@@ -439,15 +439,15 @@
         log.warning('list_of_tables value missing ... setting default (comment out the lot per %)')
 
     return text.replace(VALUE_SLOT, '%')
 
 
 @no_type_check
 def dispatch_driver_weaver(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Dispatch the driver weaver by mapping to handled groups per source marker."""
     dispatch = {
         '%%_PATCH_%_TOC_%_LEVEL_%%': weave_driver_toc_level,
         '%%_PATCH_%_LOF_%%': weave_driver_list_of_figures,
         '%%_PATCH_%_LOT_%%': weave_driver_list_of_tables,
@@ -466,15 +466,15 @@
     if completed and completed[-1]:
         completed.append('\n')
     return completed
 
 
 @no_type_check
 def weave_meta_part_header_title(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the header_title from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_HEADER_%_TITLE_%%')
     """
     if mapper.get('header_title'):
@@ -482,27 +482,27 @@
     else:
         log.warning('header_title value missing ... setting default (the title value)')
         return text.replace(VALUE_SLOT, mapper['title'])
 
 
 @no_type_check
 def weave_meta_part_title(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the title from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_MAIN_%_TITLE_%%')
     """
     return text.replace(VALUE_SLOT, mapper['title'])
 
 
 @no_type_check
 def weave_meta_part_sub_title(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the sub_title from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_SUB_%_TITLE_%%')
     """
     if mapper.get('sub_title'):
@@ -510,15 +510,15 @@
     else:
         log.warning('sub_title value missing ... setting default (single space)')
         return text.replace(VALUE_SLOT, ' ')
 
 
 @no_type_check
 def weave_meta_part_header_type(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the header_type from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_TYPE_%%')
     """
     if mapper.get('header_type'):
@@ -526,15 +526,15 @@
     else:
         log.warning('header_type value missing ... setting default (Engineering Document)')
         return text.replace(VALUE_SLOT, 'Engineering Document')
 
 
 @no_type_check
 def weave_meta_part_header_id_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the header_id_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_ID_%_LABEL_%%')
     """
     if mapper.get('header_id_show', None) is not None and not mapper['header_id_show']:
@@ -549,15 +549,15 @@
     else:
         log.warning('header_id_label value missing ... setting default(Doc. ID:)')
         return text.replace(VALUE_SLOT, 'Doc. ID:')
 
 
 @no_type_check
 def weave_meta_part_header_id(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the header_id from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_ID_%%')
     """
     if mapper.get('header_id_show', None) is not None and not mapper['header_id_show']:
@@ -569,15 +569,15 @@
     else:
         log.warning('header_id value missing ... setting default (P99999)')
         return text.replace(VALUE_SLOT, 'P99999')
 
 
 @no_type_check
 def weave_meta_part_issue(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the issue from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_ISSUE_%%')
     """
     if mapper.get('issue'):
@@ -585,15 +585,15 @@
     else:
         log.warning('issue value missing ... setting default (01)')
         return text.replace(VALUE_SLOT, '01')
 
 
 @no_type_check
 def weave_meta_part_revision(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the revision from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_REVISION_%%')
     """
     if mapper.get('revision'):
@@ -601,15 +601,15 @@
     else:
         log.warning('revision value missing ... setting default (00)')
         return text.replace(VALUE_SLOT, '00')
 
 
 @no_type_check
 def weave_meta_part_header_date_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the header_date_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_DATE_%_LABEL_%%')
     """
     if mapper.get('header_date_show', None) is not None and not mapper['header_date_show']:
@@ -624,15 +624,15 @@
     else:
         log.warning('header_date_label value missing ... setting default(Date:)')
         return text.replace(VALUE_SLOT, 'Date:')
 
 
 @no_type_check
 def weave_meta_part_header_date(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the header_date from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_DATE_%%')
     """
     if mapper.get('header_date_show', None) is not None and not mapper['header_date_show']:
@@ -660,15 +660,15 @@
         else:
             log.warning(f'header_date value missing ... setting default as today({pub_date_today})')
             return text.replace(VALUE_SLOT, pub_date_today)
 
 
 @no_type_check
 def weave_meta_part_footer_frame_note(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the footer_frame_note from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_FRAME_%_NOTE_%%')
     """
     if mapper.get('footer_frame_note'):
@@ -676,15 +676,15 @@
     else:
         log.warning('footer_frame_note value missing ... setting default (VERY CONSEQUENTIAL)')
         return text.replace(VALUE_SLOT, 'VERY CONSEQUENTIAL')
 
 
 @no_type_check
 def weave_meta_part_footer_page_number_prefix(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the footer_page_number_prefix from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_FOOT_%_PAGE_%_COUNTER_%_LABEL_%%')
     """
     if mapper.get('footer_page_number_prefix'):
@@ -692,15 +692,15 @@
     else:
         log.warning('footer_page_number_prefix value missing ... setting default (Page)')
         return text.replace(VALUE_SLOT, 'Page')
 
 
 @no_type_check
 def weave_meta_part_change_log_issue_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the change_log_issue_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_CHANGELOG_%_ISSUE_%_LABEL_%%')
     """
     if mapper.get('change_log_issue_label'):
@@ -708,15 +708,15 @@
     else:
         log.warning('change_log_issue_label value missing ... setting default (Iss.)')
         return text.replace(VALUE_SLOT, 'Iss.')
 
 
 @no_type_check
 def weave_meta_part_change_log_revision_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the change_log_revision_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_CHANGELOG_%_REVISION_%_LABEL_%%')
     """
     if mapper.get('change_log_revision_label'):
@@ -724,15 +724,15 @@
     else:
         log.warning('change_log_revision_label value missing ... setting default (Rev.)')
         return text.replace(VALUE_SLOT, 'Rev.')
 
 
 @no_type_check
 def weave_meta_part_change_log_date_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the change_log_date_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_CHANGELOG_%_DATE_%_LABEL_%%')
     """
     if mapper.get('change_log_date_label'):
@@ -740,15 +740,15 @@
     else:
         log.warning('change_log_date_label value missing ... setting default (Date)')
         return text.replace(VALUE_SLOT, 'Date')
 
 
 @no_type_check
 def weave_meta_part_change_log_author_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the change_log_author_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_CHANGELOG_%_AUTHOR_%_LABEL_%%')
     """
     if mapper.get('change_log_author_label'):
@@ -756,15 +756,15 @@
     else:
         log.warning('change_log_author_label value missing ... setting default (Author)')
         return text.replace(VALUE_SLOT, 'Author')
 
 
 @no_type_check
 def weave_meta_part_change_log_description_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the change_log_description_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_CHANGELOG_%_DESCRIPTION_%_LABEL_%%')
     """
     if mapper.get('change_log_description_label'):
@@ -772,15 +772,15 @@
     else:
         log.warning('change_log_description_label value missing ... setting default (Description)')
         return text.replace(VALUE_SLOT, 'Description')
 
 
 @no_type_check
 def weave_meta_part_approvals_adjustable_vertical_space(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the approvals_adjustable_vertical_space from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_APPROVALS_%_ADJUSTABLE_%_VERTICAL_%_SPACE_%%')
     """
     if mapper.get('approvals_adjustable_vertical_space'):
@@ -791,15 +791,15 @@
             f' setting default ({WEAVE_DEFAULTS["adjustable_vertical_space"]})'
         )
         return text.replace(VALUE_SLOT, WEAVE_DEFAULTS['adjustable_vertical_space'])
 
 
 @no_type_check
 def weave_meta_part_approvals_role_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the approvals_role_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_APPROVALS_%_ROLE_%_LABEL_%%')
     """
     if mapper.get('approvals_role_label'):
@@ -807,15 +807,15 @@
     else:
         log.warning('approvals_role_label value missing ... setting default (Approvals)')
         return text.replace(VALUE_SLOT, 'Approvals')
 
 
 @no_type_check
 def weave_meta_part_approvals_name_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the approvals_name_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_APPROVALS_%_NAME_%_LABEL_%%')
     """
     if mapper.get('approvals_name_label'):
@@ -823,15 +823,15 @@
     else:
         log.warning('approvals_name_label value missing ... setting default (Name)')
         return text.replace(VALUE_SLOT, 'Name')
 
 
 @no_type_check
 def weave_meta_part_approvals_date_and_signature_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the approvals_date_and_signature_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_APPROVALS_%_DATE_%_AND_%_SIGNATURE_%_LABEL_%%')
     """
     if mapper.get('approvals_date_and_signature_label'):
@@ -839,15 +839,15 @@
     else:
         log.warning('approvals_date_and_signature_label value missing ... setting default (Date and Signature)')
         return text.replace(VALUE_SLOT, 'Date and Signature')
 
 
 @no_type_check
 def weave_meta_part_header_issue_revision_combined_label(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the header_issue_revision_combined_label from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_ISSUE_%_REVISION_%_COMBINED_%_LABEL_%%')
     """
     do_show_key = 'header_issue_revision_combined_show'
@@ -863,15 +863,15 @@
     else:
         log.warning('header_issue_revision_combined_label value missing ... setting default(Issue, Revision:)')
         return text.replace(VALUE_SLOT, 'Issue, Revision:')
 
 
 @no_type_check
 def weave_meta_part_header_issue_revision_combined(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the header_issue_revision_combined from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_ISSUE_%_REVISION_%_COMBINED_%%')
     """
     do_show_key = 'header_issue_revision_combined_show'
@@ -887,15 +887,15 @@
             ' default (Iss \\theMetaIssCode, Rev \\theMetaRevCode)'
         )
         return text.replace(VALUE_SLOT, r'Iss \theMetaIssCode, Rev \theMetaRevCode')
 
 
 @no_type_check
 def weave_meta_part_proprietary_information(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Weave in the proprietary_information from mapper or default.
 
     Trigger is text.rstrip().endswith('%%_PATCH_%_PROPRIETARY_%_INFORMATION_%_LABEL_%%')
     """
     if mapper.get('proprietary_information'):
@@ -913,15 +913,15 @@
     else:
         log.warning('proprietary_information value missing ... setting default (Proprietary Information MISSING)')
         return text.replace(VALUE_SLOT, 'Proprietary Information MISSING')
 
 
 @no_type_check
 def dispatch_meta_weaver(
-    mapper: dict[str, str | int | bool | None],
+    mapper: dict[str, Union[str, int, bool, None]],
     text: str,
 ) -> str:
     """Dispatch the meta weaver by mapping to handled groups per source marker."""
     dispatch = {
         '%%_PATCH_%_HEADER_%_TITLE_%%': weave_meta_part_header_title,
         '%%_PATCH_%_MAIN_%_TITLE_%%': weave_meta_part_title,
         '%%_PATCH_%_SUB_%_TITLE_%%': weave_meta_part_sub_title,
@@ -961,15 +961,15 @@
     if completed and completed[-1]:
         completed.append('\n')
     return completed
 
 
 @no_type_check
 def weave(
-    doc_root: str | pathlib.Path, structure_name: str, target_key: str, facet_key: str, options: dict[str, bool]
+    doc_root: Union[str, pathlib.Path], structure_name: str, target_key: str, facet_key: str, options: dict[str, bool]
 ) -> int:
     """Later alligator."""
     log.info(LOG_SEPARATOR)
     log.info('entered meta weave function ...')
     target_code = target_key
     facet_code = facet_key
     if not facet_code.strip() or not target_code.strip():
```

### Comparing `liitos-2023.6.17/liitos/patch.py` & `liitos-2023.6.22/liitos/patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/render.py` & `liitos-2023.6.22/liitos/render.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 """Render the concat document to pdf."""
 import json
 import os
 import pathlib
 import re
 import shutil
 import time
-from typing import no_type_check
+from typing import Union, no_type_check
 
 import yaml
 
 import liitos.captions as cap
 import liitos.concat as con
 import liitos.description_lists as dsc
 import liitos.figures as fig
 import liitos.gather as gat
 import liitos.labels as lab
 import liitos.patch as pat
 import liitos.tables as tab
 import liitos.tools as too
 from liitos import (
     ENCODING,
-    FILTER_CS_LIST,
     FROM_FORMAT_SPEC,
     LATEX_PAYLOAD_NAME,
     LOG_SEPARATOR,
-    TOOL_VERSION_COMMAND_MAP,
     log,
     parse_csl,
 )
 
 DOC_BASE = pathlib.Path('..', '..')
 STRUCTURE_PATH = DOC_BASE / 'structure.yml'
 IMAGES_FOLDER = 'images/'
@@ -37,30 +35,37 @@
 INTER_PROCESS_SYNC_SECS = 0.1
 INTER_PROCESS_SYNC_ATTEMPTS = 10
 VENDORED_SVG_PAT = re.compile(r'^.+\]\([^.]+\.[^.]+\.svg\ .+$')
 
 
 @no_type_check
 def der(
-    doc_root: str | pathlib.Path, structure_name: str, target_key: str, facet_key: str, options: dict[str, bool | str]
+    doc_root: Union[str, pathlib.Path],
+    structure_name: str,
+    target_key: str,
+    facet_key: str,
+    options: dict[str, Union[bool, str]],
 ) -> int:
     """Later alligator."""
     log.info(LOG_SEPARATOR)
     log.info('entered render function ...')
     target_code = target_key
     facet_code = facet_key
     if not facet_code.strip() or not target_code.strip():
         log.error(f'render requires non-empty target ({target_code}) and facet ({facet_code}) codes')
         return 2
 
     log.info(f'parsed target ({target_code}) and facet ({facet_code}) from request')
 
     from_format_spec = options.get('from_format_spec', FROM_FORMAT_SPEC)
-    filter_cs_list = parse_csl(options.get('filter_cs_list', FILTER_CS_LIST))
-    log.info(f'parsed from-format-spec ({from_format_spec}) and filters ({", ".join(filter_cs_list)}) from request')
+    filter_cs_list = parse_csl(options.get('filter_cs_list', ''))
+    if filter_cs_list:
+        log.info(f'parsed from-format-spec ({from_format_spec}) and filters ({", ".join(filter_cs_list)}) from request')
+    else:
+        log.info(f'parsed from-format-spec ({from_format_spec}) and no filters from request')
 
     structure, asset_map = gat.prelude(
         doc_root=doc_root, structure_name=structure_name, target_key=target_key, facet_key=facet_key, command='render'
     )
     log.info(f'prelude teleported processor into the document root at ({os.getcwd()}/)')
 
     rel_concat_folder_path = pathlib.Path('render/pdf/')
@@ -194,15 +199,16 @@
                         lines[slot] = fine
                         dia_path_old = src.replace('.svg', '.png')
                         dia_path_new = f'{stem}.png'
                         dia_fine_rstrip = dia_path_new.rstrip()
                         if dia_path_old and dia_path_new:
                             special_patching.append((dia_path_old, dia_path_new))
                             log.info(
-                                f'post-action[#{slot + 1}]: adding to queue for sync move: ({dia_path_old}) -> ({dia_path_new})'
+                                f'post-action[#{slot + 1}]: adding to queue for sync move: ({dia_path_old})'
+                                f' -> ({dia_path_new})'
                             )
                         else:
                             log.warning(f'- old: {src.rstrip()}')
                             log.warning(f'- new: {dia_fine_rstrip}')
                         continue
                 if '.svg' in line:
                     fine = line.replace('.svg', '.png')
@@ -308,26 +314,28 @@
         log.info(LOG_SEPARATOR)
 
         # <<< prototyping
 
         fmt_spec = from_format_spec
         in_doc = 'document.md'
         out_doc = LATEX_PAYLOAD_NAME
-        filters = [added_prefix for expr in filter_cs_list for added_prefix in ('--filter', expr)]
         markdown_to_latex_command = [
             'pandoc',
             '--verbose',
             '-f',
             fmt_spec,
             '-t',
             'latex',
             in_doc,
             '-o',
             out_doc,
-        ] + filters
+        ]
+        if filter_cs_list:
+            filters = [added_prefix for expr in filter_cs_list for added_prefix in ('--filter', expr)]
+            markdown_to_latex_command += filters
         log.info(LOG_SEPARATOR)
         log.info(f'executing ({" ".join(markdown_to_latex_command)}) ...')
         if code := too.delegate(markdown_to_latex_command, 'markdown-to-latex'):
             return code
 
         log.info(LOG_SEPARATOR)
         log.info(f'load text lines from intermediate {LATEX_PAYLOAD_NAME} file before internal transforms ...')
```

### Comparing `liitos-2023.6.17/liitos/tables.py` & `liitos-2023.6.22/liitos/tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Apply all pairs in patch module on document."""
 import re
 from collections.abc import Iterable, Iterator
-from typing import no_type_check
+from typing import Union, no_type_check
 
 from liitos import log
 
 # The "target pattern for a line base minimal regex parser"
 _ = r"""
 \columns=
 
@@ -100,15 +100,15 @@
 COMMA = ','
 
 
 class Table:
     """Some adhoc structure to encapsulate tje source and target table."""
 
     SourceMapType = list[tuple[int, str]]
-    ColumnsType = dict[str, dict[str, float | int | str]]
+    ColumnsType = dict[str, dict[str, Union[float, int, str]]]
 
     # ---- begin of LBP skeleton / shape ---
     LBP_STARTSWITH_TAB_ENV_BEGIN = r'\begin{longtable}[]{'
     LBP_REAL_INNER_COLW_PAT = re.compile(r'^(?P<clspec>.+)\\real{(?P<cwval>[0-9.]+)}}\s*$')
     LBP_REAL_OUTER_COLW_PAT = re.compile(r'^(?P<clspec>.+)\\real{(?P<cwval>[0-9.]+)}}@{}}\s*$')
     # Width lines for header:
     FUT_LSPLIT_ONCE_FOR_PREFIX_VAL_COMMA_RIGHT = '}}'
@@ -449,15 +449,15 @@
             log.error(f'failed to parse columns values from {text_line.strip()} with err: {err}')
             return False, text_line, []
     else:
         return False, text_line, []
 
 
 @no_type_check
-def patch(incoming: Iterable[str], lookup: dict[str, str] | None = None) -> list[str]:
+def patch(incoming: Iterable[str], lookup: Union[dict[str, str], None] = None) -> list[str]:
     """Later alligator. \\columns=,0.2,0.7 as mandatory trigger"""
     table_section, head, annotation = False, False, False
     table_ranges = []
     guess_slot = 0
     table_range = {}
     has_column = False
     has_font_size = False
```

### Comparing `liitos-2023.6.17/liitos/template_loader.py` & `liitos-2023.6.22/liitos/template_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Loader function for templates."""
 import pathlib
 import pkgutil
+from typing import Union
 
 from liitos import ENCODING
 
 RESOURCES = (
     'templates/approvals.yml',
     'templates/bookmatter.tex.in',
     'templates/changes.yml',
@@ -25,15 +26,15 @@
     if is_complete_path:
         with open(resource, 'rt', encoding=ENCODING) as handle:
             return handle.read()
     else:
         return pkgutil.get_data(__package__, resource).decode(encoding=ENCODING)  # type: ignore
 
 
-def eject(argv: list[str] | None = None) -> int:
+def eject(argv: Union[list[str], None] = None) -> int:
     """Eject the templates into the folder given (default EJECTED) and create the folder if it does not exist."""
     argv = argv if argv else ['']
     into = argv[0]
     if not into.strip():
         into = 'EJECTED'
     into_path = pathlib.Path(into)
     (into_path / 'templates').mkdir(parents=True, exist_ok=True)
```

### Comparing `liitos-2023.6.17/liitos/templates/bookmatter.tex.in` & `liitos-2023.6.22/liitos/templates/bookmatter.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/templates/driver.tex.in` & `liitos-2023.6.22/liitos/templates/driver.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/templates/meta.yml` & `liitos-2023.6.22/liitos/templates/meta.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/templates/metadata.tex.in` & `liitos-2023.6.22/liitos/templates/metadata.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/templates/mkdocs.yml.in` & `liitos-2023.6.22/liitos/templates/mkdocs.yml.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/templates/publisher.tex.in` & `liitos-2023.6.22/liitos/templates/publisher.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/templates/setup.tex.in` & `liitos-2023.6.22/liitos/templates/setup.tex.in`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/templates/vocabulary.yml` & `liitos-2023.6.22/liitos/templates/vocabulary.yml`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/liitos/tools.py` & `liitos-2023.6.22/liitos/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime as dti
 import difflib
 import hashlib
 import pathlib
 import subprocess  # nosec B404
-from typing import Any, Callable, no_type_check
+from typing import Any, Callable, Union, no_type_check
 
 import foran.foran as api  # type: ignore
 from foran.report import generate_report  # type: ignore
 from taksonomia.taksonomia import Taxonomy  # type: ignore
 
 from liitos import ENCODING, LATEX_PAYLOAD_NAME, TOOL_VERSION_COMMAND_MAP, ToolKey, log
 
@@ -19,15 +19,15 @@
 CHUNK_SIZE = 2 << 15
 TS_FORMAT = '%Y-%m-%d %H:%M:%S.%f +00:00'
 LOG_SEPARATOR = '- ' * 80
 INTER_PROCESS_SYNC_SECS = 0.1
 INTER_PROCESS_SYNC_ATTEMPTS = 10
 
 
-def hash_file(path: pathlib.Path, hasher: Callable[..., Any] | None = None) -> str:
+def hash_file(path: pathlib.Path, hasher: Union[Callable[..., Any], None] = None) -> str:
     """Return the SHA512 hex digest of the data from file."""
     if hasher is None:
         hasher = hashlib.sha512
     the_hash = hasher()
     with open(path, 'rb') as handle:
         while chunk := handle.read(CHUNK_SIZE):
             the_hash.update(chunk)
@@ -117,15 +117,15 @@
     for line in unified_diff(left, right, left_label, right_label):
         for fine in line.split('\n'):
             log.info(fine)
     log.info(LOG_SEPARATOR)
 
 
 @no_type_check
-def ensure_separate_log_lines(sourcer: Callable, *args: list[object] | None):
+def ensure_separate_log_lines(sourcer: Callable, *args: Union[list[object], None]):
     """Wrapping idiom breaking up any strings containing newlines."""
     log.info(LOG_SEPARATOR)
     for line in sourcer(*args) if args else sourcer():
         for fine in line.split('\n'):
             log.info(fine)
     log.info(LOG_SEPARATOR)
 
@@ -177,15 +177,15 @@
 @no_type_check
 def execute_filter(
     the_filter: Callable,
     head: str,
     backup: str,
     label: str,
     text_lines: list[str],
-    lookup: dict[str, str] | None = None,
+    lookup: Union[dict[str, str], None] = None,
 ) -> list[str]:
     """Chain filter calls by storing in and out lies in files and return the resulting lines."""
     log.info(LOG_SEPARATOR)
     log.info(head)
     doc_before_caps_patch = backup
     with open(doc_before_caps_patch, 'wt', encoding=ENCODING) as handle:
         handle.write('\n'.join(text_lines))
```

### Comparing `liitos-2023.6.17/liitos.egg-info/PKG-INFO` & `liitos-2023.6.22/liitos.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liitos
-Version: 2023.6.17
+Version: 2023.6.22
 Summary: Splice (Finnish liitos) contributions.
 Author-email: Stefan Hagen <stefan@hagen.link>
 Maintainer-email: Stefan Hagen <stefan@hagen.link>
 Project-URL: Homepage, https://git.sr.ht/~sthagen/liitos
 Project-URL: Bug-Tracker, https://todo.sr.ht/~sthagen/liitos
 Project-URL: Documentation, https://codes.dilettant.life/docs/liitos
 Project-URL: Source-Code, https://git.sr.ht/~sthagen/liitos
@@ -12,15 +12,16 @@
 Keywords: developer-tools,validation,verification
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Liitos
 
 Splice (Finnish: liitos) contributions.
```

### Comparing `liitos-2023.6.17/liitos.egg-info/SOURCES.txt` & `liitos-2023.6.22/liitos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/pyproject.toml` & `liitos-2023.6.22/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "liitos"
-version = "2023.6.17"
+version = "2023.6.22"
 description = "Splice (Finnish liitos) contributions."
 readme = "README.md"
 authors = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 maintainers = [{ name = "Stefan Hagen", email = "stefan@hagen.link" }]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3.9",
 ]
 keywords = ["developer-tools", "validation", "verification"]
 dependencies = [
     "PyYAML >= 6.0",
-    "foran >= 2022.12.7",
+    "foran >= 2023.6.19",
     "shellingham >= 1.5.0.post1",
-    "taksonomia >= 2023.1.24",
+    "taksonomia >= 2023.6.18",
     "treelib >= 1.6.4",
-    "typer >= 0.7.0",
+    "typer >= 0.9.0",
 ]
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = ["black", "coverage", "hypothesis", "mypy", "pytest", "pytest-cov", "pytest-flake8", "ruff"]
 
 [project.urls]
 Homepage = "https://git.sr.ht/~sthagen/liitos"
 Bug-Tracker = "https://todo.sr.ht/~sthagen/liitos"
@@ -44,15 +45,15 @@
 [tool.setuptools.packages.find]
 include = ["liitos", "liitos.templates", "example"]
 exclude = ["test*"]
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ["py310", "py311"]
+target-version = ["py39", "py310", "py311", "py312"]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.report]
 precision = 2
 exclude_lines = [
```

### Comparing `liitos-2023.6.17/test/test_captions.py` & `liitos-2023.6.22/test/test_captions.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_cli.py` & `liitos-2023.6.22/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_concat.py` & `liitos-2023.6.22/test/test_concat.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_eject.py` & `liitos-2023.6.22/test/test_eject.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_figures.py` & `liitos-2023.6.22/test/test_figures.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_gather.py` & `liitos-2023.6.22/test/test_gather.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_labels.py` & `liitos-2023.6.22/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_meta.py` & `liitos-2023.6.22/test/test_meta.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_patch.py` & `liitos-2023.6.22/test/test_patch.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_tables.py` & `liitos-2023.6.22/test/test_tables.py`

 * *Files identical despite different names*

### Comparing `liitos-2023.6.17/test/test_tools.py` & `liitos-2023.6.22/test/test_tools.py`

 * *Files identical despite different names*

