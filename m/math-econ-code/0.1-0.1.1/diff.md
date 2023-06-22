# Comparing `tmp/math_econ_code-0.1.tar.gz` & `tmp/math_econ_code-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "math_econ_code-0.1.tar", last modified: Thu Jun 22 08:39:35 2023, max compression
+gzip compressed data, was "math_econ_code-0.1.1.tar", last modified: Thu Jun 22 08:46:22 2023, max compression
```

## Comparing `math_econ_code-0.1.tar` & `math_econ_code-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 08:39:35.194639 math_econ_code-0.1/
--rw-rw-rw-   0        0        0    35813 2023-06-22 08:32:08.000000 math_econ_code-0.1/LICENSE
--rw-rw-rw-   0        0        0      230 2023-06-22 08:39:35.194639 math_econ_code-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 08:39:35.193081 math_econ_code-0.1/math_econ_code.egg-info/
--rw-rw-rw-   0        0        0      230 2023-06-22 08:39:34.000000 math_econ_code-0.1/math_econ_code.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      180 2023-06-22 08:39:34.000000 math_econ_code-0.1/math_econ_code.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 08:39:34.000000 math_econ_code-0.1/math_econ_code.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 08:39:34.000000 math_econ_code-0.1/math_econ_code.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7879 2023-06-22 08:36:41.000000 math_econ_code-0.1/pymec_lp.py
--rw-rw-rw-   0        0        0       42 2023-06-22 08:39:35.195593 math_econ_code-0.1/setup.cfg
--rw-rw-rw-   0        0        0      353 2023-06-22 08:38:36.000000 math_econ_code-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 08:46:22.793063 math_econ_code-0.1.1/
+-rw-rw-rw-   0        0        0    35813 2023-06-22 08:32:08.000000 math_econ_code-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      232 2023-06-22 08:46:22.792062 math_econ_code-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 08:46:22.791063 math_econ_code-0.1.1/math_econ_code.egg-info/
+-rw-rw-rw-   0        0        0      232 2023-06-22 08:46:21.000000 math_econ_code-0.1.1/math_econ_code.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-22 08:46:22.000000 math_econ_code-0.1.1/math_econ_code.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 08:46:21.000000 math_econ_code-0.1.1/math_econ_code.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-22 08:46:22.000000 math_econ_code-0.1.1/math_econ_code.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7879 2023-06-22 08:36:41.000000 math_econ_code-0.1.1/meclp.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 08:46:22.793063 math_econ_code-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      352 2023-06-22 08:45:59.000000 math_econ_code-0.1.1/setup.py
```

### Comparing `math_econ_code-0.1/LICENSE` & `math_econ_code-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `math_econ_code-0.1/pymec_lp.py` & `math_econ_code-0.1.1/meclp.py`

 * *Files identical despite different names*

