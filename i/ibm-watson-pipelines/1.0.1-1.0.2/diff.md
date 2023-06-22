# Comparing `tmp/ibm-watson-pipelines-1.0.1.tar.gz` & `tmp/ibm-watson-pipelines-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/travis/build/AILifecycle/ibm-watson-pipelines/dist/.tmp-v1vp30ez/ibm-watson-pipelines-1.0.1.tar", last modified: Thu May 25 15:33:06 2023, max compression
+gzip compressed data, was "/home/travis/build/AILifecycle/ibm-watson-pipelines/dist/.tmp-e6870j6l/ibm-watson-pipelines-1.0.2.tar", last modified: Thu Jun 22 12:12:38 2023, max compression
```

## Comparing `ibm-watson-pipelines-1.0.1.tar` & `ibm-watson-pipelines-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-25 15:33:06.925584 ibm-watson-pipelines-1.0.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11358 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     8382 2023-05-25 15:33:06.925584 ibm-watson-pipelines-1.0.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     7826 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-25 15:33:06.921584 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/
--rw-rw-r--   0 travis    (2000) travis    (2000)      610 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    40454 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/client.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8643 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/client_errors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    26558 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/cpd_paths.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7158 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/version.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-25 15:33:06.921584 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8382 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      531 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      147 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-05-25 15:33:06.000000 ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-05-25 15:33:06.925584 ibm-watson-pipelines-1.0.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1120 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-05-25 15:33:06.925584 ibm-watson-pipelines-1.0.1/test/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9595 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/test/test_cpd_path_methods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9071 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/test/test_cpd_path_parsing.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-05-25 15:32:18.000000 ibm-watson-pipelines-1.0.1/test/test_storage_client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-22 12:12:38.161820 ibm-watson-pipelines-1.0.2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11358 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8382 2023-06-22 12:12:38.161820 ibm-watson-pipelines-1.0.2/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7826 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-22 12:12:38.157820 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      610 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    40454 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/client.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8643 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/client_errors.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    26558 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/cpd_paths.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7158 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/version.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-22 12:12:38.157820 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8382 2023-06-22 12:12:38.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      531 2023-06-22 12:12:38.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-06-22 12:12:38.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      154 2023-06-22 12:12:38.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2023-06-22 12:12:38.000000 ibm-watson-pipelines-1.0.2/ibm_watson_pipelines.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-06-22 12:12:38.161820 ibm-watson-pipelines-1.0.2/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1127 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-06-22 12:12:38.161820 ibm-watson-pipelines-1.0.2/test/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9595 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/test/test_cpd_path_methods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9071 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/test/test_cpd_path_parsing.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3207 2023-06-22 12:11:22.000000 ibm-watson-pipelines-1.0.2/test/test_storage_client.py
```

### Comparing `ibm-watson-pipelines-1.0.1/LICENSE` & `ibm-watson-pipelines-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/PKG-INFO` & `ibm-watson-pipelines-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson-pipelines
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python utilities for IBM Watson Pipelines
 Home-page: https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=functions-watson-pipelines
 Author: Rafał Bigaj, Maksymilian Erazmus
 Author-email: rafal.bigaj@pl.ibm.com, maksymilian.erazmus1@pl.ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibm-watson-pipelines-1.0.1/README.md` & `ibm-watson-pipelines-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/__init__.py` & `ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/client.py` & `ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/client.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/client_errors.py` & `ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/client_errors.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/cpd_paths.py` & `ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/cpd_paths.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines/utils.py` & `ibm-watson-pipelines-1.0.2/ibm_watson_pipelines/utils.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/PKG-INFO` & `ibm-watson-pipelines-1.0.2/ibm_watson_pipelines.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibm-watson-pipelines
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python utilities for IBM Watson Pipelines
 Home-page: https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=functions-watson-pipelines
 Author: Rafał Bigaj, Maksymilian Erazmus
 Author-email: rafal.bigaj@pl.ibm.com, maksymilian.erazmus1@pl.ibm.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ibm-watson-pipelines-1.0.1/ibm_watson_pipelines.egg-info/SOURCES.txt` & `ibm-watson-pipelines-1.0.2/ibm_watson_pipelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/setup.py` & `ibm-watson-pipelines-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ibm-watson-pipelines",
-    version="1.0.1",
+    version="1.0.2",
     author="Rafał Bigaj, Maksymilian Erazmus",
     author_email="rafal.bigaj@pl.ibm.com, maksymilian.erazmus1@pl.ibm.com",
     description="Python utilities for IBM Watson Pipelines",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.ibm.com/docs/en/cloud-paks/cp-data/4.6.x?topic=functions-watson-pipelines",
     packages=setuptools.find_packages(),
@@ -21,15 +21,15 @@
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
     install_requires = [
         'ibm_cloud_sdk_core>=3.11.3',
         'ibm-cos-sdk>=2.10.0',
         'attrs>=21.2.0',
-        'kfp>=1.8.11',
+        'kfp>=1.8.11,<2.0.0',
         'requests>=2.25.1',
         'responses>=0.13.4',
         'pytest>=6.2.5',
         'typing-extensions>=3.7.4',
     ],
     include_package_data=True,
 )
```

### Comparing `ibm-watson-pipelines-1.0.1/test/test_cpd_path_methods.py` & `ibm-watson-pipelines-1.0.2/test/test_cpd_path_methods.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/test/test_cpd_path_parsing.py` & `ibm-watson-pipelines-1.0.2/test/test_cpd_path_parsing.py`

 * *Files identical despite different names*

### Comparing `ibm-watson-pipelines-1.0.1/test/test_storage_client.py` & `ibm-watson-pipelines-1.0.2/test/test_storage_client.py`

 * *Files identical despite different names*

