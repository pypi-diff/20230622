# Comparing `tmp/PyCompGeomAlgorithms-1.0.2.tar.gz` & `tmp/PyCompGeomAlgorithms-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyCompGeomAlgorithms-1.0.2.tar", last modified: Thu Jun 22 19:12:48 2023, max compression
+gzip compressed data, was "PyCompGeomAlgorithms-1.0.3.tar", last modified: Thu Jun 22 19:31:24 2023, max compression
```

## Comparing `PyCompGeomAlgorithms-1.0.2.tar` & `PyCompGeomAlgorithms-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 19:12:48.698697 PyCompGeomAlgorithms-1.0.2/
--rw-rw-rw-   0        0        0     1104 2023-06-22 11:36:14.000000 PyCompGeomAlgorithms-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      568 2023-06-22 19:12:48.699955 PyCompGeomAlgorithms-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 19:12:48.644660 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/
-drwxrwxrwx   0        0        0        0 2023-06-22 19:12:48.696684 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/
--rw-rw-rw-   0        0        0      568 2023-06-22 19:12:48.000000 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-06-22 19:12:48.000000 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 19:12:48.000000 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 19:12:48.000000 PyCompGeomAlgorithms-1.0.2/PyCompGeomAlgorithms/PyCompGeomAlgorithms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2199 2023-06-22 12:13:13.000000 PyCompGeomAlgorithms-1.0.2/README.md
--rw-rw-rw-   0        0        0       88 2023-06-22 19:12:11.000000 PyCompGeomAlgorithms-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      726 2023-06-22 19:12:48.704933 PyCompGeomAlgorithms-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.565957 PyCompGeomAlgorithms-1.0.3/
+-rw-rw-rw-   0        0        0     1104 2023-06-22 11:36:14.000000 PyCompGeomAlgorithms-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      480 2023-06-22 19:31:24.563928 PyCompGeomAlgorithms-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.499572 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:54:06.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/__init__.py
+-rw-rw-rw-   0        0        0    11303 2023-06-22 11:18:29.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/core.py
+-rw-rw-rw-   0        0        0     1707 2023-06-22 10:26:23.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/graham.py
+-rw-rw-rw-   0        0        0      920 2023-06-22 10:15:40.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/jarvis.py
+-rw-rw-rw-   0        0        0     2536 2023-06-22 08:22:43.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/kd_tree.py
+-rw-rw-rw-   0        0        0     2762 2023-06-22 10:31:47.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/preparata.py
+-rw-rw-rw-   0        0        0     2315 2023-06-22 11:31:48.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms/quickhull.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.527246 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/
+-rw-rw-rw-   0        0        0      480 2023-06-22 19:31:24.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      674 2023-06-22 19:31:24.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 19:31:24.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2023-06-22 19:31:24.000000 PyCompGeomAlgorithms-1.0.3/PyCompGeomAlgorithms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2199 2023-06-22 12:13:13.000000 PyCompGeomAlgorithms-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 19:31:24.565957 PyCompGeomAlgorithms-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-06-22 19:26:25.000000 PyCompGeomAlgorithms-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.531329 PyCompGeomAlgorithms-1.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:57:15.000000 PyCompGeomAlgorithms-1.0.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 19:31:24.559852 PyCompGeomAlgorithms-1.0.3/tests/algorithms/
+-rw-rw-rw-   0        0        0        0 2023-06-22 07:57:09.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/__init__.py
+-rw-rw-rw-   0        0        0     1866 2023-06-22 11:34:41.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_entities.py
+-rw-rw-rw-   0        0        0     4056 2023-06-22 10:37:10.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_graham.py
+-rw-rw-rw-   0        0        0      603 2023-06-22 10:37:22.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_jarvis.py
+-rw-rw-rw-   0        0        0     2521 2023-06-22 10:37:32.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_kd_tree.py
+-rw-rw-rw-   0        0        0     3420 2023-06-22 10:37:48.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_preparata.py
+-rw-rw-rw-   0        0        0     3128 2023-06-22 11:31:06.000000 PyCompGeomAlgorithms-1.0.3/tests/algorithms/test_quickhull.py
```

### Comparing `PyCompGeomAlgorithms-1.0.2/LICENSE` & `PyCompGeomAlgorithms-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyCompGeomAlgorithms-1.0.2/README.md` & `PyCompGeomAlgorithms-1.0.3/README.md`

 * *Files identical despite different names*

