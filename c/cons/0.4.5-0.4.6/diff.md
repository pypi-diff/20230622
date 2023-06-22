# Comparing `tmp/cons-0.4.5.tar.gz` & `tmp/cons-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cons-0.4.5.tar", last modified: Wed Jan 19 22:46:44 2022, max compression
+gzip compressed data, was "cons-0.4.6.tar", last modified: Thu Jun 22 17:56:49 2023, max compression
```

## Comparing `cons-0.4.5.tar` & `cons-0.4.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 22:46:44.073158 cons-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-01-19 22:46:43.000000 cons-0.4.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-01-19 22:46:43.000000 cons-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4730 2022-01-19 22:46:44.073158 cons-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2765 2022-01-19 22:46:43.000000 cons-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 22:46:44.073158 cons-0.4.5/cons/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-01-19 22:46:43.000000 cons-0.4.5/cons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-01-19 22:46:44.073158 cons-0.4.5/cons/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     7715 2022-01-19 22:46:43.000000 cons-0.4.5/cons/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      969 2022-01-19 22:46:43.000000 cons-0.4.5/cons/unify.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-19 22:46:44.073158 cons-0.4.5/cons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4730 2022-01-19 22:46:44.000000 cons-0.4.5/cons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-01-19 22:46:44.000000 cons-0.4.5/cons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-19 22:46:44.000000 cons-0.4.5/cons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-01-19 22:46:44.000000 cons-0.4.5/cons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-19 22:46:44.000000 cons-0.4.5/cons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-01-19 22:46:44.073158 cons-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1595 2022-01-19 22:46:43.000000 cons-0.4.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    80044 2022-01-19 22:46:43.000000 cons-0.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:56:49.301961 cons-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-22 17:56:47.000000 cons-0.4.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-22 17:56:47.000000 cons-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-22 17:56:49.301961 cons-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-22 17:56:47.000000 cons-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:56:49.301961 cons-0.4.6/cons/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 17:56:47.000000 cons-0.4.6/cons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-22 17:56:49.301961 cons-0.4.6/cons/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7712 2023-06-22 17:56:47.000000 cons-0.4.6/cons/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-22 17:56:47.000000 cons-0.4.6/cons/unify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:56:49.301961 cons-0.4.6/cons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-06-22 17:56:49.000000 cons-0.4.6/cons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 17:56:49.000000 cons-0.4.6/cons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:56:49.000000 cons-0.4.6/cons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 17:56:49.000000 cons-0.4.6/cons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 17:56:49.000000 cons-0.4.6/cons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-22 17:56:49.301961 cons-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-22 17:56:47.000000 cons-0.4.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-06-22 17:56:47.000000 cons-0.4.6/versioneer.py
```

### Comparing `cons-0.4.5/LICENSE.txt` & `cons-0.4.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cons-0.4.5/PKG-INFO` & `cons-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cons
-Version: 0.4.5
+Version: 0.4.6
 Summary: An implementation of Lisp/Scheme-like cons in Python.
 Home-page: https://github.com/pythological/python-cons
 Author: Brandon T. Willard
 Author-email: brandonwillard+cons@gmail.com
 License: LGPL-3
-Description: [![Build Status](https://travis-ci.org/pythological/python-cons.svg?branch=master)](https://travis-ci.org/pythological/python-cons) [![Coverage Status](https://coveralls.io/repos/github/pythological/python-cons/badge.svg?branch=master)](https://coveralls.io/github/pythological/python-cons?branch=master) [![PyPI](https://img.shields.io/pypi/v/cons)](https://pypi.org/project/cons/)
+Description: [![Build Status](https://travis-ci.org/pythological/python-cons.svg?branch=main)](https://travis-ci.org/pythological/python-cons) [![Coverage Status](https://coveralls.io/repos/github/pythological/python-cons/badge.svg?branch=main)](https://coveralls.io/github/pythological/python-cons?branch=main) [![PyPI](https://img.shields.io/pypi/v/cons)](https://pypi.org/project/cons/)
         
         # Python `cons`
         
         An implementation of [`cons`][cons] in Python.
         
         ## Usage and Design
         
@@ -114,16 +114,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cons-0.4.5/README.md` & `cons-0.4.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://travis-ci.org/pythological/python-cons.svg?branch=master)](https://travis-ci.org/pythological/python-cons) [![Coverage Status](https://coveralls.io/repos/github/pythological/python-cons/badge.svg?branch=master)](https://coveralls.io/github/pythological/python-cons?branch=master) [![PyPI](https://img.shields.io/pypi/v/cons)](https://pypi.org/project/cons/)
+[![Build Status](https://travis-ci.org/pythological/python-cons.svg?branch=main)](https://travis-ci.org/pythological/python-cons) [![Coverage Status](https://coveralls.io/repos/github/pythological/python-cons/badge.svg?branch=main)](https://coveralls.io/github/pythological/python-cons?branch=main) [![PyPI](https://img.shields.io/pypi/v/cons)](https://pypi.org/project/cons/)
 
 # Python `cons`
 
 An implementation of [`cons`][cons] in Python.
 
 ## Usage and Design
```

### Comparing `cons-0.4.5/cons/core.py` & `cons-0.4.6/cons/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,23 +96,21 @@
         else:
             raise ValueError("Number of arguments must be greater than 2.")
 
         return res
 
     @classmethod
     def cons_merge(cls, car_part, cdr_part):
-
         if cdr_part is None:
             cdr_part = default_ConsNull()
 
         if isinstance(cdr_part, Mapping):
             cdr_part = cdr_part.items()
 
         if isinstance(cdr_part, ItemsView):
-
             return OrderedDict(chain((car_part,), cdr_part))
 
         elif hasattr(cdr_part, "__add__") or hasattr(cdr_part, "__radd__"):
             # TODO: What about adding `list.extend`?  We're already
             # constructing an instance of the CDR type.
             return type(cdr_part)((car_part,)) + cdr_part
 
@@ -138,15 +136,14 @@
 
 
 cons = ConsPair
 
 
 class MaybeConsType(ABCMeta):
     def __subclasscheck__(self, o):
-
         if issubclass(o, tuple(_cdr.funcs.keys())) and not issubclass(o, NonCons):
             return True
 
         return False
 
 
 class MaybeCons(metaclass=MaybeConsType):
```

### Comparing `cons-0.4.5/cons/unify.py` & `cons-0.4.6/cons/unify.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from unification.core import _reify, _unify, construction_sentinel
 
 from .core import ConsError, ConsPair, MaybeCons, car, cdr, cons
 
 
 def _unify_Cons(lcons, rcons, s):
-
     lcons_ = lcons
     rcons_ = rcons
 
     if isinstance(lcons, Iterator):
         lcons, lcons_ = tee(lcons)
 
     if isinstance(rcons, Iterator):
```

### Comparing `cons-0.4.5/cons.egg-info/PKG-INFO` & `cons-0.4.6/cons.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: cons
-Version: 0.4.5
+Version: 0.4.6
 Summary: An implementation of Lisp/Scheme-like cons in Python.
 Home-page: https://github.com/pythological/python-cons
 Author: Brandon T. Willard
 Author-email: brandonwillard+cons@gmail.com
 License: LGPL-3
-Description: [![Build Status](https://travis-ci.org/pythological/python-cons.svg?branch=master)](https://travis-ci.org/pythological/python-cons) [![Coverage Status](https://coveralls.io/repos/github/pythological/python-cons/badge.svg?branch=master)](https://coveralls.io/github/pythological/python-cons?branch=master) [![PyPI](https://img.shields.io/pypi/v/cons)](https://pypi.org/project/cons/)
+Description: [![Build Status](https://travis-ci.org/pythological/python-cons.svg?branch=main)](https://travis-ci.org/pythological/python-cons) [![Coverage Status](https://coveralls.io/repos/github/pythological/python-cons/badge.svg?branch=main)](https://coveralls.io/github/pythological/python-cons?branch=main) [![PyPI](https://img.shields.io/pypi/v/cons)](https://pypi.org/project/cons/)
         
         # Python `cons`
         
         An implementation of [`cons`][cons] in Python.
         
         ## Usage and Design
         
@@ -114,16 +114,16 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: DFSG approved
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `cons-0.4.5/setup.cfg` & `cons-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `cons-0.4.5/setup.py` & `cons-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: DFSG approved",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)",  # noqa: E501
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
     ],
 )
```

### Comparing `cons-0.4.5/versioneer.py` & `cons-0.4.6/versioneer.py`

 * *Files identical despite different names*

