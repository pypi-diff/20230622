# Comparing `tmp/batch-mailchimp-1.1.0.tar.gz` & `tmp/batch-mailchimp-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batch-mailchimp-1.1.0.tar", last modified: Tue Jun 20 18:38:54 2023, max compression
+gzip compressed data, was "batch-mailchimp-1.1.1.tar", last modified: Wed Jun 21 07:37:11 2023, max compression
```

## Comparing `batch-mailchimp-1.1.0.tar` & `batch-mailchimp-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/batch_mailchimp/
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/batch_mailchimp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/batch_mailchimp/batches_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/batch_mailchimp/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/batch_mailchimp/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 18:38:54.000000 batch-mailchimp-1.1.0/batch_mailchimp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 18:38:54.884643 batch-mailchimp-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-06-20 18:38:46.000000 batch-mailchimp-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:37:11.520433 batch-mailchimp-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-21 07:37:03.000000 batch-mailchimp-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-21 07:37:11.520433 batch-mailchimp-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-21 07:37:03.000000 batch-mailchimp-1.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:37:11.520433 batch-mailchimp-1.1.1/batch_mailchimp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-06-21 07:37:03.000000 batch-mailchimp-1.1.1/batch_mailchimp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-06-21 07:37:03.000000 batch-mailchimp-1.1.1/batch_mailchimp/batches_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-21 07:37:03.000000 batch-mailchimp-1.1.1/batch_mailchimp/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-21 07:37:03.000000 batch-mailchimp-1.1.1/batch_mailchimp/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 07:37:11.520433 batch-mailchimp-1.1.1/batch_mailchimp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-21 07:37:11.000000 batch-mailchimp-1.1.1/batch_mailchimp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-21 07:37:11.000000 batch-mailchimp-1.1.1/batch_mailchimp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 07:37:11.000000 batch-mailchimp-1.1.1/batch_mailchimp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-21 07:37:11.000000 batch-mailchimp-1.1.1/batch_mailchimp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-21 07:37:11.000000 batch-mailchimp-1.1.1/batch_mailchimp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 07:37:11.520433 batch-mailchimp-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-21 07:37:03.000000 batch-mailchimp-1.1.1/setup.py
```

### Comparing `batch-mailchimp-1.1.0/LICENSE` & `batch-mailchimp-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.0/PKG-INFO` & `batch-mailchimp-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python client for MailChimp Marketing API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
 Keywords: mailchimp marketing api client wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 
 Python BatchMailchimp
 =====================
```

### Comparing `batch-mailchimp-1.1.0/README.rst` & `batch-mailchimp-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.0/batch_mailchimp/__init__.py` & `batch-mailchimp-1.1.1/batch_mailchimp/__init__.py`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.0/batch_mailchimp/batches_api.py` & `batch-mailchimp-1.1.1/batch_mailchimp/batches_api.py`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.0/batch_mailchimp/collections.py` & `batch-mailchimp-1.1.1/batch_mailchimp/collections.py`

 * *Files identical despite different names*

### Comparing `batch-mailchimp-1.1.0/batch_mailchimp.egg-info/PKG-INFO` & `batch-mailchimp-1.1.1/batch_mailchimp.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: batch-mailchimp
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python client for MailChimp Marketing API, with batch support
 Home-page: https://github.com/FullFact/python-batchmailchimp
 Author: Andy Lulham
 Author-email: andy.lulham@fullfact.org
 License: MIT
 Keywords: mailchimp marketing api client wrapper
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
 
 Python BatchMailchimp
 =====================
```

### Comparing `batch-mailchimp-1.1.0/setup.py` & `batch-mailchimp-1.1.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,26 +8,24 @@
 
 setup(
     name="batch-mailchimp",
     description="A python client for MailChimp Marketing API, with batch support",
     url="https://github.com/FullFact/python-batchmailchimp",
     author="Andy Lulham",
     author_email="andy.lulham@fullfact.org",
-    version="1.1.0",
+    version="1.1.1",
     packages=find_packages(),
     license="MIT",
     keywords="mailchimp marketing api client wrapper",
     long_description=readme,
     install_requires=["mailchimp-marketing>=3.0.80"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ],
 )
```

