# Comparing `tmp/robot_rumble-0.0.1.tar.gz` & `tmp/robot_rumble-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot_rumble-0.0.1.tar", last modified: Wed Jun 21 07:59:52 2023, max compression
+gzip compressed data, was "robot_rumble-0.0.2.tar", last modified: Thu Jun 22 02:27:26 2023, max compression
```

## Comparing `robot_rumble-0.0.1.tar` & `robot_rumble-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 07:59:52.245689 robot_rumble-0.0.1/
--rw-rw-rw-   0        0        0       21 2023-06-20 11:01:41.000000 robot_rumble-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      366 2023-06-21 07:59:52.245689 robot_rumble-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       89 2023-06-19 03:26:44.000000 robot_rumble-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 07:59:52.235631 robot_rumble-0.0.1/Robot_Rumble.egg-info/
--rw-rw-rw-   0        0        0      366 2023-06-21 07:59:52.000000 robot_rumble-0.0.1/Robot_Rumble.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-06-21 07:59:52.000000 robot_rumble-0.0.1/Robot_Rumble.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 07:59:52.000000 robot_rumble-0.0.1/Robot_Rumble.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-21 07:59:52.000000 robot_rumble-0.0.1/Robot_Rumble.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 07:59:52.000000 robot_rumble-0.0.1/Robot_Rumble.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-21 07:59:52.000000 robot_rumble-0.0.1/Robot_Rumble.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-06-19 11:22:00.000000 robot_rumble-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-21 07:59:52.235631 robot_rumble-0.0.1/robot_rumble/
--rw-rw-rw-   0        0        0        0 2023-06-20 07:01:45.000000 robot_rumble-0.0.1/robot_rumble/__init__.py
--rw-rw-rw-   0        0        0     7004 2023-06-21 07:58:56.000000 robot_rumble-0.0.1/robot_rumble/main.py
--rw-rw-rw-   0        0        0       42 2023-06-21 07:59:52.245689 robot_rumble-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      658 2023-06-21 07:58:56.000000 robot_rumble-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 02:27:26.457485 robot_rumble-0.0.2/
+-rw-rw-rw-   0        0        0       34 2023-06-22 02:26:55.000000 robot_rumble-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      366 2023-06-22 02:27:26.454198 robot_rumble-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2023-06-19 03:26:44.000000 robot_rumble-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 02:27:26.420374 robot_rumble-0.0.2/Robot_Rumble.egg-info/
+-rw-rw-rw-   0        0        0      366 2023-06-22 02:27:26.000000 robot_rumble-0.0.2/Robot_Rumble.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      629 2023-06-22 02:27:26.000000 robot_rumble-0.0.2/Robot_Rumble.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 02:27:26.000000 robot_rumble-0.0.2/Robot_Rumble.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-22 02:27:26.000000 robot_rumble-0.0.2/Robot_Rumble.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-06-22 02:27:26.000000 robot_rumble-0.0.2/Robot_Rumble.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-22 02:27:26.000000 robot_rumble-0.0.2/Robot_Rumble.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-06-19 11:22:00.000000 robot_rumble-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-22 02:27:26.430475 robot_rumble-0.0.2/robot_rumble/
+-rw-rw-rw-   0        0        0        0 2023-06-20 07:01:45.000000 robot_rumble-0.0.2/robot_rumble/__init__.py
+-rw-rw-rw-   0        0        0     7004 2023-06-21 07:58:56.000000 robot_rumble-0.0.2/robot_rumble/main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 02:27:26.450810 robot_rumble-0.0.2/robot_rumble/sprites/
+-rw-rw-rw-   0        0        0    13070 2023-06-19 03:26:44.000000 robot_rumble-0.0.2/robot_rumble/sprites/Robot_idle.png
+-rw-rw-rw-   0        0        0    43769 2023-06-19 03:26:44.000000 robot_rumble-0.0.2/robot_rumble/sprites/Robot_run.png
+-rw-rw-rw-   0        0        0      555 2023-06-19 03:26:44.000000 robot_rumble-0.0.2/robot_rumble/sprites/table.png
+-rw-rw-rw-   0        0        0       42 2023-06-22 02:27:26.457485 robot_rumble-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      658 2023-06-22 02:27:00.000000 robot_rumble-0.0.2/setup.py
```

### Comparing `robot_rumble-0.0.1/Robot_Rumble.egg-info/SOURCES.txt` & `robot_rumble-0.0.2/Robot_Rumble.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,8 +11,11 @@
 robot_rumble/__init__.py
 robot_rumble/main.py
 robot_rumble.egg-info/PKG-INFO
 robot_rumble.egg-info/SOURCES.txt
 robot_rumble.egg-info/dependency_links.txt
 robot_rumble.egg-info/entry_points.txt
 robot_rumble.egg-info/requires.txt
-robot_rumble.egg-info/top_level.txt
+robot_rumble.egg-info/top_level.txt
+robot_rumble/sprites/Robot_idle.png
+robot_rumble/sprites/Robot_run.png
+robot_rumble/sprites/table.png
```

### Comparing `robot_rumble-0.0.1/robot_rumble/main.py` & `robot_rumble-0.0.2/robot_rumble/main.py`

 * *Files identical despite different names*

### Comparing `robot_rumble-0.0.1/setup.py` & `robot_rumble-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='robot_rumble',
-    version='0.0.1',
+    version='0.0.2',
     packages=["robot_rumble"],
     url='https://github.com/guptat07/Robot-Rumble',
     license='',
     author='Tony Gupta, Anthony Liao, Maya Singh, Kaylee Conrad',
     author_email='kaymconrad@gmail.com',
     description='2D Side-Scroller Game for UF CEN4930 Performant Programming (in Japan!)',
     install_requires=['arcade>=2.6.17'],
```

