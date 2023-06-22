# Comparing `tmp/aeppl-nightly-0.1.4.dev20230620.tar.gz` & `tmp/aeppl-nightly-0.1.4.dev20230621.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeppl-nightly-0.1.4.dev20230620.tar", last modified: Tue Jun 20 00:32:44 2023, max compression
+gzip compressed data, was "aeppl-nightly-0.1.4.dev20230621.tar", last modified: Wed Jun 21 00:34:31 2023, max compression
```

## Comparing `aeppl-nightly-0.1.4.dev20230620.tar` & `aeppl-nightly-0.1.4.dev20230621.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:32:44.517624 aeppl-nightly-0.1.4.dev20230620/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-20 00:32:44.517624 aeppl-nightly-0.1.4.dev20230620/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:32:44.521623 aeppl-nightly-0.1.4.dev20230620/aeppl/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-20 00:32:44.521623 aeppl-nightly-0.1.4.dev20230620/aeppl/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/dists.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/aeppl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:32:44.509623 aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-20 00:32:44.000000 aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-20 00:32:44.000000 aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 00:32:44.000000 aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 00:32:44.000000 aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 00:32:44.000000 aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-20 00:32:44.000000 aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-20 00:32:44.517624 aeppl-nightly-0.1.4.dev20230620/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 00:32:44.517624 aeppl-nightly-0.1.4.dev20230620/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_composite_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_convolutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_dist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_joint_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_logprob.py
--rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-20 00:32:26.000000 aeppl-nightly-0.1.4.dev20230620/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:31.929402 aeppl-nightly-0.1.4.dev20230621/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-21 00:34:31.929402 aeppl-nightly-0.1.4.dev20230621/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:31.933402 aeppl-nightly-0.1.4.dev20230621/aeppl/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-21 00:34:31.933402 aeppl-nightly-0.1.4.dev20230621/aeppl/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8455 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/dists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15197 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24329 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11894 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30605 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/aeppl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:31.925402 aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-21 00:34:31.000000 aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-21 00:34:31.000000 aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:34:31.000000 aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 00:34:31.000000 aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-21 00:34:31.000000 aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-21 00:34:31.000000 aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-21 00:34:31.933402 aeppl-nightly-0.1.4.dev20230621/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 00:34:31.929402 aeppl-nightly-0.1.4.dev20230621/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5967 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5208 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_composite_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_convolutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25605 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_dist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_joint_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40106 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_logprob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22582 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6965 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11007 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22973 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4717 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-21 00:34:17.000000 aeppl-nightly-0.1.4.dev20230621/versioneer.py
```

### Comparing `aeppl-nightly-0.1.4.dev20230620/LICENSE` & `aeppl-nightly-0.1.4.dev20230621/LICENSE`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/PKG-INFO` & `aeppl-nightly-0.1.4.dev20230621/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.4.dev20230620
+Version: 0.1.4.dev20230621
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.4.dev20230620/README.md` & `aeppl-nightly-0.1.4.dev20230621/README.md`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/abstract.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/censoring.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/convolutions.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/cumsum.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/dists.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/dists.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/joint_logprob.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/logprob.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/mixture.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/printing.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/rewriting.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/scan.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/tensor.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/transforms.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl/utils.py` & `aeppl-nightly-0.1.4.dev20230621/aeppl/utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/PKG-INFO` & `aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeppl-nightly
-Version: 0.1.4.dev20230620
+Version: 0.1.4.dev20230621
 Summary: PPL tools for Aesara
 Home-page: https://github.com/aesara-devs/aeppl
 Author: aesara-devs
 Author-email: aesara.devs@gmail.com
 Keywords: aeppl,math,probability,symbolic,probabilistic programming
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `aeppl-nightly-0.1.4.dev20230620/aeppl_nightly.egg-info/SOURCES.txt` & `aeppl-nightly-0.1.4.dev20230621/aeppl_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/setup.cfg` & `aeppl-nightly-0.1.4.dev20230621/setup.cfg`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/setup.py` & `aeppl-nightly-0.1.4.dev20230621/setup.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_abstract.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_abstract.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_censoring.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_censoring.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_composite_logprob.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_composite_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_convolutions.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_convolutions.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_cumsum.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_cumsum.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_dist.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_dist.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_joint_logprob.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_joint_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_logprob.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_logprob.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_mixture.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_mixture.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_printing.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_printing.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_rewriting.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_rewriting.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_scan.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_tensor.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_transforms.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/tests/test_utils.py` & `aeppl-nightly-0.1.4.dev20230621/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aeppl-nightly-0.1.4.dev20230620/versioneer.py` & `aeppl-nightly-0.1.4.dev20230621/versioneer.py`

 * *Files identical despite different names*

