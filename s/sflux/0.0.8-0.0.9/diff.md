# Comparing `tmp/sflux-0.0.8.tar.gz` & `tmp/sflux-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sflux-0.0.8.tar", last modified: Wed Nov 30 13:51:55 2022, max compression
+gzip compressed data, was "sflux-0.0.9.tar", last modified: Wed Nov 30 14:08:49 2022, max compression
```

## Comparing `sflux-0.0.8.tar` & `sflux-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:51:55.780612 sflux-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2022-11-30 13:51:42.000000 sflux-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      556 2022-11-30 13:51:55.780612 sflux-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      128 2022-11-30 13:51:42.000000 sflux-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-30 13:51:42.000000 sflux-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      622 2022-11-30 13:51:55.780612 sflux-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:51:55.780612 sflux-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:51:55.780612 sflux-0.0.8/src/sflux/
--rw-r--r--   0 runner    (1001) docker     (122)      113 2022-11-30 13:51:42.000000 sflux-0.0.8/src/sflux/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9869 2022-11-30 13:51:42.000000 sflux-0.0.8/src/sflux/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2022-11-30 13:51:42.000000 sflux-0.0.8/src/sflux/measurement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2022-11-30 13:51:42.000000 sflux-0.0.8/src/sflux/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 13:51:55.780612 sflux-0.0.8/src/sflux.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      556 2022-11-30 13:51:55.000000 sflux-0.0.8/src/sflux.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      292 2022-11-30 13:51:55.000000 sflux-0.0.8/src/sflux.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 13:51:55.000000 sflux-0.0.8/src/sflux.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-30 13:51:55.000000 sflux-0.0.8/src/sflux.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        6 2022-11-30 13:51:55.000000 sflux-0.0.8/src/sflux.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:08:49.107969 sflux-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2022-11-30 14:08:36.000000 sflux-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2022-11-30 14:08:49.107969 sflux-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2022-11-30 14:08:36.000000 sflux-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2022-11-30 14:08:36.000000 sflux-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2022-11-30 14:08:49.107969 sflux-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:08:49.107969 sflux-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:08:49.107969 sflux-0.0.9/src/sflux/
+-rw-r--r--   0 runner    (1001) docker     (122)      113 2022-11-30 14:08:36.000000 sflux-0.0.9/src/sflux/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9869 2022-11-30 14:08:36.000000 sflux-0.0.9/src/sflux/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2058 2022-11-30 14:08:36.000000 sflux-0.0.9/src/sflux/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2202 2022-11-30 14:08:36.000000 sflux-0.0.9/src/sflux/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:08:49.107969 sflux-0.0.9/src/sflux.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      556 2022-11-30 14:08:49.000000 sflux-0.0.9/src/sflux.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      292 2022-11-30 14:08:49.000000 sflux-0.0.9/src/sflux.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 14:08:49.000000 sflux-0.0.9/src/sflux.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-30 14:08:49.000000 sflux-0.0.9/src/sflux.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2022-11-30 14:08:49.000000 sflux-0.0.9/src/sflux.egg-info/top_level.txt
```

### Comparing `sflux-0.0.8/LICENSE` & `sflux-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sflux-0.0.8/PKG-INFO` & `sflux-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflux
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple python interface for InfluxDB2.0
 Home-page: https://github.com/perrytec/sflux.git
 Author: perrytec
 Author-email: hello@perry.sg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sflux-0.0.8/setup.cfg` & `sflux-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sflux
-version = 0.0.8
+version = 0.0.9
 author = perrytec
 author_email = hello@perry.sg
 description = A simple python interface for InfluxDB2.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/perrytec/sflux.git
 classifiers =
```

### Comparing `sflux-0.0.8/src/sflux/client.py` & `sflux-0.0.9/src/sflux/client.py`

 * *Files identical despite different names*

### Comparing `sflux-0.0.8/src/sflux/measurement.py` & `sflux-0.0.9/src/sflux/measurement.py`

 * *Files identical despite different names*

### Comparing `sflux-0.0.8/src/sflux/utils.py` & `sflux-0.0.9/src/sflux/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,18 @@
 
     def in_(self, iterable: (list, tuple)):
         return f'contains(value: {self}, set: {self._parse_other(iterable)})'
 
     def not_in_(self, iterable: (list, tuple)):
         return f'not contains(value: {self}, set: {self._parse_other(iterable)})'
 
+    def exists(self):
+        """Implements `exists` from FluxQL"""
+        return f'exists {self}'
+
     def __repr__(self):
         return f'r["{self.column}"]'
 
     def _parse_other(self, other):
         if isinstance(other, (list, tuple)):
             return '[' + ','.join([self._parse_other(elem) for elem in other]) + ']'
         if isinstance(other, str):
```

### Comparing `sflux-0.0.8/src/sflux.egg-info/PKG-INFO` & `sflux-0.0.9/src/sflux.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sflux
-Version: 0.0.8
+Version: 0.0.9
 Summary: A simple python interface for InfluxDB2.0
 Home-page: https://github.com/perrytec/sflux.git
 Author: perrytec
 Author-email: hello@perry.sg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

