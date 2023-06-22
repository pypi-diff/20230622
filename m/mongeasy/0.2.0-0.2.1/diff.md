# Comparing `tmp/mongeasy-0.2.0.tar.gz` & `tmp/mongeasy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongeasy-0.2.0.tar", last modified: Thu Jun 22 11:20:02 2023, max compression
+gzip compressed data, was "mongeasy-0.2.1.tar", last modified: Thu Jun 22 13:24:46 2023, max compression
```

## Comparing `mongeasy-0.2.0.tar` & `mongeasy-0.2.1.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.565595 mongeasy-0.2.0/
--rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 mongeasy-0.2.0/LICENSE
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.486252 mongeasy-0.2.0/Mongeasy.egg-info/
--rw-r--r--   0 javv       (501) staff       (20)    19200 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/PKG-INFO
--rw-r--r--   0 javv       (501) staff       (20)     1070 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/SOURCES.txt
--rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/dependency_links.txt
--rw-r--r--   0 javv       (501) staff       (20)       47 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/entry_points.txt
--rw-r--r--   0 javv       (501) staff       (20)       15 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/requires.txt
--rw-r--r--   0 javv       (501) staff       (20)       30 2023-06-22 11:20:02.000000 mongeasy-0.2.0/Mongeasy.egg-info/top_level.txt
--rw-r--r--   0 javv       (501) staff       (20)    19200 2023-06-22 11:20:02.565718 mongeasy-0.2.0/PKG-INFO
--rw-r--r--   0 javv       (501) staff       (20)    18389 2023-06-22 10:57:41.000000 mongeasy-0.2.0/README.md
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.517148 mongeasy-0.2.0/mongeasy/
--rw-r--r--   0 javv       (501) staff       (20)      645 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/base_dict.py
--rw-r--r--   0 javv       (501) staff       (20)     3557 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/connection.py
--rw-r--r--   0 javv       (501) staff       (20)     4349 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/core.py
--rw-r--r--   0 javv       (501) staff       (20)    14041 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/document.py
--rw-r--r--   0 javv       (501) staff       (20)     2696 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/dynamics.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.518563 mongeasy-0.2.0/mongeasy/examples/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/examples/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/exceptions.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.523055 mongeasy-0.2.0/mongeasy/plugins/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/plugins/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     4101 2023-06-22 10:57:41.000000 mongeasy-0.2.0/mongeasy/plugins/registry.py
--rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/resultlist.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.527867 mongeasy-0.2.0/mongeasy/utils/
--rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/utils/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 mongeasy-0.2.0/mongeasy/utils/utils.py
--rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 mongeasy-0.2.0/pyproject.toml
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.555198 mongeasy-0.2.0/sample_plugins/
--rw-r--r--   0 javv       (501) staff       (20)      786 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)      366 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/connection_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      290 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/delete_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      299 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/init_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      576 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/pydantic_validator.py
--rw-r--r--   0 javv       (501) staff       (20)      356 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/query_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      295 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/save_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)      347 2023-06-22 10:57:41.000000 mongeasy-0.2.0/sample_plugins/validator_plugin.py
--rw-r--r--   0 javv       (501) staff       (20)     1013 2023-06-22 11:20:02.566931 mongeasy-0.2.0/setup.cfg
--rw-r--r--   0 javv       (501) staff       (20)     1072 2023-06-22 10:57:41.000000 mongeasy-0.2.0/setup.py
-drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 11:20:02.564971 mongeasy-0.2.0/tests/
--rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 mongeasy-0.2.0/tests/__init__.py
--rw-r--r--   0 javv       (501) staff       (20)    13161 2023-06-22 10:57:41.000000 mongeasy-0.2.0/tests/test_mongeasy.py
--rw-r--r--   0 javv       (501) staff       (20)     2508 2023-06-22 10:57:41.000000 mongeasy-0.2.0/tests/test_plugins.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.400606 mongeasy-0.2.1/
+-rw-r--r--   0 javv       (501) staff       (20)     1074 2023-06-03 04:53:57.000000 mongeasy-0.2.1/LICENSE
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.375086 mongeasy-0.2.1/Mongeasy.egg-info/
+-rw-r--r--   0 javv       (501) staff       (20)    19125 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)      990 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/SOURCES.txt
+-rw-r--r--   0 javv       (501) staff       (20)        1 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/dependency_links.txt
+-rw-r--r--   0 javv       (501) staff       (20)      822 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/requires.txt
+-rw-r--r--   0 javv       (501) staff       (20)       30 2023-06-22 13:24:46.000000 mongeasy-0.2.1/Mongeasy.egg-info/top_level.txt
+-rw-r--r--   0 javv       (501) staff       (20)    19125 2023-06-22 13:24:46.399958 mongeasy-0.2.1/PKG-INFO
+-rw-r--r--   0 javv       (501) staff       (20)    18389 2023-06-22 10:57:41.000000 mongeasy-0.2.1/README.md
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.386446 mongeasy-0.2.1/mongeasy/
+-rw-r--r--   0 javv       (501) staff       (20)      623 2023-06-22 13:22:39.000000 mongeasy-0.2.1/mongeasy/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     2692 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/base_dict.py
+-rw-r--r--   0 javv       (501) staff       (20)     3557 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/connection.py
+-rw-r--r--   0 javv       (501) staff       (20)     4349 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/core.py
+-rw-r--r--   0 javv       (501) staff       (20)    14041 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/document.py
+-rw-r--r--   0 javv       (501) staff       (20)     2696 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/dynamics.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.387584 mongeasy-0.2.1/mongeasy/examples/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/examples/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1792 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/exceptions.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.388846 mongeasy-0.2.1/mongeasy/plugins/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     4101 2023-06-22 10:57:41.000000 mongeasy-0.2.1/mongeasy/plugins/registry.py
+-rw-r--r--   0 javv       (501) staff       (20)     4842 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/resultlist.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.389968 mongeasy-0.2.1/mongeasy/utils/
+-rw-r--r--   0 javv       (501) staff       (20)        0 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/utils/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)     1755 2023-06-03 04:53:57.000000 mongeasy-0.2.1/mongeasy/utils/utils.py
+-rw-r--r--   0 javv       (501) staff       (20)       89 2023-06-03 04:53:57.000000 mongeasy-0.2.1/pyproject.toml
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.396902 mongeasy-0.2.1/sample_plugins/
+-rw-r--r--   0 javv       (501) staff       (20)      786 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)      366 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/connection_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      290 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/delete_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      299 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/init_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      576 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/pydantic_validator.py
+-rw-r--r--   0 javv       (501) staff       (20)      356 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/query_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      295 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/save_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)      347 2023-06-22 10:57:41.000000 mongeasy-0.2.1/sample_plugins/validator_plugin.py
+-rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-22 13:24:46.400821 mongeasy-0.2.1/setup.cfg
+-rw-r--r--   0 javv       (501) staff       (20)     1206 2023-06-22 13:23:53.000000 mongeasy-0.2.1/setup.py
+drwxr-xr-x   0 javv       (501) staff       (20)        0 2023-06-22 13:24:46.399501 mongeasy-0.2.1/tests/
+-rw-r--r--   0 javv       (501) staff       (20)       38 2023-06-03 04:53:57.000000 mongeasy-0.2.1/tests/__init__.py
+-rw-r--r--   0 javv       (501) staff       (20)    13161 2023-06-22 10:57:41.000000 mongeasy-0.2.1/tests/test_mongeasy.py
+-rw-r--r--   0 javv       (501) staff       (20)     2508 2023-06-22 10:57:41.000000 mongeasy-0.2.1/tests/test_plugins.py
```

### Comparing `mongeasy-0.2.0/LICENSE` & `mongeasy-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/Mongeasy.egg-info/PKG-INFO` & `mongeasy-0.2.1/Mongeasy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mongeasy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
-Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mongeasy-0.2.0/Mongeasy.egg-info/SOURCES.txt` & `mongeasy-0.2.1/Mongeasy.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 setup.py
 Mongeasy.egg-info/PKG-INFO
 Mongeasy.egg-info/SOURCES.txt
 Mongeasy.egg-info/dependency_links.txt
-Mongeasy.egg-info/entry_points.txt
 Mongeasy.egg-info/requires.txt
 Mongeasy.egg-info/top_level.txt
 mongeasy/__init__.py
 mongeasy/base_dict.py
 mongeasy/connection.py
 mongeasy/core.py
 mongeasy/document.py
 mongeasy/dynamics.py
 mongeasy/exceptions.py
 mongeasy/resultlist.py
 mongeasy.egg-info/PKG-INFO
 mongeasy.egg-info/SOURCES.txt
 mongeasy.egg-info/dependency_links.txt
-mongeasy.egg-info/entry_points.txt
 mongeasy.egg-info/requires.txt
 mongeasy.egg-info/top_level.txt
 mongeasy/examples/__init__.py
 mongeasy/plugins/__init__.py
 mongeasy/plugins/registry.py
 mongeasy/utils/__init__.py
 mongeasy/utils/utils.py
```

### Comparing `mongeasy-0.2.0/PKG-INFO` & `mongeasy-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: mongeasy
-Version: 0.2.0
+Version: 0.2.1
 Summary: Easy to use wrapper around pymongo for easy access to MongoDB.
 Home-page: https://github.com/artheadsweden/mongeasy
 Author: Joakim Wassberg
 Author-email: joakim.wassberg@arthead.se
 License: MIT
-Project-URL: Bug Tracker, https://github.com/artheadsweden/mongeasy/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `mongeasy-0.2.0/README.md` & `mongeasy-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/__init__.py` & `mongeasy-0.2.1/mongeasy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Top-level package for Mongeasy."""
 
 __author__ = """Joakim Wassberg"""
 __email__ = 'joakim.wassberg@arthead.se'
-__version__ = '0.2.0'
 
 from mongeasy.connection import MongeasyConnection
 from mongeasy.exceptions import MongeasyDBConnectionError
 from mongeasy.dynamics import create_document_class
 from mongeasy.core import Query
 from mongeasy.plugins.registry import PluginRegistry, Hook, plugin_dispatcher
```

### Comparing `mongeasy-0.2.0/mongeasy/base_dict.py` & `mongeasy-0.2.1/mongeasy/base_dict.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/connection.py` & `mongeasy-0.2.1/mongeasy/connection.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/core.py` & `mongeasy-0.2.1/mongeasy/core.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/document.py` & `mongeasy-0.2.1/mongeasy/document.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/dynamics.py` & `mongeasy-0.2.1/mongeasy/dynamics.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/exceptions.py` & `mongeasy-0.2.1/mongeasy/exceptions.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/plugins/registry.py` & `mongeasy-0.2.1/mongeasy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/resultlist.py` & `mongeasy-0.2.1/mongeasy/resultlist.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/mongeasy/utils/utils.py` & `mongeasy-0.2.1/mongeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/sample_plugins/__init__.py` & `mongeasy-0.2.1/sample_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/sample_plugins/pydantic_validator.py` & `mongeasy-0.2.1/sample_plugins/pydantic_validator.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/setup.py` & `mongeasy-0.2.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
+def parse_requirements(filename):
+    with open(filename, 'r') as file:
+        return file.read().splitlines()
+
+
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 with open("LICENSE", encoding="utf8") as f:
     license = f.read()
 
 setup(
     name="mongeasy",
-    version="0.2.0",
+    version="0.2.1",
     author="Joakim Wassberg",
     author_email="joakim.wassberg@arthead.se",
     description="Easy to use wrapper around pymongo for easy access to MongoDB.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/artheadsweden/mongeasy",
     license="MIT",
@@ -26,9 +31,9 @@
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Database",
     ],
     packages=find_packages(),
-    install_requires=["pymongo>=4.3.3"],
+    install_requires=parse_requirements('requirements.txt'),
 )
```

### Comparing `mongeasy-0.2.0/tests/test_mongeasy.py` & `mongeasy-0.2.1/tests/test_mongeasy.py`

 * *Files identical despite different names*

### Comparing `mongeasy-0.2.0/tests/test_plugins.py` & `mongeasy-0.2.1/tests/test_plugins.py`

 * *Files identical despite different names*

