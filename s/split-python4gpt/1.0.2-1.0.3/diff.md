# Comparing `tmp/split_python4gpt-1.0.2.tar.gz` & `tmp/split_python4gpt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "split_python4gpt-1.0.2.tar", last modified: Thu Jun 22 14:03:48 2023, max compression
+gzip compressed data, was "split_python4gpt-1.0.3.tar", last modified: Thu Jun 22 14:27:52 2023, max compression
```

## Comparing `split_python4gpt-1.0.2.tar` & `split_python4gpt-1.0.3.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:48.739462 split_python4gpt-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:48.735463 split_python4gpt-1.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:48.739462 split_python4gpt-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-22 14:03:48.739462 split_python4gpt-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/pydoc-markdown.yml
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-22 14:03:48.743462 split_python4gpt-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:48.735463 split_python4gpt-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:48.739462 split_python4gpt-1.0.2/src/split_python4gpt/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/src/split_python4gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/src/split_python4gpt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/src/split_python4gpt/minifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:48.739462 split_python4gpt-1.0.2/src/split_python4gpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-22 14:03:48.000000 split_python4gpt-1.0.2/src/split_python4gpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-22 14:03:48.000000 split_python4gpt-1.0.2/src/split_python4gpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:03:48.000000 split_python4gpt-1.0.2/src/split_python4gpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 14:03:48.000000 split_python4gpt-1.0.2/src/split_python4gpt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:03:48.000000 split_python4gpt-1.0.2/src/split_python4gpt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 14:03:48.000000 split_python4gpt-1.0.2/src/split_python4gpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 14:03:48.000000 split_python4gpt-1.0.2/src/split_python4gpt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:48.739462 split_python4gpt-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:03:48.739462 split_python4gpt-1.0.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/tests/data/in_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/tests/data/out_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/tests/test_minifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-22 14:03:34.000000 split_python4gpt-1.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:27:52.696661 split_python4gpt-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:27:52.692661 split_python4gpt-1.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:27:52.696661 split_python4gpt-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-22 14:27:52.696661 split_python4gpt-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/pydoc-markdown.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-22 14:27:52.696661 split_python4gpt-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:27:52.692661 split_python4gpt-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:27:52.696661 split_python4gpt-1.0.3/src/split_python4gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/src/split_python4gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/src/split_python4gpt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/src/split_python4gpt/minifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:27:52.696661 split_python4gpt-1.0.3/src/split_python4gpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-22 14:27:52.000000 split_python4gpt-1.0.3/src/split_python4gpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-22 14:27:52.000000 split_python4gpt-1.0.3/src/split_python4gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:27:52.000000 split_python4gpt-1.0.3/src/split_python4gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-22 14:27:52.000000 split_python4gpt-1.0.3/src/split_python4gpt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 14:27:52.000000 split_python4gpt-1.0.3/src/split_python4gpt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-22 14:27:52.000000 split_python4gpt-1.0.3/src/split_python4gpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-22 14:27:52.000000 split_python4gpt-1.0.3/src/split_python4gpt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:27:52.696661 split_python4gpt-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 14:27:52.696661 split_python4gpt-1.0.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/tests/data/in_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/tests/data/out_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/tests/test_minifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-06-22 14:27:39.000000 split_python4gpt-1.0.3/tox.ini
```

### Comparing `split_python4gpt-1.0.2/.coveragerc` & `split_python4gpt-1.0.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/.github/workflows/ci.yml` & `split_python4gpt-1.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/.gitignore` & `split_python4gpt-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/.pre-commit-config.yaml` & `split_python4gpt-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/LICENSE.txt` & `split_python4gpt-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/setup.cfg` & `split_python4gpt-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/setup.py` & `split_python4gpt-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/src/split_python4gpt/__init__.py` & `split_python4gpt-1.0.3/src/split_python4gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/src/split_python4gpt/minifier.py` & `split_python4gpt-1.0.3/src/split_python4gpt/minifier.py`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/src/split_python4gpt.egg-info/SOURCES.txt` & `split_python4gpt-1.0.3/src/split_python4gpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `split_python4gpt-1.0.2/tox.ini` & `split_python4gpt-1.0.3/tox.ini`

 * *Files identical despite different names*

