# Comparing `tmp/pytest_compare-0.2.4.tar.gz` & `tmp/pytest_compare-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_compare-0.2.4.tar", last modified: Thu Mar 30 05:41:55 2023, max compression
+gzip compressed data, was "pytest_compare-0.2.5.tar", last modified: Thu Jun 22 04:52:46 2023, max compression
```

## Comparing `pytest_compare-0.2.4.tar` & `pytest_compare-0.2.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:41:55.650820 pytest_compare-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-03-30 05:41:55.650820 pytest_compare-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:41:55.646820 pytest_compare-0.2.4/pytest_compare/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pytest_compare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pytest_compare/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:41:55.650820 pytest_compare-0.2.4/pytest_compare/dict/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pytest_compare/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pytest_compare/dict/dict.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:41:55.650820 pytest_compare-0.2.4/pytest_compare/native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pytest_compare/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pytest_compare/native/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:41:55.650820 pytest_compare-0.2.4/pytest_compare/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pytest_compare/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-30 05:41:35.000000 pytest_compare-0.2.4/pytest_compare/pandas/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 05:41:55.650820 pytest_compare-0.2.4/pytest_compare.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-03-30 05:41:55.000000 pytest_compare-0.2.4/pytest_compare.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-30 05:41:55.000000 pytest_compare-0.2.4/pytest_compare.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 05:41:55.000000 pytest_compare-0.2.4/pytest_compare.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-30 05:41:55.000000 pytest_compare-0.2.4/pytest_compare.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-30 05:41:55.000000 pytest_compare-0.2.4/pytest_compare.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 05:41:55.650820 pytest_compare-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:52:46.283949 pytest_compare-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-22 04:52:46.283949 pytest_compare-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:52:46.279949 pytest_compare-0.2.5/pytest_compare/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pytest_compare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pytest_compare/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:52:46.283949 pytest_compare-0.2.5/pytest_compare/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pytest_compare/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pytest_compare/dict/dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:52:46.283949 pytest_compare-0.2.5/pytest_compare/native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pytest_compare/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pytest_compare/native/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:52:46.283949 pytest_compare-0.2.5/pytest_compare/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pytest_compare/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-22 04:52:23.000000 pytest_compare-0.2.5/pytest_compare/pandas/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 04:52:46.283949 pytest_compare-0.2.5/pytest_compare.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-22 04:52:46.000000 pytest_compare-0.2.5/pytest_compare.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-22 04:52:46.000000 pytest_compare-0.2.5/pytest_compare.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 04:52:46.000000 pytest_compare-0.2.5/pytest_compare.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 04:52:46.000000 pytest_compare-0.2.5/pytest_compare.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 04:52:46.000000 pytest_compare-0.2.5/pytest_compare.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 04:52:46.283949 pytest_compare-0.2.5/setup.cfg
```

### Comparing `pytest_compare-0.2.4/LICENSE` & `pytest_compare-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_compare-0.2.4/PKG-INFO` & `pytest_compare-0.2.5/pytest_compare.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytest_compare
-Version: 0.2.4
+Name: pytest-compare
+Version: 0.2.5
 Summary: pytest plugin for comparing call arguments.
 Author-email: Ilya Michlin <ilyamichlin1@gmail.com>
 Project-URL: homepage, https://pytesty.github.io/pytest-compare/
 Project-URL: documentation, https://pytesty.github.io/pytest-compare/documentation/
 Project-URL: repository, https://github.com/pytesty/pytest-compare/
 Project-URL: license, https://pytesty.github.io/pytest-compare/license/
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,17 +25,16 @@
 License-File: LICENSE
 
 # pytest-compare
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pytest_compare.svg)](https://pypi.org/project/pytest-compare/)
 [![License](https://camo.githubusercontent.com/2439ed6934e5c87e17a7d562cfb92c91d2a673d8/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f726168756c646b6a61696e2f6769746875622d70726f66696c652d726561646d652d67656e657261746f723f7374796c653d666c61742d737175617265)](https://pytesty.github.io/pytest-compare/license/)
 [![Documentation](https://readthedocs.org/projects/pytest/badge/?version=latest)](https://pytesty.github.io/pytest-compare/documentation/)
-[![DOI](https://github.com/pytest-dev/pytest/workflows/test/badge.svg)](https://github.com/pytesty/pytest-compare/actions?query=workflow%3Atests)
 [![Downloads](https://static.pepy.tech/badge/pytest-compare/month)](https://pepy.tech/project/pytest-compare)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)x
 
 # What is it?
 The `pytest-compare` helps validate method call arguments when testing python code.
 
 `pytest-compare` is designed to work with [assert methods](https://docs.python.org/3/library/unittest.mock.html#the-mock-class). While python native variables can be easily compared, a more complicated structures sometimes do not. For example validating a `pd.DataFrame` will raise an exception. This is where `pytest-compare` comes in. It allows this kind of structures to be easily compared.
 
 # How to install
```

### Comparing `pytest_compare-0.2.4/README.md` & `pytest_compare-0.2.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # pytest-compare
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pytest_compare.svg)](https://pypi.org/project/pytest-compare/)
 [![License](https://camo.githubusercontent.com/2439ed6934e5c87e17a7d562cfb92c91d2a673d8/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f726168756c646b6a61696e2f6769746875622d70726f66696c652d726561646d652d67656e657261746f723f7374796c653d666c61742d737175617265)](https://pytesty.github.io/pytest-compare/license/)
 [![Documentation](https://readthedocs.org/projects/pytest/badge/?version=latest)](https://pytesty.github.io/pytest-compare/documentation/)
-[![DOI](https://github.com/pytest-dev/pytest/workflows/test/badge.svg)](https://github.com/pytesty/pytest-compare/actions?query=workflow%3Atests)
 [![Downloads](https://static.pepy.tech/badge/pytest-compare/month)](https://pepy.tech/project/pytest-compare)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)x
 
 # What is it?
 The `pytest-compare` helps validate method call arguments when testing python code.
 
 `pytest-compare` is designed to work with [assert methods](https://docs.python.org/3/library/unittest.mock.html#the-mock-class). While python native variables can be easily compared, a more complicated structures sometimes do not. For example validating a `pd.DataFrame` will raise an exception. This is where `pytest-compare` comes in. It allows this kind of structures to be easily compared.
 
 # How to install
```

### Comparing `pytest_compare-0.2.4/pyproject.toml` & `pytest_compare-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 dependencies = [
-    "typeguard",
+    "typeguard<4.0.0",
 ]
 
 
 [project.optional-dependencies]
 pandas = ["pandas"]
```

### Comparing `pytest_compare-0.2.4/pytest_compare/base.py` & `pytest_compare-0.2.5/pytest_compare/base.py`

 * *Files identical despite different names*

### Comparing `pytest_compare-0.2.4/pytest_compare/dict/dict.py` & `pytest_compare-0.2.5/pytest_compare/dict/dict.py`

 * *Files identical despite different names*

### Comparing `pytest_compare-0.2.4/pytest_compare/native/native.py` & `pytest_compare-0.2.5/pytest_compare/native/native.py`

 * *Files identical despite different names*

### Comparing `pytest_compare-0.2.4/pytest_compare/pandas/pandas.py` & `pytest_compare-0.2.5/pytest_compare/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `pytest_compare-0.2.4/pytest_compare.egg-info/PKG-INFO` & `pytest_compare-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: pytest-compare
-Version: 0.2.4
+Name: pytest_compare
+Version: 0.2.5
 Summary: pytest plugin for comparing call arguments.
 Author-email: Ilya Michlin <ilyamichlin1@gmail.com>
 Project-URL: homepage, https://pytesty.github.io/pytest-compare/
 Project-URL: documentation, https://pytesty.github.io/pytest-compare/documentation/
 Project-URL: repository, https://github.com/pytesty/pytest-compare/
 Project-URL: license, https://pytesty.github.io/pytest-compare/license/
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,17 +25,16 @@
 License-File: LICENSE
 
 # pytest-compare
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/pytest_compare.svg)](https://pypi.org/project/pytest-compare/)
 [![License](https://camo.githubusercontent.com/2439ed6934e5c87e17a7d562cfb92c91d2a673d8/68747470733a2f2f696d672e736869656c64732e696f2f6769746875622f6c6963656e73652f726168756c646b6a61696e2f6769746875622d70726f66696c652d726561646d652d67656e657261746f723f7374796c653d666c61742d737175617265)](https://pytesty.github.io/pytest-compare/license/)
 [![Documentation](https://readthedocs.org/projects/pytest/badge/?version=latest)](https://pytesty.github.io/pytest-compare/documentation/)
-[![DOI](https://github.com/pytest-dev/pytest/workflows/test/badge.svg)](https://github.com/pytesty/pytest-compare/actions?query=workflow%3Atests)
 [![Downloads](https://static.pepy.tech/badge/pytest-compare/month)](https://pepy.tech/project/pytest-compare)
-[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)x
 
 # What is it?
 The `pytest-compare` helps validate method call arguments when testing python code.
 
 `pytest-compare` is designed to work with [assert methods](https://docs.python.org/3/library/unittest.mock.html#the-mock-class). While python native variables can be easily compared, a more complicated structures sometimes do not. For example validating a `pd.DataFrame` will raise an exception. This is where `pytest-compare` comes in. It allows this kind of structures to be easily compared.
 
 # How to install
```

