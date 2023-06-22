# Comparing `tmp/pybox-toolkit-0.1.8.dev5.tar.gz` & `tmp/pybox-toolkit-0.1.9.dev67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybox-toolkit-0.1.8.dev5.tar", last modified: Mon Jun 19 10:05:14 2023, max compression
+gzip compressed data, was "pybox-toolkit-0.1.9.dev67.tar", last modified: Thu Jun 22 08:25:26 2023, max compression
```

## Comparing `pybox-toolkit-0.1.8.dev5.tar` & `pybox-toolkit-0.1.9.dev67.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.877593 pybox-toolkit-0.1.8.dev5/
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-19 10:05:14.877593 pybox-toolkit-0.1.8.dev5/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-19 10:05:14.877593 pybox-toolkit-0.1.8.dev5/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.869593 pybox-toolkit-0.1.8.dev5/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.873593 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/
--rw-r--r--   0 root         (0) root         (0)      479 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-19 10:05:14.000000 pybox-toolkit-0.1.8.dev5/src/pybox_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.873593 pybox-toolkit-0.1.8.dev5/src/toolkit/
--rw-rw-rw-   0 root         (0) root         (0)    15168 2023-06-19 10:04:42.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.873593 pybox-toolkit-0.1.8.dev5/src/toolkit/graphing/
--rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/graphing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.873593 pybox-toolkit-0.1.8.dev5/src/toolkit/test/
--rw-rw-rw-   0 root         (0) root         (0)     5222 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-19 10:05:14.877593 pybox-toolkit-0.1.8.dev5/src/toolkit/typing/
--rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/typing/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      839 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/typing/si.py
--rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-12 14:14:31.000000 pybox-toolkit-0.1.8.dev5/src/toolkit/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      840 2023-06-22 08:25:08.000000 pybox-toolkit-0.1.9.dev67/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       36 2023-05-24 11:41:58.000000 pybox-toolkit-0.1.9.dev67/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.638242 pybox-toolkit-0.1.9.dev67/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      480 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 08:25:26.000000 pybox-toolkit-0.1.9.dev67/src/pybox_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/toolkit/
+-rw-rw-rw-   0 root         (0) root         (0)    15168 2023-06-19 10:02:57.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/toolkit/graphing/
+-rw-rw-rw-   0 root         (0) root         (0)     1724 2023-06-05 18:07:33.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/graphing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/toolkit/test/
+-rw-rw-rw-   0 root         (0) root         (0)     5222 2023-06-19 08:45:59.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 08:25:26.642242 pybox-toolkit-0.1.9.dev67/src/toolkit/typing/
+-rw-rw-rw-   0 root         (0) root         (0)     9875 2023-06-05 19:32:07.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/typing/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      839 2023-05-31 11:15:50.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/typing/si.py
+-rw-rw-rw-   0 root         (0) root         (0)     7802 2023-06-05 17:56:01.000000 pybox-toolkit-0.1.9.dev67/src/toolkit/utils.py
```

### Comparing `pybox-toolkit-0.1.8.dev5/pyproject.toml` & `pybox-toolkit-0.1.9.dev67/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev5/src/toolkit/__init__.py` & `pybox-toolkit-0.1.9.dev67/src/toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev5/src/toolkit/graphing/__init__.py` & `pybox-toolkit-0.1.9.dev67/src/toolkit/graphing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev5/src/toolkit/test/__init__.py` & `pybox-toolkit-0.1.9.dev67/src/toolkit/test/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev5/src/toolkit/typing/__init__.py` & `pybox-toolkit-0.1.9.dev67/src/toolkit/typing/__init__.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev5/src/toolkit/typing/si.py` & `pybox-toolkit-0.1.9.dev67/src/toolkit/typing/si.py`

 * *Files identical despite different names*

### Comparing `pybox-toolkit-0.1.8.dev5/src/toolkit/utils.py` & `pybox-toolkit-0.1.9.dev67/src/toolkit/utils.py`

 * *Files identical despite different names*

