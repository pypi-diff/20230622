# Comparing `tmp/assistant_improve_toolkit-1.3.8.tar.gz` & `tmp/assistant_improve_toolkit-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/assistant_improve_toolkit-1.3.8.tar", last modified: Tue Jun 14 16:31:38 2022, max compression
+gzip compressed data, was "assistant_improve_toolkit-1.3.9.tar", last modified: Thu Jun 22 21:07:54 2023, max compression
```

## Comparing `assistant_improve_toolkit-1.3.8.tar` & `assistant_improve_toolkit-1.3.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/
--rwxr-xr-x   0 runner    (1001) docker     (121)    10174 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6931 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6108 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    47406 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/computation_func.py
--rw-r--r--   0 runner    (1001) docker     (121)    15438 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/cos_op.py
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4242 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/fetch_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/version.py
--rw-r--r--   0 runner    (1001) docker     (121)   109055 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/visualize_func.py
--rw-r--r--   0 runner    (1001) docker     (121)    12611 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/watson_assistant_func.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6931 2022-06-14 16:31:37.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 16:31:37.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-14 16:31:37.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/src/main/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-14 16:31:38.000000 assistant_improve_toolkit-1.3.8/src/main/python/
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    46395 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/python/computation_func.py
--rw-r--r--   0 runner    (1001) docker     (121)    15438 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/python/cos_op.py
--rw-r--r--   0 runner    (1001) docker     (121)     2868 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/python/export_csv_for_intent_recommendation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4242 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/python/fetch_logs.py
--rw-r--r--   0 runner    (1001) docker     (121)   107935 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/python/visualize_func.py
--rw-r--r--   0 runner    (1001) docker     (121)    10984 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/python/watson_assistant_func.py
--rw-r--r--   0 runner    (1001) docker     (121)     6296 2022-06-14 16:29:28.000000 assistant_improve_toolkit-1.3.8/src/main/python/watson_assistant_func_skip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.384123 assistant_improve_toolkit-1.3.9/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10174 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-22 21:07:54.384123 assistant_improve_toolkit-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-22 21:07:54.384123 assistant_improve_toolkit-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.376123 assistant_improve_toolkit-1.3.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.380123 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47406 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/computation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/cos_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/fetch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109055 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/visualize_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12611 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/watson_assistant_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.380123 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 21:07:54.000000 assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.380123 assistant_improve_toolkit-1.3.9/src/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 21:07:54.384123 assistant_improve_toolkit-1.3.9/src/main/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46395 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/computation_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/cos_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/export_csv_for_intent_recommendation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/fetch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107935 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/visualize_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/watson_assistant_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-06-22 20:50:35.000000 assistant_improve_toolkit-1.3.9/src/main/python/watson_assistant_func_skip.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `assistant_improve_toolkit-1.3.8/LICENSE` & `assistant_improve_toolkit-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/PKG-INFO` & `assistant_improve_toolkit-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant_improve_toolkit
-Version: 1.3.8
+Version: 1.3.9
 Summary: Assistant Improve Toolkit
 Home-page: https://github.com/watson-developer-cloud/assistant-improve-recommendations-notebook
 Author: IBM Watson
 Author-email: watdevex@us.ibm.com
 Maintainer: Zhe Zhang
 Maintainer-email: zhangzhe@us.ibm.com
 License: Apache 2.0
```

### Comparing `assistant_improve_toolkit-1.3.8/README.md` & `assistant_improve_toolkit-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/setup.py` & `assistant_improve_toolkit-1.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 # Learn more about it at: http://github.com/fabiommendes/python-boilerplate/
 #
 
 import setuptools
 from os import path
 
-__version__ = '1.3.7'
+__version__ = '1.3.8'
 
 # read contents of README file
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as file:
     readme_file = file.read()
 
 setuptools.setup(
@@ -45,14 +45,14 @@
         'pandas==1.2.1',
         'bokeh==2.0.0',
         'tqdm==4.43.0',
         'scikit-learn>=0.21.3',
         'matplotlib==3.2.1',
         'XlsxWriter==1.2.8',
         'ibm-watson==5.1.0',
-        'numpy==1.20.3',
+        'numpy==1.25.0',
         'requests==2.26'
     ],
 
     zip_safe=False,
     platforms='any',
 )
```

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/__init__.py` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/computation_func.py` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/computation_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/cos_op.py` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/cos_op.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/export_csv_for_intent_recommendation.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/fetch_logs.py` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/visualize_func.py` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/visualize_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit/watson_assistant_func.py` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit/watson_assistant_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/PKG-INFO` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assistant-improve-toolkit
-Version: 1.3.8
+Version: 1.3.9
 Summary: Assistant Improve Toolkit
 Home-page: https://github.com/watson-developer-cloud/assistant-improve-recommendations-notebook
 Author: IBM Watson
 Author-email: watdevex@us.ibm.com
 Maintainer: Zhe Zhang
 Maintainer-email: zhangzhe@us.ibm.com
 License: Apache 2.0
```

### Comparing `assistant_improve_toolkit-1.3.8/src/assistant_improve_toolkit.egg-info/SOURCES.txt` & `assistant_improve_toolkit-1.3.9/src/assistant_improve_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/main/python/__init__.py` & `assistant_improve_toolkit-1.3.9/src/main/python/__init__.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/main/python/computation_func.py` & `assistant_improve_toolkit-1.3.9/src/main/python/computation_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/main/python/cos_op.py` & `assistant_improve_toolkit-1.3.9/src/main/python/cos_op.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/main/python/export_csv_for_intent_recommendation.py` & `assistant_improve_toolkit-1.3.9/src/main/python/export_csv_for_intent_recommendation.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/main/python/fetch_logs.py` & `assistant_improve_toolkit-1.3.9/src/main/python/fetch_logs.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/main/python/visualize_func.py` & `assistant_improve_toolkit-1.3.9/src/main/python/visualize_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/main/python/watson_assistant_func.py` & `assistant_improve_toolkit-1.3.9/src/main/python/watson_assistant_func.py`

 * *Files identical despite different names*

### Comparing `assistant_improve_toolkit-1.3.8/src/main/python/watson_assistant_func_skip.py` & `assistant_improve_toolkit-1.3.9/src/main/python/watson_assistant_func_skip.py`

 * *Files identical despite different names*

