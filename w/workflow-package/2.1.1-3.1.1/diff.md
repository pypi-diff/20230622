# Comparing `tmp/workflow_package-2.1.1.tar.gz` & `tmp/workflow_package-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workflow_package-2.1.1.tar", last modified: Thu Jun 22 06:23:33 2023, max compression
+gzip compressed data, was "workflow_package-3.1.1.tar", last modified: Thu Jun 22 06:32:48 2023, max compression
```

## Comparing `workflow_package-2.1.1.tar` & `workflow_package-3.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 06:23:33.747482 workflow_package-2.1.1/
--rw-rw-rw-   0        0        0      231 2023-06-22 06:23:33.744658 workflow_package-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-22 06:18:32.000000 workflow_package-2.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 06:23:33.749488 workflow_package-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      259 2023-06-22 06:19:36.000000 workflow_package-2.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:23:33.663537 workflow_package-2.1.1/workflow/
--rw-rw-rw-   0        0        0        0 2023-06-22 06:17:15.000000 workflow_package-2.1.1/workflow/__init__.py
--rw-rw-rw-   0        0        0     7726 2023-06-22 06:05:09.000000 workflow_package-2.1.1/workflow/workflow_details.py
-drwxrwxrwx   0        0        0        0 2023-06-22 06:23:33.738622 workflow_package-2.1.1/workflow_package.egg-info/
--rw-rw-rw-   0        0        0      231 2023-06-22 06:23:33.000000 workflow_package-2.1.1/workflow_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-06-22 06:23:33.000000 workflow_package-2.1.1/workflow_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 06:23:33.000000 workflow_package-2.1.1/workflow_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 06:23:33.000000 workflow_package-2.1.1/workflow_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 06:32:48.584388 workflow_package-3.1.1/
+-rw-rw-rw-   0        0        0      288 2023-06-22 06:32:48.582087 workflow_package-3.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-22 06:18:32.000000 workflow_package-3.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-22 06:32:48.585138 workflow_package-3.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      374 2023-06-22 06:32:23.000000 workflow_package-3.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:32:48.553139 workflow_package-3.1.1/workflow/
+-rw-rw-rw-   0        0        0        0 2023-06-22 06:17:15.000000 workflow_package-3.1.1/workflow/__init__.py
+-rw-rw-rw-   0        0        0      373 2023-06-22 06:31:48.000000 workflow_package-3.1.1/workflow/setup.py
+-rw-rw-rw-   0        0        0     7726 2023-06-22 06:05:09.000000 workflow_package-3.1.1/workflow/workflow_details.py
+drwxrwxrwx   0        0        0        0 2023-06-22 06:32:48.579126 workflow_package-3.1.1/workflow_package.egg-info/
+-rw-rw-rw-   0        0        0      288 2023-06-22 06:32:48.000000 workflow_package-3.1.1/workflow_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-22 06:32:48.000000 workflow_package-3.1.1/workflow_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 06:32:48.000000 workflow_package-3.1.1/workflow_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 06:32:48.000000 workflow_package-3.1.1/workflow_package.egg-info/top_level.txt
```

### Comparing `workflow_package-2.1.1/workflow/workflow_details.py` & `workflow_package-3.1.1/workflow/workflow_details.py`

 * *Files identical despite different names*

