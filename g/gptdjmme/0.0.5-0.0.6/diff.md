# Comparing `tmp/gptdjmme-0.0.5.tar.gz` & `tmp/gptdjmme-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gptdjmme-0.0.5.tar", last modified: Thu Jun 22 16:54:35 2023, max compression
+gzip compressed data, was "dist\gptdjmme-0.0.6.tar", last modified: Thu Jun 22 17:01:15 2023, max compression
```

## Comparing `gptdjmme-0.0.5.tar` & `gptdjmme-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 16:54:35.324283 gptdjmme-0.0.5/
--rw-rw-rw-   0        0        0     1967 2023-06-22 16:54:35.323284 gptdjmme-0.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 16:54:35.321287 gptdjmme-0.0.5/gptdjmme.egg-info/
--rw-rw-rw-   0        0        0     1967 2023-06-22 16:54:35.000000 gptdjmme-0.0.5/gptdjmme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2023-06-22 16:54:35.000000 gptdjmme-0.0.5/gptdjmme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 16:54:35.000000 gptdjmme-0.0.5/gptdjmme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-22 16:54:35.000000 gptdjmme-0.0.5/gptdjmme.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 16:54:35.000000 gptdjmme-0.0.5/gptdjmme.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 16:54:35.324283 gptdjmme-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1043 2023-06-22 16:54:25.000000 gptdjmme-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:01:15.890902 gptdjmme-0.0.6/
+-rw-rw-rw-   0        0        0     1967 2023-06-22 17:01:15.889888 gptdjmme-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-22 17:01:15.887887 gptdjmme-0.0.6/gptdjmme.egg-info/
+-rw-rw-rw-   0        0        0     1967 2023-06-22 17:01:15.000000 gptdjmme-0.0.6/gptdjmme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2023-06-22 17:01:15.000000 gptdjmme-0.0.6/gptdjmme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 17:01:15.000000 gptdjmme-0.0.6/gptdjmme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-22 17:01:15.000000 gptdjmme-0.0.6/gptdjmme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 17:01:15.000000 gptdjmme-0.0.6/gptdjmme.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 17:01:15.891888 gptdjmme-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1045 2023-06-22 17:01:14.000000 gptdjmme-0.0.6/setup.py
```

### Comparing `gptdjmme-0.0.5/PKG-INFO` & `gptdjmme-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdjmme
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package to clone yourself with GPT
 Author: Daniel J. McDonald
 Author-email: <daniel@danielmcdonald.dev>
 Keywords: python,gpt,openai,ai,chatbot,clone,me
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gptdjmme-0.0.5/gptdjmme.egg-info/PKG-INFO` & `gptdjmme-0.0.6/gptdjmme.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdjmme
-Version: 0.0.5
+Version: 0.0.6
 Summary: A python package to clone yourself with GPT
 Author: Daniel J. McDonald
 Author-email: <daniel@danielmcdonald.dev>
 Keywords: python,gpt,openai,ai,chatbot,clone,me
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gptdjmme-0.0.5/setup.py` & `gptdjmme-0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-with codecs.open(os.path.join(here, 'me_gpt/README.md'), encoding='utf-8') as f:
+with codecs.open(os.path.join(here, 'gptdjmme/README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'A python package to clone yourself with GPT'
 LONG_DESCRIPTION = 'A python package to clone yourself with GPT'
 
 # Setting up
 setup(
     name="gptdjmme",
     version=VERSION,
```

