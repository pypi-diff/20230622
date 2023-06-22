# Comparing `tmp/MarChie-0.1.tar.gz` & `tmp/marchie-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MarChie-0.1.tar", last modified: Wed Jun 21 23:14:59 2023, max compression
+gzip compressed data, was "marchie-0.2.tar", last modified: Thu Jun 22 06:57:02 2023, max compression
```

## Comparing `MarChie-0.1.tar` & `marchie-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-21 23:14:59.280019 MarChie-0.1/
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-21 23:14:59.278677 MarChie-0.1/MarChie/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     1839 2023-06-21 23:03:27.000000 MarChie-0.1/MarChie/__init__.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    21932 2023-06-21 23:03:23.000000 MarChie-0.1/MarChie/end_behavior.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    66537 2023-06-21 23:02:04.000000 MarChie-0.1/MarChie/marchie.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    12275 2023-06-21 19:09:49.000000 MarChie-0.1/MarChie/structure.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    53009 2023-06-21 23:03:22.000000 MarChie-0.1/MarChie/test.py
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-21 23:14:59.279471 MarChie-0.1/MarChie.egg-info/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     6687 2023-06-21 23:14:59.000000 MarChie-0.1/MarChie.egg-info/PKG-INFO
--rw-r--r--   0 maxschmaltz   (501) staff       (20)      262 2023-06-21 23:14:59.000000 MarChie-0.1/MarChie.egg-info/SOURCES.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)        1 2023-06-21 23:14:59.000000 MarChie-0.1/MarChie.egg-info/dependency_links.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)       15 2023-06-21 23:14:59.000000 MarChie-0.1/MarChie.egg-info/requires.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)        8 2023-06-21 23:14:59.000000 MarChie-0.1/MarChie.egg-info/top_level.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     6687 2023-06-21 23:14:59.279849 MarChie-0.1/PKG-INFO
--rw-r--r--   0 maxschmaltz   (501) staff       (20)       38 2023-06-21 23:14:59.280069 MarChie-0.1/setup.cfg
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     1197 2023-06-21 23:14:44.000000 MarChie-0.1/setup.py
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

### Comparing `MarChie-0.1/MarChie/__init__.py` & `marchie-0.2/marchie/__init__.py`

 * *Files identical despite different names*

### Comparing `MarChie-0.1/MarChie/end_behavior.py` & `marchie-0.2/marchie/end_behavior.py`

 * *Files identical despite different names*

### Comparing `MarChie-0.1/MarChie/marchie.py` & `marchie-0.2/marchie/marchie.py`

 * *Files identical despite different names*

### Comparing `MarChie-0.1/MarChie/structure.py` & `marchie-0.2/marchie/structure.py`

 * *Files identical despite different names*

### Comparing `MarChie-0.1/MarChie/test.py` & `marchie-0.2/marchie/test.py`

 * *Files identical despite different names*

### Comparing `MarChie-0.1/MarChie.egg-info/PKG-INFO` & `marchie-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: MarChie
-Version: 0.1
+Name: marchie
+Version: 0.2
 Summary: MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
 Home-page: https://github.com/maxschmaltz/MarChie
 Author: Max Schmaltz
 Author-email: schmaltzmax@gmail.com
 License: Apache Software License
 Keywords: markov chain,mathematics
 Classifier: Development Status :: 4 - Beta
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 
-# `MarChie`: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
+# MarChie: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
 
-[![PyPI version](https://badge.fury.io/py/MarChie.svg)](https://badge.fury.io/py/MarChie)
+[![Generic badge](https://img.shields.io/badge/PyPI-0.1-green.svg)](https://pypi.org/project/MarChie/)
 [![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 
 
 ----------
 
@@ -93,20 +93,20 @@
 
 `March` is a `pip`-installable package. You can access it directly from PyPI:
 
 ```bash
 pip install MarChie
 ```
 
-The main object that is really intended to be used is `class MarChie.marchie.March`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
+The main object that is really intended to be used is `class marchie.marchie.March`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
 
 ```python
 
 >>> import numpy as np
->>> from March.marchie import March
+>>> from marchie.marchie import March
 
 >>> trans_mat = np.array([
     [1,     0,     0  ],
     [0.8,   0.2,   0  ],
     [0.3,   0.5,   0.2]
 ])
 >>> init_distr = np.array(
```

### Comparing `MarChie-0.1/PKG-INFO` & `marchie-0.2/marchie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: MarChie
-Version: 0.1
+Name: marchie
+Version: 0.2
 Summary: MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
 Home-page: https://github.com/maxschmaltz/MarChie
 Author: Max Schmaltz
 Author-email: schmaltzmax@gmail.com
 License: Apache Software License
 Keywords: markov chain,mathematics
 Classifier: Development Status :: 4 - Beta
@@ -15,17 +15,17 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 
-# `MarChie`: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
+# MarChie: a Compact Open Source Tool for Analyzing Discrete **Mar**kov **Ch**ains
 
-[![PyPI version](https://badge.fury.io/py/MarChie.svg)](https://badge.fury.io/py/MarChie)
+[![Generic badge](https://img.shields.io/badge/PyPI-0.1-green.svg)](https://pypi.org/project/MarChie/)
 [![Generic badge](https://img.shields.io/badge/GitHub-Source-red.svg)](https://github.com/maxschmaltz/MarChie)
 [![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 
 
 ----------
 
@@ -93,20 +93,20 @@
 
 `March` is a `pip`-installable package. You can access it directly from PyPI:
 
 ```bash
 pip install MarChie
 ```
 
-The main object that is really intended to be used is `class MarChie.marchie.March`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
+The main object that is really intended to be used is `class marchie.marchie.March`. The class requires only transition probability matrix and (optionally) initial state probability distribution vector as arguments; if you provide no initial distribution vector, it will be generated.
 
 ```python
 
 >>> import numpy as np
->>> from March.marchie import March
+>>> from marchie.marchie import March
 
 >>> trans_mat = np.array([
     [1,     0,     0  ],
     [0.8,   0.2,   0  ],
     [0.3,   0.5,   0.2]
 ])
 >>> init_distr = np.array(
```

### Comparing `MarChie-0.1/setup.py` & `marchie-0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 desc = '''
     MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
     '''
 with open('./MarChie/README.md') as readme: long_description = readme.read()
 
 setuptools.setup(
-    name='MarChie',
-    version='0.1',
+    name='marchie',
+    version='0.2',
     author='Max Schmaltz',
     author_email='schmaltzmax@gmail.com',
     description=desc,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/maxschmaltz/MarChie',
     packages=[
-        'MarChie'
+        'marchie'
     ],
     install_requires=[
         'numpy',
         'graphviz'
     ],
     license='Apache Software License',
     keywords='markov chain, mathematics',
```

