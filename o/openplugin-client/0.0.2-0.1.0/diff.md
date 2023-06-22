# Comparing `tmp/openplugin-client-0.0.2.tar.gz` & `tmp/openplugin-client-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openplugin-client-0.0.2.tar", last modified: Wed Jun 21 22:18:14 2023, max compression
+gzip compressed data, was "openplugin-client-0.1.0.tar", last modified: Thu Jun 22 14:49:38 2023, max compression
```

## Comparing `openplugin-client-0.0.2.tar` & `openplugin-client-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:18:14.990580 openplugin-client-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-21 22:18:14.990580 openplugin-client-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:18:14.990580 openplugin-client-0.0.2/openplugin/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-21 22:18:04.000000 openplugin-client-0.0.2/openplugin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 22:18:14.990580 openplugin-client-0.0.2/openplugin_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-21 22:18:14.000000 openplugin-client-0.0.2/openplugin_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-21 22:18:14.000000 openplugin-client-0.0.2/openplugin_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 22:18:14.000000 openplugin-client-0.0.2/openplugin_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-21 22:18:14.000000 openplugin-client-0.0.2/openplugin_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 22:18:14.990580 openplugin-client-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-21 22:18:04.000000 openplugin-client-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/openplugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 14:49:28.000000 openplugin-client-0.1.0/openplugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-06-22 14:49:28.000000 openplugin-client-0.1.0/openplugin/openplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-22 14:49:28.000000 openplugin-client-0.1.0/openplugin/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/openplugin_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-22 14:49:38.000000 openplugin-client-0.1.0/openplugin_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 14:49:38.892600 openplugin-client-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-22 14:49:28.000000 openplugin-client-0.1.0/setup.py
```

### Comparing `openplugin-client-0.0.2/PKG-INFO` & `openplugin-client-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugin-client
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugin-client-0.0.2/openplugin_client.egg-info/PKG-INFO` & `openplugin-client-0.1.0/openplugin_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: openplugin-client
-Version: 0.0.2
+Version: 0.1.0
 Summary: Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API
 Home-page: UNKNOWN
 Author: Sebastian Sosa
 Author-email: 1sebastian1sosa1@gmail.com
 License: UNKNOWN
 Description: Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API
 Keywords: python,openai,chatgpt,chat,plugin
```

### Comparing `openplugin-client-0.0.2/setup.py` & `openplugin-client-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup, find_packages
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name='openplugin-client', 
-        version="0.0.2",
+        version="0.1.0",
         author="Sebastian Sosa",
         author_email="1sebastian1sosa1@gmail.com",
         description='Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API',
         long_description='Python package that provides tooling for using ChatGPT packages with OpenAI Chat Completion API',
         packages=find_packages(),
         install_requires=[
-            
+            'pyyaml',
+            'requests'
         ], # add any additional packages
         
         keywords=[
             'python',
             'openai',
             'chatgpt',
             'chat',
-            'plugin',
+            'plugin'
         ],
         classifiers= [
             "Development Status :: 2 - Pre-Alpha",
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
```

