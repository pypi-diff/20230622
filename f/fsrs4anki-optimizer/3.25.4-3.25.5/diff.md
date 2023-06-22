# Comparing `tmp/fsrs4anki_optimizer-3.25.4.tar.gz` & `tmp/fsrs4anki_optimizer-3.25.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsrs4anki_optimizer-3.25.4.tar", last modified: Thu Jun 22 06:42:16 2023, max compression
+gzip compressed data, was "fsrs4anki_optimizer-3.25.5.tar", last modified: Thu Jun 22 07:08:36 2023, max compression
```

## Comparing `fsrs4anki_optimizer-3.25.4.tar` & `fsrs4anki_optimizer-3.25.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44545 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 06:42:16.000000 fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 06:42:16.381275 fsrs4anki_optimizer-3.25.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 06:42:06.000000 fsrs4anki_optimizer-3.25.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44545 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/fsrs4anki_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 07:08:36.000000 fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 07:08:36.642032 fsrs4anki_optimizer-3.25.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 07:08:27.000000 fsrs4anki_optimizer-3.25.5/setup.py
```

### Comparing `fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/__main__.py` & `fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/__main__.py`

 * *Files identical despite different names*

### Comparing `fsrs4anki_optimizer-3.25.4/fsrs4anki_optimizer/fsrs4anki_optimizer.py` & `fsrs4anki_optimizer-3.25.5/fsrs4anki_optimizer/fsrs4anki_optimizer.py`

 * *Files identical despite different names*

