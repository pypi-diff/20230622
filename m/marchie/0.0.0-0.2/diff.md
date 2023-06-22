# Comparing `tmp/marchie-0.0.0.tar.gz` & `tmp/marchie-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marchie-0.0.0.tar", last modified: Thu Jun 22 07:02:32 2023, max compression
+gzip compressed data, was "marchie-0.2.tar", last modified: Thu Jun 22 06:57:02 2023, max compression
```

## Comparing `marchie-0.0.0.tar` & `marchie-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 07:02:32.857376 marchie-0.0.0/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     6704 2023-06-22 07:02:32.857147 marchie-0.0.0/PKG-INFO
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 07:02:32.854930 marchie-0.0.0/marchie/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     1839 2023-06-21 23:03:27.000000 marchie-0.0.0/marchie/__init__.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    21932 2023-06-21 23:03:23.000000 marchie-0.0.0/marchie/end_behavior.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    66537 2023-06-21 23:02:04.000000 marchie-0.0.0/marchie/marchie.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    12275 2023-06-21 19:09:49.000000 marchie-0.0.0/marchie/structure.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    53009 2023-06-21 23:03:22.000000 marchie-0.0.0/marchie/test.py
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 07:02:32.856742 marchie-0.0.0/marchie.egg-info/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     6704 2023-06-22 07:02:32.000000 marchie-0.0.0/marchie.egg-info/PKG-INFO
--rw-r--r--   0 maxschmaltz   (501) staff       (20)      262 2023-06-22 07:02:32.000000 marchie-0.0.0/marchie.egg-info/SOURCES.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)        1 2023-06-22 07:02:32.000000 marchie-0.0.0/marchie.egg-info/dependency_links.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)       15 2023-06-22 07:02:32.000000 marchie-0.0.0/marchie.egg-info/requires.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)        8 2023-06-22 07:02:32.000000 marchie-0.0.0/marchie.egg-info/top_level.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)       38 2023-06-22 07:02:32.857449 marchie-0.0.0/setup.cfg
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     1199 2023-06-22 07:00:55.000000 marchie-0.0.0/setup.py
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 06:57:02.443795 marchie-0.2/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     6700 2023-06-22 06:57:02.443555 marchie-0.2/PKG-INFO
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 06:57:02.441798 marchie-0.2/marchie/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     1839 2023-06-21 23:03:27.000000 marchie-0.2/marchie/__init__.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    21932 2023-06-21 23:03:23.000000 marchie-0.2/marchie/end_behavior.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    66537 2023-06-21 23:02:04.000000 marchie-0.2/marchie/marchie.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    12275 2023-06-21 19:09:49.000000 marchie-0.2/marchie/structure.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    53009 2023-06-21 23:03:22.000000 marchie-0.2/marchie/test.py
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 06:57:02.443028 marchie-0.2/marchie.egg-info/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     6700 2023-06-22 06:57:02.000000 marchie-0.2/marchie.egg-info/PKG-INFO
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)      262 2023-06-22 06:57:02.000000 marchie-0.2/marchie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)        1 2023-06-22 06:57:02.000000 marchie-0.2/marchie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)       15 2023-06-22 06:57:02.000000 marchie-0.2/marchie.egg-info/requires.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)        8 2023-06-22 06:57:02.000000 marchie-0.2/marchie.egg-info/top_level.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)       38 2023-06-22 06:57:02.443872 marchie-0.2/setup.cfg
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     1197 2023-06-22 06:54:28.000000 marchie-0.2/setup.py
```

### Comparing `marchie-0.0.0/PKG-INFO` & `marchie-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marchie
-Version: 0.0.0
+Version: 0.2
 Summary: MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
 Home-page: https://github.com/maxschmaltz/MarChie
 Author: Max Schmaltz
 Author-email: schmaltzmax@gmail.com
 License: Apache Software License
 Keywords: markov chain,mathematics
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 
 # MarChie: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
 
-[![Generic badge](https://img.shields.io/badge/PyPI-0.0.0-green.svg)](https://pypi.org/project/MarChie/)
+[![Generic badge](https://img.shields.io/badge/PyPI-0.1-green.svg)](https://pypi.org/project/MarChie/)
 [![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 
 
 ----------
```

### Comparing `marchie-0.0.0/marchie/__init__.py` & `marchie-0.2/marchie/__init__.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.0/marchie/end_behavior.py` & `marchie-0.2/marchie/end_behavior.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.0/marchie/marchie.py` & `marchie-0.2/marchie/marchie.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.0/marchie/structure.py` & `marchie-0.2/marchie/structure.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.0/marchie/test.py` & `marchie-0.2/marchie/test.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.0/marchie.egg-info/PKG-INFO` & `marchie-0.2/marchie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marchie
-Version: 0.0.0
+Version: 0.2
 Summary: MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
 Home-page: https://github.com/maxschmaltz/MarChie
 Author: Max Schmaltz
 Author-email: schmaltzmax@gmail.com
 License: Apache Software License
 Keywords: markov chain,mathematics
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 
 # MarChie: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
 
-[![Generic badge](https://img.shields.io/badge/PyPI-0.0.0-green.svg)](https://pypi.org/project/MarChie/)
+[![Generic badge](https://img.shields.io/badge/PyPI-0.1-green.svg)](https://pypi.org/project/MarChie/)
 [![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 
 
 ----------
```

### Comparing `marchie-0.0.0/setup.py` & `marchie-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 desc = '''
     MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
     '''
-with open('./marchie/README.md') as readme: long_description = readme.read()
+with open('./MarChie/README.md') as readme: long_description = readme.read()
 
 setuptools.setup(
     name='marchie',
-    version='0.0.0',
+    version='0.2',
     author='Max Schmaltz',
     author_email='schmaltzmax@gmail.com',
     description=desc,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/maxschmaltz/MarChie',
     packages=[
```

