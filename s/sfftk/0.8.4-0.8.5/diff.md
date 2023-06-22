# Comparing `tmp/sfftk-0.8.4.tar.gz` & `tmp/sfftk-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sfftk-0.8.4.tar", last modified: Thu Feb  9 11:18:25 2023, max compression
+gzip compressed data, was "dist/sfftk-0.8.5.tar", last modified: Thu Jun 22 09:33:02 2023, max compression
```

## Comparing `sfftk-0.8.4.tar` & `sfftk-0.8.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    11338 2018-11-08 12:03:33.000000 sfftk-0.8.4/LICENSE
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     7474 2023-02-09 11:18:25.000000 sfftk-0.8.4/PKG-INFO
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     6040 2022-10-17 10:31:32.000000 sfftk-0.8.4/README.rst
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       38 2023-02-09 11:18:25.000000 sfftk-0.8.4/setup.cfg
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     2591 2023-01-27 13:32:39.000000 sfftk-0.8.4/setup.py
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       98 2023-02-09 11:18:04.000000 sfftk-0.8.4/sfftk/__init__.py
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk/core/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       32 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/core/__init__.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     8798 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/core/configs.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    69274 2023-01-27 13:32:39.000000 sfftk-0.8.4/sfftk/core/parser.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    22286 2023-01-19 14:08:08.000000 sfftk-0.8.4/sfftk/core/prep.py
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk/formats/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/__init__.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    10552 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/am.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     2971 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/base.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     4184 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/ilastik.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    28706 2022-11-30 11:01:16.000000 sfftk-0.8.4/sfftk/formats/map.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    14244 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/mod.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     8239 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/seg.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     7851 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/stl.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     8445 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/surf.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     4779 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/formats/survos.py
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk/notes/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     2479 2022-10-19 12:12:22.000000 sfftk-0.8.4/sfftk/notes/__init__.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    34065 2022-10-19 12:12:22.000000 sfftk-0.8.4/sfftk/notes/find.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    46292 2023-02-09 11:18:04.000000 sfftk-0.8.4/sfftk/notes/modify.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    18943 2023-01-19 14:46:12.000000 sfftk-0.8.4/sfftk/notes/view.py
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk/readers/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)      690 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/readers/__init__.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)      830 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/readers/amreader.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     1872 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/readers/ilastikreader.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    18972 2023-01-20 16:53:37.000000 sfftk-0.8.4/sfftk/readers/mapreader.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    40708 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/readers/modreader.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     9443 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/readers/segreader.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     1785 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/readers/stlreader.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     5251 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/readers/surfreader.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     3068 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/readers/survosreader.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)      342 2018-12-06 11:15:04.000000 sfftk-0.8.4/sfftk/sff.conf
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    24577 2022-11-28 14:33:53.000000 sfftk-0.8.4/sfftk/sff.py
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk/test_data/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       48 2018-12-05 14:37:08.000000 sfftk-0.8.4/sfftk/test_data/__init__.py
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk/unittests/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     1539 2022-10-17 10:31:32.000000 sfftk-0.8.4/sfftk/unittests/__init__.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)   106812 2023-01-27 13:32:39.000000 sfftk-0.8.4/sfftk/unittests/test_core.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    31035 2022-11-28 14:33:53.000000 sfftk-0.8.4/sfftk/unittests/test_formats.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    25868 2022-11-28 14:33:53.000000 sfftk-0.8.4/sfftk/unittests/test_main.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)   109808 2023-02-09 11:18:04.000000 sfftk-0.8.4/sfftk/unittests/test_notes.py
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    25416 2023-01-20 16:56:26.000000 sfftk-0.8.4/sfftk/unittests/test_readers.py
-drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk.egg-info/
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     7474 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk.egg-info/PKG-INFO
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     1100 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk.egg-info/SOURCES.txt
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)        1 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk.egg-info/dependency_links.txt
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       39 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk.egg-info/entry_points.txt
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       75 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk.egg-info/requires.txt
--rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)        6 2023-02-09 11:18:25.000000 sfftk-0.8.4/sfftk.egg-info/top_level.txt
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    11338 2018-11-08 12:03:33.000000 sfftk-0.8.5/LICENSE
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     7474 2023-06-22 09:33:02.000000 sfftk-0.8.5/PKG-INFO
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     6040 2022-10-17 10:31:32.000000 sfftk-0.8.5/README.rst
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       38 2023-06-22 09:33:02.000000 sfftk-0.8.5/setup.cfg
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     2591 2023-01-27 13:32:39.000000 sfftk-0.8.5/setup.py
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       98 2023-06-21 11:40:18.000000 sfftk-0.8.5/sfftk/__init__.py
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk/core/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       32 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/core/__init__.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     8798 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/core/configs.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    69274 2023-06-08 14:05:18.000000 sfftk-0.8.5/sfftk/core/parser.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    22245 2023-06-21 11:10:47.000000 sfftk-0.8.5/sfftk/core/prep.py
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk/formats/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/__init__.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    10552 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/am.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     2971 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/base.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     4184 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/ilastik.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    28706 2022-11-30 11:01:16.000000 sfftk-0.8.5/sfftk/formats/map.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    14244 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/mod.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     8239 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/seg.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     7851 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/stl.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     8445 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/surf.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     4779 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/formats/survos.py
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk/notes/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     2479 2022-10-19 12:12:22.000000 sfftk-0.8.5/sfftk/notes/__init__.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    34065 2022-10-19 12:12:22.000000 sfftk-0.8.5/sfftk/notes/find.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    46253 2023-06-21 13:24:06.000000 sfftk-0.8.5/sfftk/notes/modify.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    18943 2023-01-19 14:46:12.000000 sfftk-0.8.5/sfftk/notes/view.py
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk/readers/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)      690 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/readers/__init__.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)      830 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/readers/amreader.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     1872 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/readers/ilastikreader.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    18972 2023-01-20 16:53:37.000000 sfftk-0.8.5/sfftk/readers/mapreader.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    40708 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/readers/modreader.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     9443 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/readers/segreader.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     2269 2023-06-21 11:15:48.000000 sfftk-0.8.5/sfftk/readers/stlreader.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     5251 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/readers/surfreader.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     3068 2022-10-17 10:31:32.000000 sfftk-0.8.5/sfftk/readers/survosreader.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)      342 2018-12-06 11:15:04.000000 sfftk-0.8.5/sfftk/sff.conf
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    24768 2023-06-21 11:14:56.000000 sfftk-0.8.5/sfftk/sff.py
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk/test_data/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       48 2018-12-05 14:37:08.000000 sfftk-0.8.5/sfftk/test_data/__init__.py
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk/unittests/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     1568 2023-06-21 11:11:24.000000 sfftk-0.8.5/sfftk/unittests/__init__.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)   107073 2023-06-21 11:40:18.000000 sfftk-0.8.5/sfftk/unittests/test_core.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    31035 2022-11-28 14:33:53.000000 sfftk-0.8.5/sfftk/unittests/test_formats.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    26468 2023-06-21 11:32:43.000000 sfftk-0.8.5/sfftk/unittests/test_main.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)   109797 2023-06-21 13:25:32.000000 sfftk-0.8.5/sfftk/unittests/test_notes.py
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)    26000 2023-06-21 11:15:48.000000 sfftk-0.8.5/sfftk/unittests/test_readers.py
+drwxr-xr-x   0 pkorir   (1454627118) EBI\Domain Users (384566875)        0 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk.egg-info/
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     7474 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk.egg-info/PKG-INFO
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)     1100 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk.egg-info/SOURCES.txt
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)        1 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk.egg-info/dependency_links.txt
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       39 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk.egg-info/entry_points.txt
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)       75 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk.egg-info/requires.txt
+-rw-r--r--   0 pkorir   (1454627118) EBI\Domain Users (384566875)        6 2023-06-22 09:33:02.000000 sfftk-0.8.5/sfftk.egg-info/top_level.txt
```

### Comparing `sfftk-0.8.4/LICENSE` & `sfftk-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/PKG-INFO` & `sfftk-0.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfftk
-Version: 0.8.4
+Version: 0.8.5
 Summary: Toolkit for working with EMDB-SFF and other segmentation file formats
 Home-page: https://emdb-empiar.github.io/EMDB-SFF/
 Author: Paul K. Korir, PhD
 Author-email: pkorir@ebi.ac.uk, paul.korir@gmail.com
 License: Apache License
 Project-URL: Report Issues, https://github.com/emdb-empiar/sfftk/issues
 Project-URL: Documentation, http://sfftk.readthedocs.io/en/latest/index.html
```

### Comparing `sfftk-0.8.4/README.rst` & `sfftk-0.8.5/README.rst`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/setup.py` & `sfftk-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/core/configs.py` & `sfftk-0.8.5/sfftk/core/configs.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/core/parser.py` & `sfftk-0.8.5/sfftk/core/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1304,15 +1304,15 @@
                 print_date(f"error: one or more masks missing; please verify that all paths are correct")
                 return 65, configs
             if not _mask_all_correct_files(args):
                 print_date(f"error: one or more invalid file formats; please retry")
                 return 65, configs
             if not _masks_have_same_dimensions(args):
                 print_date(
-                    f"error: inhomogenious masks: dimension differs between masks (use --verbose to view details)")
+                    f"error: inhomogeneous masks: dimension differs between masks (use --verbose to view details)")
                 return 65, configs
             if not _masks_have_mode_zero(args):
                 print_date(f"error: mode must be zero (0); please run `sff prep binmap` first on all masks")
                 return 65, configs
 
     # view
     elif args.subcommand == 'view':
```

### Comparing `sfftk-0.8.4/sfftk/core/prep.py` & `sfftk-0.8.5/sfftk/core/prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 import mrcfile
 import numpy
 import numpy.lib.mixins
 from sfftkrw.core import _str
 from sfftkrw.core.print_tools import print_date
 from stl import Mesh
 
-from sfftk.readers.mapreader import Map
-
 
 def _label_generator():
     yield from (*range(1, 128), *range(-128, 0))
 
 
 class MergedMask:
     """This class describes a special mask used to perform mask merging. It automatically handles
```

### Comparing `sfftk-0.8.4/sfftk/formats/am.py` & `sfftk-0.8.5/sfftk/formats/am.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/formats/base.py` & `sfftk-0.8.5/sfftk/formats/base.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/formats/ilastik.py` & `sfftk-0.8.5/sfftk/formats/ilastik.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/formats/map.py` & `sfftk-0.8.5/sfftk/formats/map.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/formats/mod.py` & `sfftk-0.8.5/sfftk/formats/mod.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/formats/seg.py` & `sfftk-0.8.5/sfftk/formats/seg.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/formats/stl.py` & `sfftk-0.8.5/sfftk/formats/stl.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/formats/surf.py` & `sfftk-0.8.5/sfftk/formats/surf.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/formats/survos.py` & `sfftk-0.8.5/sfftk/formats/survos.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/notes/__init__.py` & `sfftk-0.8.5/sfftk/notes/__init__.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/notes/find.py` & `sfftk-0.8.5/sfftk/notes/find.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/notes/modify.py` & `sfftk-0.8.5/sfftk/notes/modify.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,22 +86,22 @@
                 except KeyError:
                     description = ''
             else:
                 print_date(
                     "Could not find label and description for external reference {}:{}".format(self.resource,
                                                                                                self.accession))
         elif self.resource == 'EMDB':
-            url = "https://www.ebi.ac.uk/pdbe/api/emdb/entry/all/{}".format(self.accession)
+            url = "https://www.ebi.ac.uk/emdb/api/entry/{}".format(self.accession)
             response = requests.get(url)
             if response.status_code == 200:
                 self._result = json.loads(response.text)
                 # label
-                label = list(self._result.keys())[0]
+                label = self._result['emdb_id']
                 # description
-                description = self._result[label][0]['deposition']['title']
+                description = self._result['admin']['title']
             else:
                 print_date(
                     "Could not find label and description for external reference {}:{}".format(self.resource,
                                                                                                self.accession))
         elif self.resource == "PDB":
             url = "https://www.ebi.ac.uk/pdbe/search/pdb/select?q={}&wt=json".format(self.accession)
             response = requests.get(url)
@@ -170,15 +170,15 @@
                         )
                     )
             else:
                 print_date(
                     "Could not find label and description for external reference {}:{}".format(self.resource,
                                                                                                self.accession))
         elif self.resource == 'EMPIAR':
-            url = "https://www.ebi.ac.uk/pdbe/emdb/empiar/api/entry/{}".format(self.accession)
+            url = "https://www.ebi.ac.uk/empiar/api/entry/{}".format(self.accession)
             response = requests.get(url)
             if response.status_code == 200:
                 self._result = json.loads(response.text)
                 try:
                     # label
                     label = self._result[self.accession]["title"]
                     # description
```

### Comparing `sfftk-0.8.4/sfftk/notes/view.py` & `sfftk-0.8.5/sfftk/notes/view.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/readers/__init__.py` & `sfftk-0.8.5/sfftk/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/readers/amreader.py` & `sfftk-0.8.5/sfftk/readers/amreader.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/readers/ilastikreader.py` & `sfftk-0.8.5/sfftk/readers/ilastikreader.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/readers/mapreader.py` & `sfftk-0.8.5/sfftk/readers/mapreader.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/readers/modreader.py` & `sfftk-0.8.5/sfftk/readers/modreader.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/readers/segreader.py` & `sfftk-0.8.5/sfftk/readers/segreader.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/readers/stlreader.py` & `sfftk-0.8.5/sfftk/readers/stlreader.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,7 +54,22 @@
 
         # we now need to reverse the vertex_ids dict
         vertices = _dict(zip(vertex_ids.values(), vertex_ids.keys()))
 
         name = "{}#{}".format(os.path.basename(fn), mesh_id)
         meshes.append((name, vertices, polygons))
     return meshes
+
+
+def compute_bounding_box(fn):
+    """Compute the bounding box for an STL file
+
+    Required to check that the transform has correctly aligned the segmentation with the image
+
+    :param str fn: filename
+    :return: a `list` of `tuple`s of the form `((x_min, y_min, z_min), (x_max, y_max, z_max))`
+    :rtype: list
+    """
+    from stl import mesh
+    my_stl = mesh.Mesh.from_file(fn)
+    bounds_min, bound_max = my_stl.min_, my_stl.max_
+    return list(zip(bounds_min, bound_max))
```

### Comparing `sfftk-0.8.4/sfftk/readers/surfreader.py` & `sfftk-0.8.5/sfftk/readers/surfreader.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/readers/survosreader.py` & `sfftk-0.8.5/sfftk/readers/survosreader.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/sff.py` & `sfftk-0.8.5/sfftk/sff.py`

 * *Files 2% similar despite different names*

```diff
@@ -488,16 +488,19 @@
                 print("*" * 50)
                 print("CCP4 Mask Segmentation")
                 print("*" * 50)
                 # fixme: use _str
                 print(str(seg.segments[0].annotation._map_obj))
                 print("*" * 50)
         elif re.match(r'.*\.stl$', args.from_file, re.IGNORECASE):
+            from .readers import stlreader
             print("*" * 50)
             print("STL Segmentation")
+            bounding_box = stlreader.compute_bounding_box(args.from_file)
+            print("Bounding box: X={}; Y={}; Z={}".format(*bounding_box))
             print("*" * 50)
         else:
             print_date("Not implemented view for files of type .{}".format(args.from_file.split('.')[-1]), sys.stderr)
     return 0
 
 
 def handle_config(args, configs):
```

### Comparing `sfftk-0.8.4/sfftk/unittests/__init__.py` & `sfftk-0.8.5/sfftk/unittests/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import os
 import random
 import sys
+import pathlib
 from unittest import TestCase
 
 from sfftkrw.core import _xrange
 
 from .. import BASE_DIR
 
 __author__ = 'Paul K. Korir, PhD'
 __email__ = 'pkorir@ebi.ac.uk, paul.korir@gmail.com'
 __date__ = '2016-06-15'
 __updated__ = '2018-02-14'
 
 # path to test data
-TEST_DATA_PATH = os.path.join(BASE_DIR, 'test_data')
+TEST_DATA_PATH = pathlib.Path(os.path.join(BASE_DIR, 'test_data'))
 
 
 # helper functions
 def _random_integer(start=1, stop=1000): return random.randint(start, stop)
 
 
 def _random_float(multiplier=1): return random.random() * multiplier
```

### Comparing `sfftk-0.8.4/sfftk/unittests/test_core.py` & `sfftk-0.8.5/sfftk/unittests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 from . import TEST_DATA_PATH
 from .. import BASE_DIR
 from ..core.configs import Configs, get_config_file_path, load_configs, \
     get_configs, set_configs, del_configs
 from ..core.parser import Parser, parse_args, tool_list, _get_file_extension, _set_subtype_index, cli
 from ..core.prep import bin_map, transform_stl_mesh, construct_transformation_matrix, check_mask_is_binary
+from ..readers.stlreader import compute_bounding_box
 from ..notes import RESOURCE_LIST
 
 rw = RandomWords()
 li = LoremIpsum()
 
 TEST_DATA_PATH = pathlib.Path(TEST_DATA_PATH)
 BASE_DIR = pathlib.Path(BASE_DIR)
@@ -943,14 +944,19 @@
         self.assertTrue(args.print_csv)
         args, _ = cli("view --transform --print-ssv file.map")
         self.assertTrue(args.print_ssv)
         # if we specify --image then we only accept .map/.mrc/.rec
         args, _ = cli("view --transform file.sff")
         self.assertEqual(64, args)
 
+    def test_view_stl_bounds(self):
+        """Test that we can view the bounds of an STL file"""
+        args, _ = cli("view file.stl")
+        self.assertEqual('file.stl', args.from_file)
+
 
 class TestCoreParserNotesReadOnly(Py23FixTestCase):
     @classmethod
     def setUpClass(cls):
         cls.config_fn = os.path.join(BASE_DIR, 'sff.conf')
         cls.stderr("notes ro tests...")
 
@@ -2372,15 +2378,16 @@
 
         )
 
         _ = mergemask(args, configs)
         self.assertTrue(os.path.exists("my_masks.map"))
         self.assertTrue(os.path.exists("my_masks.json"))
         # check that header of my_masks.map is correct
-        with mrcfile.open('my_masks.map') as merged, mrcfile.open(TEST_DATA_PATH / 'segmentations' / 'mergeable_1.map') as mergeable:
+        with mrcfile.open('my_masks.map') as merged, mrcfile.open(
+                TEST_DATA_PATH / 'segmentations' / 'mergeable_1.map') as mergeable:
             self.assertEqual(mergeable.voxel_size, merged.voxel_size)
             self.assertEqual(mergeable.header.mapr, merged.header.mapr)
             self.assertEqual(mergeable.header.mapc, merged.header.mapc)
             self.assertEqual(mergeable.header.maps, merged.header.maps)
             self.assertEqual(mergeable.header.nx, merged.header.nx)
             self.assertEqual(mergeable.header.ny, merged.header.ny)
             self.assertEqual(mergeable.header.nz, merged.header.nz)
```

### Comparing `sfftk-0.8.4/sfftk/unittests/test_formats.py` & `sfftk-0.8.5/sfftk/unittests/test_formats.py`

 * *Files identical despite different names*

### Comparing `sfftk-0.8.4/sfftk/unittests/test_main.py` & `sfftk-0.8.5/sfftk/unittests/test_main.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,14 +469,28 @@
             os.path.join(TEST_DATA_PATH, 'segmentations', 'test_data.map'),
             self.config_fn,
         ), use_shlex=True)
         sys.stdout = StringIO()
         Main.handle_view(args, configs)
         self.assertRegex(sys.stdout.getvalue(), r"(?m)^[[].*?(\d+\.\d*)*.*?[]]$")
 
+    def test_view_bounding_box(self):
+        """Test that we can view the bounding box of an STL file"""
+        args, configs = parse_args('view {} --config-path {}'.format(
+            os.path.join(TEST_DATA_PATH, 'segmentations', 'test_data.stl'),
+            self.config_fn,
+        ), use_shlex=True)
+        sys.stdout = StringIO()
+        Main.handle_view(args, configs)
+        self.assertRegex(
+            sys.stdout.getvalue(),
+            r"(?m).*?STL Segmentation\nBounding box: X=\(\d+\.\d*, \d+\.\d*\); Y=\(\d+\.\d*, \d+\.\d*\); "
+            r"Z=\(\d+\.\d*, \d+\.\d*\).*"
+        )
+
     def test_read_mod(self):
         """Test that we can view .mod"""
         args, configs = parse_args('view {} --config-path {} --show-chunks'.format(
             os.path.join(TEST_DATA_PATH, 'segmentations', 'test_data.mod'),
             self.config_fn,
         ), use_shlex=True)
         self.assertEqual(0, Main.handle_view(args, configs))
```

### Comparing `sfftk-0.8.4/sfftk/unittests/test_notes.py` & `sfftk-0.8.5/sfftk/unittests/test_notes.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                          description)
         self.assertCountEqual(ext_ref._get_text(), [label, description])
         self.assertEqual(ext_ref.iri, urlenc3)
 
     def test_emdb(self):
         """Test that sfftk.notes.modify.ExternalReference object works correctly"""
         resource = 'EMDB'
-        url = 'https://www.ebi.ac.uk/pdbe/emdb/EMD-8654'
+        url = 'https://www.ebi.ac.uk/emdb/EMD-8654'
         accession = 'EMD-8654'
         # likely to change
         label = 'EMD-8654'
         description = 'Zika virus-infected Vero E6 cell at 48 hpi: dual-axis tilt series tomogram from 3 serial sections'
         ext_ref = modify.ExternalReference(
             resource=resource,
             url=url,
@@ -138,15 +138,15 @@
         self.assertEqual(ext_ref.description,
                          description)
         self.assertCountEqual(ext_ref._get_text(), [label, description])
 
     def test_empiar(self):
         """Test that sfftk.notes.modify.ExternalReference object works correctly"""
         resource = 'EMPIAR'
-        url = 'https://www.ebi.ac.uk/pdbe/emdb/empiar/entry/10087/'
+        url = 'https://www.ebi.ac.uk/empiar/api/entry/10087/'
         accession = 'EMPIAR-10087'
         label = 'Soft X-ray tomography of Plasmodium falciparum infected human erythrocytes stalled in egress by the ' \
                 'inhibitors Compound 2 and E64'
         description = 'SXT'
         ext_ref = modify.ExternalReference(
             resource=resource,
             url=url,
```

### Comparing `sfftk-0.8.4/sfftk/unittests/test_readers.py` & `sfftk-0.8.5/sfftk/unittests/test_readers.py`

 * *Files 2% similar despite different names*

```diff
@@ -490,14 +490,25 @@
             self.assertTrue(len(vertices) > 0)
             self.assertTrue(len(polygons) > 0)
             polygon_ids = list()
             for a, b, c in _dict_iter_values(polygons):
                 polygon_ids += [a, b, c]
             self.assertCountEqual(set(vertices.keys()), set(polygon_ids))
 
+    def test_compute_bounding_box(self):
+        """Test that we can compute the bounding box of an STL file"""
+        test_stl_file = TEST_DATA_PATH / 'segmentations' / 'test_data.stl'
+        x, y, z = stlreader.compute_bounding_box(test_stl_file)
+        self.assertAlmostEqual(x[0], 89.08, places=3)
+        self.assertAlmostEqual(x[1], 271.337, places=3)
+        self.assertAlmostEqual(y[0], 78.1158, places=3)
+        self.assertAlmostEqual(y[1], 266.757, places=3)
+        self.assertAlmostEqual(z[0], 100.887, places=3)
+        self.assertAlmostEqual(z[1], 240.9, places=3)
+
 
 class TestReaders_surfreader(Py23FixTestCase):
     @classmethod
     def setUpClass(cls):
         super(TestReaders_surfreader, cls).setUpClass()
         cls.surf_file = os.path.join(TEST_DATA_PATH, 'segmentations', 'test_data.surf')
         cls.header, cls.segments = surfreader.get_data(cls.surf_file)  # only one mesh here
```

### Comparing `sfftk-0.8.4/sfftk.egg-info/PKG-INFO` & `sfftk-0.8.5/sfftk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sfftk
-Version: 0.8.4
+Version: 0.8.5
 Summary: Toolkit for working with EMDB-SFF and other segmentation file formats
 Home-page: https://emdb-empiar.github.io/EMDB-SFF/
 Author: Paul K. Korir, PhD
 Author-email: pkorir@ebi.ac.uk, paul.korir@gmail.com
 License: Apache License
 Project-URL: Report Issues, https://github.com/emdb-empiar/sfftk/issues
 Project-URL: Documentation, http://sfftk.readthedocs.io/en/latest/index.html
```

### Comparing `sfftk-0.8.4/sfftk.egg-info/SOURCES.txt` & `sfftk-0.8.5/sfftk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

