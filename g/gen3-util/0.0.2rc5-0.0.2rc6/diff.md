# Comparing `tmp/gen3_util-0.0.2rc5.tar.gz` & `tmp/gen3_util-0.0.2rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3_util-0.0.2rc5.tar", last modified: Thu Jun 22 16:39:51 2023, max compression
+gzip compressed data, was "gen3_util-0.0.2rc6.tar", last modified: Thu Jun 22 17:06:11 2023, max compression
```

## Comparing `gen3_util-0.0.2rc5.tar` & `gen3_util-0.0.2rc6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.767754 gen3_util-0.0.2rc5/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc5/LICENSE
--rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-22 16:39:51.767543 gen3_util-0.0.2rc5/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     6374 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc5/README.md
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.722665 gen3_util-0.0.2rc5/gen3_util/
--rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc5/gen3_util/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.738152 gen3_util-0.0.2rc5/gen3_util/access/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1819 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc5/gen3_util/access/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1948 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc5/gen3_util/access/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1869 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc5/gen3_util/access/requestor.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.748699 gen3_util-0.0.2rc5/gen3_util/buckets/
--rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/buckets/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc5/gen3_util/buckets/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/buckets/lister.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.749701 gen3_util-0.0.2rc5/gen3_util/cli/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4469 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc5/gen3_util/cli/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc5/gen3_util/cli/cli.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.750044 gen3_util-0.0.2rc5/gen3_util/common/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4119 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc5/gen3_util/common/__init__.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.751065 gen3_util-0.0.2rc5/gen3_util/config/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2425 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/config/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      485 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/config/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/config/config.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.756908 gen3_util-0.0.2rc5/gen3_util/files/
--rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/gen3_util/files/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/gen3_util/files/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      920 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/files/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/files/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/files/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142    13289 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/files/uploader.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.759513 gen3_util-0.0.2rc5/gen3_util/meta/
--rw-r--r--   0 walsbr   (320923486) 1971611142     4117 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/meta/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1291 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/meta/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc5/gen3_util/meta/downloader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     5483 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/meta/importer.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      191 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/meta/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/meta/remover.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      208 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/meta/uploader.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/gen3_util/meta/validator.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.763260 gen3_util-0.0.2rc5/gen3_util/projects/
--rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/gen3_util/projects/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/gen3_util/projects/cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-22 16:34:30.000000 gen3_util-0.0.2rc5/gen3_util/projects/creator.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/gen3_util/projects/lister.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1040 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/gen3_util/projects/remover.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.733444 gen3_util-0.0.2rc5/gen3_util.egg-info/
--rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-22 16:39:51.000000 gen3_util-0.0.2rc5/gen3_util.egg-info/PKG-INFO
--rw-r--r--   0 walsbr   (320923486) 1971611142     1502 2023-06-22 16:39:51.000000 gen3_util-0.0.2rc5/gen3_util.egg-info/SOURCES.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-06-22 16:39:51.000000 gen3_util-0.0.2rc5/gen3_util.egg-info/dependency_links.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-06-22 16:39:51.000000 gen3_util-0.0.2rc5/gen3_util.egg-info/entry_points.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-06-22 16:39:51.000000 gen3_util-0.0.2rc5/gen3_util.egg-info/requires.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-06-22 16:39:51.000000 gen3_util-0.0.2rc5/gen3_util.egg-info/top_level.txt
--rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-06-22 16:39:51.767822 gen3_util-0.0.2rc5/setup.cfg
--rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-06-22 16:36:54.000000 gen3_util-0.0.2rc5/setup.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.720146 gen3_util-0.0.2rc5/tests/
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.765196 gen3_util-0.0.2rc5/tests/integration/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc5/tests/integration/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc5/tests/integration/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2941 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/tests/integration/test_access.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/tests/integration/test_buckets.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     2055 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/tests/integration/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1225 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/tests/integration/test_project.py
-drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 16:39:51.767231 gen3_util-0.0.2rc5/tests/unit/
--rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc5/tests/unit/__init__.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc5/tests/unit/conftest.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     3222 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/tests/unit/test_cli.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc5/tests/unit/test_coding_conventions.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc5/tests/unit/test_config.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/tests/unit/test_files.py
--rw-r--r--   0 walsbr   (320923486) 1971611142      867 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc5/tests/unit/test_meta.py
--rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc5/tests/unit/test_validate_directory.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.202558 gen3_util-0.0.2rc6/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1065 2023-05-04 14:32:05.000000 gen3_util-0.0.2rc6/LICENSE
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-22 17:06:11.202393 gen3_util-0.0.2rc6/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     6374 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/README.md
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.136662 gen3_util-0.0.2rc6/gen3_util/
+-rw-r--r--   0 walsbr   (320923486) 1971611142       71 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/gen3_util/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.158931 gen3_util-0.0.2rc6/gen3_util/access/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1819 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/access/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1948 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/access/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1869 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/access/requestor.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.161379 gen3_util-0.0.2rc6/gen3_util/buckets/
+-rw-r--r--   0 walsbr   (320923486) 1971611142      803 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/buckets/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      629 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/buckets/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      474 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/buckets/lister.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.167312 gen3_util-0.0.2rc6/gen3_util/cli/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4469 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/cli/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/cli/cli.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.187335 gen3_util-0.0.2rc6/gen3_util/common/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4119 2023-06-21 17:42:54.000000 gen3_util-0.0.2rc6/gen3_util/common/__init__.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.189243 gen3_util-0.0.2rc6/gen3_util/config/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2425 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/config/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      485 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/config/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      503 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/config/config.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.194244 gen3_util-0.0.2rc6/gen3_util/files/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1285 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/files/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2246 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/files/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      920 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/files/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      192 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/files/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      202 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/files/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142    13289 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/files/uploader.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.196817 gen3_util-0.0.2rc6/gen3_util/meta/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     4117 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1291 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      210 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/gen3_util/meta/downloader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5483 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/importer.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      191 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      201 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/remover.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      208 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/uploader.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3248 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/gen3_util/meta/validator.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.198287 gen3_util-0.0.2rc6/gen3_util/projects/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2247 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/projects/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1667 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/projects/cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1901 2023-06-22 16:34:30.000000 gen3_util-0.0.2rc6/gen3_util/projects/creator.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      793 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/gen3_util/projects/lister.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1078 2023-06-22 17:04:30.000000 gen3_util-0.0.2rc6/gen3_util/projects/remover.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.154913 gen3_util-0.0.2rc6/gen3_util.egg-info/
+-rw-r--r--   0 walsbr   (320923486) 1971611142     7059 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/PKG-INFO
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1502 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/SOURCES.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142        1 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/dependency_links.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       53 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/entry_points.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142      128 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/requires.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       16 2023-06-22 17:06:11.000000 gen3_util-0.0.2rc6/gen3_util.egg-info/top_level.txt
+-rw-r--r--   0 walsbr   (320923486) 1971611142       38 2023-06-22 17:06:11.202607 gen3_util-0.0.2rc6/setup.cfg
+-rw-r--r--   0 walsbr   (320923486) 1971611142     5580 2023-06-22 17:05:57.000000 gen3_util-0.0.2rc6/setup.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.130195 gen3_util-0.0.2rc6/tests/
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.200055 gen3_util-0.0.2rc6/tests/integration/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/integration/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      108 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/integration/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2941 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/tests/integration/test_access.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      433 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/integration/test_buckets.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     2055 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/tests/integration/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1225 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/integration/test_project.py
+drwxr-xr-x   0 walsbr   (320923486) 1971611142        0 2023-06-22 17:06:11.202131 gen3_util-0.0.2rc6/tests/unit/
+-rw-r--r--   0 walsbr   (320923486) 1971611142        0 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/unit/__init__.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      322 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/unit/conftest.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     3222 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/unit/test_cli.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      565 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/unit/test_coding_conventions.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      551 2023-05-05 20:31:25.000000 gen3_util-0.0.2rc6/tests/unit/test_config.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1760 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/unit/test_files.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142      867 2023-06-21 17:42:55.000000 gen3_util-0.0.2rc6/tests/unit/test_meta.py
+-rw-r--r--   0 walsbr   (320923486) 1971611142     1546 2023-05-10 23:31:00.000000 gen3_util-0.0.2rc6/tests/unit/test_validate_directory.py
```

### Comparing `gen3_util-0.0.2rc5/LICENSE` & `gen3_util-0.0.2rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/PKG-INFO` & `gen3_util-0.0.2rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3_util
-Version: 0.0.2rc5
+Version: 0.0.2rc6
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.2rc5/README.md` & `gen3_util-0.0.2rc6/README.md`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/access/__init__.py` & `gen3_util-0.0.2rc6/gen3_util/access/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/access/cli.py` & `gen3_util-0.0.2rc6/gen3_util/access/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/access/requestor.py` & `gen3_util-0.0.2rc6/gen3_util/access/requestor.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/buckets/__init__.py` & `gen3_util-0.0.2rc6/gen3_util/buckets/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/buckets/cli.py` & `gen3_util-0.0.2rc6/gen3_util/buckets/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/cli/__init__.py` & `gen3_util-0.0.2rc6/gen3_util/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/cli/cli.py` & `gen3_util-0.0.2rc6/gen3_util/cli/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/common/__init__.py` & `gen3_util-0.0.2rc6/gen3_util/common/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/config/__init__.py` & `gen3_util-0.0.2rc6/gen3_util/config/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/files/__init__.py` & `gen3_util-0.0.2rc6/gen3_util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/files/cli.py` & `gen3_util-0.0.2rc6/gen3_util/files/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/files/downloader.py` & `gen3_util-0.0.2rc6/gen3_util/files/downloader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/files/uploader.py` & `gen3_util-0.0.2rc6/gen3_util/files/uploader.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/meta/__init__.py` & `gen3_util-0.0.2rc6/gen3_util/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/meta/cli.py` & `gen3_util-0.0.2rc6/gen3_util/meta/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/meta/importer.py` & `gen3_util-0.0.2rc6/gen3_util/meta/importer.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/meta/validator.py` & `gen3_util-0.0.2rc6/gen3_util/meta/validator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/projects/__init__.py` & `gen3_util-0.0.2rc6/gen3_util/projects/__init__.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/projects/cli.py` & `gen3_util-0.0.2rc6/gen3_util/projects/cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/projects/creator.py` & `gen3_util-0.0.2rc6/gen3_util/projects/creator.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/projects/lister.py` & `gen3_util-0.0.2rc6/gen3_util/projects/lister.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/gen3_util/projects/remover.py` & `gen3_util-0.0.2rc6/gen3_util/projects/remover.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 
     try:
         response = submission.delete_project(program=program, project=project)
         response.raise_for_status()
 
         return ProjectSummaries(**{
             'endpoint': auth.endpoint,
-            'projects': [project_id],
+            'projects': {project_id: {'exists': False}},
             'messages': [f'Deleted {project_id}']
         })
 
     except HTTPError as e:
         return ProjectSummaries(**{
             'endpoint': auth.endpoint,
-            'projects': [project_id],
+            'projects': {project_id: {'exists': False}},
             'messages': [f'Error deleting {project_id}: {e} {e.response.text}']
         })
```

### Comparing `gen3_util-0.0.2rc5/gen3_util.egg-info/PKG-INFO` & `gen3_util-0.0.2rc6/gen3_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen3-util
-Version: 0.0.2rc5
+Version: 0.0.2rc6
 Summary: Commons utilities
 Home-page: https://github.com/ACED-IDP/gen3_util
 Author: Ellrott Lab
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ACED-IDP/gen3_util/issues
 Project-URL: Source, https://github.com/ACED-IDP/gen3_util
 Keywords: gen3 bioinformatics
```

### Comparing `gen3_util-0.0.2rc5/gen3_util.egg-info/SOURCES.txt` & `gen3_util-0.0.2rc6/gen3_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/setup.py` & `gen3_util-0.0.2rc6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name='gen3_util',  # Required
 
     # Versions should comply with PEP 440:
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.2-rc5',  # Required
+    version='0.0.2-rc6',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Commons utilities',
     # Optional
```

### Comparing `gen3_util-0.0.2rc5/tests/integration/test_access.py` & `gen3_util-0.0.2rc6/tests/integration/test_access.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/tests/integration/test_files.py` & `gen3_util-0.0.2rc6/tests/integration/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/tests/integration/test_project.py` & `gen3_util-0.0.2rc6/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/tests/unit/test_cli.py` & `gen3_util-0.0.2rc6/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/tests/unit/test_coding_conventions.py` & `gen3_util-0.0.2rc6/tests/unit/test_coding_conventions.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/tests/unit/test_config.py` & `gen3_util-0.0.2rc6/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/tests/unit/test_files.py` & `gen3_util-0.0.2rc6/tests/unit/test_files.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/tests/unit/test_meta.py` & `gen3_util-0.0.2rc6/tests/unit/test_meta.py`

 * *Files identical despite different names*

### Comparing `gen3_util-0.0.2rc5/tests/unit/test_validate_directory.py` & `gen3_util-0.0.2rc6/tests/unit/test_validate_directory.py`

 * *Files identical despite different names*

