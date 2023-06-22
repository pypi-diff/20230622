# Comparing `tmp/packed-0.2.2.tar.gz` & `tmp/packed-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packed-0.2.2.tar", last modified: Fri Nov  4 09:16:46 2022, max compression
+gzip compressed data, was "packed-0.2.3.tar", last modified: Thu Jun 22 17:22:14 2023, max compression
```

## Comparing `packed-0.2.2.tar` & `packed-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:16:46.641348 packed-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-04 09:16:40.000000 packed-0.2.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-11-04 09:16:46.641348 packed-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-11-04 09:16:40.000000 packed-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:16:46.641348 packed-0.2.2/packed/
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-11-04 09:16:40.000000 packed-0.2.2/packed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-11-04 09:16:40.000000 packed-0.2.2/packed/_packable.py
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-11-04 09:16:40.000000 packed-0.2.2/packed/_packer.py
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-11-04 09:16:40.000000 packed-0.2.2/packed/_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-04 09:16:40.000000 packed-0.2.2/packed/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 09:16:40.000000 packed-0.2.2/packed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:16:46.641348 packed-0.2.2/packed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-11-04 09:16:46.000000 packed-0.2.2/packed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-04 09:16:46.000000 packed-0.2.2/packed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 09:16:46.000000 packed-0.2.2/packed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-04 09:16:46.000000 packed-0.2.2/packed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-04 09:16:46.000000 packed-0.2.2/packed.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-11-04 09:16:46.641348 packed-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-11-04 09:16:40.000000 packed-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:22:14.814278 packed-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 17:22:00.000000 packed-0.2.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-22 17:22:14.814278 packed-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-22 17:22:00.000000 packed-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:22:14.814278 packed-0.2.3/packed/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-22 17:22:00.000000 packed-0.2.3/packed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-22 17:22:00.000000 packed-0.2.3/packed/_packable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-22 17:22:00.000000 packed-0.2.3/packed/_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-22 17:22:00.000000 packed-0.2.3/packed/_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 17:22:00.000000 packed-0.2.3/packed/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:22:00.000000 packed-0.2.3/packed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:22:14.814278 packed-0.2.3/packed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-22 17:22:14.000000 packed-0.2.3/packed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-22 17:22:14.000000 packed-0.2.3/packed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:22:14.000000 packed-0.2.3/packed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-22 17:22:14.000000 packed-0.2.3/packed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 17:22:14.000000 packed-0.2.3/packed.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-22 17:22:14.818277 packed-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 17:22:00.000000 packed-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:22:14.814278 packed-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-06-22 17:22:00.000000 packed-0.2.3/tests/test_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-22 17:22:00.000000 packed-0.2.3/tests/test_exported_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-22 17:22:00.000000 packed-0.2.3/tests/test_packable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-22 17:22:00.000000 packed-0.2.3/tests/test_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-06-22 17:22:00.000000 packed-0.2.3/tests/test_resolver.py
```

### Comparing `packed-0.2.2/LICENSE.txt` & `packed-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packed-0.2.2/PKG-INFO` & `packed-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: packed
-Version: 0.2.2
-Home-page: https://github.com/nikitanovosibirsk/packed
+Version: 0.2.3
+Home-page: https://github.com/tsv1/packed
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
 
 # packed
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/packed/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/packed)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/packed/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/packed)
 [![PyPI](https://img.shields.io/pypi/v/packed.svg?style=flat-square)](https://pypi.python.org/pypi/packed/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/packed?style=flat-square)](https://pypi.python.org/pypi/packed/)
 [![Python Version](https://img.shields.io/pypi/pyversions/packed.svg?style=flat-square)](https://pypi.python.org/pypi/packed/)
 
 ## Installation
 
 ```sh
```

### Comparing `packed-0.2.2/README.md` & `packed-0.2.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # packed
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/packed/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/packed)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/packed/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/packed)
 [![PyPI](https://img.shields.io/pypi/v/packed.svg?style=flat-square)](https://pypi.python.org/pypi/packed/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/packed?style=flat-square)](https://pypi.python.org/pypi/packed/)
 [![Python Version](https://img.shields.io/pypi/pyversions/packed.svg?style=flat-square)](https://pypi.python.org/pypi/packed/)
 
 ## Installation
 
 ```sh
```

### Comparing `packed-0.2.2/packed/__init__.py` & `packed-0.2.3/packed/__init__.py`

 * *Files identical despite different names*

### Comparing `packed-0.2.2/packed/_packable.py` & `packed-0.2.3/packed/_packable.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Union, cast
+from typing import Any, Union
 
 from ._resolver import AnyClass, Resolver
 
 __all__ = ("Packable",)
 
 
 class Packable:
@@ -11,11 +11,11 @@
 
     def __call__(self, cls_or_name: Union[str, AnyClass]) -> Any:
         if not isinstance(cls_or_name, str):
             self._resolver.register(cls=cls_or_name)
             return cls_or_name
 
         def wrapped(cls: AnyClass) -> AnyClass:
-            self._resolver.register(cls=cls, name=cast(str, cls_or_name))
+            self._resolver.register(cls=cls, name=cls_or_name)
             return cls
 
         return wrapped
```

### Comparing `packed-0.2.2/packed/_packer.py` & `packed-0.2.3/packed/_packer.py`

 * *Files identical despite different names*

### Comparing `packed-0.2.2/packed/_resolver.py` & `packed-0.2.3/packed/_resolver.py`

 * *Files identical despite different names*

### Comparing `packed-0.2.2/packed.egg-info/PKG-INFO` & `packed-0.2.3/packed.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: packed
-Version: 0.2.2
-Home-page: https://github.com/nikitanovosibirsk/packed
+Version: 0.2.3
+Home-page: https://github.com/tsv1/packed
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
 
 # packed
 
-[![Codecov](https://img.shields.io/codecov/c/github/nikitanovosibirsk/packed/master.svg?style=flat-square)](https://codecov.io/gh/nikitanovosibirsk/packed)
+[![Codecov](https://img.shields.io/codecov/c/github/tsv1/packed/master.svg?style=flat-square)](https://codecov.io/gh/tsv1/packed)
 [![PyPI](https://img.shields.io/pypi/v/packed.svg?style=flat-square)](https://pypi.python.org/pypi/packed/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/packed?style=flat-square)](https://pypi.python.org/pypi/packed/)
 [![Python Version](https://img.shields.io/pypi/pyversions/packed.svg?style=flat-square)](https://pypi.python.org/pypi/packed/)
 
 ## Installation
 
 ```sh
```

### Comparing `packed-0.2.2/setup.cfg` & `packed-0.2.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.2
+current_version = 0.2.3
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
```

### Comparing `packed-0.2.2/setup.py` & `packed-0.2.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,29 +9,30 @@
 def find_dev_required():
     with open("requirements-dev.txt") as f:
         return f.read().splitlines()
 
 
 setup(
     name="packed",
-    version="0.2.2",
+    version="0.2.3",
     description="",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="Nikita Tsvetkov",
-    author_email="nikitanovosibirsk@yandex.com",
+    author_email="tsv1@fastmail.com",
     python_requires=">=3.7",
-    url="https://github.com/nikitanovosibirsk/packed",
+    url="https://github.com/tsv1/packed",
     license="Apache-2.0",
-    packages=find_packages(exclude=("tests",)),
+    packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"packed": ["py.typed"]},
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

