# Comparing `tmp/py_madvr-1.4.3.tar.gz` & `tmp/py_madvr-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_madvr-1.4.3.tar", last modified: Mon Jun 19 17:17:45 2023, max compression
+gzip compressed data, was "py_madvr-1.4.4.tar", last modified: Thu Jun 22 03:05:54 2023, max compression
```

## Comparing `py_madvr-1.4.3.tar` & `py_madvr-1.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:45.661504 py_madvr-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-19 17:17:34.000000 py_madvr-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 17:17:45.661504 py_madvr-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-19 17:17:34.000000 py_madvr-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:45.661504 py_madvr-1.4.3/madvr/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-19 17:17:34.000000 py_madvr-1.4.3/madvr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-19 17:17:34.000000 py_madvr-1.4.3/madvr/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-19 17:17:34.000000 py_madvr-1.4.3/madvr/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    16643 2023-06-19 17:17:34.000000 py_madvr-1.4.3/madvr/madvr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:45.661504 py_madvr-1.4.3/py_madvr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-19 17:17:45.000000 py_madvr-1.4.3/py_madvr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-19 17:17:45.000000 py_madvr-1.4.3/py_madvr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 17:17:45.000000 py_madvr-1.4.3/py_madvr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 17:17:45.000000 py_madvr-1.4.3/py_madvr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 17:17:45.661504 py_madvr-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-19 17:17:34.000000 py_madvr-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:45.661504 py_madvr-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 17:17:34.000000 py_madvr-1.4.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-19 17:17:34.000000 py_madvr-1.4.3/tests/testMadVR.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:54.013437 py_madvr-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-22 03:05:39.000000 py_madvr-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-22 03:05:54.013437 py_madvr-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-22 03:05:39.000000 py_madvr-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:54.009437 py_madvr-1.4.4/madvr/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 03:05:39.000000 py_madvr-1.4.4/madvr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-22 03:05:39.000000 py_madvr-1.4.4/madvr/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-22 03:05:39.000000 py_madvr-1.4.4/madvr/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-06-22 03:05:39.000000 py_madvr-1.4.4/madvr/madvr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:54.009437 py_madvr-1.4.4/py_madvr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-22 03:05:53.000000 py_madvr-1.4.4/py_madvr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 03:05:54.000000 py_madvr-1.4.4/py_madvr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 03:05:53.000000 py_madvr-1.4.4/py_madvr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-22 03:05:53.000000 py_madvr-1.4.4/py_madvr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 03:05:54.013437 py_madvr-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-22 03:05:39.000000 py_madvr-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:54.013437 py_madvr-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 03:05:39.000000 py_madvr-1.4.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-22 03:05:39.000000 py_madvr-1.4.4/tests/testMadVR.py
```

### Comparing `py_madvr-1.4.3/LICENSE` & `py_madvr-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.3/PKG-INFO` & `py_madvr-1.4.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_madvr
-Version: 1.4.3
+Version: 1.4.4
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.3/madvr/commands.py` & `py_madvr-1.4.4/madvr/commands.py`

 * *Files identical despite different names*

### Comparing `py_madvr-1.4.3/madvr/madvr.py` & `py_madvr-1.4.4/madvr/madvr.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         await self._clear_attr()
         self.logger.debug("connection is closed")
 
     async def open_connection(self) -> None:
         """Open a connection"""
         self.logger.debug("Starting open connection")
         try:
+            self.stop_reconnect.clear()
             await self._reconnect()
         except AckError as err:
             self.logger.error(err)
 
     def stop(self):
         """Stop reconnecting"""
         self.stop_reconnect.set()
```

### Comparing `py_madvr-1.4.3/py_madvr.egg-info/PKG-INFO` & `py_madvr-1.4.4/py_madvr.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-madvr
-Version: 1.4.3
+Version: 1.4.4
 Summary: A package to control MadVR Envy over IP
 Home-page: https://github.com/iloveicedgreentea/py-madvr
 Author: iloveicedgreentea
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `py_madvr-1.4.3/setup.py` & `py_madvr-1.4.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="py_madvr",
-    version="1.4.3",
+    version="1.4.4",
     author="iloveicedgreentea",
     description="A package to control MadVR Envy over IP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/iloveicedgreentea/py-madvr",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `py_madvr-1.4.3/tests/testMadVR.py` & `py_madvr-1.4.4/tests/testMadVR.py`

 * *Files identical despite different names*

