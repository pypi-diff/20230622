# Comparing `tmp/marchie-0.0.2.tar.gz` & `tmp/marchie-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marchie-0.0.2.tar", last modified: Thu Jun 22 08:23:02 2023, max compression
+gzip compressed data, was "marchie-0.0.3.tar", last modified: Thu Jun 22 08:43:21 2023, max compression
```

## Comparing `marchie-0.0.2.tar` & `marchie-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:23:02.729572 marchie-0.0.2/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    11356 2023-06-21 19:22:24.000000 marchie-0.0.2/LICENSE
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     6726 2023-06-22 08:23:02.729334 marchie-0.0.2/PKG-INFO
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     5840 2023-06-22 08:22:05.000000 marchie-0.0.2/README.md
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:23:02.727739 marchie-0.0.2/marchie/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     1877 2023-06-22 08:17:43.000000 marchie-0.0.2/marchie/__init__.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    21932 2023-06-21 23:03:23.000000 marchie-0.0.2/marchie/end_behavior.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    66511 2023-06-22 07:39:53.000000 marchie-0.0.2/marchie/marchie.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    12275 2023-06-21 19:09:49.000000 marchie-0.0.2/marchie/structure.py
--rw-r--r--   0 maxschmaltz   (501) staff       (20)    53045 2023-06-22 08:17:58.000000 marchie-0.0.2/marchie/test.py
-drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:23:02.728920 marchie-0.0.2/marchie.egg-info/
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     6726 2023-06-22 08:23:02.000000 marchie-0.0.2/marchie.egg-info/PKG-INFO
--rw-r--r--   0 maxschmaltz   (501) staff       (20)      280 2023-06-22 08:23:02.000000 marchie-0.0.2/marchie.egg-info/SOURCES.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)        1 2023-06-22 08:23:02.000000 marchie-0.0.2/marchie.egg-info/dependency_links.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)       15 2023-06-22 08:23:02.000000 marchie-0.0.2/marchie.egg-info/requires.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)        8 2023-06-22 08:23:02.000000 marchie-0.0.2/marchie.egg-info/top_level.txt
--rw-r--r--   0 maxschmaltz   (501) staff       (20)       38 2023-06-22 08:23:02.729638 marchie-0.0.2/setup.cfg
--rw-r--r--   0 maxschmaltz   (501) staff       (20)     1240 2023-06-22 08:09:50.000000 marchie-0.0.2/setup.py
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:43:21.451887 marchie-0.0.3/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    11356 2023-06-21 19:22:24.000000 marchie-0.0.3/LICENSE
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     6726 2023-06-22 08:43:21.451352 marchie-0.0.3/PKG-INFO
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     5840 2023-06-22 08:22:05.000000 marchie-0.0.3/README.md
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:43:21.448649 marchie-0.0.3/marchie/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     1877 2023-06-22 08:17:43.000000 marchie-0.0.3/marchie/__init__.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    21932 2023-06-21 23:03:23.000000 marchie-0.0.3/marchie/end_behavior.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    66511 2023-06-22 08:38:26.000000 marchie-0.0.3/marchie/marchie.py
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    12275 2023-06-21 19:09:49.000000 marchie-0.0.3/marchie/structure.py
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:43:21.450318 marchie-0.0.3/marchie.egg-info/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     6726 2023-06-22 08:43:21.000000 marchie-0.0.3/marchie.egg-info/PKG-INFO
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)      278 2023-06-22 08:43:21.000000 marchie-0.0.3/marchie.egg-info/SOURCES.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)        1 2023-06-22 08:43:21.000000 marchie-0.0.3/marchie.egg-info/dependency_links.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)       15 2023-06-22 08:43:21.000000 marchie-0.0.3/marchie.egg-info/requires.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)        8 2023-06-22 08:43:21.000000 marchie-0.0.3/marchie.egg-info/top_level.txt
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)       38 2023-06-22 08:43:21.452144 marchie-0.0.3/setup.cfg
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)     1240 2023-06-22 08:36:15.000000 marchie-0.0.3/setup.py
+drwxr-xr-x   0 maxschmaltz   (501) staff       (20)        0 2023-06-22 08:43:21.450613 marchie-0.0.3/tests/
+-rw-r--r--   0 maxschmaltz   (501) staff       (20)    53045 2023-06-22 08:17:58.000000 marchie-0.0.3/tests/test.py
```

### Comparing `marchie-0.0.2/LICENSE` & `marchie-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `marchie-0.0.2/PKG-INFO` & `marchie-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marchie
-Version: 0.0.2
+Version: 0.0.3
 Summary: MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
 Home-page: https://github.com/maxschmaltz/MarChie
 Author: Max Schmaltz
 Author-email: schmaltzmax@gmail.com
 License: Apache Software License
 Keywords: markov chain,mathematics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `marchie-0.0.2/README.md` & `marchie-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `marchie-0.0.2/marchie/__init__.py` & `marchie-0.0.3/marchie/__init__.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.2/marchie/end_behavior.py` & `marchie-0.0.3/marchie/end_behavior.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.2/marchie/marchie.py` & `marchie-0.0.3/marchie/marchie.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.2/marchie/structure.py` & `marchie-0.0.3/marchie/structure.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.2/marchie/test.py` & `marchie-0.0.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `marchie-0.0.2/marchie.egg-info/PKG-INFO` & `marchie-0.0.3/marchie.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: marchie
-Version: 0.0.2
+Version: 0.0.3
 Summary: MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
 Home-page: https://github.com/maxschmaltz/MarChie
 Author: Max Schmaltz
 Author-email: schmaltzmax@gmail.com
 License: Apache Software License
 Keywords: markov chain,mathematics
 Classifier: Development Status :: 4 - Beta
```

### Comparing `marchie-0.0.2/setup.py` & `marchie-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 desc = '''
     MarChie: a Compact Open Source Tool for Analyzing Discrete Markov Chains.
     '''
 with open('./README.md') as readme: long_description = readme.read()
 
 setuptools.setup(
     name='marchie',
-    version='0.0.2',
+    version='0.0.3',
     author='Max Schmaltz',
     author_email='schmaltzmax@gmail.com',
     description=desc,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/maxschmaltz/MarChie',
     # packages=[
```

