# Comparing `tmp/nics-0.8.0.tar.gz` & `tmp/nics-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-4u127gpc/nics-0.8.0.tar", last modified: Thu Jun 22 10:54:22 2023, max compression
+gzip compressed data, was "/home/runner/work/now-i-can-sleep/now-i-can-sleep/dist/.tmp-bepw_mzg/nics-0.9.0.tar", last modified: Thu Jun 22 10:58:26 2023, max compression
```

## Comparing `nics-0.8.0.tar` & `nics-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:22.000000 nics-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-22 10:53:55.000000 nics-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 10:54:22.000000 nics-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 10:53:55.000000 nics-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:22.000000 nics-0.8.0/nics/
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-22 10:53:55.000000 nics-0.8.0/nics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 10:53:55.000000 nics-0.8.0/nics/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:22.000000 nics-0.8.0/nics/compile/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-22 10:53:55.000000 nics-0.8.0/nics/compile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:22.000000 nics-0.8.0/nics/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 10:53:55.000000 nics-0.8.0/nics/wizard/step1.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 10:53:55.000000 nics-0.8.0/nics/wizard/step2.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 10:53:55.000000 nics-0.8.0/nics/wizard/step3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:54:22.000000 nics-0.8.0/nics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 10:54:22.000000 nics-0.8.0/nics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 10:54:22.000000 nics-0.8.0/nics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:54:22.000000 nics-0.8.0/nics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 10:54:22.000000 nics-0.8.0/nics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 10:54:22.000000 nics-0.8.0/nics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 10:54:22.000000 nics-0.8.0/nics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-22 10:53:55.000000 nics-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 10:54:22.000000 nics-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-22 10:53:55.000000 nics-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:58:26.000000 nics-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-22 10:58:01.000000 nics-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 10:58:26.000000 nics-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 10:58:01.000000 nics-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:58:26.000000 nics-0.9.0/nics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-22 10:58:01.000000 nics-0.9.0/nics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-22 10:58:01.000000 nics-0.9.0/nics/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:58:26.000000 nics-0.9.0/nics/compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-22 10:58:01.000000 nics-0.9.0/nics/compile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:58:26.000000 nics-0.9.0/nics/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 10:58:01.000000 nics-0.9.0/nics/wizard/step1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 10:58:01.000000 nics-0.9.0/nics/wizard/step2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-22 10:58:01.000000 nics-0.9.0/nics/wizard/step3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 10:58:26.000000 nics-0.9.0/nics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-22 10:58:26.000000 nics-0.9.0/nics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-22 10:58:26.000000 nics-0.9.0/nics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 10:58:26.000000 nics-0.9.0/nics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 10:58:26.000000 nics-0.9.0/nics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-22 10:58:26.000000 nics-0.9.0/nics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-22 10:58:26.000000 nics-0.9.0/nics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-22 10:58:01.000000 nics-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 10:58:26.000000 nics-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-22 10:58:01.000000 nics-0.9.0/setup.py
```

### Comparing `nics-0.8.0/LICENSE` & `nics-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nics-0.8.0/PKG-INFO` & `nics-0.9.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 0.8.0
+Version: 0.9.0
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-0.8.0/nics/__init__.py` & `nics-0.9.0/nics/__init__.py`

 * *Files identical despite different names*

### Comparing `nics-0.8.0/nics/compile/__init__.py` & `nics-0.9.0/nics/compile/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     printer(f'DEBUG: os.path.isdir(container): {os.path.isdir(container)}.')
     printer(f'DEBUG: os.path.isdir(target): {os.path.isdir(target)}.')
 
     printer(f'DEBUG: os.listdir(container): {os.listdir(container)}.')
     printer(f'DEBUG: os.listdir(target): {os.listdir(target)}.')
 
     settings = KeyCrate(
-        os.path.join(container, '_nics', 'settings.txt'),
+        os.path.join(container, 'settings.txt'),
         key_is_var=True, eval_value=True
     )
     
     printer(f'DEBUG: settings.export(): {settings.export()}')
 
     header = header_writer(container)
```

### Comparing `nics-0.8.0/nics.egg-info/PKG-INFO` & `nics-0.9.0/nics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nics
-Version: 0.8.0
+Version: 0.9.0
 Summary: Automated docs repo generator
 Home-page: https://nvfp.github.io/now-i-can-sleep
 Author: Nicholas Valentinus
 Author-email: nvfastplease@gmail.com
 License: MIT
 Project-URL: documentation, https://nvfp.github.io/now-i-can-sleep/docs
 Project-URL: report bugs, https://github.com/nvfp/now-i-can-sleep/issues
```

### Comparing `nics-0.8.0/pyproject.toml` & `nics-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "nics"
-version = "0.8.0"
+version = "0.9.0"
 description = "Automated docs repo generator"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
 authors = [
   	{email = "nvfastplease@gmail.com"},
 ]
```

