# Comparing `tmp/python-dispatch-sphinx-0.2.1.tar.gz` & `tmp/python-dispatch-sphinx-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-dispatch-sphinx-0.2.1.tar", last modified: Mon Dec 19 20:20:45 2022, max compression
+gzip compressed data, was "python-dispatch-sphinx-0.2.2.tar", last modified: Thu Jun 22 16:52:11 2023, max compression
```

## Comparing `python-dispatch-sphinx-0.2.1.tar` & `python-dispatch-sphinx-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:20:45.032844 python-dispatch-sphinx-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-19 20:19:53.000000 python-dispatch-sphinx-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-19 20:19:53.000000 python-dispatch-sphinx-0.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2022-12-19 20:20:45.032844 python-dispatch-sphinx-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      682 2022-12-19 20:19:53.000000 python-dispatch-sphinx-0.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:20:45.032844 python-dispatch-sphinx-0.2.1/pydispatch_sphinx/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2022-12-19 20:19:53.000000 python-dispatch-sphinx-0.2.1/pydispatch_sphinx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2022-12-19 20:19:53.000000 python-dispatch-sphinx-0.2.1/pydispatch_sphinx/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)     5610 2022-12-19 20:19:53.000000 python-dispatch-sphinx-0.2.1/pydispatch_sphinx/documenters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 20:20:45.032844 python-dispatch-sphinx-0.2.1/python_dispatch_sphinx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2022-12-19 20:20:45.000000 python-dispatch-sphinx-0.2.1/python_dispatch_sphinx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      373 2022-12-19 20:20:45.000000 python-dispatch-sphinx-0.2.1/python_dispatch_sphinx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 20:20:45.000000 python-dispatch-sphinx-0.2.1/python_dispatch_sphinx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2022-12-19 20:20:45.000000 python-dispatch-sphinx-0.2.1/python_dispatch_sphinx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-19 20:20:45.000000 python-dispatch-sphinx-0.2.1/python_dispatch_sphinx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2022-12-19 20:20:45.032844 python-dispatch-sphinx-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 20:19:53.000000 python-dispatch-sphinx-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:52:11.277652 python-dispatch-sphinx-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-22 16:52:11.277652 python-dispatch-sphinx-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:52:11.277652 python-dispatch-sphinx-0.2.2/pydispatch_sphinx/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/pydispatch_sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/pydispatch_sphinx/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5610 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/pydispatch_sphinx/documenters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:52:11.277652 python-dispatch-sphinx-0.2.2/python_dispatch_sphinx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-22 16:52:11.000000 python-dispatch-sphinx-0.2.2/python_dispatch_sphinx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-22 16:52:11.000000 python-dispatch-sphinx-0.2.2/python_dispatch_sphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 16:52:11.000000 python-dispatch-sphinx-0.2.2/python_dispatch_sphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-22 16:52:11.000000 python-dispatch-sphinx-0.2.2/python_dispatch_sphinx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 16:52:11.000000 python-dispatch-sphinx-0.2.2/python_dispatch_sphinx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-22 16:52:11.277652 python-dispatch-sphinx-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 16:52:11.277652 python-dispatch-sphinx-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/tests/test_sphinx_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-06-22 16:52:04.000000 python-dispatch-sphinx-0.2.2/tests/test_sphinx_properties.py
```

### Comparing `python-dispatch-sphinx-0.2.1/LICENSE` & `python-dispatch-sphinx-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-dispatch-sphinx-0.2.1/PKG-INFO` & `python-dispatch-sphinx-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dispatch-sphinx
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sphinx extension for python-dispatch
 Home-page: https://github.com/nocarryr/python-dispatch
 Author: Matthew Reid
 Author-email: matt@nomadic-recording.com
 License: MIT
 Project-URL: Documentation, https://python-dispatch.readthedocs.io
 Project-URL: Source, https://github.com/nocarryr/python-dispatch
```

### Comparing `python-dispatch-sphinx-0.2.1/README.rst` & `python-dispatch-sphinx-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `python-dispatch-sphinx-0.2.1/pydispatch_sphinx/__init__.py` & `python-dispatch-sphinx-0.2.2/pydispatch_sphinx/__init__.py`

 * *Files identical despite different names*

### Comparing `python-dispatch-sphinx-0.2.1/pydispatch_sphinx/directives.py` & `python-dispatch-sphinx-0.2.2/pydispatch_sphinx/directives.py`

 * *Files identical despite different names*

### Comparing `python-dispatch-sphinx-0.2.1/pydispatch_sphinx/documenters.py` & `python-dispatch-sphinx-0.2.2/pydispatch_sphinx/documenters.py`

 * *Files identical despite different names*

### Comparing `python-dispatch-sphinx-0.2.1/python_dispatch_sphinx.egg-info/PKG-INFO` & `python-dispatch-sphinx-0.2.2/python_dispatch_sphinx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-dispatch-sphinx
-Version: 0.2.1
+Version: 0.2.2
 Summary: Sphinx extension for python-dispatch
 Home-page: https://github.com/nocarryr/python-dispatch
 Author: Matthew Reid
 Author-email: matt@nomadic-recording.com
 License: MIT
 Project-URL: Documentation, https://python-dispatch.readthedocs.io
 Project-URL: Source, https://github.com/nocarryr/python-dispatch
```

### Comparing `python-dispatch-sphinx-0.2.1/setup.cfg` & `python-dispatch-sphinx-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = False
 
 [metadata]
 name = python-dispatch-sphinx
-version = 0.2.1
+version = 0.2.2
 author = Matthew Reid
 author_email = matt@nomadic-recording.com
 url = https://github.com/nocarryr/python-dispatch
 project_urls = 
 	Documentation = https://python-dispatch.readthedocs.io
 	Source = https://github.com/nocarryr/python-dispatch
 	Tracker = https://github.com/nocarryr/python-dispatch/issues
```

