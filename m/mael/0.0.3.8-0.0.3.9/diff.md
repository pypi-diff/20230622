# Comparing `tmp/mael-0.0.3.8.tar.gz` & `tmp/mael-0.0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mael-0.0.3.8.tar", last modified: Fri Mar 17 11:10:52 2023, max compression
+gzip compressed data, was "mael-0.0.3.9.tar", last modified: Fri Mar 17 11:13:46 2023, max compression
```

## Comparing `mael-0.0.3.8.tar` & `mael-0.0.3.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:10:52.313217 mael-0.0.3.8/
--rw-r--r--   0 otsukakenji   (501) staff       (20)     3876 2023-03-17 09:42:01.000000 mael-0.0.3.8/LICENSE
--rw-r--r--   0 otsukakenji   (501) staff       (20)       59 2023-03-17 10:33:09.000000 mael-0.0.3.8/MANIFEST.in
--rw-r--r--   0 otsukakenji   (501) staff       (20)      295 2023-03-17 11:10:52.313055 mael-0.0.3.8/PKG-INFO
--rw-r--r--   0 otsukakenji   (501) staff       (20)       56 2023-03-17 10:16:58.000000 mael-0.0.3.8/README.rst
-drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:10:52.308859 mael-0.0.3.8/mael/
--rw-r--r--   0 otsukakenji   (501) staff       (20)        0 2023-03-17 10:30:03.000000 mael-0.0.3.8/mael/__init__.py
--rw-r--r--   0 otsukakenji   (501) staff       (20)     3326 2023-03-17 02:42:21.000000 mael-0.0.3.8/mael/column_config.py
--rw-r--r--   0 otsukakenji   (501) staff       (20)     9497 2023-03-17 02:46:38.000000 mael-0.0.3.8/mael/excel_builder.py
--rw-r--r--   0 otsukakenji   (501) staff       (20)     1499 2023-03-16 22:26:20.000000 mael-0.0.3.8/mael/initializer.py
--rw-r--r--   0 otsukakenji   (501) staff       (20)     1475 2023-03-17 02:39:34.000000 mael-0.0.3.8/mael/main.py
-drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:10:52.306503 mael-0.0.3.8/mael/templates/
-drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:10:52.310526 mael-0.0.3.8/mael/templates/normal/
--rw-r--r--   0 otsukakenji   (501) staff       (20)       23 2023-03-17 02:40:39.000000 mael-0.0.3.8/mael/templates/normal/README.md
--rw-r--r--   0 otsukakenji   (501) staff       (20)      444 2023-03-17 02:23:47.000000 mael-0.0.3.8/mael/templates/normal/Sample 1.md
--rw-r--r--   0 otsukakenji   (501) staff       (20)      444 2023-03-17 02:23:47.000000 mael-0.0.3.8/mael/templates/normal/Sample 2.md
-drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:10:52.311201 mael-0.0.3.8/mael/templates/normal/config/
--rw-r--r--   0 otsukakenji   (501) staff       (20)        0 2023-03-16 21:28:24.000000 mael-0.0.3.8/mael/templates/normal/config/columns.yml
--rw-r--r--   0 otsukakenji   (501) staff       (20)       10 2023-03-17 02:40:39.000000 mael-0.0.3.8/mael/templates/normal/config/ignore.txt
--rw-r--r--   0 otsukakenji   (501) staff       (20)      160 2023-03-16 21:30:20.000000 mael-0.0.3.8/mael/templates/normal/config/variables.ini
-drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:10:52.311954 mael-0.0.3.8/mael/templates/test_case/
--rw-r--r--   0 otsukakenji   (501) staff       (20)       23 2023-03-17 02:40:39.000000 mael-0.0.3.8/mael/templates/test_case/README.md
--rw-r--r--   0 otsukakenji   (501) staff       (20)      449 2023-03-17 02:23:47.000000 mael-0.0.3.8/mael/templates/test_case/Scenario 1.md
--rw-r--r--   0 otsukakenji   (501) staff       (20)      449 2023-03-16 22:36:30.000000 mael-0.0.3.8/mael/templates/test_case/Scenario 2.md
-drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:10:52.312759 mael-0.0.3.8/mael/templates/test_case/config/
--rw-r--r--   0 otsukakenji   (501) staff       (20)      738 2023-03-16 22:02:31.000000 mael-0.0.3.8/mael/templates/test_case/config/columns.yml
--rw-r--r--   0 otsukakenji   (501) staff       (20)       10 2023-03-17 02:40:39.000000 mael-0.0.3.8/mael/templates/test_case/config/ignore.txt
--rw-r--r--   0 otsukakenji   (501) staff       (20)      160 2023-03-16 21:30:20.000000 mael-0.0.3.8/mael/templates/test_case/config/variables.ini
-drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:10:52.309753 mael-0.0.3.8/mael.egg-info/
--rw-r--r--   0 otsukakenji   (501) staff       (20)      295 2023-03-17 11:10:52.000000 mael-0.0.3.8/mael.egg-info/PKG-INFO
--rw-r--r--   0 otsukakenji   (501) staff       (20)      773 2023-03-17 11:10:52.000000 mael-0.0.3.8/mael.egg-info/SOURCES.txt
--rw-r--r--   0 otsukakenji   (501) staff       (20)        1 2023-03-17 11:10:52.000000 mael-0.0.3.8/mael.egg-info/dependency_links.txt
--rw-r--r--   0 otsukakenji   (501) staff       (20)       40 2023-03-17 11:10:52.000000 mael-0.0.3.8/mael.egg-info/entry_points.txt
--rw-r--r--   0 otsukakenji   (501) staff       (20)       16 2023-03-17 11:10:52.000000 mael-0.0.3.8/mael.egg-info/requires.txt
--rw-r--r--   0 otsukakenji   (501) staff       (20)        5 2023-03-17 11:10:52.000000 mael-0.0.3.8/mael.egg-info/top_level.txt
--rw-r--r--   0 otsukakenji   (501) staff       (20)       38 2023-03-17 11:10:52.313357 mael-0.0.3.8/setup.cfg
--rw-r--r--   0 otsukakenji   (501) staff       (20)     1267 2023-03-17 11:10:50.000000 mael-0.0.3.8/setup.py
+drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:13:46.814997 mael-0.0.3.9/
+-rw-r--r--   0 otsukakenji   (501) staff       (20)     3876 2023-03-17 09:42:01.000000 mael-0.0.3.9/LICENSE
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       59 2023-03-17 10:33:09.000000 mael-0.0.3.9/MANIFEST.in
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      295 2023-03-17 11:13:46.814738 mael-0.0.3.9/PKG-INFO
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       56 2023-03-17 10:16:58.000000 mael-0.0.3.9/README.rst
+drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:13:46.809587 mael-0.0.3.9/mael/
+-rw-r--r--   0 otsukakenji   (501) staff       (20)        0 2023-03-17 10:30:03.000000 mael-0.0.3.9/mael/__init__.py
+-rw-r--r--   0 otsukakenji   (501) staff       (20)     3326 2023-03-17 02:42:21.000000 mael-0.0.3.9/mael/column_config.py
+-rw-r--r--   0 otsukakenji   (501) staff       (20)     9497 2023-03-17 02:46:38.000000 mael-0.0.3.9/mael/excel_builder.py
+-rw-r--r--   0 otsukakenji   (501) staff       (20)     1499 2023-03-16 22:26:20.000000 mael-0.0.3.9/mael/initializer.py
+-rw-r--r--   0 otsukakenji   (501) staff       (20)     1475 2023-03-17 02:39:34.000000 mael-0.0.3.9/mael/main.py
+drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:13:46.806705 mael-0.0.3.9/mael/templates/
+drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:13:46.811742 mael-0.0.3.9/mael/templates/normal/
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       23 2023-03-17 02:40:39.000000 mael-0.0.3.9/mael/templates/normal/README.md
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      444 2023-03-17 02:23:47.000000 mael-0.0.3.9/mael/templates/normal/Sample 1.md
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      444 2023-03-17 02:23:47.000000 mael-0.0.3.9/mael/templates/normal/Sample 2.md
+drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:13:46.812528 mael-0.0.3.9/mael/templates/normal/config/
+-rw-r--r--   0 otsukakenji   (501) staff       (20)        0 2023-03-16 21:28:24.000000 mael-0.0.3.9/mael/templates/normal/config/columns.yml
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       10 2023-03-17 02:40:39.000000 mael-0.0.3.9/mael/templates/normal/config/ignore.txt
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      160 2023-03-16 21:30:20.000000 mael-0.0.3.9/mael/templates/normal/config/variables.ini
+drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:13:46.813394 mael-0.0.3.9/mael/templates/test_case/
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       23 2023-03-17 02:40:39.000000 mael-0.0.3.9/mael/templates/test_case/README.md
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      449 2023-03-17 02:23:47.000000 mael-0.0.3.9/mael/templates/test_case/Scenario 1.md
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      449 2023-03-16 22:36:30.000000 mael-0.0.3.9/mael/templates/test_case/Scenario 2.md
+drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:13:46.814412 mael-0.0.3.9/mael/templates/test_case/config/
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      738 2023-03-16 22:02:31.000000 mael-0.0.3.9/mael/templates/test_case/config/columns.yml
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       10 2023-03-17 02:40:39.000000 mael-0.0.3.9/mael/templates/test_case/config/ignore.txt
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      160 2023-03-16 21:30:20.000000 mael-0.0.3.9/mael/templates/test_case/config/variables.ini
+drwxr-xr-x   0 otsukakenji   (501) staff       (20)        0 2023-03-17 11:13:46.810807 mael-0.0.3.9/mael.egg-info/
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      295 2023-03-17 11:13:46.000000 mael-0.0.3.9/mael.egg-info/PKG-INFO
+-rw-r--r--   0 otsukakenji   (501) staff       (20)      773 2023-03-17 11:13:46.000000 mael-0.0.3.9/mael.egg-info/SOURCES.txt
+-rw-r--r--   0 otsukakenji   (501) staff       (20)        1 2023-03-17 11:13:46.000000 mael-0.0.3.9/mael.egg-info/dependency_links.txt
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       40 2023-03-17 11:13:46.000000 mael-0.0.3.9/mael.egg-info/entry_points.txt
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       16 2023-03-17 11:13:46.000000 mael-0.0.3.9/mael.egg-info/requires.txt
+-rw-r--r--   0 otsukakenji   (501) staff       (20)        5 2023-03-17 11:13:46.000000 mael-0.0.3.9/mael.egg-info/top_level.txt
+-rw-r--r--   0 otsukakenji   (501) staff       (20)       38 2023-03-17 11:13:46.815187 mael-0.0.3.9/setup.cfg
+-rw-r--r--   0 otsukakenji   (501) staff       (20)     1275 2023-03-17 11:13:43.000000 mael-0.0.3.9/setup.py
```

### Comparing `mael-0.0.3.8/LICENSE` & `mael-0.0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mael-0.0.3.8/mael/column_config.py` & `mael-0.0.3.9/mael/column_config.py`

 * *Files identical despite different names*

### Comparing `mael-0.0.3.8/mael/excel_builder.py` & `mael-0.0.3.9/mael/excel_builder.py`

 * *Files identical despite different names*

### Comparing `mael-0.0.3.8/mael/initializer.py` & `mael-0.0.3.9/mael/initializer.py`

 * *Files identical despite different names*

### Comparing `mael-0.0.3.8/mael/main.py` & `mael-0.0.3.9/mael/main.py`

 * *Files identical despite different names*

### Comparing `mael-0.0.3.8/mael/templates/test_case/config/columns.yml` & `mael-0.0.3.9/mael/templates/test_case/config/columns.yml`

 * *Files identical despite different names*

### Comparing `mael-0.0.3.8/mael.egg-info/SOURCES.txt` & `mael-0.0.3.9/mael.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mael-0.0.3.8/setup.py` & `mael-0.0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
     long_description = f.read()
 
 setup(
     name='mael',
     packages=find_packages(),
     # package_dir={'': 'mael'},
     # packages=find_packages(where='mael'),
-    version='0.0.3.8',
-    py_modules=['mael.main', 'mael.initializer', 'mael.excel_builder', 'mael.column_config'],
+    version='0.0.3.9',
+    py_modules=['mael', 'mael.main', 'mael.initializer', 'mael.excel_builder', 'mael.column_config'],
     install_requires=[
         'pyyaml',
         'openpyxl'
     ],
     entry_points={
         'console_scripts': ['mael=mael.main:main'],
     },
```

