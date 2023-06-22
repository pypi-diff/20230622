# Comparing `tmp/pybox-toolkit-0.1.9.dev67.tar.gz` & `tmp/pybox-toolkit-0.1.9.dev79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.9.dev67.tar", last modified: Thu Jun 22 08:25:26 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.9.dev79.tar", last modified: Thu Jun 22 11:00:47 2023, max compression
```

## Comparing `pybox-toolkit-0.1.9.dev67.tar` & `pybox-toolkit-0.1.9.dev79.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-22 08:25:08.000000 pybox-toolkit-0.1.9.dev67/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 11:41:58.000000 pybox-toolkit-0.1.9.dev67/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.638242 pybox-toolkit-0.1.9.dev67/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15168 2023-06-19 10:02:57.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/graphing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5222 2023-06-19 08:45:59.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-05 19:32:07.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-31 11:15:50.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-05 17:56:01.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-22 08:25:42.000000 pybox-toolkit-0.1.9.dev79/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 11:45:04.000000 pybox-toolkit-0.1.9.dev79/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 11:00:47.000000 pybox-toolkit-0.1.9.dev79/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15168 2023-06-19 10:02:46.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/graphing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2023-06-19 08:29:38.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 11:00:47.104117 pybox-toolkit-0.1.9.dev79/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-12 14:14:27.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-01 16:04:17.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-12 14:14:27.000000 pybox-toolkit-0.1.9.dev79/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.9.dev67/pyproject.toml` & `pybox-toolkit-0.1.9.dev79/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev67/src/toolkit/__init__.py` & `pybox-toolkit-0.1.9.dev79/src/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev67/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.9.dev79/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev67/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.9.dev79/src/toolkit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev67/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.9.dev79/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev67/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.9.dev79/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.9.dev67/src/toolkit/utils.py` & `pybox-toolkit-0.1.9.dev79/src/toolkit/utils.py`

 * *Files identical despite different names*

