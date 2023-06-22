# Comparing `tmp/robot_rumble-0.0.3.tar.gz` & `tmp/robot_rumble-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot_rumble-0.0.3.tar", last modified: Thu Jun 22 05:12:41 2023, max compression
+gzip compressed data, was "robot_rumble-0.0.4.tar", last modified: Thu Jun 22 05:16:36 2023, max compression
```

## Comparing `robot_rumble-0.0.3.tar` & `robot_rumble-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 05:12:41.681155 robot_rumble-0.0.3/
--rw-rw-rw-   0        0        0       34 2023-06-22 04:47:36.000000 robot_rumble-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      366 2023-06-22 05:12:41.681155 robot_rumble-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       89 2023-06-22 04:47:36.000000 robot_rumble-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 05:12:41.670039 robot_rumble-0.0.3/Robot_Rumble.egg-info/
--rw-rw-rw-   0        0        0      366 2023-06-22 05:12:41.000000 robot_rumble-0.0.3/Robot_Rumble.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-06-22 05:12:41.000000 robot_rumble-0.0.3/Robot_Rumble.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 05:12:41.000000 robot_rumble-0.0.3/Robot_Rumble.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-22 05:12:41.000000 robot_rumble-0.0.3/Robot_Rumble.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-06-22 05:12:41.000000 robot_rumble-0.0.3/Robot_Rumble.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-22 05:12:41.000000 robot_rumble-0.0.3/Robot_Rumble.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-06-22 04:47:36.000000 robot_rumble-0.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-22 05:12:41.676515 robot_rumble-0.0.3/robot_rumble/
--rw-rw-rw-   0        0        0        0 2023-06-22 04:47:36.000000 robot_rumble-0.0.3/robot_rumble/__init__.py
--rw-rw-rw-   0        0        0     7264 2023-06-22 05:10:11.000000 robot_rumble-0.0.3/robot_rumble/main.py
--rw-rw-rw-   0        0        0       42 2023-06-22 05:12:41.681155 robot_rumble-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      685 2023-06-22 05:10:35.000000 robot_rumble-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 05:16:36.353623 robot_rumble-0.0.4/
+-rw-rw-rw-   0        0        0       29 2023-06-22 05:15:01.000000 robot_rumble-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      366 2023-06-22 05:16:36.348673 robot_rumble-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       89 2023-06-22 04:47:36.000000 robot_rumble-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 05:16:36.309927 robot_rumble-0.0.4/Robot_Rumble.egg-info/
+-rw-rw-rw-   0        0        0      366 2023-06-22 05:16:36.000000 robot_rumble-0.0.4/Robot_Rumble.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2023-06-22 05:16:36.000000 robot_rumble-0.0.4/Robot_Rumble.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 05:16:36.000000 robot_rumble-0.0.4/Robot_Rumble.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-22 05:16:36.000000 robot_rumble-0.0.4/Robot_Rumble.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-06-22 05:16:36.000000 robot_rumble-0.0.4/Robot_Rumble.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-22 05:16:36.000000 robot_rumble-0.0.4/Robot_Rumble.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-06-22 04:47:36.000000 robot_rumble-0.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-22 05:16:36.318608 robot_rumble-0.0.4/robot_rumble/
+-rw-rw-rw-   0        0        0        0 2023-06-22 04:47:36.000000 robot_rumble-0.0.4/robot_rumble/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 05:16:36.345158 robot_rumble-0.0.4/robot_rumble/assets/
+-rw-rw-rw-   0        0        0     8196 2023-06-22 05:01:00.000000 robot_rumble-0.0.4/robot_rumble/assets/.DS_Store
+-rw-rw-rw-   0        0        0      260 2023-06-22 05:01:00.000000 robot_rumble-0.0.4/robot_rumble/assets/Platforms.tsx
+-rw-rw-rw-   0        0        0    13037 2023-06-22 05:01:00.000000 robot_rumble-0.0.4/robot_rumble/assets/Prototype.json
+-rw-rw-rw-   0        0        0    13070 2023-06-22 05:01:00.000000 robot_rumble-0.0.4/robot_rumble/assets/Robot_idle.png
+-rw-rw-rw-   0        0        0    43769 2023-06-22 05:01:00.000000 robot_rumble-0.0.4/robot_rumble/assets/Robot_run.png
+-rw-rw-rw-   0        0        0      555 2023-06-22 05:01:00.000000 robot_rumble-0.0.4/robot_rumble/assets/table.png
+-rw-rw-rw-   0        0        0     7264 2023-06-22 05:10:11.000000 robot_rumble-0.0.4/robot_rumble/main.py
+-rw-rw-rw-   0        0        0       42 2023-06-22 05:16:36.353623 robot_rumble-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-06-22 05:16:32.000000 robot_rumble-0.0.4/setup.py
```

### Comparing `robot_rumble-0.0.3/Robot_Rumble.egg-info/SOURCES.txt` & `robot_rumble-0.0.4/Robot_Rumble.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -11,8 +11,14 @@
 robot_rumble/__init__.py
 robot_rumble/main.py
 robot_rumble.egg-info/PKG-INFO
 robot_rumble.egg-info/SOURCES.txt
 robot_rumble.egg-info/dependency_links.txt
 robot_rumble.egg-info/entry_points.txt
 robot_rumble.egg-info/requires.txt
-robot_rumble.egg-info/top_level.txt
+robot_rumble.egg-info/top_level.txt
+robot_rumble/assets/.DS_Store
+robot_rumble/assets/Platforms.tsx
+robot_rumble/assets/Prototype.json
+robot_rumble/assets/Robot_idle.png
+robot_rumble/assets/Robot_run.png
+robot_rumble/assets/table.png
```

### Comparing `robot_rumble-0.0.3/robot_rumble/main.py` & `robot_rumble-0.0.4/robot_rumble/main.py`

 * *Files identical despite different names*

### Comparing `robot_rumble-0.0.3/setup.py` & `robot_rumble-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='robot_rumble',
-    version='0.0.3',
+    version='0.0.4',
     packages=["robot_rumble"],
     url='https://github.com/guptat07/Robot-Rumble',
     license='',
     author='Tony Gupta, Anthony Liao, Maya Singh, Kaylee Conrad',
     author_email='kaymconrad@gmail.com',
     description='2D Side-Scroller Game for UF CEN4930 Performant Programming (in Japan!)',
     readme = "README.md",
```

