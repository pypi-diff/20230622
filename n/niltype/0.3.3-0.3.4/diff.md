# Comparing `tmp/niltype-0.3.3.tar.gz` & `tmp/niltype-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "niltype-0.3.3.tar", last modified: Fri Nov  4 10:04:18 2022, max compression
+gzip compressed data, was "niltype-0.3.4.tar", last modified: Thu Jun 22 15:26:25 2023, max compression
```

## Comparing `niltype-0.3.3.tar` & `niltype-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:04:18.616379 niltype-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-11-04 10:04:10.000000 niltype-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-11-04 10:04:18.616379 niltype-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-11-04 10:04:10.000000 niltype-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:04:18.616379 niltype-0.3.3/niltype/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-11-04 10:04:10.000000 niltype-0.3.3/niltype/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-04 10:04:10.000000 niltype-0.3.3/niltype/_nilable.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-11-04 10:04:10.000000 niltype-0.3.3/niltype/_niltype.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-04 10:04:10.000000 niltype-0.3.3/niltype/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 10:04:10.000000 niltype-0.3.3/niltype/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:04:18.616379 niltype-0.3.3/niltype.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-11-04 10:04:18.000000 niltype-0.3.3/niltype.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      257 2022-11-04 10:04:18.000000 niltype-0.3.3/niltype.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 10:04:18.000000 niltype-0.3.3/niltype.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-04 10:04:18.000000 niltype-0.3.3/niltype.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-11-04 10:04:18.620379 niltype-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-11-04 10:04:10.000000 niltype-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:25.801982 niltype-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-22 15:26:12.000000 niltype-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 15:26:25.801982 niltype-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-22 15:26:12.000000 niltype-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:25.801982 niltype-0.3.4/niltype/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/_nilable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/_niltype.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:12.000000 niltype-0.3.4/niltype/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:25.801982 niltype-0.3.4/niltype.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 15:26:25.000000 niltype-0.3.4/niltype.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-22 15:26:25.000000 niltype-0.3.4/niltype.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:26:25.000000 niltype-0.3.4/niltype.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 15:26:25.000000 niltype-0.3.4/niltype.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-22 15:26:25.801982 niltype-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-22 15:26:12.000000 niltype-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:26:25.801982 niltype-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-22 15:26:12.000000 niltype-0.3.4/tests/test_niltype.py
```

### Comparing `niltype-0.3.3/LICENSE` & `niltype-0.3.4/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Nikita Novosibirsk
+Copyright (c) 2020 Nikita Tsvetkov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `niltype-0.3.3/PKG-INFO` & `niltype-0.3.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: niltype
-Version: 0.3.3
+Version: 0.3.4
 Summary: Like a None
-Home-page: https://github.com/nikitanovosibirsk/niltype
+Home-page: https://github.com/tsv1/niltype
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nil Type
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/niltype/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/niltype)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/niltype/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/niltype)
 [![PyPI](https://img.shields.io/pypi/v/niltype.svg?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/niltype?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 [![Python Version](https://img.shields.io/pypi/pyversions/niltype.svg?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 
 Null value for cases when `None` is part of a data model
 
 ```python
```

### Comparing `niltype-0.3.3/README.md` & `niltype-0.3.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Nil Type
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/niltype/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/niltype)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/niltype/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/niltype)
 [![PyPI](https://img.shields.io/pypi/v/niltype.svg?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/niltype?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 [![Python Version](https://img.shields.io/pypi/pyversions/niltype.svg?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 
 Null value for cases when `None` is part of a data model
 
 ```python
```

### Comparing `niltype-0.3.3/niltype/_niltype.py` & `niltype-0.3.4/niltype/_niltype.py`

 * *Files identical despite different names*

### Comparing `niltype-0.3.3/niltype.egg-info/PKG-INFO` & `niltype-0.3.4/niltype.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: niltype
-Version: 0.3.3
+Version: 0.3.4
 Summary: Like a None
-Home-page: https://github.com/nikitanovosibirsk/niltype
+Home-page: https://github.com/tsv1/niltype
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Software Development
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Nil Type
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/niltype/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/niltype)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/niltype/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/niltype)
 [![PyPI](https://img.shields.io/pypi/v/niltype.svg?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/niltype?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 [![Python Version](https://img.shields.io/pypi/pyversions/niltype.svg?style=flat-square)](https://pypi.python.org/pypi/niltype/)
 
 Null value for cases when `None` is part of a data model
 
 ```python
```

### Comparing `niltype-0.3.3/setup.cfg` & `niltype-0.3.4/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.3
+current_version = 0.3.4
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

