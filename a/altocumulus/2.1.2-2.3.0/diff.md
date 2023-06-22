# Comparing `tmp/altocumulus-2.1.2.tar.gz` & `tmp/altocumulus-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altocumulus-2.1.2.tar", last modified: Tue Aug 16 05:37:43 2022, max compression
+gzip compressed data, was "altocumulus-2.3.0.tar", last modified: Thu Jun 22 05:35:26 2023, max compression
```

## Comparing `altocumulus-2.1.2.tar` & `altocumulus-2.3.0.tar`

### file list

```diff
@@ -1,84 +1,110 @@
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.263977 altocumulus-2.1.2/
--rw-r--r--   0 yangy197   (501) staff       (20)     1203 2022-01-12 02:16:12.000000 altocumulus-2.1.2/.gitignore
--rw-r--r--   0 yangy197   (501) staff       (20)     1532 2022-01-12 02:16:12.000000 altocumulus-2.1.2/LICENSE
--rw-r--r--   0 yangy197   (501) staff       (20)     2440 2022-08-16 05:37:43.263421 altocumulus-2.1.2/PKG-INFO
--rw-r--r--   0 yangy197   (501) staff       (20)     1502 2022-01-12 04:40:03.000000 altocumulus-2.1.2/README.rst
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.227567 altocumulus-2.1.2/alto/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1151 2022-08-04 20:06:39.000000 altocumulus-2.1.2/alto/__main__.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.229369 altocumulus-2.1.2/alto/commands/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/__init__.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.233203 altocumulus-2.1.2/alto/commands/cromwell/
--rw-r--r--   0 yangy197   (501) staff       (20)      838 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/cromwell/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1011 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/cromwell/abort.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1025 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/cromwell/check_status.py
--rw-r--r--   0 yangy197   (501) staff       (20)     3088 2022-04-10 19:34:01.000000 altocumulus-2.1.2/alto/commands/cromwell/get_logs.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1061 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/cromwell/get_metadata.py
--rw-r--r--   0 yangy197   (501) staff       (20)     5121 2022-08-16 05:29:23.000000 altocumulus-2.1.2/alto/commands/cromwell/list_jobs.py
--rw-r--r--   0 yangy197   (501) staff       (20)     8441 2022-08-12 19:12:13.000000 altocumulus-2.1.2/alto/commands/cromwell/run.py
--rw-r--r--   0 yangy197   (501) staff       (20)     3624 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/parse_monitoring_log.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1713 2022-08-12 20:54:19.000000 altocumulus-2.1.2/alto/commands/query.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.236108 altocumulus-2.1.2/alto/commands/terra/
--rw-r--r--   0 yangy197   (501) staff       (20)      721 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/terra/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2329 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/terra/add_method.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2179 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/terra/remove_method.py
--rw-r--r--   0 yangy197   (501) staff       (20)     7184 2022-02-15 19:08:54.000000 altocumulus-2.1.2/alto/commands/terra/run.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1454 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/commands/terra/storage_estimate.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2617 2022-05-03 04:00:34.000000 altocumulus-2.1.2/alto/commands/upload.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.237626 altocumulus-2.1.2/alto/tests/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     2167 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/command_tests.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.238187 altocumulus-2.1.2/alto/tests/inputs/
--rw-r--r--   0 yangy197   (501) staff       (20)      232 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/echo.wdl
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.223402 altocumulus-2.1.2/alto/tests/inputs/flowcell1/
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.239985 altocumulus-2.1.2/alto/tests/inputs/flowcell1/s1/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell1/s1/s1_I1.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell1/s1/s1_R1.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell1/s1/s1_R2.fastq.gz
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.241474 altocumulus-2.1.2/alto/tests/inputs/flowcell1/s2/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell1/s2/s2_I1.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell1/s2/s2_R1.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell1/s2/s2_R2.fastq.gz
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.223807 altocumulus-2.1.2/alto/tests/inputs/flowcell2/
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.243588 altocumulus-2.1.2/alto/tests/inputs/flowcell2/s1/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell2/s1/s1_I1.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell2/s1/s1_R1.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell2/s1/s1_R2.fastq.gz
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.245291 altocumulus-2.1.2/alto/tests/inputs/flowcell2/s2/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell2/s2/s2_I1.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell2/s2/s2_R1.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/flowcell2/s2/s2_R2.fastq.gz
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.246532 altocumulus-2.1.2/alto/tests/inputs/test_sample/
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/test_sample/test_sample_S1_L001_I1_001.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/test_sample/test_sample_S1_L001_R1_001.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/inputs/test_sample/test_sample_S1_L001_R2_001.fastq.gz
--rw-r--r--   0 yangy197   (501) staff       (20)       37 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/tests/test.json
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.250942 altocumulus-2.1.2/alto/utils/
--rw-r--r--   0 yangy197   (501) staff       (20)      883 2022-02-15 19:08:54.000000 altocumulus-2.1.2/alto/utils/__init__.py
--rw-r--r--   0 yangy197   (501) staff       (20)     5000 2022-08-12 20:53:40.000000 altocumulus-2.1.2/alto/utils/bcl_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)     5802 2022-03-16 04:05:51.000000 altocumulus-2.1.2/alto/utils/dockstore_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)     1498 2022-08-12 20:53:40.000000 altocumulus-2.1.2/alto/utils/fastq_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)     6298 2022-01-12 02:16:12.000000 altocumulus-2.1.2/alto/utils/firecloud_utils.py
--rw-r--r--   0 yangy197   (501) staff       (20)    11117 2022-08-15 23:57:54.000000 altocumulus-2.1.2/alto/utils/io_utils.py
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.255435 altocumulus-2.1.2/altocumulus.egg-info/
--rw-r--r--   0 yangy197   (501) staff       (20)     2440 2022-08-16 05:37:42.000000 altocumulus-2.1.2/altocumulus.egg-info/PKG-INFO
--rw-r--r--   0 yangy197   (501) staff       (20)     2030 2022-08-16 05:37:43.000000 altocumulus-2.1.2/altocumulus.egg-info/SOURCES.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        1 2022-08-16 05:37:42.000000 altocumulus-2.1.2/altocumulus.egg-info/dependency_links.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       44 2022-08-16 05:37:42.000000 altocumulus-2.1.2/altocumulus.egg-info/entry_points.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        1 2022-01-12 02:47:42.000000 altocumulus-2.1.2/altocumulus.egg-info/not-zip-safe
--rw-r--r--   0 yangy197   (501) staff       (20)       75 2022-08-16 05:37:42.000000 altocumulus-2.1.2/altocumulus.egg-info/requires.txt
--rw-r--r--   0 yangy197   (501) staff       (20)        5 2022-08-16 05:37:43.000000 altocumulus-2.1.2/altocumulus.egg-info/top_level.txt
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.261267 altocumulus-2.1.2/docs/
--rw-r--r--   0 yangy197   (501) staff       (20)      609 2022-01-12 02:16:12.000000 altocumulus-2.1.2/docs/Makefile
-drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2022-08-16 05:37:43.262420 altocumulus-2.1.2/docs/_static/
--rw-r--r--   0 yangy197   (501) staff       (20)       30 2022-03-16 04:17:19.000000 altocumulus-2.1.2/docs/_static/custom.css
--rw-r--r--   0 yangy197   (501) staff       (20)     6236 2022-08-16 05:29:35.000000 altocumulus-2.1.2/docs/conf.py
--rw-r--r--   0 yangy197   (501) staff       (20)      131 2022-01-12 02:16:12.000000 altocumulus-2.1.2/docs/index.rst
--rw-r--r--   0 yangy197   (501) staff       (20)      308 2022-01-12 04:40:03.000000 altocumulus-2.1.2/docs/installation.rst
--rw-r--r--   0 yangy197   (501) staff       (20)     3778 2022-08-16 05:33:06.000000 altocumulus-2.1.2/docs/release_notes.rst
--rw-r--r--   0 yangy197   (501) staff       (20)       63 2022-01-12 02:16:12.000000 altocumulus-2.1.2/docs/requirements.txt
--rw-r--r--   0 yangy197   (501) staff       (20)    17266 2022-08-12 20:53:40.000000 altocumulus-2.1.2/docs/usage.rst
--rw-r--r--   0 yangy197   (501) staff       (20)      106 2022-01-12 02:16:12.000000 altocumulus-2.1.2/pyproject.toml
--rw-r--r--   0 yangy197   (501) staff       (20)       75 2022-08-04 20:06:39.000000 altocumulus-2.1.2/requirements.txt
--rw-r--r--   0 yangy197   (501) staff       (20)       38 2022-08-16 05:37:43.264195 altocumulus-2.1.2/setup.cfg
--rw-r--r--   0 yangy197   (501) staff       (20)     1579 2022-08-12 20:53:40.000000 altocumulus-2.1.2/setup.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.433923 altocumulus-2.3.0/
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.364404 altocumulus-2.3.0/.github/
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.370542 altocumulus-2.3.0/.github/workflows/
+-rw-r--r--   0 yangy197   (501) staff       (20)      613 2022-08-26 18:23:40.000000 altocumulus-2.3.0/.github/workflows/test.yml
+-rw-r--r--   0 yangy197   (501) staff       (20)     1228 2023-03-14 07:06:24.000000 altocumulus-2.3.0/.gitignore
+-rw-r--r--   0 yangy197   (501) staff       (20)      772 2023-06-16 08:15:29.000000 altocumulus-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 yangy197   (501) staff       (20)     1532 2022-08-26 18:23:40.000000 altocumulus-2.3.0/LICENSE
+-rw-r--r--   0 yangy197   (501) staff       (20)       28 2022-11-05 00:26:26.000000 altocumulus-2.3.0/MANIFEST.in
+-rw-r--r--   0 yangy197   (501) staff       (20)     4340 2023-06-22 05:35:26.433311 altocumulus-2.3.0/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)     1502 2022-08-26 18:23:40.000000 altocumulus-2.3.0/README.rst
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.371449 altocumulus-2.3.0/alto/
+-rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/__init__.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1202 2022-09-04 00:47:28.000000 altocumulus-2.3.0/alto/__main__.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.374203 altocumulus-2.3.0/alto/__pycache__/
+-rw-r--r--   0 yangy197   (501) staff       (20)      142 2022-08-26 18:23:58.000000 altocumulus-2.3.0/alto/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)      133 2023-03-14 06:56:18.000000 altocumulus-2.3.0/alto/__pycache__/__init__.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1253 2022-09-04 00:52:07.000000 altocumulus-2.3.0/alto/__pycache__/__main__.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1297 2023-03-14 06:56:18.000000 altocumulus-2.3.0/alto/__pycache__/__main__.pypy39.pyc
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.378857 altocumulus-2.3.0/alto/altocumulus.egg-info/
+-rw-r--r--   0 yangy197   (501) staff       (20)     4365 2022-09-04 22:18:57.000000 altocumulus-2.3.0/alto/altocumulus.egg-info/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)     1455 2022-09-04 22:18:57.000000 altocumulus-2.3.0/alto/altocumulus.egg-info/SOURCES.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        1 2022-09-04 22:18:57.000000 altocumulus-2.3.0/alto/altocumulus.egg-info/dependency_links.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       44 2022-09-04 22:18:57.000000 altocumulus-2.3.0/alto/altocumulus.egg-info/entry_points.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        1 2022-09-04 22:15:55.000000 altocumulus-2.3.0/alto/altocumulus.egg-info/not-zip-safe
+-rw-r--r--   0 yangy197   (501) staff       (20)       99 2022-09-04 22:18:57.000000 altocumulus-2.3.0/alto/altocumulus.egg-info/requires.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       21 2022-09-04 22:18:57.000000 altocumulus-2.3.0/alto/altocumulus.egg-info/top_level.txt
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.381066 altocumulus-2.3.0/alto/commands/
+-rw-r--r--   0 yangy197   (501) staff       (20)        0 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/__init__.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.385910 altocumulus-2.3.0/alto/commands/__pycache__/
+-rw-r--r--   0 yangy197   (501) staff       (20)      151 2022-08-26 18:23:58.000000 altocumulus-2.3.0/alto/commands/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)      142 2023-03-14 06:56:20.000000 altocumulus-2.3.0/alto/commands/__pycache__/__init__.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     5004 2023-06-16 08:15:39.000000 altocumulus-2.3.0/alto/commands/__pycache__/parse_monitoring_log.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1817 2022-09-01 18:19:38.000000 altocumulus-2.3.0/alto/commands/__pycache__/query.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     2347 2022-08-26 18:23:59.000000 altocumulus-2.3.0/alto/commands/__pycache__/upload.cpython-39.pyc
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.395023 altocumulus-2.3.0/alto/commands/cromwell/
+-rw-r--r--   0 yangy197   (501) staff       (20)     1109 2023-06-16 08:23:26.000000 altocumulus-2.3.0/alto/commands/cromwell/__init__.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.406684 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/
+-rw-r--r--   0 yangy197   (501) staff       (20)     1004 2023-06-16 08:34:41.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1063 2023-03-14 06:56:20.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/__init__.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1233 2022-08-26 18:23:58.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/abort.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1341 2023-03-14 06:56:20.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/abort.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1252 2022-08-26 18:23:58.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/check_status.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1374 2023-03-14 06:56:20.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/check_status.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     2576 2023-03-14 07:11:55.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/get_logs.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     2835 2023-03-14 06:56:20.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/get_logs.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1316 2022-08-26 18:23:59.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/get_metadata.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     2729 2023-06-22 05:28:01.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/get_task_status.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     4156 2022-08-26 18:23:59.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/list_jobs.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     7890 2022-09-12 19:47:21.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1414 2023-02-28 21:35:10.000000 altocumulus-2.3.0/alto/commands/cromwell/__pycache__/timing.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1137 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/cromwell/abort.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1151 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/cromwell/check_status.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     3198 2023-03-14 07:06:24.000000 altocumulus-2.3.0/alto/commands/cromwell/get_logs.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1193 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/cromwell/get_metadata.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2681 2023-06-22 05:32:25.000000 altocumulus-2.3.0/alto/commands/cromwell/get_task_status.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     5157 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/cromwell/list_jobs.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    10773 2022-09-05 18:43:30.000000 altocumulus-2.3.0/alto/commands/cromwell/run.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1392 2023-02-28 08:15:17.000000 altocumulus-2.3.0/alto/commands/cromwell/timing.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     7033 2023-06-16 08:15:29.000000 altocumulus-2.3.0/alto/commands/parse_monitoring_log.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.410099 altocumulus-2.3.0/alto/commands/terra/
+-rw-r--r--   0 yangy197   (501) staff       (20)      807 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/terra/__init__.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.413146 altocumulus-2.3.0/alto/commands/terra/__pycache__/
+-rw-r--r--   0 yangy197   (501) staff       (20)      870 2022-08-26 18:23:59.000000 altocumulus-2.3.0/alto/commands/terra/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     2005 2022-08-26 18:23:59.000000 altocumulus-2.3.0/alto/commands/terra/__pycache__/add_method.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1639 2022-08-26 18:23:59.000000 altocumulus-2.3.0/alto/commands/terra/__pycache__/remove_method.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     6290 2023-02-28 21:35:12.000000 altocumulus-2.3.0/alto/commands/terra/__pycache__/run.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1483 2022-08-26 18:23:59.000000 altocumulus-2.3.0/alto/commands/terra/__pycache__/storage_estimate.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     2647 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/terra/add_method.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2456 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/terra/remove_method.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     7751 2023-02-28 08:15:17.000000 altocumulus-2.3.0/alto/commands/terra/run.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     1566 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/terra/storage_estimate.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2825 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/commands/upload.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.417053 altocumulus-2.3.0/alto/utils/
+-rw-r--r--   0 yangy197   (501) staff       (20)      968 2022-08-26 18:23:40.000000 altocumulus-2.3.0/alto/utils/__init__.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.423785 altocumulus-2.3.0/alto/utils/__pycache__/
+-rw-r--r--   0 yangy197   (501) staff       (20)     1092 2022-08-26 18:23:58.000000 altocumulus-2.3.0/alto/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     1153 2023-03-14 06:56:20.000000 altocumulus-2.3.0/alto/utils/__pycache__/__init__.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     3960 2023-03-14 07:12:09.000000 altocumulus-2.3.0/alto/utils/__pycache__/bcl_utils.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     5140 2023-02-28 21:35:09.000000 altocumulus-2.3.0/alto/utils/__pycache__/dockstore_utils.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     5315 2023-03-14 06:56:20.000000 altocumulus-2.3.0/alto/utils/__pycache__/dockstore_utils.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     2129 2023-03-14 07:12:09.000000 altocumulus-2.3.0/alto/utils/__pycache__/fastq_utils.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     5442 2023-02-28 21:35:09.000000 altocumulus-2.3.0/alto/utils/__pycache__/firecloud_utils.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     6005 2023-03-14 06:56:20.000000 altocumulus-2.3.0/alto/utils/__pycache__/firecloud_utils.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     9192 2023-03-14 07:11:55.000000 altocumulus-2.3.0/alto/utils/__pycache__/io_utils.cpython-39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     9735 2023-03-14 06:56:21.000000 altocumulus-2.3.0/alto/utils/__pycache__/io_utils.pypy39.pyc
+-rw-r--r--   0 yangy197   (501) staff       (20)     5354 2023-03-14 07:06:24.000000 altocumulus-2.3.0/alto/utils/bcl_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     5903 2023-02-28 08:15:17.000000 altocumulus-2.3.0/alto/utils/dockstore_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     2280 2023-03-14 07:06:24.000000 altocumulus-2.3.0/alto/utils/fastq_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)     6561 2023-02-28 08:15:17.000000 altocumulus-2.3.0/alto/utils/firecloud_utils.py
+-rw-r--r--   0 yangy197   (501) staff       (20)    12460 2023-03-14 07:06:24.000000 altocumulus-2.3.0/alto/utils/io_utils.py
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.426921 altocumulus-2.3.0/altocumulus.egg-info/
+-rw-r--r--   0 yangy197   (501) staff       (20)     4340 2023-06-22 05:35:26.000000 altocumulus-2.3.0/altocumulus.egg-info/PKG-INFO
+-rw-r--r--   0 yangy197   (501) staff       (20)     3494 2023-06-22 05:35:26.000000 altocumulus-2.3.0/altocumulus.egg-info/SOURCES.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        1 2023-06-22 05:35:26.000000 altocumulus-2.3.0/altocumulus.egg-info/dependency_links.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)       44 2023-06-22 05:35:26.000000 altocumulus-2.3.0/altocumulus.egg-info/entry_points.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        1 2022-09-04 23:44:30.000000 altocumulus-2.3.0/altocumulus.egg-info/not-zip-safe
+-rw-r--r--   0 yangy197   (501) staff       (20)      106 2023-06-22 05:35:26.000000 altocumulus-2.3.0/altocumulus.egg-info/requires.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)        5 2023-06-22 05:35:26.000000 altocumulus-2.3.0/altocumulus.egg-info/top_level.txt
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.431581 altocumulus-2.3.0/docs/
+-rw-r--r--   0 yangy197   (501) staff       (20)      609 2022-08-26 18:23:40.000000 altocumulus-2.3.0/docs/Makefile
+drwxr-xr-x   0 yangy197   (501) staff       (20)        0 2023-06-22 05:35:26.432299 altocumulus-2.3.0/docs/_static/
+-rw-r--r--   0 yangy197   (501) staff       (20)       30 2022-08-26 18:23:40.000000 altocumulus-2.3.0/docs/_static/custom.css
+-rw-r--r--   0 yangy197   (501) staff       (20)     6220 2022-11-05 01:03:20.000000 altocumulus-2.3.0/docs/conf.py
+-rw-r--r--   0 yangy197   (501) staff       (20)      131 2022-08-26 18:23:40.000000 altocumulus-2.3.0/docs/index.rst
+-rw-r--r--   0 yangy197   (501) staff       (20)      309 2022-08-26 18:23:40.000000 altocumulus-2.3.0/docs/installation.rst
+-rw-r--r--   0 yangy197   (501) staff       (20)     4197 2023-06-22 05:32:25.000000 altocumulus-2.3.0/docs/release_notes.rst
+-rw-r--r--   0 yangy197   (501) staff       (20)       63 2022-08-26 18:23:40.000000 altocumulus-2.3.0/docs/requirements.txt
+-rw-r--r--   0 yangy197   (501) staff       (20)    17339 2023-06-22 05:32:25.000000 altocumulus-2.3.0/docs/usage.rst
+-rw-r--r--   0 yangy197   (501) staff       (20)     2193 2023-03-14 07:06:24.000000 altocumulus-2.3.0/pyproject.toml
+-rw-r--r--   0 yangy197   (501) staff       (20)       38 2023-06-22 05:35:26.434091 altocumulus-2.3.0/setup.cfg
```

### Comparing `altocumulus-2.1.2/.gitignore` & `altocumulus-2.3.0/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -98,7 +98,10 @@
 .ropeproject
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
+
+# macOS cache
+.DS_Store
```

### Comparing `altocumulus-2.1.2/LICENSE` & `altocumulus-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `altocumulus-2.1.2/README.rst` & `altocumulus-2.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `altocumulus-2.1.2/alto/__main__.py` & `altocumulus-2.3.0/alto/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 import sys
 import argparse
-from alto.commands import terra, upload, parse_monitoring_log, cromwell, query
 
 import requests
 from requests.packages.urllib3.exceptions import InsecureRequestWarning
+
+from alto.commands import cromwell, parse_monitoring_log, terra, upload
+
+
 requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
 
 try:
     from importlib.metadata import version
 except ImportError:  # < Python 3.8: Use backport module
     from importlib_metadata import version
 
-def main():
-    str2module = {'terra': terra, 'upload': upload, 'parse_monitoring_log': parse_monitoring_log, 'cromwell': cromwell, 'query': query}
 
-    parser = argparse.ArgumentParser(description='Run an altocumulus command.')
-    parser.add_argument('command', help='The command', choices=['terra', 'upload', 'parse_monitoring_log', 'cromwell', 'query'])
-    parser.add_argument('command_args', help='The command arguments', nargs=argparse.REMAINDER)
-    parser.add_argument('-v', '--version', action="version", version=version('altocumulus'))
+def main():
+    str2module = {
+        "terra": terra,
+        "upload": upload,
+        "parse_monitoring_log": parse_monitoring_log,
+        "cromwell": cromwell,
+    }
+
+    parser = argparse.ArgumentParser(description="Run an altocumulus command.")
+    parser.add_argument(
+        "command",
+        help="The command",
+        choices=["terra", "upload", "parse_monitoring_log", "cromwell", "query"],
+    )
+    parser.add_argument("command_args", help="The command arguments", nargs=argparse.REMAINDER)
+    parser.add_argument("-v", "--version", action="version", version=version("altocumulus"))
     my_args = parser.parse_args()
 
     cmd = str2module[my_args.command]
-    sys.argv[0] = f'alto {my_args.command}'
+    sys.argv[0] = f"alto {my_args.command}"
     cmd.main(my_args.command_args)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `altocumulus-2.1.2/alto/commands/cromwell/abort.py` & `altocumulus-2.3.0/alto/commands/cromwell/abort.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,45 @@
-import argparse, requests
+import argparse
+
+import requests
 
 
 def abort_job(server, port, job_id):
     resp = requests.post(f"http://{server}:{port}/api/workflows/v1/{job_id}/abort")
     resp_dict = resp.json()
 
     if resp.status_code == 200:
         print(f"Job {resp_dict['id']} is in status {resp_dict['status']}.")
     else:
-        print(resp_dict['message'])
+        print(resp_dict["message"])
+
 
 def main(argv):
     parser = argparse.ArgumentParser(
         description="Abort a running workflow job on a Cromwell server."
     )
-    parser.add_argument('-s', '--server', dest='server', action='store', required=True,
-        help="Server hostname or IP address."
+    parser.add_argument(
+        "-s",
+        "--server",
+        dest="server",
+        action="store",
+        required=True,
+        help="Server hostname or IP address.",
     )
-    parser.add_argument('-p', '--port', dest='port', action='store', default='8000',
-        help="Port number for Cromwell service. The default port is 8000."
+    parser.add_argument(
+        "-p",
+        "--port",
+        dest="port",
+        action="store",
+        default="8000",
+        help="Port number for Cromwell service. The default port is 8000.",
     )
-    parser.add_argument('--id', dest='job_id', action='store', required=True,
-        help="Workflow ID returned in 'alto cromwell run' command."
+    parser.add_argument(
+        "--id",
+        dest="job_id",
+        action="store",
+        required=True,
+        help="Workflow ID returned in 'alto cromwell run' command.",
     )
 
     args = parser.parse_args(argv)
     abort_job(args.server, args.port, args.job_id)
```

### Comparing `altocumulus-2.1.2/alto/commands/cromwell/check_status.py` & `altocumulus-2.3.0/alto/commands/cromwell/check_status.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,46 @@
-import argparse, requests
+import argparse
+
+import requests
 
 
 def get_status(server, port, job_id):
     resp = requests.get(f"http://{server}:{port}/api/workflows/v1/{job_id}/status")
     resp_dict = resp.json()
 
     if resp.status_code == 200:
         print(f"Job {resp_dict['id']} is in status {resp_dict['status']}.")
     else:
-        print(resp_dict['message'])
+        print(resp_dict["message"])
+
 
 def main(argv):
     parser = argparse.ArgumentParser(
         description="Check the current status for a workflow on a Cromwell server."
     )
-    parser.add_argument('-s', '--server', dest='server', action='store', required=True,
-        help="Server hostname or IP address."
+    parser.add_argument(
+        "-s",
+        "--server",
+        dest="server",
+        action="store",
+        required=True,
+        help="Server hostname or IP address.",
     )
-    parser.add_argument('-p', '--port', dest='port', action='store', default='8000',
-        help="Port number for Cromwell service. The default port is 8000."
+    parser.add_argument(
+        "-p",
+        "--port",
+        dest="port",
+        action="store",
+        default="8000",
+        help="Port number for Cromwell service. The default port is 8000.",
     )
-    parser.add_argument('--id', dest='job_id', action='store', required=True,
-        help="Workflow ID returned in 'alto cromwell run' command."
+    parser.add_argument(
+        "--id",
+        dest="job_id",
+        action="store",
+        required=True,
+        help="Workflow ID returned in 'alto cromwell run' command.",
     )
 
     args = parser.parse_args(argv)
 
     get_status(args.server, args.port, args.job_id)
```

### Comparing `altocumulus-2.1.2/alto/commands/cromwell/get_logs.py` & `altocumulus-2.3.0/alto/commands/cromwell/get_logs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,98 @@
-import argparse, requests
+import argparse
+from subprocess import CalledProcessError
+
+import requests
 
 from alto.utils import run_command
-from subprocess import CalledProcessError
 
 
 def get_localize_path(cloud_uri, job_id):
-    uri_list = cloud_uri.split('://')
-    backend = 'local'
+    uri_list = cloud_uri.split("://")
+    backend = "local"
     if len(uri_list) > 1:
-        backend = 'aws' if uri_list[0] == 's3' else 'gcp'
+        backend = "aws" if uri_list[0] == "s3" else "gcp"
 
-    local_path = cloud_uri[cloud_uri.find(job_id):]
+    local_path = cloud_uri[cloud_uri.find(job_id) :]
 
     return backend, local_path
 
 
 def get_remote_log_file(cloud_uri, job_id, profile):
-    backend, local_path = get_localize_path(cloud_uri, job_id)
+    _, local_path = get_localize_path(cloud_uri, job_id)
     try:
-        strato_cmd = ['strato', 'cp', '--backend', backend, '--quiet', cloud_uri, local_path]
+        strato_cmd = ["strato", "cp", "--quiet", cloud_uri, local_path]
         if profile is not None:
-            strato_cmd.extend(['--profile', profile])
+            strato_cmd.extend(["--profile", profile])
         run_command(strato_cmd, dry_run=False)
     except CalledProcessError:
         print(f"{cloud_uri} does not exist.")
 
 
 def get_logs(server, port, top_job_id, cur_job_id, profile):
     # For tasks directly called by current job
     resp_logs = requests.get(f"http://{server}:{port}/api/workflows/v1/{cur_job_id}/logs")
     logs_dict = resp_logs.json()
     if resp_logs.status_code != 200:
-        raise Exception(logs_dict['message'])
+        raise Exception(logs_dict["message"])
 
     processed_tasks = set()
-    if 'calls' in logs_dict.keys():
-        for task_name, log_list in logs_dict['calls'].items():
+    if "calls" in logs_dict.keys():
+        for task_name, log_list in logs_dict["calls"].items():
             for log in log_list:
-                get_remote_log_file(log['stderr'], top_job_id, profile)
-                get_remote_log_file(log['stdout'], top_job_id, profile)
+                get_remote_log_file(log["stderr"], top_job_id, profile)
+                get_remote_log_file(log["stdout"], top_job_id, profile)
             processed_tasks.add(task_name)
 
     resp_meta = requests.get(f"http://{server}:{port}/api/workflows/v1/{cur_job_id}/metadata")
     meta_dict = resp_meta.json()
     if resp_meta.status_code != 200:
-        raise Exception(meta_dict['message'])
+        raise Exception(meta_dict["message"])
 
     # For tasks with subworkflow ID
-    if 'calls' in meta_dict.keys():
-        for task_name, task_list in meta_dict['calls'].items():
+    if "calls" in meta_dict.keys():
+        for task_name, task_list in meta_dict["calls"].items():
             if task_name not in processed_tasks:
                 for task in task_list:
-                    if 'subWorkflowId' in task.keys():
-                        subworkflow_id = task['subWorkflowId']
+                    if "subWorkflowId" in task.keys():
+                        subworkflow_id = task["subWorkflowId"]
                         get_logs(server, port, top_job_id, subworkflow_id, profile)
 
 
 def main(argv):
-    parser = argparse.ArgumentParser(
-        description="Get the logs for a submitted job."
-    )
-    parser.add_argument('-s', '--server', dest='server', action='store', required=True,
-        help="Server hostname or IP address."
+    parser = argparse.ArgumentParser(description="Get the logs for a submitted job.")
+    parser.add_argument(
+        "-s",
+        "--server",
+        dest="server",
+        action="store",
+        required=True,
+        help="Server hostname or IP address.",
     )
-    parser.add_argument('-p', '--port', dest='port', action='store', default='8000',
-        help="Port number for Cromwell service. The default port is 8000."
+    parser.add_argument(
+        "-p",
+        "--port",
+        dest="port",
+        action="store",
+        default="8000",
+        help="Port number for Cromwell service. The default port is 8000.",
     )
-    parser.add_argument('--id', dest='job_id', action='store', required=True,
-        help="Workflow ID returned in 'alto cromwell run' command."
+    parser.add_argument(
+        "--id",
+        dest="job_id",
+        action="store",
+        required=True,
+        help="Workflow ID returned in 'alto cromwell run' command.",
     )
-    parser.add_argument('--profile', dest='profile', type=str,
-        help="AWS profile. Only works if dealing with AWS, and if not set, use the default profile."
+    parser.add_argument(
+        "--profile",
+        dest="profile",
+        type=str,
+        help="AWS profile. Only works if dealing with AWS, and if not set, use the default profile.",
     )
 
     args = parser.parse_args(argv)
 
     # Create log folder even if there is no log file.
-    run_command(['mkdir', '-p', args.job_id], dry_run=False)
+    run_command(["mkdir", "-p", args.job_id], dry_run=False)
 
     get_logs(args.server, args.port, args.job_id, args.job_id, args.profile)
```

### Comparing `altocumulus-2.1.2/alto/commands/cromwell/list_jobs.py` & `altocumulus-2.3.0/alto/commands/cromwell/list_jobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
-import argparse
+import time
 import getpass
-import requests
-import pandas as pd
+import argparse
 from datetime import datetime
-from dateutil import parser
-import time
 from typing import List, Optional
 
+import pandas as pd
+import requests
+from dateutil import parser
+
 
 def datetime_from_utc_to_local(utc_datetime: str) -> str:
     if not utc_datetime:
         return ""
     now_timestamp = time.time()
-    offset = datetime.fromtimestamp(now_timestamp) - datetime.utcfromtimestamp(
-        now_timestamp
-    )
+    offset = datetime.fromtimestamp(now_timestamp) - datetime.utcfromtimestamp(now_timestamp)
     return (parser.parse(utc_datetime) + offset).strftime("%d %b %Y, %H:%M:%S")
 
 
 class bcolors:
     SUCCESS = "\033[92m"
     FAILED = "\033[91m"
     ENDC = "\033[0m"
@@ -89,17 +88,20 @@
         else:
             res["creator"] = ""
         res["submission"] = datetime_from_utc_to_local(res.get("submission", ""))
         res["start"] = datetime_from_utc_to_local(res.get("start", ""))
         res["end"] = datetime_from_utc_to_local(res.get("end", ""))
     if resp.status_code == 200:
         df_jobs = pd.DataFrame.from_records(resp_dict["results"])
-        if 'name' in df_jobs:
-            df_jobs.loc[(df_jobs['name'].isna()) & (df_jobs['status'].isin(['Submitted', 'Running'])), 'name'] = '<under checking>'
-            df_jobs['name'] = df_jobs['name'].fillna('<failed before exec>')
+        if "name" in df_jobs:
+            df_jobs.loc[
+                (df_jobs["name"].isna()) & (df_jobs["status"].isin(["Submitted", "Running"])),
+                "name",
+            ] = "<parsing workflow>"
+            df_jobs["name"] = df_jobs["name"].fillna("<failed before exec>")
         show_jobs(df_jobs, num_shown=num_shown)
     else:
         print(resp_dict["message"])
 
 
 def main(argv):
     parser = argparse.ArgumentParser(description="List jobs submitted to the server.")
```

### Comparing `altocumulus-2.1.2/alto/commands/cromwell/run.py` & `altocumulus-2.3.0/alto/commands/terra/run.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,200 +1,190 @@
-import argparse, getpass, json, os, requests, time, zipfile
-from alto.utils.io_utils import read_wdl_inputs, upload_to_cloud_bucket
-from alto.utils import parse_dockstore_workflow, get_dockstore_workflow
-
-cur_pid = os.getpid()
-wf_label_filename = f".{cur_pid}.workflow_labels.json"
-wf_option_filename = f".{cur_pid}.workflow_options.json"
-
-
-def parse_bucket_folder_url(bucket):
-    assert '://' in bucket, "Bucket folder URL must start with 's3://' or 'gs://'."
-
-    res = bucket.split('://')
-    backend = 'aws'
-    if res[0] == 'gs':
-        backend = 'gcp'
-
-    res2 = res[1].split('/')  # Remove the trailing slash if exists.
-    bucket_id = res2[0]
-    bucket_folder = '/'.join(res2[1:])
-
-    return (backend, bucket_id, bucket_folder)
-
-
-def wait_and_check(server, port, job_id, time_out, freq=60):
-    url = f"http://{server}:{port}/api/workflows/v1/{job_id}/status"
-
-    time_out_seconds = time_out * 3600
-    seconds_passed = 0
-    status = ""
-
-    while seconds_passed < time_out_seconds:
-        time.sleep(freq)
-        seconds_passed += freq
-        resp = requests.get(url)
-        resp_dict = resp.json()
-        if resp.status_code == 200:
-            if resp_dict['status'] in ['Succeeded', 'Failed', 'Aborted']:
-                status = resp_dict['status']
-                break
-        else:
-            print(resp_dict['message'])
-            break
-
-    if seconds_passed >= time_out_seconds:
-        print(f"{time_out}-hour time-out is reached!")
-
-    return status
-
+import argparse
+from typing import Union
 
-def parse_workflow_str(method_str, no_ssl_verify):
-    is_url = False
-    workflow_str = method_str
-
-    if "://" in method_str:
-        assert method_str.split("://")[0] in ['http', 'https'], "Only http or https URL is acceptable!"
-        is_url = True
-    elif ":" in method_str:
-        organization, collection, workflow, version = parse_dockstore_workflow(method_str)
-        workflow_def = get_dockstore_workflow(organization, collection, workflow, version, ssl_verify=not no_ssl_verify)
-        is_url = True
-        workflow_str = workflow_def['url']
-
-    return workflow_str, is_url
-
-def check_zip(dependency_str):
-    is_dependency = False
-    if os.path.isfile(dependency_str) and zipfile.is_zipfile(dependency_str):
-        is_dependency = True
-    return is_dependency
-
-def submit_to_cromwell(server, port, method_str, wf_input_path, out_json, bucket, no_cache, no_ssl_verify, time_out, profile, dependency_str):
-    files = dict()
-    data = dict()
-    label_dict = dict()
-
-    # Process job's workflow WDL
-    workflow_str, is_url = parse_workflow_str(method_str, no_ssl_verify)
-    if is_url:
-        data['workflowUrl'] = workflow_str
-    else:
-        files['workflowSource'] = open(workflow_str, 'rb')
-
-    # Process workflow WDL's dependency
-    if dependency_str is not None:
-        if check_zip(dependency_str):
-            files['workflowDependencies'] = open(dependency_str, 'rb')
+from alto.utils import (
+    get_dockstore_workflow,
+    get_firecloud_workflow,
+    get_workspace_info,
+    parse_dockstore_workflow,
+    parse_firecloud_workflow,
+    parse_workspace,
+    prefix_float,
+    read_wdl_inputs,
+    submit_a_job_to_terra,
+    update_workflow_config_in_workspace,
+    upload_to_cloud_bucket,
+)
+
+
+def detect_workflow_source(workflow_string: str) -> str:
+    """Detect if a workflow is from Dockerstore or Broad Methods Repository."""
+    if workflow_string.find(":") >= 0:
+        return "Dockstore"
+    return "Broad Methods Repository"
+
+
+def convert_inputs(inputs: dict) -> dict:
+    """Convert elements in the dictionary loaded by json to formats that Terra accepts as inputs."""
+    results = {}
+    for key, value in inputs.items():
+        if isinstance(value, bool):
+            value = "true" if value else "false"
+        elif isinstance(value, str) and value.startswith(prefix_float):
+            # input is float, prefix_float + 'float'
+            value = value[len(prefix_float) :]
+        elif isinstance(value, str):
+            value = f'"{value}"'
+        elif isinstance(value, list) and len(value) > 0 and isinstance(value[0], str):
+            for i in range(len(value)):
+                value[i] = f'"{value[i]}"'
+            value = f'[{",".join(value)}]'
         else:
-            raise Exception('Dependency zip file does not exist or is not given in zip format.')
-
-    # Process job's workflow inputs
-    inputs = read_wdl_inputs(wf_input_path)
+            value = str(value)
+        results[key] = value
+    return results
+
+
+def submit_to_terra(
+    workflow_string: str,
+    workspace: str,
+    wdl_inputs: Union[str, dict],
+    out_json: str = None,
+    bucket_folder: str = None,
+    use_callcache: bool = True,
+) -> str:
+    """Submit a workflow to Terra. The workflow can from either Dockstore or Broad Methods
+    Repository.
+
+    Parameters
+    ----------
+    workflow_string: `str`
+        String indicating which workflow to use. The workflow can come from either Dockstore or Broad Methods Repository. If it comes from Dockstore, specify the name as organization:collection:name:version (e.g. broadinstitute:cumulus:cumulus:1.5.0) and the default version would be used if version is omitted. If it comes from Broad Methods Repository, specify the name as namespace/name/version (e.g. cumulus/cumulus/43) and the latest snapshot would be used if version is omitted.
+
+    workspace: `str`
+        Terra Workspace name, which consists of a namespace and a name.
+
+    wdl_inputs: `str` or `dict`
+        Workflow inputs specified as a JSON file. If wdl_inputs is `str`, it refers to the path to the JSON file. Otherwise, it is a dictionary representing an in-memory JSON.
+
+    out_json: `str`, optional (default: None)
+        Path for the updated JSON file where local paths are replaced by gs URLs. Specify this parameter implies that users want altocumulus to transfer local files to the workspace-asscociated Google Bucket.
+
+    bucket_folder: `str`, optional (default: None)
+        This pamameter refers to a local path under the workspace-associated Google Bucket. Local files will be uploaded under this folder.
+
+    use_callcache: `bool`, optional (default: True)
+        If use call caching.
+
+    Returns
+    -------
+    `str` object.
+        A URL referring to the job status would be returned.
+
+    Examples
+    --------
+    >>> status_url = submit_to_terra('broadinstitute:cumulus:cumulus', 'kco-tech/Cumulus', 'cumulus_inputs.json', out_json = 'cumulus_inputs_updated.json', bucket_folder = 'cumulus_input', cache = True)
+    """
+    inputs = read_wdl_inputs(wdl_inputs)  # read inputs from JSON
+
+    # check method
+    workflow_def = None
+    config_namespace = config_name = None
+    if detect_workflow_source(workflow_string) == "Dockstore":
+        organization, collection, workflow, version = parse_dockstore_workflow(workflow_string)
+        config_namespace = collection
+        config_name = workflow
+        workflow_def = get_dockstore_workflow(organization, collection, workflow, version)
+    else:
+        namespace, name, version = parse_firecloud_workflow(workflow_string)
+        config_namespace = namespace
+        config_name = name
+        workflow_def = get_firecloud_workflow(namespace, name, version)
+
+    # check workspace
+    workspace_namespace, workspace_name = parse_workspace(workspace)
+    workspace_def = get_workspace_info(workspace_namespace, workspace_name)
 
-    # Upload input data to cloud bucket if needed.
+    # upload input data to google bucket and generate modified JSON input file
     if out_json is not None:
-        backend, bucket_id, bucket_folder = parse_bucket_folder_url(bucket)
-        upload_to_cloud_bucket(
-            inputs=inputs,
-            backend=backend,
-            bucket=bucket_id,
-            bucket_folder=bucket_folder,
-            out_json=out_json,
-            dry_run=False,
-            verbose=True if time_out is None else False,
-            profile=profile,
-        )
-
-    files['workflowInputs'] = open(wf_input_path if out_json is None else out_json, 'rb')
-
-    # Add username to the job labels
-    label_dict['creator'] = getpass.getuser()
-
-    with open(wf_label_filename, 'w') as fp:
-        json.dump(label_dict, fp)
-    files['labels'] = open(wf_label_filename, 'rb')
-
-    # Process job's workflow options.
-    if no_cache:
-        wf_option_dict = {
-            'read_from_cache': False,
-        }
-        with open(wf_option_filename, 'w') as fp:
-            json.dump(wf_option_dict, fp)
-        files['workflowOptions'] = open(wf_option_filename, 'rb')
-
-    # Send HTTP request to Cromwell server
-    try:
-        resp = requests.post(
-            f"http://{server}:{port}/api/workflows/v1",
-            files=files,
-            data=data,
-        )
-    finally:
-        # Remove intermediate input files
-        if os.path.exists(wf_label_filename):
-            os.remove(wf_label_filename)
-        if os.path.exists(wf_option_filename):
-            os.remove(wf_option_filename)
-
-    # Process response.
-    resp_dict = resp.json()
-
-    if resp.status_code == 201:
-        if time_out is None:
-            print(f"Job {resp_dict['id']} is in status {resp_dict['status']}.")
-    else:
-        print(resp_dict['message'])
+        bucket = workspace_def["bucketName"]
+        upload_to_cloud_bucket(inputs, "gcp", bucket, bucket_folder, out_json, False)
 
-    # Enter the monitor mode
-    if time_out is not None:
-        status = wait_and_check(server, port, resp_dict['id'], time_out)
-        print(f"{{\"job_id\": \"{resp_dict['id']}\", \"status\": \"{status}\"}}")
+    # update workflow configuration in the workspace
+    method_body = {
+        "namespace": config_namespace,
+        "name": config_name,
+        "rootEntityType": None,  # Do not use data model
+        "inputs": convert_inputs(inputs),
+        "outputs": {},
+        "prerequisites": {},
+        "methodRepoMethod": {"methodUri": workflow_def["methodUri"]},
+        "methodConfigVersion": 1,
+        "deleted": False,
+    }
+    update_workflow_config_in_workspace(
+        config_namespace, config_name, method_body, workspace_namespace, workspace_name
+    )
+
+    # submit a job to terra
+    return submit_a_job_to_terra(
+        workspace_namespace,
+        workspace_name,
+        config_namespace,
+        config_name,
+        use_callcache=use_callcache,
+    )
 
 
 def main(argv):
-    parser = argparse.ArgumentParser(description="Submit WDL jobs to a Cromwell server for execution. \
-        Workflows should be from Dockstore. For Dockstore workflows, collection and name would be used as config namespace and name respectively. \
-        If local files are detected, automatically upload files to the workspace Google Cloud bucket. \
-        After a successful submission, a URL pointing to the job status would be printed out."
-    )
-    parser.add_argument('-s', '--server', dest='server', action='store', required=True,
-        help="Server hostname or IP address."
-    )
-    parser.add_argument('-p', '--port', dest='port', action='store', default='8000',
-        help="Port number for Cromwell service. The default port is 8000."
-    )
-    parser.add_argument('-m', '--method', dest='method_str', action='store', required=True,
-        help="Three forms of workflow WDL file is accepted: \
-              (1) Workflow name from Dockstore, with name specified as \"organization:collection:name:version\" (e.g. \"broadinstitute:cumulus:cumulus:1.5.0\"). If 'version' part is not specified, the default version defined on Dockstore would be used. \
-              (2) An HTTP or HTTPS URL of a WDL file. \
-              (3) A local path to a WDL file."
-    )
-    parser.add_argument('-d', '--dependency', dest='dependency_str', action='store',
-        help="ZIP file containing workflow source files that are used \
-              to resolve local imports. This zip bundle will be unpacked \
-              in a sandbox accessible to the workflow."
-    )
-    parser.add_argument('-i', '--input', dest='input', action='store', required=True,
-        help="Path to a local JSON file specifying workflow inputs."
-    )
-    parser.add_argument('-o', '--upload', dest='out_json', metavar='<updated_json>', action='store',
-        help="Upload files/directories to the workspace cloud bucket and output updated input json (with local path replaced by cloud bucket urls) to <updated_json>.")
-    parser.add_argument('-b', '--bucket', dest='bucket', action='store', metavar='[s3|gs]://<bucket-name>/<bucket-folder>',
-        help="Cloud bucket folder for uploading local input data. Start with 's3://' if an AWS S3 bucket is used, 'gs://' for a Google bucket. \
-        Must be specified when '-o' option is used."
-    )
-    parser.add_argument('--no-cache', dest='no_cache', action='store_true', help="Disable call-caching, i.e. do not read from cache.")
-    parser.add_argument('--no-ssl-verify', dest='no_ssl_verify', action='store_true', default=False,
-        help="Disable SSL verification for web requests. Not recommended for general usage, but can be useful for intra-networks which don't support SSL verification."
+    parser = argparse.ArgumentParser(
+        description="Submit workflows to Terra for execution. Workflows can from either Dockstore or Broad Methods Repository. If local files are detected, automatically upload files to the workspace Google Cloud bucket. For Dockstore workflows, collection and name would be used as config namespace and name respectively. Otherwise, namespace and name would be used. After a successful submission, a URL pointing to the job status would be printed out."
     )
-    parser.add_argument('--time-out', dest='time_out', type=float,
-        help="Keep on checking the job's status until time_out (in hours) is reached. Notice that if this option is set, Altocumulus won't terminate until reaching time_out."
+    parser.add_argument(
+        "-m",
+        "--method",
+        dest="method",
+        action="store",
+        required=True,
+        help="Workflow name. The workflow can come from either Dockstore or Broad Methods Repository. If it comes from Dockstore, specify the name as organization:collection:name:version (e.g. broadinstitute:cumulus:cumulus:1.5.0) and the default version would be used if version is omitted. If it comes from Broad Methods Repository, specify the name as namespace/name/version (e.g. cumulus/cumulus/43) and the latest snapshot would be used if version is omitted.",
+    )
+    parser.add_argument(
+        "-w",
+        "--workspace",
+        dest="workspace",
+        action="store",
+        required=True,
+        help="Workspace name (e.g. foo/bar). The workspace is created if it does not exist",
+    )
+    parser.add_argument(
+        "--bucket-folder",
+        metavar="<folder>",
+        dest="bucket_folder",
+        action="store",
+        help="Store inputs to <folder> under workspace" "s google bucket",
+    )
+    parser.add_argument(
+        "-i", "--input", dest="wdl_inputs", action="store", required=True, help="WDL input JSON."
+    )
+    parser.add_argument(
+        "-o",
+        "--upload",
+        dest="out_json",
+        metavar="<updated_json>",
+        action="store",
+        help="Upload files/directories to the workspace Google Cloud bucket and output updated input json (with local path replaced by google bucket urls) to <updated_json>.",
     )
-    parser.add_argument('--profile', dest='profile', type=str,
-        help="AWS profile. Only works if dealing with AWS, and if not set, use the default profile."
+    parser.add_argument(
+        "--no-cache", dest="no_cache", action="store_true", help="Disable call caching."
     )
-
     args = parser.parse_args(argv)
 
-    submit_to_cromwell(args.server, args.port, args.method_str, args.input, args.out_json, args.bucket, args.no_cache, args.no_ssl_verify, args.time_out, args.profile, args.dependency_str)
+    url = submit_to_terra(
+        args.method,
+        args.workspace,
+        args.wdl_inputs,
+        out_json=args.out_json,
+        bucket_folder=args.bucket_folder,
+        use_callcache=not args.no_cache,
+    )
+
+    print(url)
```

### Comparing `altocumulus-2.1.2/alto/commands/terra/__init__.py` & `altocumulus-2.3.0/alto/commands/terra/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 import sys
 import argparse
-from . import run, add_method, remove_method, storage_estimate
+
+from . import add_method, remove_method, run, storage_estimate
+
 
 def main(args):
-    str2module = {'run': run, 'add_method': add_method, 'remove_method': remove_method, 'storage_estimate': storage_estimate}
+    str2module = {
+        "run": run,
+        "add_method": add_method,
+        "remove_method": remove_method,
+        "storage_estimate": storage_estimate,
+    }
 
-    parser = argparse.ArgumentParser(description='Run a terra sub-command.')
-    parser.add_argument('subcommand', help='The sub-command', choices=['run', 'add_method', 'remove_method', 'storage_estimate'])
-    parser.add_argument('subcommand_args', help='The sub-command arguments', nargs=argparse.REMAINDER)
+    parser = argparse.ArgumentParser(description="Run a terra sub-command.")
+    parser.add_argument(
+        "subcommand",
+        help="The sub-command",
+        choices=["run", "add_method", "remove_method", "storage_estimate"],
+    )
+    parser.add_argument(
+        "subcommand_args", help="The sub-command arguments", nargs=argparse.REMAINDER
+    )
     my_args = parser.parse_args(args)
 
     subcmd = str2module[my_args.subcommand]
-    sys.argv[0] = f'alto terra {my_args.subcommand}'
+    sys.argv[0] = f"alto terra {my_args.subcommand}"
     subcmd.main(my_args.subcommand_args)
```

### Comparing `altocumulus-2.1.2/alto/commands/terra/add_method.py` & `altocumulus-2.3.0/alto/commands/terra/add_method.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,77 @@
 import os
 import argparse
 
 from firecloud import api as fapi
-from alto.utils import *
 
+from alto.utils import get_firecloud_workflow
 
 
 def main(argv):
-    parser = argparse.ArgumentParser(description='Add one or more methods to Broad Methods Repository.')
-    parser.add_argument('-n', '--namespace', dest='namespace', action='store', required=True, help='Methods namespace')
-    parser.add_argument('-p', '--public', dest='public', action='store_true', help='Make methods publicly readable')
-    parser.add_argument(dest='wdl', help='Path to WDL file.', nargs='+')
+    parser = argparse.ArgumentParser(
+        description="Add one or more methods to Broad Methods Repository."
+    )
+    parser.add_argument(
+        "-n",
+        "--namespace",
+        dest="namespace",
+        action="store",
+        required=True,
+        help="Methods namespace",
+    )
+    parser.add_argument(
+        "-p", "--public", dest="public", action="store_true", help="Make methods publicly readable"
+    )
+    parser.add_argument(dest="wdl", help="Path to WDL file.", nargs="+")
     args = parser.parse_args(argv)
 
     namespace = args.namespace
     public = args.public
 
     n_success = 0
     for wdl in args.wdl:
         method_name = os.path.basename(wdl)
-        suffix = method_name.lower().rfind('.wdl')
+        suffix = method_name.lower().rfind(".wdl")
         if suffix != -1:
             method_name = method_name[0:suffix]
 
         method_acl = []
         try:
             existing_method = get_firecloud_workflow(namespace, method_name)
-            method_acl = fapi.get_repository_method_acl(namespace=existing_method['namespace'], method=existing_method['name'], snapshot_id=existing_method['snapshotId']).json()
+            method_acl = fapi.get_repository_method_acl(
+                namespace=existing_method["namespace"],
+                method=existing_method["name"],
+                snapshot_id=existing_method["snapshotId"],
+            ).json()
         except ValueError:
             pass
 
         if public:
             existing_public_user = False
             for i in range(len(method_acl)):
-                if method_acl[i]['user'] == 'public':
+                if method_acl[i]["user"] == "public":
                     existing_public_user = True
-                    method_acl[i] = dict(user='public', role='READER')
+                    method_acl[i] = dict(user="public", role="READER")
                     break
             if not existing_public_user:
-                method_acl.append(dict(user='public', role='READER'))
+                method_acl.append(dict(user="public", role="READER"))
 
-        result = fapi.update_repository_method(namespace=namespace, method=method_name, wdl=wdl, synopsis='')
+        result = fapi.update_repository_method(
+            namespace=namespace, method=method_name, wdl=wdl, synopsis=""
+        )
         if result.status_code == 201:
             result = result.json()
             if len(method_acl) > 0:
-                fapi.update_repository_method_acl(namespace=result['namespace'], method=result['name'], snapshot_id=result['snapshotId'], acl_updates=method_acl)
-            print(f'Workflow {method_name} is imported! See https://api.firecloud.org/ga4gh/v1/tools/{result["namespace"]}:{result["name"]}/versions/{result["snapshotId"]}/plain-WDL/descriptor')
+                fapi.update_repository_method_acl(
+                    namespace=result["namespace"],
+                    method=result["name"],
+                    snapshot_id=result["snapshotId"],
+                    acl_updates=method_acl,
+                )
+            print(
+                f'Workflow {method_name} is imported! See https://api.firecloud.org/ga4gh/v1/tools/{result["namespace"]}:{result["name"]}/versions/{result["snapshotId"]}/plain-WDL/descriptor'
+            )
             n_success += 1
         else:
-            print(f'Unable to add workflow {method_name} - {result.json()}')
+            print(f"Unable to add workflow {method_name} - {result.json()}")
 
-    print(f'Successfully added {n_success} workflows.')
+    print(f"Successfully added {n_success} workflows.")
```

### Comparing `altocumulus-2.1.2/alto/commands/terra/remove_method.py` & `altocumulus-2.3.0/alto/commands/terra/remove_method.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,58 @@
 import argparse
 
 from firecloud import api as fapi
-from alto.utils import *
-
 
 
 def main(argv):
-    parser = argparse.ArgumentParser(description='Remove methods from Broad Methods Repository.')
-    parser.add_argument('-m', '--method', dest='method', action='store', required=True, help='Method takes the format of namespace/name/version. If only namespace is provided, delete all methods under that namespace. If both namespace and name are provided, delete all snapshots for that method. If namespace, name and version are provided, only delete the specific snapshot.')
+    parser = argparse.ArgumentParser(description="Remove methods from Broad Methods Repository.")
+    parser.add_argument(
+        "-m",
+        "--method",
+        dest="method",
+        action="store",
+        required=True,
+        help="Method takes the format of namespace/name/version. If only namespace is provided, delete all methods under that namespace. If both namespace and name are provided, delete all snapshots for that method. If namespace, name and version are provided, only delete the specific snapshot.",
+    )
     args = parser.parse_args(argv)
 
-    fields = args.method.split('/')
+    fields = args.method.split("/")
     if len(fields) == 0:
-        raise ValueError('No namespace specified!')
+        raise ValueError("No namespace specified!")
 
     method_namespace = fields[0]
     method_name = fields[1] if len(fields) > 0 else None
     method_version = fields[2] if len(fields) > 1 else None
 
     methods = fapi.list_repository_methods(namespace=method_namespace, name=method_name).json()
     if len(methods) == 0:
-        raise ValueError('No methods found')
+        raise ValueError("No methods found")
 
     if method_name is None:  # delete all methods under specified namespace
         for method in methods:
-            if method['namespace'] == method_namespace:
-                fapi.delete_repository_method(method['namespace'], method['name'], method['snapshotId'])
+            if method["namespace"] == method_namespace:
+                fapi.delete_repository_method(
+                    method["namespace"], method["name"], method["snapshotId"]
+                )
                 print(f'Deleted {method["namespace"]}/{method["name"]}/{method["snapshotId"]}')
     elif method_version is None:  # delete all versions
         for selected_method in methods:
-            if selected_method['namespace'] == method_namespace and selected_method['name'] == method_name:
-                fapi.delete_repository_method(selected_method['namespace'], selected_method['name'], selected_method['snapshotId'])
-                print(f'Deleted {selected_method["namespace"]}/{selected_method["name"]}/{selected_method["snapshotId"]}')
-    else: # delete the specific version
+            if (
+                selected_method["namespace"] == method_namespace
+                and selected_method["name"] == method_name
+            ):
+                fapi.delete_repository_method(
+                    selected_method["namespace"],
+                    selected_method["name"],
+                    selected_method["snapshotId"],
+                )
+                print(
+                    f'Deleted {selected_method["namespace"]}/{selected_method["name"]}/{selected_method["snapshotId"]}'
+                )
+    else:  # delete the specific version
         selected_method = methods[0]
-        fapi.delete_repository_method(selected_method['namespace'], selected_method['name'], selected_method['snapshotId'])
-        print(f'Deleted {selected_method["namespace"]}/{selected_method["name"]}/{selected_method["snapshotId"]}')
+        fapi.delete_repository_method(
+            selected_method["namespace"], selected_method["name"], selected_method["snapshotId"]
+        )
+        print(
+            f'Deleted {selected_method["namespace"]}/{selected_method["name"]}/{selected_method["snapshotId"]}'
+        )
```

### Comparing `altocumulus-2.1.2/alto/commands/terra/storage_estimate.py` & `altocumulus-2.3.0/alto/commands/terra/storage_estimate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 import argparse
 from urllib.parse import urljoin
-from firecloud import api as fapi
 
+from firecloud import api as fapi
 
 
 def main(argv):
-    parser = argparse.ArgumentParser(description='Export workspace storage cost estimates associated with the user to TSV')
-    parser.add_argument('--output', help='Output TSV path', required=True)
-    parser.add_argument('--access', help='Workspace access levels', choices=['owner', 'reader', 'writer'], action='append')
+    parser = argparse.ArgumentParser(
+        description="Export workspace storage cost estimates associated with the user to TSV"
+    )
+    parser.add_argument("--output", help="Output TSV path", required=True)
+    parser.add_argument(
+        "--access",
+        help="Workspace access levels",
+        choices=["owner", "reader", "writer"],
+        action="append",
+    )
     args = parser.parse_args(argv)
 
     workspaces = fapi.list_workspaces().json()
 
     access = args.access
     if access is None:
         access = []
     output = args.output
     access_filter = set()
-    if 'reader' in access:
-        access_filter.add('READER')
-    if 'writer' in access:
-        access_filter.add('WRITER')
-    if 'owner' in access or len(access) == 0:
-        access_filter.add('PROJECT_OWNER')
+    if "reader" in access:
+        access_filter.add("READER")
+    if "writer" in access:
+        access_filter.add("WRITER")
+    if "owner" in access or len(access) == 0:
+        access_filter.add("PROJECT_OWNER")
 
-    with open(output, 'wt') as out:
-        out.write('namespace\tname\testimate\n')
+    with open(output, "wt") as out:
+        out.write("namespace\tname\testimate\n")
         for w in workspaces:
-            if w['accessLevel'] in access_filter:
-                namespace = w['workspace']['namespace']
-                name = w['workspace']['name']
+            if w["accessLevel"] in access_filter:
+                namespace = w["workspace"]["namespace"]
+                name = w["workspace"]["name"]
 
                 headers = fapi._fiss_agent_header()
                 root_url = fapi.fcconfig.root_url
-                r = fapi.__SESSION.get(urljoin(root_url, f'workspaces/{namespace}/{name}/storageCostEstimate'), headers=headers).json()
-                estimate = r['estimate']
-                out.write(f'{namespace}\t{name}\t{estimate}\n')
+                r = fapi.__SESSION.get(
+                    urljoin(root_url, f"workspaces/{namespace}/{name}/storageCostEstimate"),
+                    headers=headers,
+                ).json()
+                estimate = r["estimate"]
+                out.write(f"{namespace}\t{name}\t{estimate}\n")
```

### Comparing `altocumulus-2.1.2/alto/commands/upload.py` & `altocumulus-2.3.0/alto/commands/upload.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,85 @@
 import os
 import argparse
 
-from alto.utils import upload_to_cloud_bucket, parse_workspace, get_workspace_info, read_wdl_inputs
-
+from alto.utils import get_workspace_info, parse_workspace, read_wdl_inputs, upload_to_cloud_bucket
 
 
 def main(argv):
-    parser = argparse.ArgumentParser(description='Upload files/directories to a Cloud (gcp or aws) bucket.')
+    parser = argparse.ArgumentParser(
+        description="Upload files/directories to a Cloud (gcp or aws) bucket."
+    )
 
     group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument('-b', '--bucket', dest='bucket', action='store',
-                        help='Cloud bucket url including scheme (e.g. gs://my_bucket). If bucket starts with gs, backend is gcp; otherwise, bucket should start with s3 and backend is aws.')
-    group.add_argument('-w', '--workspace', dest='workspace', action='store', help='Terra workspace name (e.g. foo/bar).')
-
-    parser.add_argument('--bucket-folder', metavar='<folder>', dest='bucket_folder', action='store',
-                        help='Store inputs to <folder> under workspace''s bucket')
-    parser.add_argument('--dry-run', dest='dry_run', action='store_true',
-                        help='Causes upload to run in "dry run" mode, i.e., just outputting what would be uploaded without actually doing any uploading.')
-    parser.add_argument('-o', dest='out_json', action='store', metavar='<updated_json>', help='Output updated input JSON file to <updated_json>')
-    parser.add_argument('--profile', dest='profile', action='store', help='AWS profile. Only works if dealing with AWS S3 buckets, and if not set, use the default profile.')
-    parser.add_argument(dest='input', help='Input JSONs or files (e.g. sample sheet).', nargs='+')
-
+    group.add_argument(
+        "-b",
+        "--bucket",
+        dest="bucket",
+        action="store",
+        help="Cloud bucket url including scheme (e.g. gs://my_bucket). If bucket starts with gs, backend is gcp; otherwise, bucket should start with s3 and backend is aws.",
+    )
+    group.add_argument(
+        "-w",
+        "--workspace",
+        dest="workspace",
+        action="store",
+        help="Terra workspace name (e.g. foo/bar).",
+    )
+
+    parser.add_argument(
+        "--bucket-folder",
+        metavar="<folder>",
+        dest="bucket_folder",
+        action="store",
+        help="Store inputs to <folder> under workspace" "s bucket",
+    )
+    parser.add_argument(
+        "--dry-run",
+        dest="dry_run",
+        action="store_true",
+        help='Causes upload to run in "dry run" mode, i.e., just outputting what would be uploaded without actually doing any uploading.',
+    )
+    parser.add_argument(
+        "-o",
+        dest="out_json",
+        action="store",
+        metavar="<updated_json>",
+        help="Output updated input JSON file to <updated_json>",
+    )
+    parser.add_argument(
+        "--profile",
+        dest="profile",
+        action="store",
+        help="AWS profile. Only works if dealing with AWS S3 buckets, and if not set, use the default profile.",
+    )
+    parser.add_argument(dest="input", help="Input JSONs or files (e.g. sample sheet).", nargs="+")
 
     args = parser.parse_args(argv)
 
     if args.bucket is not None:
-        if args.bucket.startswith('gs://'):
-            backend = 'gcp'
-        elif args.bucket.startswith('s3://'):
-            backend = 'aws'
+        if args.bucket.startswith("gs://"):
+            backend = "gcp"
+        elif args.bucket.startswith("s3://"):
+            backend = "aws"
         else:
-            raise ValueError(f'Unable to recognize the backend from bucket {args.bucket}!')
+            raise ValueError(f"Unable to recognize the backend from bucket {args.bucket}!")
         bucket = args.bucket[5:]
     else:
-        backend = 'gcp'
+        backend = "gcp"
         workspace_namespace, workspace_name = parse_workspace(args.workspace)
         workspace_def = get_workspace_info(workspace_namespace, workspace_name)
-        bucket = workspace_def['bucketName']
+        bucket = workspace_def["bucketName"]
 
     inputs = {}
     for path in args.input:
-        if not os.path.exists(path) or path.endswith('.json'):
+        if not os.path.exists(path) or path.endswith(".json"):
             inputs.update(read_wdl_inputs(path))
         else:
             import uuid
+
             inputs.update({str(uuid.uuid1()): path})
 
     upload_to_cloud_bucket(
         inputs=inputs,
         backend=backend,
         bucket=bucket,
         bucket_folder=args.bucket_folder,
```

### Comparing `altocumulus-2.1.2/alto/utils/__init__.py` & `altocumulus-2.3.0/alto/utils/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import subprocess
 from typing import List
 
 
 prefix_float = "_&@&_"
 
+
 def run_command(
     command: List[str],
     dry_run: bool,
     suppress_stdout: bool = False,
     suppress_stderr: bool = False,
 ) -> None:
-    """ Print command and execute it (if dry_run == False).
-    """
+    """Print command and execute it (if dry_run == False)."""
     cur_stdout = subprocess.DEVNULL if suppress_stdout else None
     cur_stderr = subprocess.DEVNULL if suppress_stderr else None
 
     if not suppress_stdout:
-        print(' '.join(command))
+        print(" ".join(command))
 
     if not dry_run:
         subprocess.check_call(command, stdout=cur_stdout, stderr=cur_stderr)
 
-from .io_utils import read_wdl_inputs, upload_to_cloud_bucket
-from .dockstore_utils import parse_dockstore_workflow, get_dockstore_workflow
-from .firecloud_utils import parse_firecloud_workflow, get_firecloud_workflow, parse_workspace, get_workspace_info, update_workflow_config_in_workspace, submit_a_job_to_terra
+
+from .dockstore_utils import get_dockstore_workflow, parse_dockstore_workflow  # noqa: F401, E402
+from .firecloud_utils import (  # noqa: F401, E402
+    get_firecloud_workflow,
+    get_workspace_info,
+    parse_firecloud_workflow,
+    parse_workspace,
+    submit_a_job_to_terra,
+    update_workflow_config_in_workspace,
+)
+from .io_utils import read_wdl_inputs, upload_to_cloud_bucket  # noqa: F401, E402
```

### Comparing `altocumulus-2.1.2/alto/utils/bcl_utils.py` & `altocumulus-2.3.0/alto/utils/bcl_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 import os
 from typing import List, Optional
+
 from alto.utils import run_command
 
+
 class lane_manager:
     def __init__(self):
         self.lanes = set()
         self.isall = False
 
     def update_lanes(self, lane_str: str):
-        if lane_str == '*':
+        if lane_str == "*":
             self.isall = True
             self.lanes.clear()
         else:
-            fields = lane_str.split('-')
+            fields = lane_str.split("-")
             assert len(fields) <= 2
             if len(fields) == 1:
                 self.lanes.add(int(lane_str))
             else:
                 for i in range(int(fields[0]), int(fields[1]) + 1):
                     self.lanes.add(i)
 
     def get_lanes(self) -> List[str]:
         if self.isall or len(self.lanes) == 0:
-            return ['*']
+            return ["*"]
         res = []
         for lane in list(self.lanes):
-            res.append(f'L{lane:03}')
+            res.append(f"L{lane:03}")
         return res
 
 
 def path_is_bcl(path: str) -> bool:
-    """If path represents BCL files of one sequencing flowcell.
-    """
-    return os.path.exists(f'{path}/RunInfo.xml')
+    """If path represents BCL files of one sequencing flowcell."""
+    return os.path.exists(f"{path}/RunInfo.xml")
 
 
 def transfer_flowcell(
     source: str,
     dest: str,
-    backend: str,
     lanes: List[str],
     dry_run: bool,
     profile: Optional[str] = None,
     verbose: bool = True,
 ) -> None:
-    """Transfer one flowcell (with selected lanes) to cloud
+    """Transfer one flowcell (with selected lanes) to cloud.
 
     Parameters
     ----------
     source: `str`
         Local path to the flowcell directory.
     dest: `str`
         Cloud address to copy the flowcell to. For example, it should be something like 'gs://my_bucket/flowecell' for copying to Google bucket.
-    backend: `str`
-        Cloud backend, choosing from 'gcp' and 'aws'.
     lanes: `List[str]`
         A list of lanes to copy to cloud.
     dry_run: `bool`
         If dry run, only print commands but do not execute.
     profile: `str`, optional, default: `None`
         If not None, use this profile for AWS backend.
     verbose: `bool`, optional, default: `True`
@@ -67,59 +65,112 @@
     -------
     None
 
     Examples
     --------
     >>> transfer_flowcell('flowcell', 'gs://my_bucket/flowcell', 'gcp', ['*'], False)
     """
-    strato_cmd = ['strato', 'cp', '--backend', backend, '--ionice', '--quiet', f'{source}/RunInfo.xml', f'{dest}/RunInfo.xml']
+    strato_cmd = [
+        "strato",
+        "cp",
+        "--ionice",
+        "--quiet",
+        f"{source}/RunInfo.xml",
+        f"{dest}/RunInfo.xml",
+    ]
     if profile is not None:
-        strato_cmd.extend(['--profile', profile])
+        strato_cmd.extend(["--profile", profile])
     run_command(strato_cmd, dry_run, suppress_stdout=not verbose)
 
-    if not os.path.exists(f'{source}/RTAComplete.txt'):
-        raise FileNotFoundError("Cannot find RTAComplete.txt. Please check if sequencing is completed!")
-    strato_cmd = ['strato', 'cp', '--backend', backend, '--ionice', '--quiet', f'{source}/RTAComplete.txt', f'{dest}/RTAComplete.txt']
+    if not os.path.exists(f"{source}/RTAComplete.txt"):
+        raise FileNotFoundError(
+            "Cannot find RTAComplete.txt. Please check if sequencing is completed!"
+        )
+    strato_cmd = [
+        "strato",
+        "cp",
+        "--ionice",
+        "--quiet",
+        f"{source}/RTAComplete.txt",
+        f"{dest}/RTAComplete.txt",
+    ]
     if profile is not None:
-        strato_cmd.extend(['--profile', profile])
+        strato_cmd.extend(["--profile", profile])
     run_command(strato_cmd, dry_run, suppress_stdout=not verbose)
 
-    if os.path.exists(f'{source}/runParameters.xml'):
-        strato_cmd = ['strato', 'cp', '--backend', backend, '--ionice', '--quiet', f'{source}/runParameters.xml', f'{dest}/runParameters.xml']
-    elif os.path.exists(f'{source}/RunParameters.xml'):
-        strato_cmd = ['strato', 'cp', '--backend', backend, '--ionice', '--quiet', f'{source}/RunParameters.xml', f'{dest}/RunParameters.xml']
+    if os.path.exists(f"{source}/runParameters.xml"):
+        strato_cmd = [
+            "strato",
+            "cp",
+            "--ionice",
+            "--quiet",
+            f"{source}/runParameters.xml",
+            f"{dest}/runParameters.xml",
+        ]
+    elif os.path.exists(f"{source}/RunParameters.xml"):
+        strato_cmd = [
+            "strato",
+            "cp",
+            "--ionice",
+            "--quiet",
+            f"{source}/RunParameters.xml",
+            f"{dest}/RunParameters.xml",
+        ]
     else:
         raise FileNotFoundError("Cannot find either runParameters.xml or RunParameters.xml!")
     if profile is not None:
-        strato_cmd.extend(['--profile', profile])
+        strato_cmd.extend(["--profile", profile])
     run_command(strato_cmd, dry_run, suppress_stdout=not verbose)
 
-    basecall_string = '{0}/Data/Intensities/BaseCalls'
-    if len(lanes) == 1 and lanes[0] == '*':
+    basecall_string = "{0}/Data/Intensities/BaseCalls"
+    if len(lanes) == 1 and lanes[0] == "*":
         # find all lanes
         lanes = []
-        with os.scandir(path = basecall_string.format(source)) as dirobj:
+        with os.scandir(path=basecall_string.format(source)) as dirobj:
             for entry in dirobj:
-                if entry.is_dir() and entry.name.startswith('L0'):
+                if entry.is_dir() and entry.name.startswith("L0"):
                     lanes.append(entry.name)
     # copy bcl files
     for lane in lanes:
-        lane_string = basecall_string + '/{1}'
-        strato_cmd = ['strato', 'sync', '--backend', backend, '--ionice', '-m', '--quiet', lane_string.format(source, lane), lane_string.format(dest, lane)]
+        lane_string = basecall_string + "/{1}"
+        strato_cmd = [
+            "strato",
+            "sync",
+            "--ionice",
+            "-m",
+            "--quiet",
+            lane_string.format(source, lane),
+            lane_string.format(dest, lane),
+        ]
         if profile is not None:
-            strato_cmd.extend(['--profile', profile])
+            strato_cmd.extend(["--profile", profile])
         run_command(strato_cmd, dry_run, suppress_stdout=not verbose)
 
     # copy locs files
-    locs_string = '{0}/Data/Intensities/s.locs'
+    locs_string = "{0}/Data/Intensities/s.locs"
     if os.path.exists(locs_string.format(source)):
-        strato_cmd = ['strato', 'cp', '--backend', backend, '--ionice', '--quiet', locs_string.format(source), locs_string.format(dest)]
+        strato_cmd = [
+            "strato",
+            "cp",
+            "--ionice",
+            "--quiet",
+            locs_string.format(source),
+            locs_string.format(dest),
+        ]
         if profile is not None:
-            strato_cmd.extend(['--profile', profile])
+            strato_cmd.extend(["--profile", profile])
         run_command(strato_cmd, dry_run, suppress_stdout=not verbose)
     else:
-        locs_string = '{0}/Data/Intensities/{1}'
+        locs_string = "{0}/Data/Intensities/{1}"
         for lane in lanes:
-            strato_cmd = ['strato', 'sync', '--backend', backend, '--ionice', '-m', '--quiet', locs_string.format(source, lane), locs_string.format(dest, lane)]
+            strato_cmd = [
+                "strato",
+                "sync",
+                "--ionice",
+                "-m",
+                "--quiet",
+                locs_string.format(source, lane),
+                locs_string.format(dest, lane),
+            ]
             if profile is not None:
-                strato_cmd.extend(['--profile', profile])
+                strato_cmd.extend(["--profile", profile])
             run_command(strato_cmd, dry_run, suppress_stdout=not verbose)
```

### Comparing `altocumulus-2.1.2/alto/utils/dockstore_utils.py` & `altocumulus-2.3.0/alto/utils/dockstore_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
-import requests
-from urllib.parse import urljoin
 from typing import Tuple
+from urllib.parse import urljoin
 
+import requests
 
-dockstore_api = "https://dockstore.org/api/"
 
+dockstore_api = "https://dockstore.org/api/"
 
 
 def parse_dockstore_workflow(workflow_string: str) -> Tuple[str, str, str, str]:
     """Split a Dockstore workflow string.
 
     Parameters
     ----------
@@ -21,17 +21,19 @@
     `tuple` object.
         A tuple containing organization, collection, workflow and version strings.
 
     Examples
     --------
     >>> organization, collection, workflow, version = parse_dockstore_workflow('broadinstitute:cumulus:cumulus:1.5.0')
     """
-    fields = workflow_string.split(':')
+    fields = workflow_string.split(":")
     if len(fields) < 3 or len(fields) > 4:
-        raise ValueError(f"workflow_string should contain only 3 or 4 items. But {workflow_string} contains {len(fields)} items!")
+        raise ValueError(
+            f"workflow_string should contain only 3 or 4 items. But {workflow_string} contains {len(fields)} items!"
+        )
 
     organization = fields[0]
     collection = fields[1]
     workflow = fields[2]
     version = fields[3] if len(fields) == 4 else None
 
     return organization, collection, workflow, version
@@ -40,15 +42,16 @@
 def get_dockstore_workflow(
     organization: str,
     collection: str,
     workflow: str,
     version: str = None,
     ssl_verify: bool = True,
 ) -> dict:
-    """Locate a workflow using the organization, collection and workflow hierachy and return results in a dictionary.
+    """Locate a workflow using the organization, collection and workflow hierachy and return results
+    in a dictionary.
 
     Parameters
     ----------
     organization: `str`
         The organization that workflow belongs to. You can find this string by clicking an organization in Dockstore and extract the basename in the URL. For example, this is the URL for Broad Institute 'https://dockstore.org/organizations/BroadInstitute' and you can infer Broad Institute's organization name is 'BroadInstitute'. This parameter is case-insensitive.
     collection: `str`
         The collection that the workflow belongs to. Similarly you can find the collection name using URL (e.g. 'https://dockstore.org/organizations/BroadInstitute/collections/Cumulus' suggests 'Cumulus' is the collection name). The collection must be under the organization and is case-insensitive.
@@ -71,37 +74,46 @@
             'methodPath': Method path that can be recognized by the Terra platform.
             'methodUri': Uniform Resource Identifier that can be recognized by the Terra platform.
 
     Examples
     --------
     >>> results = get_dockstore_workflow('broadinstitute', 'cumulus', 'cumulus')
     """
-    org = requests.get(urljoin(dockstore_api, f"organizations/name/{organization}"), verify=ssl_verify)
+    org = requests.get(
+        urljoin(dockstore_api, f"organizations/name/{organization}"), verify=ssl_verify
+    )
     if org.status_code != 200:
         raise ValueError(f"Unable to locate organization {organization} - {org.content.decode()}!")
-    coll = requests.get(urljoin(dockstore_api, f"organizations/{organization}/collections/{collection}/name"), verify=ssl_verify)
+    coll = requests.get(
+        urljoin(dockstore_api, f"organizations/{organization}/collections/{collection}/name"),
+        verify=ssl_verify,
+    )
     if coll.status_code != 200:
         raise ValueError(f"Unable to locate collection {collection} - {coll.content.decode()}!")
 
-    workflow_l = workflow.lower() # convert to lowercase
+    workflow_l = workflow.lower()  # convert to lowercase
     find_workflow = False
     for entry in coll.json()["entries"]:
         workflow_name = os.path.basename(entry["entryPath"]).lower()
         if workflow_l == workflow_name:
             find_workflow = True
             break
 
     if not find_workflow:
         raise ValueError(f"Unable to locate workflow {workflow} from collection {collection}!")
 
     workflow_id = entry["id"]
 
-    workflow_entry = requests.get(urljoin(dockstore_api, f"workflows/published/{workflow_id}"), verify=ssl_verify)
+    workflow_entry = requests.get(
+        urljoin(dockstore_api, f"workflows/published/{workflow_id}"), verify=ssl_verify
+    )
     if workflow_entry.status_code != 200:
-        raise ValueError(f"Unable to fetch information for workflow {workflow} - {workflow_entry.content.decode()}!")
+        raise ValueError(
+            f"Unable to fetch information for workflow {workflow} - {workflow_entry.content.decode()}!"
+        )
 
     workflow_content = workflow_entry.json()
 
     if version is None:
         version = workflow_content["defaultVersion"]
         print(f"Workflow version is not specified. Using default version {version} instead.")
 
@@ -117,24 +129,24 @@
 
     if version_item["hidden"]:
         raise ValueError(f"Version {version} of workflow {workflow} is hidden. Unable to use it!")
 
     version = version_item["name"]
     workflow_path = version_item["workflow_path"]
 
-    table = str.maketrans({'/': '%2F'})
+    table = str.maketrans({"/": "%2F"})
     methodPath = workflow_content["full_workflow_path"].translate(table)
 
     # Get rid of "github.com" prefix.
-    repo_path = '/'.join(workflow_content["path"].split('/')[1:])
+    repo_path = "/".join(workflow_content["path"].split("/")[1:])
 
     results = {
         "name": workflow_content["workflowName"],
         "path": workflow_content["path"],
         "version": version,
         "workflow_path": workflow_path,
         "url": f"https://raw.githubusercontent.com/{repo_path}/{version}{workflow_path}",
         "methodPath": methodPath,
-        "methodUri": f"dockstore://{methodPath}/{version}"
+        "methodUri": f"dockstore://{methodPath}/{version}",
     }
 
     return results
```

### Comparing `altocumulus-2.1.2/alto/utils/firecloud_utils.py` & `altocumulus-2.3.0/alto/utils/firecloud_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-import os
-import json
 import warnings
 from typing import Tuple
 
 from firecloud import api as fapi
 
-warnings.filterwarnings('ignore', 'Your application has authenticated', UserWarning, 'google')
 
+warnings.filterwarnings("ignore", "Your application has authenticated", UserWarning, "google")
 
 
 def parse_firecloud_workflow(workflow_string: str) -> Tuple[str, str, int]:
     """Split a Firecloud workflow string.
 
     Parameters
     ----------
@@ -22,27 +20,32 @@
     `tuple` object.
         A tuple containing namespace, name and version strings.
 
     Examples
     --------
     >>> method_namespace, method_name, method_version = parse_firecloud_workflow('cumulus/cumulus/43')
     """
-    fields = workflow_string.split('/')
+    fields = workflow_string.split("/")
     if len(fields) < 2 or len(fields) > 3:
-        raise ValueError(f"workflow_string should contain only 2 or 3 items. But {workflow_string} contains {len(fields)} items!")
+        raise ValueError(
+            f"workflow_string should contain only 2 or 3 items. But {workflow_string} contains {len(fields)} items!"
+        )
 
     namespace = fields[0]
     name = fields[1]
     version = int(fields[2]) if len(fields) == 3 else None
 
     return namespace, name, version
 
 
-def get_firecloud_workflow(method_namespace: str, method_name: str, method_version: int = None) -> dict:
-    """Locate a workflow using the method_namespace, method_name and method_version hierachy and return results in a dictionary.
+def get_firecloud_workflow(
+    method_namespace: str, method_name: str, method_version: int = None
+) -> dict:
+    """Locate a workflow using the method_namespace, method_name and method_version hierachy and
+    return results in a dictionary.
 
     Parameters
     ----------
     method_namespace: `str`
         The namespace that workflow belongs to (case-sensitive).
     method_name: `str`
         The workflow name (case-sensitive).
@@ -64,15 +67,17 @@
     >>> results = get_firecloud_workflow('cumulus', 'cumulus')
     """
     method_record = None
 
     if method_version is not None:
         method_def = fapi.get_repository_method(method_namespace, method_name, method_version)
         if method_def.status_code != 200:
-            raise ValueError(f"Unable to fetch workflow {method_namespace}/{method_name}/{method_version} - {method_def.json()}!")
+            raise ValueError(
+                f"Unable to fetch workflow {method_namespace}/{method_name}/{method_version} - {method_def.json()}!"
+            )
         method_record = method_def.json()
     else:
         list_methods = fapi.list_repository_methods(namespace=method_namespace, name=method_name)
         if list_methods.status_code != 200:
             raise ValueError(f"Unable to list methods - {list_methods.json()}!")
         methods = list_methods.json()
         if len(methods) == 0:
@@ -84,55 +89,84 @@
                 method_record = method
 
     results = {
         "namespace": method_record["namespace"],
         "name": method_record["name"],
         "snapshotId": method_record["snapshotId"],
         "url": f"https://api.firecloud.org/ga4gh/v1/tools/{method_record['namespace']}:{method_record['name']}/versions/{method_record['snapshotId']}/plain-WDL/descriptor",
-        "methodUri": f"agora://{method_record['namespace']}/{method_record['name']}/{method_record['snapshotId']}"
+        "methodUri": f"agora://{method_record['namespace']}/{method_record['name']}/{method_record['snapshotId']}",
     }
 
     return results
 
 
 def parse_workspace(workspace: str) -> Tuple[str, str]:
-    """Parse a workspace string
-    """
-    fields = workspace.split('/')
+    """Parse a workspace string."""
+    fields = workspace.split("/")
     if len(fields) != 2:
         raise ValueError(f"workspace {workspace} is not in the right format!")
     return fields[0], fields[1]
 
 
 def get_workspace_info(workspace_namespace: str, workspace_name: str) -> dict:
-    """Get workspace attributes using workspace_namespace and workspace_name.
-    """
+    """Get workspace attributes using workspace_namespace and workspace_name."""
     ws = fapi.get_workspace(workspace_namespace, workspace_name)
     if ws.status_code == 404:
-        raise ValueError(f"Unable to fetch information from workspace {workspace_namespace}/{workspace_name} - {ws.json()}!")
+        raise ValueError(
+            f"Unable to fetch information from workspace {workspace_namespace}/{workspace_name} - {ws.json()}!"
+        )
     return ws.json()["workspace"]
 
 
-def update_workflow_config_in_workspace(config_namespace: str, config_name: str, method_body: dict, workspace_namespace: str, workspace_name: str):
-    """Update workflow configuration in the given workspace. If config does not exist, create one.
-    """
-    config_exists = fapi.get_workspace_config(workspace_namespace, workspace_name, config_namespace, config_name)
+def update_workflow_config_in_workspace(
+    config_namespace: str,
+    config_name: str,
+    method_body: dict,
+    workspace_namespace: str,
+    workspace_name: str,
+):
+    """Update workflow configuration in the given workspace.
+
+    If config does not exist, create one.
+    """
+    config_exists = fapi.get_workspace_config(
+        workspace_namespace, workspace_name, config_namespace, config_name
+    )
     if config_exists.status_code == 200:
-        config_submission = fapi.update_workspace_config(workspace_namespace, workspace_name, config_namespace, config_name, method_body)
+        config_submission = fapi.update_workspace_config(
+            workspace_namespace, workspace_name, config_namespace, config_name, method_body
+        )
         if config_submission.status_code != 200:
-            raise ValueError(f"Unable to update workflow config {config_namespace}/{config_name} in the workspace {workspace_namespace}/{workspace_name}. Response: {config_submission.status_code} - {config_submission.json()}!")
+            raise ValueError(
+                f"Unable to update workflow config {config_namespace}/{config_name} in the workspace {workspace_namespace}/{workspace_name}. Response: {config_submission.status_code} - {config_submission.json()}!"
+            )
     else:
-        config_submission = fapi.create_workspace_config(workspace_namespace, workspace_name, method_body)
+        config_submission = fapi.create_workspace_config(
+            workspace_namespace, workspace_name, method_body
+        )
         if config_submission.status_code != 201:
-            raise ValueError(f"Unable to create workflow config {config_namespace}/{config_name} in the workspace {workspace_namespace}/{workspace_name}. Response: {config_submission.status_code} - {config_submission.json()}!")
-
-
-def submit_a_job_to_terra(workspace_namespace: str, workspace_name: str, config_namespace: str, config_name: str, use_callcache: bool = True) -> str:
-    """Create a job submission to Terra and if success, return a URL for checking job status.
-    """
-    launch_submission = fapi.create_submission(workspace_namespace, workspace_name, config_namespace, config_name, use_callcache = use_callcache)
+            raise ValueError(
+                f"Unable to create workflow config {config_namespace}/{config_name} in the workspace {workspace_namespace}/{workspace_name}. Response: {config_submission.status_code} - {config_submission.json()}!"
+            )
+
+
+def submit_a_job_to_terra(
+    workspace_namespace: str,
+    workspace_name: str,
+    config_namespace: str,
+    config_name: str,
+    use_callcache: bool = True,
+) -> str:
+    """Create a job submission to Terra and if success, return a URL for checking job status."""
+    launch_submission = fapi.create_submission(
+        workspace_namespace,
+        workspace_name,
+        config_namespace,
+        config_name,
+        use_callcache=use_callcache,
+    )
     if launch_submission.status_code != 201:
         raise ValueError(f"Unable to launch submission - {launch_submission.json()}!")
 
     submission_id = launch_submission.json()["submissionId"]
     status_url = f"https://app.terra.bio/#workspaces/{workspace_namespace}/{workspace_name}/job_history/{submission_id}"
     return status_url
```

### Comparing `altocumulus-2.1.2/alto/utils/io_utils.py` & `altocumulus-2.3.0/alto/utils/io_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,45 @@
-import os, re, json, tempfile
+import os
+import re
+import json
+import tempfile
+from collections import namedtuple
+from typing import Dict, Optional, Tuple
+from urllib.parse import urlparse
+
 import numpy as np
 import pandas as pd
-from collections import namedtuple
-from typing import Dict, Tuple, Optional
 
 from alto.utils import prefix_float, run_command
+
 from .bcl_utils import lane_manager, path_is_bcl, transfer_flowcell
-from .fastq_utils import sample_manager, path_is_fastq, transfer_fastq
+from .fastq_utils import path_is_fastq, sample_manager, transfer_fastq
+
+
+FlowcellType = namedtuple("FlowcellType", ["type", "manager"])
+
+import_pattern = '^import "(.+)"'
 
 
-FlowcellType = namedtuple('FlowcellType', ['type', 'manager'])
+def _get_scheme(path):
+    scheme = urlparse(path).scheme
+    return (
+        "file" if len(scheme) <= 1 else scheme
+    )  # for file paths: /foo/bar/test.h5ad or C:/foo/bar/test.h5ad
+
+
+def get_workflow_imports(path):
+    workflow_imports = []
+    with open(path, "rt") as f:
+        for line in f:
+            line = line.strip()
+            result = re.match(import_pattern, line)
+            if result:
+                workflow_imports.append(result.group(1))
+    return workflow_imports
 
 
 def read_wdl_inputs(input_json: str) -> dict:
     """Load inputs from either a JSON file or a JSON string.
 
     Parameters
     ----------
@@ -31,217 +57,237 @@
     """
     float_parser = lambda x: prefix_float + x
 
     assert isinstance(input_json, str)
 
     wdl_inputs = None
     if os.path.exists(input_json):
-        with open(input_json, 'r') as f:
+        with open(input_json, "r") as f:
             wdl_inputs = json.loads(f.read(), parse_float=float_parser)
     else:
         wdl_inputs = json.loads(input_json, parse_float=float_parser)
 
     return wdl_inputs
 
 
-class cloud_url_factory: # class to make sure all cloud urls are unique
-    def __init__(self, backend, bucket): # here bucket should also include bucket folder information
-        assert backend in {'gcp', 'aws'}
-        self.scheme = 'gs' if backend == 'gcp' else 's3'
+class cloud_url_factory:  # class to make sure all cloud urls are unique
+    def __init__(
+        self, backend, bucket
+    ):  # here bucket should also include bucket folder information
+        assert backend in {"gcp", "aws"}
+        self.scheme = "gs" if backend == "gcp" else "s3"
         self.bucket = bucket
         self.unique_urls = set()
 
     def get_unique_url(self, input_path: str):
         counter = 1
-        uniq_url = f'{self.scheme}://{self.bucket}/{os.path.basename(input_path)}'
+        uniq_url = f"{self.scheme}://{self.bucket}/{os.path.basename(input_path)}"
         root, ext = os.path.splitext(uniq_url)
         while uniq_url in self.unique_urls:
             counter += 1
-            uniq_url = f'{root}_{counter}{ext}'
+            uniq_url = f"{root}_{counter}{ext}"
         self.unique_urls.add(uniq_url)
 
         return uniq_url
 
 
 def transfer_data(
     source: str,
     dest: str,
-    backend: str,
     dry_run: bool,
     flowcells: Dict[str, FlowcellType] = None,
     profile: Optional[str] = None,
     verbose: bool = True,
 ) -> None:
     """Transfer source to dest (cloud destination).
-       backend, choosing from gcp and aws.
-       flowcells is a global flowcell manangement object.
+
+    backend, choosing from gcp and aws. flowcells is a global flowcell manangement object.
     """
     if verbose:
         print(f'{"Dry run: " if dry_run else ""}Uploading {source} to {dest}.')
 
-    if flowcells != None and source in flowcells:
+    if flowcells is not None and source in flowcells:
         flowcell = flowcells[source]
-        if flowcell.type == 'bcl':
+        if flowcell.type == "bcl":
             transfer_flowcell(
                 source=source,
                 dest=dest,
-                backend=backend,
                 lanes=flowcell.manager.get_lanes(),
                 dry_run=dry_run,
                 profile=profile,
                 verbose=verbose,
             )
         else:
-            assert flowcell.type == 'fastq'
+            assert flowcell.type == "fastq"
             transfer_fastq(
                 source=source,
                 dest=dest,
-                backend=backend,
-                samples=flowcell.manager.get_samples(),
+                sample_map=flowcell.manager.get_sample_map(),
                 dry_run=dry_run,
                 profile=profile,
                 verbose=verbose,
             )
     else:
         if os.path.isdir(source):
-            strato_cmd = ['strato', 'sync', '--backend', backend, '--ionice', '-m', '--quiet', source, dest]
+            strato_cmd = [
+                "strato",
+                "sync",
+                "--ionice",
+                "-m",
+                "--quiet",
+                source,
+                dest,
+            ]
         else:
-            strato_cmd = ['strato', 'cp', '--backend', backend, '--ionice', '--quiet', source, dest]
+            strato_cmd = ["strato", "cp", "--ionice", "--quiet", source, dest]
 
         if profile is not None:
             strato_cmd.extend(["--profile", profile])
         run_command(strato_cmd, dry_run, suppress_stdout=not verbose)
 
 
 def transfer_sample_sheet(
     input_file: str,
-    backend: str,
+    input_ext: str,
     input_file_to_output_url: dict,
     url_gen: cloud_url_factory,
     dry_run: bool,
     profile: Optional[str] = None,
+    nrows: Optional[int] = 10005,
     verbose: bool = True,
 ) -> Tuple[str, bool]:
     """Check sample sheet and upload files inside it.
-       input_file: sample sheet
-       backend: choosing from 'gcp' and 'aws'
-       input_file_to_output_url: global dictionary maps local files to cloud urls
-       url_gen: cloud url factory to make sure no duplicated cloud urls
-       dry_run: if dry run
-       verbose: if print info
-       profile: if not None, use for AWS backend.
+    input_file: sample sheet
+    input_ext: input file extension, either '.xlsx', '.tsv', or '.csv'
+    input_file_to_output_url: global dictionary maps local files to cloud urls
+    url_gen: cloud url factory to make sure no duplicated cloud urls
+    dry_run: if dry run
+    profile: if not None, use for AWS backend
+    nrows: load at most nrows, if loaded rows == nrows, skip; default: 10005
+    verbose: if print info
 
-       Returns: path to updated input file (if changed) and if sample sheet is changed
+    Returns: path to updated input file (if changed) and if sample sheet is changed
     """
     is_changed = False
 
     # Terminate if no access to sample sheet.
     if not os.access(input_file, os.R_OK):
         raise PermissionError(f"Need read access to '{input_file}'!")
 
-    # If cannot process, upload its original content.
-    try:
-        df = pd.read_csv(input_file, sep=None, engine='python', header=None, index_col=False)
-    except Exception:
-        return input_file, is_changed
+    if input_ext == ".csv":
+        df = pd.read_csv(input_file, sep=",", header=None, index_col=False, nrows=nrows)
+    elif input_ext == ".tsv":
+        df = pd.read_csv(input_file, sep="\t", header=None, index_col=False, nrows=nrows)
+    else:
+        assert input_ext == ".xlsx"
+        df = pd.read_excel(input_file, header=None, index_col=False, nrows=nrows)
+
+    if df.shape[0] >= nrows:
+        return (
+            input_file,
+            is_changed,
+        )  # if can load nrows, the file is too large to be a sample sheet
+
+    df = df.applymap(lambda s: s.strip() if isinstance(s, str) else s)  # only strip for strings
 
     flowcells = {}
-    col_names = np.char.array(df.iloc[0,:], unicode = True).lower()
+    col_names = np.char.array(df.iloc[0, :], unicode=True).lower()
 
     # Upload BCL folder or FASTQ files if needed.
-    if ('flowcell' in col_names) or ('location' in col_names):
-        flowcell_keyword = 'flowcell' if 'flowcell' in col_names else 'location'
+    if ("flowcell" in col_names) or ("location" in col_names):
+        flowcell_keyword = "flowcell" if "flowcell" in col_names else "location"
         df.columns = col_names
 
         sample_keyword = None
-        if 'library' in col_names:
-            sample_keyword = 'library'
-        elif 'sample' in col_names:
-            sample_keyword = 'sample'
+        if "library" in col_names:
+            sample_keyword = "library"
+        elif "sample" in col_names:
+            sample_keyword = "sample"
         else:
             raise ValueError("Cannot detect either Library or Sample column in the sample sheet!")
 
         for _, row in df[1:].iterrows():
             if isinstance(row[flowcell_keyword], str):
-                path = row[flowcell_keyword].strip()
+                path = row[flowcell_keyword]
 
                 if path.startswith("gs://") or path.startswith("s3://"):
                     continue
 
                 path = os.path.abspath(path)
                 if not os.path.exists(path):
                     raise ValueError(f"{path} does not exist!")
                 if not os.path.isdir(path):
-                    raise ValueError(f"{path} is not a folder!")
-                if not os.access(path, os.X_OK):
+                    break  # For file type Location values
+                elif not os.access(path, os.X_OK):
                     raise PermissionError(f"Need execution access to folder '{path}'!")
             else:
                 raise ValueError(f"{row[flowcell_keyword]} is not in string type!")
 
             flowcell = None
             if path in flowcells:
                 flowcell = flowcells[path]
             else:
                 if path_is_bcl(path):
-                    flowcell = FlowcellType(type='bcl', manager=lane_manager())
+                    flowcell = FlowcellType(type="bcl", manager=lane_manager())
                 elif path_is_fastq(path):
-                    flowcell = FlowcellType(type='fastq', manager=sample_manager())
+                    flowcell = FlowcellType(type="fastq", manager=sample_manager())
                 else:
                     raise ValueError(f"{path} is neither a BCL folder nor a FASTQ folder!")
                 flowcells[path] = flowcell
 
-            if flowcell.type == 'bcl':
-                flowcell.manager.update_lanes(row['lane'] if 'lane' in row else '*')
+            if flowcell.type == "bcl":
+                flowcell.manager.update_lanes(row["lane"] if "lane" in row else "*")
             else:
-                flowcell.manager.update_samples(row[sample_keyword])
+                flowcell.manager.update_sample_map(row[sample_keyword])
 
-    for _, row in df[1:].iterrows():
-        for idxc, value in row.iteritems():
+    for idxr, row in df[1:].iterrows() if input_ext != ".tsv" else df.iterrows():
+        for idxc, value in row.items():
             if isinstance(value, str) and os.path.exists(value):
                 source = os.path.abspath(value)
                 sub_url = input_file_to_output_url.get(source, None)
 
                 if sub_url is None:
                     sub_url = url_gen.get_unique_url(source)
                     transfer_data(
                         source=source,
                         dest=sub_url,
-                        backend=backend,
                         dry_run=dry_run,
                         flowcells=flowcells,
                         profile=profile,
                         verbose=verbose,
                     )
                     input_file_to_output_url[source] = sub_url
 
-                row[idxc] = sub_url
+                df.loc[idxr, idxc] = sub_url
                 is_changed = True
 
     if is_changed:
         orig_file = input_file
         input_file = tempfile.mkstemp()[1]
         if verbose:
-            print(f'Rewriting file {orig_file} to {input_file}.')
-        out_sep = ',' if orig_file.endswith('.csv') else '\t'
+            print(f"Rewriting file {orig_file} to {input_file}.")
+        out_sep = "," if orig_file.endswith(".csv") else "\t"
         df.to_csv(input_file, sep=out_sep, index=False, header=False)
 
     return input_file, is_changed
 
 
-search_inside_file_whitelist = set(['.txt', '.xlsx', '.tsv', '.csv'])
+search_inside_file_whitelist = set([".xlsx", ".tsv", ".csv"])
+
 
 def upload_to_cloud_bucket(
     inputs: Dict[str, str],
     backend: str,
     bucket: str,
     bucket_folder: str,
     out_json: str,
     dry_run: bool,
-    verbose: bool = True,
     profile: Optional[str] = None,
+    nrows: Optional[int] = 10005,
+    verbose: bool = True,
 ) -> None:
     """Check and upload local files to the cloud bucket.
 
     Parameters
     ----------
     inputs: `Dict[str, str]`
         WDL inputs loaded from a JSON file.
@@ -251,18 +297,20 @@
         Cloud bucket name. Note scheme should not be included (e.g. gs:// or s3://).
     bucket_folder: `str`
         Path under the bucket for where the uploaded file should be stored.
     out_json: `str`
         Path for the JSON file storing updated inputs.
     dry_run: `bool`
         If dry run, only print commands but do not execute.
-    verbose: `bool`, default: ``True``
-        If print out the underlying upload commands on screen.
     profile: `str`, default: ``None``
         For AWS backend only, it's used for specifying a non-default AWS profile.
+    nrows: `int`, default: 10005
+        For scanning sample sheets, if file has >= nrows lines, skip.
+    verbose: `bool`, default: ``True``
+        If print out the underlying upload commands on screen.
 
     Returns
     -------
     None
 
     Examples
     --------
@@ -274,45 +322,46 @@
     url_gen = cloud_url_factory(backend, bucket)
     input_file_to_output_url = {}
 
     for k, v in inputs.items():
         input_path = v
         if isinstance(input_path, str) and os.path.exists(input_path):
             input_path = os.path.abspath(input_path)
-            if input_path in input_file_to_output_url: # if this file has been processed, skip
+            if input_path in input_file_to_output_url:  # if this file has been processed, skip
+                inputs[k] = input_file_to_output_url[input_path]
                 continue
 
             input_url = url_gen.get_unique_url(input_path)
             input_file_to_output_url[input_path] = input_url
 
             is_changed = False
             input_path_extension = os.path.splitext(input_path)[1].lower()
 
             if input_path_extension in search_inside_file_whitelist:
                 # look inside input file to see if there are file paths within
                 input_path, is_changed = transfer_sample_sheet(
                     input_file=input_path,
-                    backend=backend,
+                    input_ext=input_path_extension,
                     input_file_to_output_url=input_file_to_output_url,
                     url_gen=url_gen,
                     dry_run=dry_run,
-                    verbose=verbose,
                     profile=profile,
+                    nrows=nrows,
+                    verbose=verbose,
                 )
 
             transfer_data(
                 source=input_path,
                 dest=input_url,
-                backend=backend,
                 dry_run=dry_run,
-                verbose=verbose,
                 profile=profile,
+                verbose=verbose,
             )
 
             inputs[k] = input_url
-            if is_changed: # delete temporary file after uploading
+            if is_changed:  # delete temporary file after uploading
                 os.remove(input_path)
 
     if out_json is not None:
-        with open(out_json, 'w') as fout:
+        with open(out_json, "w") as fout:
             res_str = json.dumps(inputs, indent=4)
-            fout.write(re.sub(f'"{prefix_float}(.+)"', r'\1', res_str))
+            fout.write(re.sub(f'"{prefix_float}(.+)"', r"\1", res_str))
```

### Comparing `altocumulus-2.1.2/docs/Makefile` & `altocumulus-2.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `altocumulus-2.1.2/docs/conf.py` & `altocumulus-2.3.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
 
 # -- Path setup --------------------------------------------------------------
 
+import sys
+
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 from pathlib import Path
-import sys
+
 
 HERE = Path(__file__).parent
 sys.path.insert(0, str(HERE.parent))
 
 
 # -- Project information -----------------------------------------------------
 
 project = "Altocumulus"
 copyright = "2021 - 2022 Genentech, Inc. and the Broad Institute, Inc. All rights reserved."
-author = (
-    "Bo Li, Yiming Yang, Rimte Rocher"
-)
+author = "Bo Li, Yiming Yang, Rimte Rocher"
 
 # The short X.Y version
-version = "2.1"
+version = "2.2"
 # The full version, including alpha/beta/rc tags
-release = "2.1.2"
+release = "2.2.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
-needs_sphinx = '1.7'
+needs_sphinx = "1.7"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
@@ -54,18 +54,15 @@
     "sphinx.ext.viewcode",
     "sphinx.ext.githubpages",
     "sphinx.ext.autosummary",
     "sphinx.ext.napoleon",
     "sphinx_autodoc_typehints",
 ]
 
-autodoc_default_options = {
-    "members": True,
-    "member-order": "bysource"
-}
+autodoc_default_options = {"members": True, "member-order": "bysource"}
 autosummary_generate = True
 todo_include_todos = False
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
@@ -89,16 +86,16 @@
 # This pattern also affects html_static_path and html_extra_path .
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 intersphinx_mapping = dict(
-    numpy=('https://docs.scipy.org/doc/numpy/', None),
-    pandas=('http://pandas.pydata.org/pandas-docs/stable/', None),
+    numpy=("https://docs.scipy.org/doc/numpy/", None),
+    pandas=("http://pandas.pydata.org/pandas-docs/stable/", None),
 )
 
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
```

### Comparing `altocumulus-2.1.2/docs/release_notes.rst` & `altocumulus-2.3.0/docs/release_notes.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,21 @@
 .. role:: small
 
+Version 2.3.0 :small:`June 21, 2023`
+----------------------------------------
+
+* Add ``cromwell get_task_status`` command to get a summary JSON file on the status of all WDL tasks of a job.
+
+Version 2.2.0 :small:`November 4, 2022`
+----------------------------------------
+
+* In ``cromwell run`` command, automatically create zip file on dependency WDLs for a local WDL workflow.
+* Remove ``query`` command.
+* Bug fix.
+
 Version 2.1.2 :small:`August 15, 2022`
 --------------------------------------
 
 * Bug fix on BCL folder and FASTQ file uploading. [PR `#30 <https://github.com/lilab-bcb/altocumulus/pull/30>`_]
 * In ``cromwell list_jobs`` command, assign informative names for jobs with ``nan`` workflow name. [PR `#31 <https://github.com/lilab-bcb/altocumulus/pull/31>`_ and `#32 <https://github.com/lilab-bcb/altocumulus/pull/32>`_]
 
 Version 2.1.1 :small:`August 12,2022`
```

### Comparing `altocumulus-2.1.2/docs/usage.rst` & `altocumulus-2.3.0/docs/usage.rst`

 * *Files 3% similar despite different names*

```diff
@@ -322,14 +322,48 @@
     A local file named ``<job-id>.metadata.json`` will be created with the job's metadata info in JSON format, where *<job-id>* is the job's ID specified.
 
 * Examples::
 
     alto cromwell get_metadata -s my-server.com --id 710ec6d3-882c-469c-8092-a0b9d5f8dd90
 
 
+``alto cromwell get_task_status``
+--------------------------------------------------------------------------------------------------------------------------------
+
+Get status of all WDL tasks of a job.
+
+Type::
+
+    alto cromwell get_task_status -h
+
+to see the usage information::
+
+    Usage:
+        alto cromwell get_task_status [-h] -s SERVER [-p PORT] --id JOB_ID
+
+* Options:
+
+    -s SERVER, -\-server SERVER
+        Server hostname or IP address.
+    -p PORT, -\-port PORT
+        Port number for Cromwell service. The default port is ``8000``.
+    -\-id JOB_ID
+        Workflow ID returned in **alto cromwell run** command.
+    -h, -\-help
+        Show this help message and exit
+
+* Outputs:
+
+    A local file named ``<job-id>.task_status.json`` will be created with the job's task status info in JSON format, where *<job-id>* is the job's ID specified.
+
+* Examples::
+
+    alto cromwell get_task_status -s my-server.com --id 710ec6d3-882c-469c-8092-a0b9d5f8dd90
+
+
 ``alto cromwell get_logs``
 --------------------------------------------------------------------------------------------------------------------------------
 
 Get the logs for a submitted job.
 
 Type::
 
@@ -447,37 +481,14 @@
     \-o <updated_json>
         Output updated input JSON file to <updated_json>
     -\-profile PROFILE
         AWS profile. Only works if dealing with AWS, and if not set, use the default profile.
     -h, -\-help
         Show this help message and exit
 
-LIMS Query
-============
-
-``alto query``
--------------------
-
-Query project metadata from a LIMS (Laboratory Information Management System) via RESTful APIs.
-
-Given one project ID, this subcommand tries to fetch and display a vareity of metadata from the project. This subcommand also provides an option to write the metadata into a CSV file if the query type is "ngs".
-
-Using this subcommand requires ``lims_query`` Python package installed. Users who want to use this subcommand need to write their own lims_query package, which should at least contain one function::
-
-    query_ngs(project_id: str) -> pandas.DataFrame
-
-* Arguments:
-
-    -\-type {ngs,project}
-        Specify query type. Choose from "ngs" for FASTQ info or "project" for project metadata.
-    \-o CSV_FILE
-        Write metadata information to a CSV file ``CSV_FILE``.
-    -h, -\-help
-        Show this help message and exit.
-
 Logs
 =====
 
 ``alto parse_monitoring_log``
 --------------------------------------------------------------------------------------------------------------------------------
 
 Output maximum CPU, memory, and disk from monitoring log file
```

