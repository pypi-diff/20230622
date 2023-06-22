# Comparing `tmp/gptdjmme-0.0.7.tar.gz` & `tmp/gptdjmme-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gptdjmme-0.0.7.tar", last modified: Thu Jun 22 17:07:22 2023, max compression
+gzip compressed data, was "dist\gptdjmme-0.0.8.tar", last modified: Thu Jun 22 17:11:47 2023, max compression
```

## Comparing `gptdjmme-0.0.7.tar` & `gptdjmme-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 17:07:22.160550 gptdjmme-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-06-22 15:12:34.000000 gptdjmme-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1990 2023-06-22 17:07:22.159547 gptdjmme-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1467 2023-06-22 15:51:30.000000 gptdjmme-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-22 17:07:22.145525 gptdjmme-0.0.7/gptdjmme/
--rw-rw-rw-   0        0        0       17 2023-06-22 17:04:50.000000 gptdjmme-0.0.7/gptdjmme/__init__.py
--rw-rw-rw-   0        0        0     5543 2023-06-22 14:39:21.000000 gptdjmme-0.0.7/gptdjmme/ai.py
--rw-rw-rw-   0        0        0     1837 2023-06-22 14:06:33.000000 gptdjmme-0.0.7/gptdjmme/db.py
--rw-rw-rw-   0        0        0      117 2023-06-22 16:28:12.000000 gptdjmme-0.0.7/gptdjmme/main.py
-drwxrwxrwx   0        0        0        0 2023-06-22 17:07:22.157547 gptdjmme-0.0.7/gptdjmme.egg-info/
--rw-rw-rw-   0        0        0     1990 2023-06-22 17:07:22.000000 gptdjmme-0.0.7/gptdjmme.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-06-22 17:07:22.000000 gptdjmme-0.0.7/gptdjmme.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 17:07:22.000000 gptdjmme-0.0.7/gptdjmme.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-22 17:07:22.000000 gptdjmme-0.0.7/gptdjmme.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-22 17:07:22.000000 gptdjmme-0.0.7/gptdjmme.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 17:07:22.161553 gptdjmme-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1036 2023-06-22 17:07:02.000000 gptdjmme-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:11:47.750229 gptdjmme-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-06-22 15:12:34.000000 gptdjmme-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1990 2023-06-22 17:11:47.749232 gptdjmme-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1467 2023-06-22 15:51:30.000000 gptdjmme-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 17:11:47.736599 gptdjmme-0.0.8/gptdjmme/
+-rw-rw-rw-   0        0        0       36 2023-06-22 17:11:03.000000 gptdjmme-0.0.8/gptdjmme/__init__.py
+-rw-rw-rw-   0        0        0     5543 2023-06-22 17:10:53.000000 gptdjmme-0.0.8/gptdjmme/ai.py
+-rw-rw-rw-   0        0        0     1837 2023-06-22 14:06:33.000000 gptdjmme-0.0.8/gptdjmme/db.py
+-rw-rw-rw-   0        0        0      117 2023-06-22 16:28:12.000000 gptdjmme-0.0.8/gptdjmme/main.py
+drwxrwxrwx   0        0        0        0 2023-06-22 17:11:47.747234 gptdjmme-0.0.8/gptdjmme.egg-info/
+-rw-rw-rw-   0        0        0     1990 2023-06-22 17:11:47.000000 gptdjmme-0.0.8/gptdjmme.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-06-22 17:11:47.000000 gptdjmme-0.0.8/gptdjmme.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 17:11:47.000000 gptdjmme-0.0.8/gptdjmme.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-06-22 17:11:47.000000 gptdjmme-0.0.8/gptdjmme.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-22 17:11:47.000000 gptdjmme-0.0.8/gptdjmme.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 17:11:47.751230 gptdjmme-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1036 2023-06-22 17:11:35.000000 gptdjmme-0.0.8/setup.py
```

### Comparing `gptdjmme-0.0.7/LICENSE` & `gptdjmme-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gptdjmme-0.0.7/PKG-INFO` & `gptdjmme-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdjmme
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to clone yourself with GPT
 Author: Daniel J. McDonald
 Author-email: <daniel@danielmcdonald.dev>
 Keywords: python,gpt,openai,ai,chatbot,clone,me
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gptdjmme-0.0.7/README.md` & `gptdjmme-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gptdjmme-0.0.7/gptdjmme/ai.py` & `gptdjmme-0.0.8/gptdjmme/ai.py`

 * *Files identical despite different names*

### Comparing `gptdjmme-0.0.7/gptdjmme/db.py` & `gptdjmme-0.0.8/gptdjmme/db.py`

 * *Files identical despite different names*

### Comparing `gptdjmme-0.0.7/gptdjmme.egg-info/PKG-INFO` & `gptdjmme-0.0.8/gptdjmme.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdjmme
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to clone yourself with GPT
 Author: Daniel J. McDonald
 Author-email: <daniel@danielmcdonald.dev>
 Keywords: python,gpt,openai,ai,chatbot,clone,me
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gptdjmme-0.0.7/setup.py` & `gptdjmme-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'A python package to clone yourself with GPT'
 LONG_DESCRIPTION = 'A python package to clone yourself with GPT'
 
 # Setting up
 setup(
     name="gptdjmme",
     version=VERSION,
```

