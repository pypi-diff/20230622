# Comparing `tmp/SFlock2-0.3.49.tar.gz` & `tmp/SFlock2-0.3.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SFlock2-0.3.49.tar", last modified: Tue Mar 28 13:34:47 2023, max compression
+gzip compressed data, was "SFlock2-0.3.50.tar", last modified: Thu Jun 22 07:08:31 2023, max compression
```

## Comparing `SFlock2-0.3.49.tar` & `SFlock2-0.3.50.tar`

### file list

```diff
@@ -1,66 +1,97 @@
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.496472 SFlock2-0.3.49/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      370 2020-06-10 09:29:08.000000 SFlock2-0.3.49/MANIFEST.in
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      855 2023-03-28 13:34:47.496142 SFlock2-0.3.49/PKG-INFO
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2712 2021-07-20 07:58:43.000000 SFlock2-0.3.49/README.md
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.442012 SFlock2-0.3.49/SFlock2.egg-info/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      855 2023-03-28 13:34:47.000000 SFlock2-0.3.49/SFlock2.egg-info/PKG-INFO
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1235 2023-03-28 13:34:47.000000 SFlock2-0.3.49/SFlock2.egg-info/SOURCES.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        1 2023-03-28 13:34:47.000000 SFlock2-0.3.49/SFlock2.egg-info/dependency_links.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       44 2023-03-28 13:34:47.000000 SFlock2-0.3.49/SFlock2.egg-info/entry_points.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      132 2023-03-28 13:34:47.000000 SFlock2-0.3.49/SFlock2.egg-info/requires.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        7 2023-03-28 13:34:47.000000 SFlock2-0.3.49/SFlock2.egg-info/top_level.txt
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       38 2023-03-28 13:34:47.496563 SFlock2-0.3.49/setup.cfg
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1880 2023-02-01 06:49:14.000000 SFlock2-0.3.49/setup.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.447711 SFlock2-0.3.49/sflock/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2022-09-09 07:46:59.000000 SFlock2-0.3.49/sflock/.DS_Store
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      335 2021-07-15 18:56:48.000000 SFlock2-0.3.49/sflock/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      100 2023-03-28 13:34:28.000000 SFlock2-0.3.49/sflock/__version__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    15303 2022-03-08 17:08:56.000000 SFlock2-0.3.49/sflock/abstracts.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.449175 SFlock2-0.3.49/sflock/aux/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        1 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/aux/__init__.py
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)     8734 2021-07-16 12:01:23.000000 SFlock2-0.3.49/sflock/aux/decode_vbe_jse.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.450651 SFlock2-0.3.49/sflock/compat/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      152 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/compat/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1295 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/compat/magic.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      564 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/config.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.456714 SFlock2-0.3.49/sflock/data/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2022-09-09 07:46:22.000000 SFlock2-0.3.49/sflock/data/.DS_Store
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      157 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       26 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/data/password.txt
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)   668240 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/poweriso.elf
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.466665 SFlock2-0.3.49/sflock/data/win32/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   536241 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/win32/magic.mgc
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   150016 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/win32/magic1.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    79360 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/win32/regex2.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    72192 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/win32/zlib1.dll
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.477659 SFlock2-0.3.49/sflock/data/win64/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    67720 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/win64/libgnurx-0.dll
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)  2944752 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/win64/magic.mgc
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   717504 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/data/win64/magic1.dll
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.483206 SFlock2-0.3.49/sflock/data/yara/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      464 2022-09-02 19:41:32.000000 SFlock2-0.3.49/sflock/data/yara/archives.yar
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    11391 2022-02-19 08:23:06.000000 SFlock2-0.3.49/sflock/data/yara/shellcodes.yar
--rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)   873032 2023-01-31 10:07:30.000000 SFlock2-0.3.49/sflock/data/zipjail.elf
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.484903 SFlock2-0.3.49/sflock/decode/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      302 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/decode/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5967 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/decode/office.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      364 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/exception.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    14652 2023-03-28 13:34:18.000000 SFlock2-0.3.49/sflock/ident.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3271 2023-01-19 07:23:25.000000 SFlock2-0.3.49/sflock/main.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1328 2021-12-08 14:30:13.000000 SFlock2-0.3.49/sflock/misc.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     4280 2022-01-14 07:58:22.000000 SFlock2-0.3.49/sflock/pick.py
-drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-03-28 13:34:47.495319 SFlock2-0.3.49/sflock/unpack/
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      309 2020-06-10 09:29:08.000000 SFlock2-0.3.49/sflock/unpack/__init__.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1276 2023-01-31 10:07:51.000000 SFlock2-0.3.49/sflock/unpack/ace.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1570 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/unpack/bup.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      945 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/unpack/cab.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1065 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/unpack/daa.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2180 2021-12-29 11:09:37.000000 SFlock2-0.3.49/sflock/unpack/eml.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1838 2021-07-16 14:34:19.000000 SFlock2-0.3.49/sflock/unpack/lzip.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2055 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/unpack/msg.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2225 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/unpack/mso.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      977 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/unpack/office.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2468 2021-12-08 17:07:57.000000 SFlock2-0.3.49/sflock/unpack/pdf.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      932 2022-03-08 17:08:34.000000 SFlock2-0.3.49/sflock/unpack/rar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5029 2022-01-14 07:58:22.000000 SFlock2-0.3.49/sflock/unpack/tar.py
--rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6216 2022-10-27 10:01:06.000000 SFlock2-0.3.49/sflock/unpack/zip7.py
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.682353 SFlock2-0.3.50/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      370 2020-06-10 09:29:08.000000 SFlock2-0.3.50/MANIFEST.in
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      855 2023-06-22 07:08:31.682082 SFlock2-0.3.50/PKG-INFO
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2712 2021-07-20 07:58:43.000000 SFlock2-0.3.50/README.md
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.594246 SFlock2-0.3.50/SFlock2.egg-info/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      855 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/PKG-INFO
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1807 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/SOURCES.txt
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        1 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/dependency_links.txt
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       44 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/entry_points.txt
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      132 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/requires.txt
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        7 2023-06-22 07:08:31.000000 SFlock2-0.3.50/SFlock2.egg-info/top_level.txt
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       38 2023-06-22 07:08:31.682435 SFlock2-0.3.50/setup.cfg
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1880 2023-02-01 06:49:14.000000 SFlock2-0.3.50/setup.py
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.603758 SFlock2-0.3.50/sflock/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2022-09-09 07:46:59.000000 SFlock2-0.3.50/sflock/.DS_Store
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      335 2021-07-15 18:56:48.000000 SFlock2-0.3.50/sflock/__init__.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      100 2023-06-22 06:35:49.000000 SFlock2-0.3.50/sflock/__version__.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    15303 2022-03-08 17:08:56.000000 SFlock2-0.3.50/sflock/abstracts.py
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.606033 SFlock2-0.3.50/sflock/aux/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)        1 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/aux/__init__.py
+-rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)     8734 2021-07-16 12:01:23.000000 SFlock2-0.3.50/sflock/aux/decode_vbe_jse.py
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.607848 SFlock2-0.3.50/sflock/compat/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      152 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/compat/__init__.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1295 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/compat/magic.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      564 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/config.py
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.616779 SFlock2-0.3.50/sflock/data/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6148 2022-09-09 07:46:22.000000 SFlock2-0.3.50/sflock/data/.DS_Store
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      157 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/__init__.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)       26 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/data/password.txt
+-rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)   668240 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/poweriso.elf
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.628566 SFlock2-0.3.50/sflock/data/win32/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   536241 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win32/magic.mgc
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   150016 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win32/magic1.dll
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    79360 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win32/regex2.dll
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    72192 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win32/zlib1.dll
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.644682 SFlock2-0.3.50/sflock/data/win64/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    67720 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win64/libgnurx-0.dll
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)  2944752 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win64/magic.mgc
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)   717504 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/data/win64/magic1.dll
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.650562 SFlock2-0.3.50/sflock/data/yara/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      464 2022-09-02 19:41:32.000000 SFlock2-0.3.50/sflock/data/yara/archives.yar
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    11391 2022-02-19 08:23:06.000000 SFlock2-0.3.50/sflock/data/yara/shellcodes.yar
+-rwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)   873032 2023-01-31 10:07:30.000000 SFlock2-0.3.50/sflock/data/zipjail.elf
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.652418 SFlock2-0.3.50/sflock/decode/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      302 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/decode/__init__.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5967 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/decode/office.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      364 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/exception.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    15097 2023-06-22 06:59:19.000000 SFlock2-0.3.50/sflock/ident.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3271 2023-01-19 07:23:25.000000 SFlock2-0.3.50/sflock/main.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1328 2021-12-08 14:30:13.000000 SFlock2-0.3.50/sflock/misc.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     4280 2022-01-14 07:58:22.000000 SFlock2-0.3.50/sflock/pick.py
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.662249 SFlock2-0.3.50/sflock/unpack/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      309 2020-06-10 09:29:08.000000 SFlock2-0.3.50/sflock/unpack/__init__.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1276 2023-01-31 10:07:51.000000 SFlock2-0.3.50/sflock/unpack/ace.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1570 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/bup.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      945 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/cab.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1065 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/daa.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2180 2021-12-29 11:09:37.000000 SFlock2-0.3.50/sflock/unpack/eml.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1838 2021-07-16 14:34:19.000000 SFlock2-0.3.50/sflock/unpack/lzip.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2055 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/msg.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2225 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/mso.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      977 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/office.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2468 2021-12-08 17:07:57.000000 SFlock2-0.3.50/sflock/unpack/pdf.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      932 2022-03-08 17:08:34.000000 SFlock2-0.3.50/sflock/unpack/rar.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5029 2022-01-14 07:58:22.000000 SFlock2-0.3.50/sflock/unpack/tar.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6216 2022-10-27 10:01:06.000000 SFlock2-0.3.50/sflock/unpack/zip7.py
+drwxr-xr-x   0 andriy.brukhovetskyy   (501) staff       (20)        0 2023-06-22 07:08:31.681150 SFlock2-0.3.50/tests/
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     5150 2022-10-27 10:16:35.000000 SFlock2-0.3.50/tests/test_7z.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3436 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_ace.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1046 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_attr.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1414 2022-01-14 07:58:22.000000 SFlock2-0.3.50/tests/test_bup.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1991 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_cab.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      974 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_daa.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1066 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_decode.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      324 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_elf.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3518 2022-12-14 17:01:41.000000 SFlock2-0.3.50/tests/test_eml.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      954 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_exts.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1599 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_file.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2833 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_ident.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      996 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_lzh.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1222 2021-07-16 14:54:32.000000 SFlock2-0.3.50/tests/test_lzip.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      704 2021-07-16 12:01:23.000000 SFlock2-0.3.50/tests/test_magic.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1169 2022-10-27 10:19:03.000000 SFlock2-0.3.50/tests/test_main.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      459 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_misc.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     3005 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_msg.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      506 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_mso.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1563 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_office.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     6870 2021-12-08 14:59:59.000000 SFlock2-0.3.50/tests/test_package.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     2093 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_pdf.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1370 2021-12-08 14:59:59.000000 SFlock2-0.3.50/tests/test_pick.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     4556 2022-01-14 07:58:22.000000 SFlock2-0.3.50/tests/test_rar.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)      524 2022-10-27 10:07:17.000000 SFlock2-0.3.50/tests/test_shellcode.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     7291 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_tar.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)    17695 2022-02-19 09:29:07.000000 SFlock2-0.3.50/tests/test_unpack.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1486 2021-07-16 16:51:56.000000 SFlock2-0.3.50/tests/test_win.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     8544 2022-01-14 07:58:22.000000 SFlock2-0.3.50/tests/test_zip.py
+-rw-r--r--   0 andriy.brukhovetskyy   (501) staff       (20)     1689 2021-12-08 17:07:57.000000 SFlock2-0.3.50/tests/test_zipify.py
```

### Comparing `SFlock2-0.3.49/PKG-INFO` & `SFlock2-0.3.50/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SFlock2
-Version: 0.3.49
+Version: 0.3.50
 Summary: Sample staging and detonation utility
 Home-page: https://github.com/doomedraven/sflock/
 Author: Hatching B.V.
 Author-email: jbr@hatching.io
 License: GPLv3
 Keywords: sflock unarchive
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SFlock2-0.3.49/README.md` & `SFlock2-0.3.50/README.md`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/SFlock2.egg-info/PKG-INFO` & `SFlock2-0.3.50/SFlock2.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SFlock2
-Version: 0.3.49
+Version: 0.3.50
 Summary: Sample staging and detonation utility
 Home-page: https://github.com/doomedraven/sflock/
 Author: Hatching B.V.
 Author-email: jbr@hatching.io
 License: GPLv3
 Keywords: sflock unarchive
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `SFlock2-0.3.49/setup.py` & `SFlock2-0.3.50/setup.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/.DS_Store` & `SFlock2-0.3.50/sflock/.DS_Store`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/abstracts.py` & `SFlock2-0.3.50/sflock/abstracts.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/aux/decode_vbe_jse.py` & `SFlock2-0.3.50/sflock/aux/decode_vbe_jse.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/compat/magic.py` & `SFlock2-0.3.50/sflock/compat/magic.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/config.py` & `SFlock2-0.3.50/sflock/config.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/.DS_Store` & `SFlock2-0.3.50/sflock/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/poweriso.elf` & `SFlock2-0.3.50/sflock/data/poweriso.elf`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/win32/magic.mgc` & `SFlock2-0.3.50/sflock/data/win32/magic.mgc`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/win32/magic1.dll` & `SFlock2-0.3.50/sflock/data/win32/magic1.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/win32/regex2.dll` & `SFlock2-0.3.50/sflock/data/win32/regex2.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/win32/zlib1.dll` & `SFlock2-0.3.50/sflock/data/win32/zlib1.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/win64/libgnurx-0.dll` & `SFlock2-0.3.50/sflock/data/win64/libgnurx-0.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/win64/magic.mgc` & `SFlock2-0.3.50/sflock/data/win64/magic.mgc`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/win64/magic1.dll` & `SFlock2-0.3.50/sflock/data/win64/magic1.dll`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/yara/shellcodes.yar` & `SFlock2-0.3.50/sflock/data/yara/shellcodes.yar`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/data/zipjail.elf` & `SFlock2-0.3.50/sflock/data/zipjail.elf`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/decode/office.py` & `SFlock2-0.3.50/sflock/decode/office.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/ident.py` & `SFlock2-0.3.50/sflock/ident.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
         ("wsf", (b".wsf",)),
         ("pdf", (b".pdf",)),
         ("vbs", (b".vbs", b".vbe")),
         ("msbuild", (b".csproj", b".vbproj", b".vcxproj", b".dbproj", b".fsproj")),
         ("zip", (b".zip",)),
         ("cpl", (b".cpl",)),
         ("ichitaro", (b".jtd", b".jtdc", b".jttc", b".jtt")),
-        ("one", (b".one", b".onetoc2"))
+        ("inf", (b".inf",)),
+        ("one", (b".one", b".onetoc2")),
     ]
 )
 
 trusted_archive_mimes = OrderedDict(
     [
         ("application/x-iso9660-image", "iso"),
     ]
@@ -84,14 +85,15 @@
         ("application/x-7z-compressed", "7z"),
         ("application/x-bzip2", "bzip2"),
         ("application/x-tar", "tar"),
         ("application/java-archive", "jar"),
         ("application/x-dosexec", "exe"),
         ("application/vnd.ms-cab-compressed", "cab"),
         ("application/pdf", "pdf"),
+        ("application/x-setupscript", "inf"),
     ]
 )
 
 trusted_archive_magics = OrderedDict(
     [
         ("ISO 9660", "iso"),
     ]
@@ -486,14 +488,34 @@
 
 def udf(f):
     if HAVE_YARA:
         matches = archives_rules.match(data=f.contents)
         if "archive_udf" in [rule.rule for rule in matches]:
             return "udf"
 
+def inf(f):
+    if f.contents.startswith(b"MZ"):
+        return None
+
+    STRINGS = [
+        # b"[version]",
+        b"Signature=",
+        b"AdvancedINF=",
+        b"[DefaultInstall_SingleUser]",
+        b"[DefaultInstall]",
+    ]
+
+    found = 0
+    for string in STRINGS:
+        found += f.contents.count(string)
+
+    if found >= 3:
+        return "inf"
+
+
 def identify(f, check_shellcode: bool = False):
     if not f.stream.read(0x1000):
         return
 
     if f.filename:
         for package, extensions in file_extensions.items():
             if f.filename.endswith(extensions):
@@ -552,8 +574,9 @@
     java,
     wsf,
     xxe,
     pub,
     vbe_jse,
     sct,
     inp,
+    inf,
 ]
```

### Comparing `SFlock2-0.3.49/sflock/main.py` & `SFlock2-0.3.50/sflock/main.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/misc.py` & `SFlock2-0.3.50/sflock/misc.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/pick.py` & `SFlock2-0.3.50/sflock/pick.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/ace.py` & `SFlock2-0.3.50/sflock/unpack/ace.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/bup.py` & `SFlock2-0.3.50/sflock/unpack/bup.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/cab.py` & `SFlock2-0.3.50/sflock/unpack/cab.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/daa.py` & `SFlock2-0.3.50/sflock/unpack/daa.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/eml.py` & `SFlock2-0.3.50/sflock/unpack/eml.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/lzip.py` & `SFlock2-0.3.50/sflock/unpack/lzip.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/msg.py` & `SFlock2-0.3.50/sflock/unpack/msg.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/mso.py` & `SFlock2-0.3.50/sflock/unpack/mso.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/office.py` & `SFlock2-0.3.50/sflock/unpack/office.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/pdf.py` & `SFlock2-0.3.50/sflock/unpack/pdf.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/rar.py` & `SFlock2-0.3.50/sflock/unpack/rar.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/tar.py` & `SFlock2-0.3.50/sflock/unpack/tar.py`

 * *Files identical despite different names*

### Comparing `SFlock2-0.3.49/sflock/unpack/zip7.py` & `SFlock2-0.3.50/sflock/unpack/zip7.py`

 * *Files identical despite different names*

