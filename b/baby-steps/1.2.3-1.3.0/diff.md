# Comparing `tmp/baby-steps-1.2.3.tar.gz` & `tmp/baby-steps-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baby-steps-1.2.3.tar", last modified: Fri Nov  4 09:59:03 2022, max compression
+gzip compressed data, was "baby-steps-1.3.0.tar", last modified: Thu Jun 22 17:15:52 2023, max compression
```

## Comparing `baby-steps-1.2.3.tar` & `baby-steps-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:59:03.401591 baby-steps-1.2.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-04 09:58:53.000000 baby-steps-1.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-11-04 09:59:03.401591 baby-steps-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2134 2022-11-04 09:58:53.000000 baby-steps-1.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:59:03.401591 baby-steps-1.2.3/baby_steps/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-04 09:58:53.000000 baby-steps-1.2.3/baby_steps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1411 2022-11-04 09:58:53.000000 baby-steps-1.2.3/baby_steps/_step.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-11-04 09:58:53.000000 baby-steps-1.2.3/baby_steps/hooks.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 09:58:53.000000 baby-steps-1.2.3/baby_steps/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 09:59:03.401591 baby-steps-1.2.3/baby_steps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-11-04 09:59:03.000000 baby-steps-1.2.3/baby_steps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-04 09:59:03.000000 baby-steps-1.2.3/baby_steps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 09:59:03.000000 baby-steps-1.2.3/baby_steps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-04 09:59:03.000000 baby-steps-1.2.3/baby_steps.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-11-04 09:59:03.401591 baby-steps-1.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      855 2022-11-04 09:58:53.000000 baby-steps-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:15:52.540635 baby-steps-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 17:15:40.000000 baby-steps-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-22 17:15:52.540635 baby-steps-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-22 17:15:40.000000 baby-steps-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:15:52.540635 baby-steps-1.3.0/baby_steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-22 17:15:40.000000 baby-steps-1.3.0/baby_steps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-22 17:15:40.000000 baby-steps-1.3.0/baby_steps/_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-22 17:15:40.000000 baby-steps-1.3.0/baby_steps/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 17:15:40.000000 baby-steps-1.3.0/baby_steps/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:15:52.540635 baby-steps-1.3.0/baby_steps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-06-22 17:15:52.000000 baby-steps-1.3.0/baby_steps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-22 17:15:52.000000 baby-steps-1.3.0/baby_steps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 17:15:52.000000 baby-steps-1.3.0/baby_steps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 17:15:52.000000 baby-steps-1.3.0/baby_steps.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-22 17:15:52.544635 baby-steps-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-22 17:15:40.000000 baby-steps-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 17:15:52.540635 baby-steps-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4608 2023-06-22 17:15:40.000000 baby-steps-1.3.0/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-06-22 17:15:40.000000 baby-steps-1.3.0/tests/test_steps.py
```

### Comparing `baby-steps-1.2.3/LICENSE` & `baby-steps-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `baby-steps-1.2.3/PKG-INFO` & `baby-steps-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: baby-steps
-Version: 1.2.3
+Version: 1.3.0
 Summary: Readability Matters
-Home-page: https://github.com/nikitanovosibirsk/baby-steps
+Home-page: https://github.com/tsv1/baby-steps
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
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Baby Steps
 
 [![PyPI](https://img.shields.io/pypi/v/baby-steps.svg?style=flat-square)](https://pypi.python.org/pypi/baby-steps/)
```

### Comparing `baby-steps-1.2.3/README.md` & `baby-steps-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `baby-steps-1.2.3/baby_steps.egg-info/PKG-INFO` & `baby-steps-1.3.0/baby_steps.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: baby-steps
-Version: 1.2.3
+Version: 1.3.0
 Summary: Readability Matters
-Home-page: https://github.com/nikitanovosibirsk/baby-steps
+Home-page: https://github.com/tsv1/baby-steps
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
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Baby Steps
 
 [![PyPI](https://img.shields.io/pypi/v/baby-steps.svg?style=flat-square)](https://pypi.python.org/pypi/baby-steps/)
```

### Comparing `baby-steps-1.2.3/setup.cfg` & `baby-steps-1.3.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.2.3
+current_version = 1.3.0
 message = bump version → {new_version}
 commit = True
 tag = True
 sign_tags = True
 
 [bumpversion:file:setup.py]
 
@@ -35,12 +35,13 @@
 
 [tool:pytest]
 testpaths = tests/
 python_files = test_*.py
 python_classes = 
 python_functions = test_*
 markers = only
+asyncio_mode = auto
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

