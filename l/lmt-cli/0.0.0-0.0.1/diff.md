# Comparing `tmp/lmt-cli-0.0.0.tar.gz` & `tmp/lmt-cli-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmt-cli-0.0.0.tar", last modified: Sun Jun 18 17:24:07 2023, max compression
+gzip compressed data, was "lmt-cli-0.0.1.tar", last modified: Thu Jun 22 16:10:29 2023, max compression
```

## Comparing `lmt-cli-0.0.0.tar` & `lmt-cli-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 17:24:07.267305 lmt-cli-0.0.0/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.0/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      378 2023-06-18 17:24:07.267305 lmt-cli-0.0.0/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      233 2023-06-18 17:13:45.000000 lmt-cli-0.0.0/README.md
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 17:24:07.267305 lmt-cli-0.0.0/lmt_cli.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      378 2023-06-18 17:24:07.000000 lmt-cli-0.0.0/lmt_cli.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      180 2023-06-18 17:24:07.000000 lmt-cli-0.0.0/lmt_cli.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-18 17:24:07.000000 lmt-cli-0.0.0/lmt_cli.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      579 2023-06-18 17:24:07.000000 lmt-cli-0.0.0/lmt_cli.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-18 17:24:07.000000 lmt-cli-0.0.0/lmt_cli.egg-info/top_level.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-18 17:24:07.267305 lmt-cli-0.0.0/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      468 2023-06-18 17:23:49.000000 lmt-cli-0.0.0/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    11357 2023-06-18 17:13:45.000000 lmt-cli-0.0.1/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7802 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7159 2023-06-22 16:04:23.000000 lmt-cli-0.0.1/README.md
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/lmt/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-06-18 20:39:32.000000 lmt-cli-0.0.1/lmt/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    14911 2023-06-22 15:56:19.000000 lmt-cli-0.0.1/lmt/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4826 2023-06-22 13:13:31.000000 lmt-cli-0.0.1/lmt/gpt_integration.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/lmt_cli.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7802 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      264 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       36 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       34 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        4 2023-06-22 16:10:29.000000 lmt-cli-0.0.1/lmt_cli.egg-info/top_level.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-06-22 16:10:29.705788 lmt-cli-0.0.1/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1170 2023-06-22 16:10:02.000000 lmt-cli-0.0.1/setup.py
```

### Comparing `lmt-cli-0.0.0/LICENSE` & `lmt-cli-0.0.1/LICENSE`

 * *Files identical despite different names*

