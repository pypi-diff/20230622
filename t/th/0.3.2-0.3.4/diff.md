# Comparing `tmp/th-0.3.2.tar.gz` & `tmp/th-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "th-0.3.2.tar", last modified: Fri Nov  4 10:06:06 2022, max compression
+gzip compressed data, was "th-0.3.4.tar", last modified: Thu Jun 22 15:19:50 2023, max compression
```

## Comparing `th-0.3.2.tar` & `th-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:06:06.552177 th-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-04 10:05:57.000000 th-0.3.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-11-04 10:06:06.552177 th-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2069 2022-11-04 10:05:57.000000 th-0.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      689 2022-11-04 10:06:06.552177 th-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-11-04 10:05:57.000000 th-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:06:06.552177 th-0.3.2/th/
--rw-r--r--   0 runner    (1001) docker     (121)     3763 2022-11-04 10:05:57.000000 th-0.3.2/th/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-11-04 10:05:57.000000 th-0.3.2/th/_error.py
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-11-04 10:05:57.000000 th-0.3.2/th/_path_holder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1116 2022-11-04 10:05:57.000000 th-0.3.2/th/_path_holder_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-04 10:05:57.000000 th-0.3.2/th/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:06:06.552177 th-0.3.2/th/operators/
--rw-r--r--   0 runner    (1001) docker     (121)      483 2022-11-04 10:05:57.000000 th-0.3.2/th/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      585 2022-11-04 10:05:57.000000 th-0.3.2/th/operators/_operator.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 10:05:57.000000 th-0.3.2/th/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 10:06:06.552177 th-0.3.2/th.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2682 2022-11-04 10:06:06.000000 th-0.3.2/th.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-11-04 10:06:06.000000 th-0.3.2/th.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 10:06:06.000000 th-0.3.2/th.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-04 10:06:06.000000 th-0.3.2/th.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        3 2022-11-04 10:06:06.000000 th-0.3.2/th.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:19:50.591343 th-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 15:19:39.000000 th-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-22 15:19:50.591343 th-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-22 15:19:39.000000 th-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 15:19:50.591343 th-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-22 15:19:39.000000 th-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:19:50.587343 th-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4271 2023-06-22 15:19:39.000000 th-0.3.4/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-06-22 15:19:39.000000 th-0.3.4/tests/test_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-22 15:19:39.000000 th-0.3.4/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-22 15:19:39.000000 th-0.3.4/tests/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-22 15:19:39.000000 th-0.3.4/tests/test_path_holder_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-22 15:19:39.000000 th-0.3.4/tests/test_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:19:50.587343 th-0.3.4/th/
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-22 15:19:39.000000 th-0.3.4/th/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 15:19:39.000000 th-0.3.4/th/_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-22 15:19:39.000000 th-0.3.4/th/_path_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-22 15:19:39.000000 th-0.3.4/th/_path_holder_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 15:19:39.000000 th-0.3.4/th/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:19:50.591343 th-0.3.4/th/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-22 15:19:39.000000 th-0.3.4/th/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-22 15:19:39.000000 th-0.3.4/th/operators/_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 15:19:39.000000 th-0.3.4/th/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 15:19:50.591343 th-0.3.4/th.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-22 15:19:50.000000 th-0.3.4/th.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 15:19:50.000000 th-0.3.4/th.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 15:19:50.000000 th-0.3.4/th.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 15:19:50.000000 th-0.3.4/th.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-22 15:19:50.000000 th-0.3.4/th.egg-info/top_level.txt
```

### Comparing `th-0.3.2/LICENSE.txt` & `th-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `th-0.3.2/PKG-INFO` & `th-0.3.4/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: th
-Version: 0.3.2
+Version: 0.3.4
 Summary: Safely accessing deeply nested values
-Home-page: https://github.com/nikitanovosibirsk/th
+Home-page: https://github.com/tsv1/th
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # th
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/th/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/th)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/th/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/th)
 [![PyPI](https://img.shields.io/pypi/v/th.svg?style=flat-square)](https://pypi.python.org/pypi/th/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/th?style=flat-square)](https://pypi.python.org/pypi/th/)
 [![Python Version](https://img.shields.io/pypi/pyversions/th.svg?style=flat-square)](https://pypi.python.org/pypi/th/)
 
 ## Overview
 
 ```python
```

### Comparing `th-0.3.2/README.md` & `th-0.3.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # th
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/th/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/th)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/th/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/th)
 [![PyPI](https://img.shields.io/pypi/v/th.svg?style=flat-square)](https://pypi.python.org/pypi/th/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/th?style=flat-square)](https://pypi.python.org/pypi/th/)
 [![Python Version](https://img.shields.io/pypi/pyversions/th.svg?style=flat-square)](https://pypi.python.org/pypi/th/)
 
 ## Overview
 
 ```python
```

### Comparing `th-0.3.2/setup.cfg` & `th-0.3.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.3.2
+current_version = 0.3.4
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `th-0.3.2/setup.py` & `th-0.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="th",
-    version="0.3.2",
+    version="0.3.4",
     description="Safely accessing deeply nested values",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
-    url="https://github.com/nikitanovosibirsk/th",
+    url="https://github.com/tsv1/th",
     license="Apache-2.0",
-    packages=find_packages(exclude=("tests",)),
+    packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"th": ["py.typed"]},
     install_requires=find_required(),
     tests_require=find_dev_required(),
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
     ],
 )
```

### Comparing `th-0.3.2/th/__init__.py` & `th-0.3.4/th/__init__.py`

 * *Files identical despite different names*

### Comparing `th-0.3.2/th/_path_holder.py` & `th-0.3.4/th/_path_holder.py`

 * *Files identical despite different names*

### Comparing `th-0.3.2/th/_path_holder_proxy.py` & `th-0.3.4/th/_path_holder_proxy.py`

 * *Files identical despite different names*

### Comparing `th-0.3.2/th/operators/_operator.py` & `th-0.3.4/th/operators/_operator.py`

 * *Files identical despite different names*

### Comparing `th-0.3.2/th.egg-info/PKG-INFO` & `th-0.3.4/th.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: th
-Version: 0.3.2
+Version: 0.3.4
 Summary: Safely accessing deeply nested values
-Home-page: https://github.com/nikitanovosibirsk/th
+Home-page: https://github.com/tsv1/th
 Author: Nikita Tsvetkov
-Author-email: nikitanovosibirsk@yandex.com
+Author-email: tsv1@fastmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # th
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/th/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/th)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/th/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/th)
 [![PyPI](https://img.shields.io/pypi/v/th.svg?style=flat-square)](https://pypi.python.org/pypi/th/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/th?style=flat-square)](https://pypi.python.org/pypi/th/)
 [![Python Version](https://img.shields.io/pypi/pyversions/th.svg?style=flat-square)](https://pypi.python.org/pypi/th/)
 
 ## Overview
 
 ```python
```

