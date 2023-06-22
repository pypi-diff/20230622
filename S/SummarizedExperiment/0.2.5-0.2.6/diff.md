# Comparing `tmp/SummarizedExperiment-0.2.5.tar.gz` & `tmp/SummarizedExperiment-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SummarizedExperiment-0.2.5.tar", last modified: Wed Jun 21 17:31:12 2023, max compression
+gzip compressed data, was "SummarizedExperiment-0.2.6.tar", last modified: Thu Jun 22 01:18:53 2023, max compression
```

## Comparing `SummarizedExperiment-0.2.5.tar` & `SummarizedExperiment-0.2.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.390227 SummarizedExperiment-0.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.398227 SummarizedExperiment-0.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.402227 SummarizedExperiment-0.2.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.402227 SummarizedExperiment-0.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-21 17:31:12.410227 SummarizedExperiment-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.394227 SummarizedExperiment-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.402227 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 17:29:45.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-21 17:31:12.000000 SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/src/summarizedexperiment/
--rw-r--r--   0 runner    (1001) docker     (123)    15507 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/BaseSE.py
--rw-r--r--   0 runner    (1001) docker     (123)    23312 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/RangeSummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/RangedSummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/SummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/src/summarizedexperiment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 17:31:12.406227 SummarizedExperiment-0.2.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/data/tenx.sub.h5
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_RSE.py
--rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_RSE_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_SE.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_SE_backed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tests/test_SE_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-21 17:29:33.000000 SummarizedExperiment-0.2.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.974466 SummarizedExperiment-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.958467 SummarizedExperiment-0.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.966467 SummarizedExperiment-0.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    14028 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-22 01:18:53.974466 SummarizedExperiment-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.970466 SummarizedExperiment-0.2.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.970466 SummarizedExperiment-0.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-22 01:18:53.974466 SummarizedExperiment-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.958467 SummarizedExperiment-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.970466 SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-22 01:18:53.000000 SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 01:18:53.000000 SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:18:53.000000 SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 01:17:48.000000 SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-22 01:18:53.000000 SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 01:18:53.000000 SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.970466 SummarizedExperiment-0.2.6/src/summarizedexperiment/
+-rw-r--r--   0 runner    (1001) docker     (123)    15507 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/src/summarizedexperiment/BaseSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23312 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/src/summarizedexperiment/RangeSummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/src/summarizedexperiment/RangedSummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/src/summarizedexperiment/SummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/src/summarizedexperiment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.974466 SummarizedExperiment-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 01:18:53.974466 SummarizedExperiment-0.2.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   986863 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/tests/data/tenx.sub.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/tests/test_RSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4726 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/tests/test_RSE_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/tests/test_SE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/tests/test_SE_backed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/tests/test_SE_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-22 01:17:36.000000 SummarizedExperiment-0.2.6/tox.ini
```

### Comparing `SummarizedExperiment-0.2.5/.coveragerc` & `SummarizedExperiment-0.2.6/.coveragerc`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/.github/workflows/pypi-publish.yml` & `SummarizedExperiment-0.2.6/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/.github/workflows/pypi-test.yml` & `SummarizedExperiment-0.2.6/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/.gitignore` & `SummarizedExperiment-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/CHANGELOG.md` & `SummarizedExperiment-0.2.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/CONTRIBUTING.rst` & `SummarizedExperiment-0.2.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/LICENSE.txt` & `SummarizedExperiment-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/PKG-INFO` & `SummarizedExperiment-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SummarizedExperiment
-Version: 0.2.5
+Version: 0.2.6
 Summary: Container to represent data from genomic experiments
 Home-page: https://github.com/BiocPy/summarizedexperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/summarizedexperiment
 Platform: any
```

### Comparing `SummarizedExperiment-0.2.5/README.md` & `SummarizedExperiment-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/docs/Makefile` & `SummarizedExperiment-0.2.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/docs/changelog.md` & `SummarizedExperiment-0.2.6/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/docs/conf.py` & `SummarizedExperiment-0.2.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/docs/index.md` & `SummarizedExperiment-0.2.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/docs/readme.md` & `SummarizedExperiment-0.2.6/docs/readme.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/docs/tutorial.md` & `SummarizedExperiment-0.2.6/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/setup.cfg` & `SummarizedExperiment-0.2.6/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 include_package_data = True
 package_dir = 
 	=src
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	biocframe>=0.2.13
 	genomicranges>=0.2.9
-	filebackedarray>=0.0.2
+	filebackedarray>=0.0.3
 	scipy
 	anndata
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `SummarizedExperiment-0.2.5/setup.py` & `SummarizedExperiment-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/PKG-INFO` & `SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SummarizedExperiment
-Version: 0.2.5
+Version: 0.2.6
 Summary: Container to represent data from genomic experiments
 Home-page: https://github.com/BiocPy/summarizedexperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/summarizedexperiment
 Platform: any
```

### Comparing `SummarizedExperiment-0.2.5/src/SummarizedExperiment.egg-info/SOURCES.txt` & `SummarizedExperiment-0.2.6/src/SummarizedExperiment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/src/summarizedexperiment/BaseSE.py` & `SummarizedExperiment-0.2.6/src/summarizedexperiment/BaseSE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/src/summarizedexperiment/RangeSummarizedExperiment.py` & `SummarizedExperiment-0.2.6/src/summarizedexperiment/RangeSummarizedExperiment.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/src/summarizedexperiment/SummarizedExperiment.py` & `SummarizedExperiment-0.2.6/src/summarizedexperiment/SummarizedExperiment.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/src/summarizedexperiment/__init__.py` & `SummarizedExperiment-0.2.6/src/summarizedexperiment/__init__.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/tests/data/tenx.sub.h5` & `SummarizedExperiment-0.2.6/tests/data/tenx.sub.h5`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/tests/test_RSE.py` & `SummarizedExperiment-0.2.6/tests/test_RSE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/tests/test_RSE_methods.py` & `SummarizedExperiment-0.2.6/tests/test_RSE_methods.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/tests/test_SE.py` & `SummarizedExperiment-0.2.6/tests/test_SE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/tests/test_SE_backed.py` & `SummarizedExperiment-0.2.6/tests/test_SE_backed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from random import random
 
 import numpy as np
 import pandas as pd
 import pytest
-from filebackedarray import H5BackedData
+from filebackedarray import H5BackedSparseData
 from summarizedexperiment.SummarizedExperiment import SummarizedExperiment
 
 __author__ = "jkanche"
 __copyright__ = "jkanche"
 __license__ = "MIT"
 
 
@@ -35,15 +35,15 @@
             "score": range(0, 1000),
             "GC": [random() for _ in range(10)] * 100,
         }
     )
 
     colData = pd.DataFrame({"treatment": ["ChIP"] * 3005,})
 
-    assay = H5BackedData("tests/data/tenx.sub.h5", "matrix")
+    assay = H5BackedSparseData("tests/data/tenx.sub.h5", "matrix")
 
     tse = SummarizedExperiment(
         assays={"counts_backed": assay},
         rowData=df_gr,
         colData=colData,
     )
 
@@ -79,15 +79,15 @@
                 "score": range(0, 200),
                 "GC": [random() for _ in range(10)] * 20,
             }
         )
 
         colData = pd.DataFrame({"treatment": ["ChIP", "Input"] * 3,})
 
-        assay = H5BackedData("tests/data/tenx.sub.h5", "matrix")
+        assay = H5BackedSparseData("tests/data/tenx.sub.h5", "matrix")
 
         tse = SummarizedExperiment(
             assays={"counts_backed": assay, "counts": counts},
             rowData=df_gr,
             colData=colData,
         )
```

### Comparing `SummarizedExperiment-0.2.5/tests/test_SE_methods.py` & `SummarizedExperiment-0.2.6/tests/test_SE_methods.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.2.5/tox.ini` & `SummarizedExperiment-0.2.6/tox.ini`

 * *Files identical despite different names*

