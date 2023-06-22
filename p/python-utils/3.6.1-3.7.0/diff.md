# Comparing `tmp/python-utils-3.6.1.tar.gz` & `tmp/python-utils-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Volumes/workspace/python-utils/dist/.tmp-5x_ekkqi/python-utils-3.6.1.tar", last modified: Sat Jun 17 11:33:55 2023, max compression
+gzip compressed data, was "/Volumes/workspace/python-utils/dist/.tmp-525c5u2e/python-utils-3.7.0.tar", last modified: Thu Jun 22 01:34:29 2023, max compression
```

## Comparing `python-utils-3.6.1.tar` & `python-utils-3.7.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-17 11:33:55.052707 python-utils-3.6.1/
--rw-r--r--   0 rick       (501) staff       (20)     1501 2021-10-31 01:51:48.000000 python-utils-3.6.1/LICENSE
--rw-r--r--   0 rick       (501) staff       (20)      281 2022-10-29 20:47:53.000000 python-utils-3.6.1/MANIFEST.in
--rw-r--r--   0 rick       (501) staff       (20)     9086 2023-06-17 11:33:55.052829 python-utils-3.6.1/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)     8642 2023-05-29 00:58:50.000000 python-utils-3.6.1/README.rst
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-17 11:33:55.040573 python-utils-3.6.1/_python_utils_tests/
--rw-r--r--   0 rick       (501) staff       (20)        0 2023-06-17 11:33:41.000000 python-utils-3.6.1/_python_utils_tests/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)       12 2021-12-16 15:50:12.000000 python-utils-3.6.1/_python_utils_tests/requirements.txt
--rw-r--r--   0 rick       (501) staff       (20)      508 2023-05-29 00:58:50.000000 python-utils-3.6.1/_python_utils_tests/test_aio.py
--rw-r--r--   0 rick       (501) staff       (20)      592 2023-02-08 16:44:13.000000 python-utils-3.6.1/_python_utils_tests/test_containers.py
--rw-r--r--   0 rick       (501) staff       (20)      897 2022-05-29 21:48:50.000000 python-utils-3.6.1/_python_utils_tests/test_decorators.py
--rw-r--r--   0 rick       (501) staff       (20)     1669 2022-05-30 22:13:21.000000 python-utils-3.6.1/_python_utils_tests/test_generators.py
--rw-r--r--   0 rick       (501) staff       (20)     1431 2022-05-29 21:48:50.000000 python-utils-3.6.1/_python_utils_tests/test_import.py
--rw-r--r--   0 rick       (501) staff       (20)      362 2022-05-29 02:02:55.000000 python-utils-3.6.1/_python_utils_tests/test_logger.py
--rw-r--r--   0 rick       (501) staff       (20)      271 2022-05-29 21:48:50.000000 python-utils-3.6.1/_python_utils_tests/test_python_utils.py
--rw-r--r--   0 rick       (501) staff       (20)     4326 2022-10-29 19:12:20.000000 python-utils-3.6.1/_python_utils_tests/test_time.py
--rw-r--r--   0 rick       (501) staff       (20)       50 2021-10-31 01:51:48.000000 python-utils-3.6.1/coverage.rc
--rw-r--r--   0 rick       (501) staff       (20)      391 2023-05-29 00:58:50.000000 python-utils-3.6.1/pyproject.toml
--rw-r--r--   0 rick       (501) staff       (20)      253 2023-05-29 00:58:50.000000 python-utils-3.6.1/pytest.ini
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-17 11:33:55.050628 python-utils-3.6.1/python_utils/
--rw-r--r--   0 rick       (501) staff       (20)      385 2023-06-17 11:33:42.000000 python-utils-3.6.1/python_utils/__about__.py
--rw-r--r--   0 rick       (501) staff       (20)     1705 2023-06-17 11:33:41.000000 python-utils-3.6.1/python_utils/__init__.py
--rw-r--r--   0 rick       (501) staff       (20)      544 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/aio.py
--rw-r--r--   0 rick       (501) staff       (20)        0 2016-05-31 10:02:50.000000 python-utils-3.6.1/python_utils/compat.py
--rw-r--r--   0 rick       (501) staff       (20)     9783 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/containers.py
--rw-r--r--   0 rick       (501) staff       (20)    11404 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/converters.py
--rw-r--r--   0 rick       (501) staff       (20)     4061 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/decorators.py
--rw-r--r--   0 rick       (501) staff       (20)      617 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/exceptions.py
--rw-r--r--   0 rick       (501) staff       (20)     5015 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/formatters.py
--rw-r--r--   0 rick       (501) staff       (20)     2609 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/generators.py
--rw-r--r--   0 rick       (501) staff       (20)     3165 2022-05-29 21:48:50.000000 python-utils-3.6.1/python_utils/import_.py
--rw-r--r--   0 rick       (501) staff       (20)     3132 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/logger.py
--rw-r--r--   0 rick       (501) staff       (20)      358 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/loguru.py
--rw-r--r--   0 rick       (501) staff       (20)        0 2022-10-29 19:12:20.000000 python-utils-3.6.1/python_utils/py.typed
--rw-r--r--   0 rick       (501) staff       (20)     4711 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/terminal.py
--rw-r--r--   0 rick       (501) staff       (20)    11304 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/time.py
--rw-r--r--   0 rick       (501) staff       (20)     3652 2023-05-29 00:58:50.000000 python-utils-3.6.1/python_utils/types.py
-drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-17 11:33:55.052464 python-utils-3.6.1/python_utils.egg-info/
--rw-r--r--   0 rick       (501) staff       (20)     9086 2023-06-17 11:33:54.000000 python-utils-3.6.1/python_utils.egg-info/PKG-INFO
--rw-r--r--   0 rick       (501) staff       (20)     1069 2023-06-17 11:33:55.000000 python-utils-3.6.1/python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 rick       (501) staff       (20)        1 2023-06-17 11:33:54.000000 python-utils-3.6.1/python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 rick       (501) staff       (20)      169 2023-06-17 11:33:54.000000 python-utils-3.6.1/python_utils.egg-info/requires.txt
--rw-r--r--   0 rick       (501) staff       (20)       13 2023-06-17 11:33:54.000000 python-utils-3.6.1/python_utils.egg-info/top_level.txt
--rw-r--r--   0 rick       (501) staff       (20)        2 2023-02-09 15:13:53.000000 python-utils-3.6.1/requirements.txt
--rw-r--r--   0 rick       (501) staff       (20)      611 2023-06-17 11:33:55.054330 python-utils-3.6.1/setup.cfg
--rw-r--r--   0 rick       (501) staff       (20)     1603 2023-06-17 11:33:42.000000 python-utils-3.6.1/setup.py
--rw-r--r--   0 rick       (501) staff       (20)     1440 2023-05-29 00:58:50.000000 python-utils-3.6.1/tox.ini
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-22 01:34:29.927550 python-utils-3.7.0/
+-rw-r--r--   0 rick       (501) staff       (20)     1501 2021-10-31 01:51:48.000000 python-utils-3.7.0/LICENSE
+-rw-r--r--   0 rick       (501) staff       (20)      281 2022-10-29 20:47:53.000000 python-utils-3.7.0/MANIFEST.in
+-rw-r--r--   0 rick       (501) staff       (20)     9086 2023-06-22 01:34:29.927775 python-utils-3.7.0/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)     8642 2023-05-29 00:58:50.000000 python-utils-3.7.0/README.rst
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-22 01:34:29.915415 python-utils-3.7.0/_python_utils_tests/
+-rw-r--r--   0 rick       (501) staff       (20)        0 2023-06-22 01:34:21.000000 python-utils-3.7.0/_python_utils_tests/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)       12 2021-12-16 15:50:12.000000 python-utils-3.7.0/_python_utils_tests/requirements.txt
+-rw-r--r--   0 rick       (501) staff       (20)      871 2023-06-22 01:34:22.000000 python-utils-3.7.0/_python_utils_tests/test_aio.py
+-rw-r--r--   0 rick       (501) staff       (20)      678 2023-06-22 01:34:22.000000 python-utils-3.7.0/_python_utils_tests/test_containers.py
+-rw-r--r--   0 rick       (501) staff       (20)     1965 2023-06-22 01:34:22.000000 python-utils-3.7.0/_python_utils_tests/test_decorators.py
+-rw-r--r--   0 rick       (501) staff       (20)     1729 2023-06-22 01:34:22.000000 python-utils-3.7.0/_python_utils_tests/test_generators.py
+-rw-r--r--   0 rick       (501) staff       (20)     1471 2023-06-22 01:34:22.000000 python-utils-3.7.0/_python_utils_tests/test_import.py
+-rw-r--r--   0 rick       (501) staff       (20)      396 2023-06-22 01:34:22.000000 python-utils-3.7.0/_python_utils_tests/test_logger.py
+-rw-r--r--   0 rick       (501) staff       (20)      271 2022-05-29 21:48:50.000000 python-utils-3.7.0/_python_utils_tests/test_python_utils.py
+-rw-r--r--   0 rick       (501) staff       (20)     4653 2023-06-22 01:34:22.000000 python-utils-3.7.0/_python_utils_tests/test_time.py
+-rw-r--r--   0 rick       (501) staff       (20)       50 2021-10-31 01:51:48.000000 python-utils-3.7.0/coverage.rc
+-rw-r--r--   0 rick       (501) staff       (20)      432 2023-06-22 01:34:22.000000 python-utils-3.7.0/pyproject.toml
+-rw-r--r--   0 rick       (501) staff       (20)      253 2023-05-29 00:58:50.000000 python-utils-3.7.0/pytest.ini
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-22 01:34:29.923937 python-utils-3.7.0/python_utils/
+-rw-r--r--   0 rick       (501) staff       (20)      385 2023-06-22 01:34:22.000000 python-utils-3.7.0/python_utils/__about__.py
+-rw-r--r--   0 rick       (501) staff       (20)     1705 2023-06-22 01:34:21.000000 python-utils-3.7.0/python_utils/__init__.py
+-rw-r--r--   0 rick       (501) staff       (20)     1270 2023-06-22 01:34:22.000000 python-utils-3.7.0/python_utils/aio.py
+-rw-r--r--   0 rick       (501) staff       (20)        0 2016-05-31 10:02:50.000000 python-utils-3.7.0/python_utils/compat.py
+-rw-r--r--   0 rick       (501) staff       (20)     9783 2023-05-29 00:58:50.000000 python-utils-3.7.0/python_utils/containers.py
+-rw-r--r--   0 rick       (501) staff       (20)    11404 2023-05-29 00:58:50.000000 python-utils-3.7.0/python_utils/converters.py
+-rw-r--r--   0 rick       (501) staff       (20)     5412 2023-06-22 01:34:22.000000 python-utils-3.7.0/python_utils/decorators.py
+-rw-r--r--   0 rick       (501) staff       (20)      617 2023-05-29 00:58:50.000000 python-utils-3.7.0/python_utils/exceptions.py
+-rw-r--r--   0 rick       (501) staff       (20)     5015 2023-05-29 00:58:50.000000 python-utils-3.7.0/python_utils/formatters.py
+-rw-r--r--   0 rick       (501) staff       (20)     2670 2023-06-22 01:34:22.000000 python-utils-3.7.0/python_utils/generators.py
+-rw-r--r--   0 rick       (501) staff       (20)     3165 2022-05-29 21:48:50.000000 python-utils-3.7.0/python_utils/import_.py
+-rw-r--r--   0 rick       (501) staff       (20)     6371 2023-06-22 01:34:22.000000 python-utils-3.7.0/python_utils/logger.py
+-rw-r--r--   0 rick       (501) staff       (20)      358 2023-05-29 00:58:50.000000 python-utils-3.7.0/python_utils/loguru.py
+-rw-r--r--   0 rick       (501) staff       (20)        0 2022-10-29 19:12:20.000000 python-utils-3.7.0/python_utils/py.typed
+-rw-r--r--   0 rick       (501) staff       (20)     4711 2023-05-29 00:58:50.000000 python-utils-3.7.0/python_utils/terminal.py
+-rw-r--r--   0 rick       (501) staff       (20)    11304 2023-05-29 00:58:50.000000 python-utils-3.7.0/python_utils/time.py
+-rw-r--r--   0 rick       (501) staff       (20)     3652 2023-05-29 00:58:50.000000 python-utils-3.7.0/python_utils/types.py
+drwxr-xr-x   0 rick       (501) staff       (20)        0 2023-06-22 01:34:29.927122 python-utils-3.7.0/python_utils.egg-info/
+-rw-r--r--   0 rick       (501) staff       (20)     9086 2023-06-22 01:34:29.000000 python-utils-3.7.0/python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 rick       (501) staff       (20)     1069 2023-06-22 01:34:29.000000 python-utils-3.7.0/python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 rick       (501) staff       (20)        1 2023-06-22 01:34:29.000000 python-utils-3.7.0/python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 rick       (501) staff       (20)      169 2023-06-22 01:34:29.000000 python-utils-3.7.0/python_utils.egg-info/requires.txt
+-rw-r--r--   0 rick       (501) staff       (20)       13 2023-06-22 01:34:29.000000 python-utils-3.7.0/python_utils.egg-info/top_level.txt
+-rw-r--r--   0 rick       (501) staff       (20)        2 2023-02-09 15:13:53.000000 python-utils-3.7.0/requirements.txt
+-rw-r--r--   0 rick       (501) staff       (20)      611 2023-06-22 01:34:29.929348 python-utils-3.7.0/setup.cfg
+-rw-r--r--   0 rick       (501) staff       (20)     1603 2023-06-17 11:33:42.000000 python-utils-3.7.0/setup.py
+-rw-r--r--   0 rick       (501) staff       (20)     1440 2023-05-29 00:58:50.000000 python-utils-3.7.0/tox.ini
```

### Comparing `python-utils-3.6.1/LICENSE` & `python-utils-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/PKG-INFO` & `python-utils-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-utils
-Version: 3.6.1
+Version: 3.7.0
 Summary: Python Utils is a module with some convenient utilities not included with the standard Python install
 Home-page: https://github.com/WoLpH/python-utils
 Author: Rick van Hattem
 Author-email: Wolph@wol.ph
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >3.8.0
```

### Comparing `python-utils-3.6.1/README.rst` & `python-utils-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/_python_utils_tests/test_generators.py` & `python-utils-3.7.0/_python_utils_tests/test_generators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import asyncio
 
 import pytest
 
 import python_utils
+from python_utils import types
 
 
 @pytest.mark.asyncio
 async def test_abatcher():
     async for batch in python_utils.abatcher(python_utils.acount(stop=9), 3):
         assert len(batch) == 3
 
     async for batch in python_utils.abatcher(python_utils.acount(stop=2), 3):
         assert len(batch) == 2
 
 
 @pytest.mark.asyncio
 async def test_abatcher_timed():
-    batches = []
+    batches: types.List[types.List[int]] = []
     async for batch in python_utils.abatcher(
         python_utils.acount(stop=10, delay=0.08), interval=0.1
     ):
         batches.append(batch)
 
     assert batches == [[0, 1, 2], [3, 4], [5, 6], [7, 8], [9]]
     assert len(batches) == 5
```

### Comparing `python-utils-3.6.1/_python_utils_tests/test_import.py` & `python-utils-3.7.0/_python_utils_tests/test_import.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from python_utils import import_
+from python_utils import import_, types
 
 
 def test_import_globals_relative_import():
     for i in range(-1, 5):
         relative_import(i)
 
 
-def relative_import(level):
-    locals_ = {}
+def relative_import(level: int):
+    locals_: types.Dict[str, types.Any] = {}
     globals_ = {'__name__': 'python_utils.import_'}
     import_.import_global('.formatters', locals_=locals_, globals_=globals_)
     assert 'camel_to_underscore' in globals_
 
 
 def test_import_globals_without_inspection():
     locals_ = {}
```

### Comparing `python-utils-3.6.1/_python_utils_tests/test_time.py` & `python-utils-3.7.0/_python_utils_tests/test_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import asyncio
 import itertools
 from datetime import timedelta
 
 import pytest
 
 import python_utils
+from python_utils import types
 
 
 @pytest.mark.parametrize(
     'timeout,interval,interval_multiplier,maximum_interval,iterable,result',
     [
         (0.2, 0.1, 0.4, 0.2, python_utils.acount, 2),
         (0.3, 0.1, 0.4, 0.2, python_utils.acount(), 3),
@@ -21,44 +22,58 @@
             python_utils.acount,
             2,
         ),
     ],
 )
 @pytest.mark.asyncio
 async def test_aio_timeout_generator(
-    timeout, interval, interval_multiplier, maximum_interval, iterable, result
+    timeout: float,
+    interval: float,
+    interval_multiplier: float,
+    maximum_interval: float,
+    iterable: types.AsyncIterable[types.Any],
+    result: int,
 ):
     i = None
     async for i in python_utils.aio_timeout_generator(
         timeout, interval, iterable, maximum_interval=maximum_interval
     ):
         pass
 
     assert i == result
 
 
 @pytest.mark.parametrize(
     'timeout,interval,interval_multiplier,maximum_interval,iterable,result',
     [
         (0.01, 0.006, 0.5, 0.01, 'abc', 'c'),
-        (0.01, 0.006, 0.5, 0.01, itertools.count, 2),
+        (0.01, 0.006, 0.5, 0.01, itertools.count, 2),  # type: ignore
         (0.01, 0.006, 0.5, 0.01, itertools.count(), 2),
         (0.01, 0.006, 1.0, None, 'abc', 'c'),
         (
             timedelta(seconds=0.01),
             timedelta(seconds=0.006),
             2.0,
             timedelta(seconds=0.01),
-            itertools.count,
+            itertools.count,  # type: ignore
             2,
         ),
     ],
 )
 def test_timeout_generator(
-    timeout, interval, interval_multiplier, maximum_interval, iterable, result
+    timeout: float,
+    interval: float,
+    interval_multiplier: float,
+    maximum_interval: float,
+    iterable: types.Union[
+        str,
+        types.Iterable[types.Any],
+        types.Callable[..., types.Iterable[types.Any]],
+    ],
+    result: int,
 ):
     i = None
     for i in python_utils.timeout_generator(
         timeout=timeout,
         interval=interval,
         interval_multiplier=interval_multiplier,
         iterable=iterable,
```

### Comparing `python-utils-3.6.1/python_utils/__init__.py` & `python-utils-3.7.0/python_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils/containers.py` & `python-utils-3.7.0/python_utils/containers.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils/converters.py` & `python-utils-3.7.0/python_utils/converters.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils/decorators.py` & `python-utils-3.7.0/python_utils/decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import functools
 import logging
 import random
 from . import types
 
-T = types.TypeVar('T')
-TC = types.TypeVar('TC', bound=types.Container[types.Any])
-P = types.ParamSpec('P')
+_T = types.TypeVar('_T')
+_TC = types.TypeVar('_TC', bound=types.Container[types.Any])
+_P = types.ParamSpec('_P')
+_S = types.TypeVar('_S', covariant=True)
 
 
 def set_attributes(**kwargs: types.Any) -> types.Callable[..., types.Any]:
     '''Decorator to set attributes on functions and classes
 
     A common usage for this pattern is the Django Admin where
     functions can get an optional short_description. To illustrate:
@@ -29,29 +30,31 @@
     ...     return ("%s %s" % (obj.first_name, obj.last_name)).upper()
 
     >>> upper_case_name.short_description = 'Name'
 
     '''
 
     def _set_attributes(
-        function: types.Callable[P, T]
-    ) -> types.Callable[P, T]:
+        function: types.Callable[_P, _T]
+    ) -> types.Callable[_P, _T]:
         for key, value in kwargs.items():
             setattr(function, key, value)
         return function
 
     return _set_attributes
 
 
 def listify(
-    collection: types.Callable[[types.Iterable[T]], TC] = list,  # type: ignore
+    collection: types.Callable[
+        [types.Iterable[_T]], _TC
+    ] = list,  # type: ignore
     allow_empty: bool = True,
 ) -> types.Callable[
-    [types.Callable[..., types.Optional[types.Iterable[T]]]],
-    types.Callable[..., TC],
+    [types.Callable[..., types.Optional[types.Iterable[_T]]]],
+    types.Callable[..., _TC],
 ]:
     '''
     Convert any generator to a list or other type of collection.
 
     >>> @listify()
     ... def generator():
     ...     yield 1
@@ -92,18 +95,18 @@
     ...     yield 'b', 2
 
     >>> dict_generator()
     {'a': 1, 'b': 2}
     '''
 
     def _listify(
-        function: types.Callable[..., types.Optional[types.Iterable[T]]]
-    ) -> types.Callable[..., TC]:
-        def __listify(*args: types.Any, **kwargs: types.Any) -> TC:
-            result: types.Optional[types.Iterable[T]] = function(
+        function: types.Callable[..., types.Optional[types.Iterable[_T]]]
+    ) -> types.Callable[..., _TC]:
+        def __listify(*args: types.Any, **kwargs: types.Any) -> _TC:
+            result: types.Optional[types.Iterable[_T]] = function(
                 *args, **kwargs
             )
             if result is None:
                 if allow_empty:
                     return collection(iter(()))
                 else:
                     raise TypeError(
@@ -130,25 +133,67 @@
     ... def demo_function(*args, **kwargs):
     ...     return 1
 
     Calls to *demo_function* will be limited to 50% approximatly.
     '''
 
     def _sample(
-        function: types.Callable[P, T]
-    ) -> types.Callable[P, types.Optional[T]]:
+        function: types.Callable[_P, _T]
+    ) -> types.Callable[_P, types.Optional[_T]]:
         @functools.wraps(function)
-        def __sample(*args: P.args, **kwargs: P.kwargs) -> types.Optional[T]:
+        def __sample(
+            *args: _P.args, **kwargs: _P.kwargs
+        ) -> types.Optional[_T]:
             if random.random() < sample_rate:
                 return function(*args, **kwargs)
             else:
                 logging.debug(
                     'Skipped execution of %r(%r, %r) due to sampling',
                     function,
                     args,
                     kwargs,
                 )  # noqa: E501
                 return None
 
         return __sample
 
     return _sample
+
+
+def wraps_classmethod(
+    wrapped: types.Callable[types.Concatenate[_S, _P], _T],
+) -> types.Callable[
+    [
+        types.Callable[types.Concatenate[types.Any, _P], _T],
+    ],
+    types.Callable[types.Concatenate[types.Type[_S], _P], _T],
+]:
+    '''
+    Like `functools.wraps`, but for wrapping classmethods with the type info
+    from a regular method
+    '''
+
+    def _wraps_classmethod(
+        wrapper: types.Callable[types.Concatenate[types.Any, _P], _T],
+    ) -> types.Callable[types.Concatenate[types.Type[_S], _P], _T]:
+        try:  # pragma: no cover
+            wrapper = functools.update_wrapper(
+                wrapper,
+                wrapped,
+                assigned=tuple(
+                    a
+                    for a in functools.WRAPPER_ASSIGNMENTS
+                    if a != '__annotations__'
+                ),
+            )
+        except AttributeError:
+            # For some reason `functools.update_wrapper` fails on some test
+            # runs but not while running actual code
+            pass
+
+        if annotations := getattr(wrapped, '__annotations__', {}):
+            annotations.pop('self', None)
+            wrapper.__annotations__ = annotations
+
+        return wrapper
+
+    return _wraps_classmethod
```

### Comparing `python-utils-3.6.1/python_utils/exceptions.py` & `python-utils-3.7.0/python_utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils/formatters.py` & `python-utils-3.7.0/python_utils/formatters.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils/generators.py` & `python-utils-3.7.0/python_utils/generators.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,18 @@
 from python_utils import types
 
 
 _T = types.TypeVar('_T')
 
 
 async def abatcher(
-    generator: types.AsyncGenerator[_T, None],
+    generator: types.Union[
+        types.AsyncGenerator[_T, None],
+        types.AsyncIterator[_T],
+    ],
     batch_size: types.Optional[int] = None,
     interval: types.Optional[types.delta_type] = None,
 ) -> types.AsyncGenerator[types.List[_T], None]:
     '''
     Asyncio generator wrapper that returns items with a given batch size or
     interval (whichever is reached first).
     '''
```

### Comparing `python-utils-3.6.1/python_utils/import_.py` & `python-utils-3.7.0/python_utils/import_.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils/terminal.py` & `python-utils-3.7.0/python_utils/terminal.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils/time.py` & `python-utils-3.7.0/python_utils/time.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils/types.py` & `python-utils-3.7.0/python_utils/types.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/python_utils.egg-info/PKG-INFO` & `python-utils-3.7.0/python_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-utils
-Version: 3.6.1
+Version: 3.7.0
 Summary: Python Utils is a module with some convenient utilities not included with the standard Python install
 Home-page: https://github.com/WoLpH/python-utils
 Author: Rick van Hattem
 Author-email: Wolph@wol.ph
 License: BSD
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >3.8.0
```

### Comparing `python-utils-3.6.1/python_utils.egg-info/SOURCES.txt` & `python-utils-3.7.0/python_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/setup.cfg` & `python-utils-3.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/setup.py` & `python-utils-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-utils-3.6.1/tox.ini` & `python-utils-3.7.0/tox.ini`

 * *Files identical despite different names*

