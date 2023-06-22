# Comparing `tmp/accern_data-0.2.0rc1.tar.gz` & `tmp/accern_data-0.2.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accern_data-0.2.0rc1.tar", last modified: Tue Dec  6 10:32:58 2022, max compression
+gzip compressed data, was "dist/accern_data-0.2.1rc1.tar", last modified: Thu Jun 22 12:07:36 2023, max compression
```

## Comparing `accern_data-0.2.0rc1.tar` & `accern_data-0.2.1rc1.tar`

### file list

```diff
@@ -1,25 +1,32 @@
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2022-12-06 10:32:58.548494 accern_data-0.2.0rc1/
--rw-r--r--   0 ankurgoswami   (501) staff       (20)     1063 2022-03-17 13:33:56.000000 accern_data-0.2.0rc1/LICENSE
--rw-r--r--   0 ankurgoswami   (501) staff       (20)     3423 2022-12-06 10:32:58.548695 accern_data-0.2.0rc1/PKG-INFO
--rw-r--r--   0 ankurgoswami   (501) staff       (20)     2692 2022-08-03 18:07:28.000000 accern_data-0.2.0rc1/README.md
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2022-12-06 10:32:58.528870 accern_data-0.2.0rc1/packages/
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2022-12-06 10:32:58.529257 accern_data-0.2.0rc1/packages/python/
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2022-12-06 10:32:58.534267 accern_data-0.2.0rc1/packages/python/accern_data/
--rw-r--r--   0 ankurgoswami   (501) staff       (20)       63 2022-12-06 10:32:46.000000 accern_data-0.2.0rc1/packages/python/accern_data/__init__.py
--rw-r--r--   0 ankurgoswami   (501) staff       (20)        0 2022-03-17 19:51:42.000000 accern_data-0.2.0rc1/packages/python/accern_data/__main__.py
--rw-r--r--   0 ankurgoswami   (501) staff       (20)    36807 2022-12-06 10:22:02.000000 accern_data-0.2.0rc1/packages/python/accern_data/accern_data.py
--rw-r--r--   0 ankurgoswami   (501) staff       (20)        0 2022-04-15 15:27:04.000000 accern_data-0.2.0rc1/packages/python/accern_data/py.typed
--rw-r--r--   0 ankurgoswami   (501) staff       (20)    10832 2022-12-06 10:22:02.000000 accern_data-0.2.0rc1/packages/python/accern_data/util.py
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2022-12-06 10:32:58.536834 accern_data-0.2.0rc1/packages/python/accern_data.egg-info/
--rw-r--r--   0 ankurgoswami   (501) staff       (20)     3423 2022-12-06 10:32:58.000000 accern_data-0.2.0rc1/packages/python/accern_data.egg-info/PKG-INFO
--rw-r--r--   0 ankurgoswami   (501) staff       (20)      552 2022-12-06 10:32:58.000000 accern_data-0.2.0rc1/packages/python/accern_data.egg-info/SOURCES.txt
--rw-r--r--   0 ankurgoswami   (501) staff       (20)        1 2022-12-06 10:32:58.000000 accern_data-0.2.0rc1/packages/python/accern_data.egg-info/dependency_links.txt
--rw-r--r--   0 ankurgoswami   (501) staff       (20)       91 2022-12-06 10:32:58.000000 accern_data-0.2.0rc1/packages/python/accern_data.egg-info/requires.txt
--rw-r--r--   0 ankurgoswami   (501) staff       (20)       12 2022-12-06 10:32:58.000000 accern_data-0.2.0rc1/packages/python/accern_data.egg-info/top_level.txt
--rw-r--r--   0 ankurgoswami   (501) staff       (20)     2288 2022-11-24 15:12:37.000000 accern_data-0.2.0rc1/pyproject.toml
--rw-r--r--   0 ankurgoswami   (501) staff       (20)     1078 2022-12-06 10:32:58.549507 accern_data-0.2.0rc1/setup.cfg
--rw-r--r--   0 ankurgoswami   (501) staff       (20)       38 2022-05-04 05:47:08.000000 accern_data-0.2.0rc1/setup.py
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2022-12-06 10:32:58.529930 accern_data-0.2.0rc1/tests/
-drwxr-xr-x   0 ankurgoswami   (501) staff       (20)        0 2022-12-06 10:32:58.540742 accern_data-0.2.0rc1/tests/data/
--rw-r--r--   0 ankurgoswami   (501) staff       (20)  1579738 2022-12-06 10:22:02.000000 accern_data-0.2.0rc1/tests/data/data-2022.csv
--rw-r--r--   0 ankurgoswami   (501) staff       (20)  4930620 2022-12-06 10:22:02.000000 accern_data-0.2.0rc1/tests/data/data-2022.json
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.313443 accern_data-0.2.1rc1/
+-rw-r--r--   0 shaunak    (501) staff       (20)     1063 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/LICENSE
+-rw-r--r--   0 shaunak    (501) staff       (20)     3423 2023-06-22 12:07:36.313640 accern_data-0.2.1rc1/PKG-INFO
+-rw-r--r--   0 shaunak    (501) staff       (20)     2692 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/README.md
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.281452 accern_data-0.2.1rc1/packages/
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.281907 accern_data-0.2.1rc1/packages/python/
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.287783 accern_data-0.2.1rc1/packages/python/accern_data/
+-rw-r--r--   0 shaunak    (501) staff       (20)       63 2023-06-21 12:50:44.000000 accern_data-0.2.1rc1/packages/python/accern_data/__init__.py
+-rw-r--r--   0 shaunak    (501) staff       (20)        0 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/packages/python/accern_data/__main__.py
+-rw-r--r--   0 shaunak    (501) staff       (20)    58411 2023-06-21 12:04:37.000000 accern_data-0.2.1rc1/packages/python/accern_data/accern_data.py
+-rw-r--r--   0 shaunak    (501) staff       (20)        0 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/packages/python/accern_data/py.typed
+-rw-r--r--   0 shaunak    (501) staff       (20)    14488 2023-06-21 12:04:37.000000 accern_data-0.2.1rc1/packages/python/accern_data/util.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.290165 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/
+-rw-r--r--   0 shaunak    (501) staff       (20)     3423 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/PKG-INFO
+-rw-r--r--   0 shaunak    (501) staff       (20)      729 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/SOURCES.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)        1 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/dependency_links.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)       91 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/requires.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)       12 2023-06-22 12:07:36.000000 accern_data-0.2.1rc1/packages/python/accern_data.egg-info/top_level.txt
+-rw-r--r--   0 shaunak    (501) staff       (20)     2288 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/pyproject.toml
+-rw-r--r--   0 shaunak    (501) staff       (20)     1078 2023-06-22 12:07:36.314359 accern_data-0.2.1rc1/setup.cfg
+-rw-r--r--   0 shaunak    (501) staff       (20)       38 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/setup.py
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.294163 accern_data-0.2.1rc1/tests/
+drwxr-xr-x   0 shaunak    (501) staff       (20)        0 2023-06-22 12:07:36.300358 accern_data-0.2.1rc1/tests/data/
+-rw-r--r--   0 shaunak    (501) staff       (20)  1579738 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/tests/data/data-2022.csv
+-rw-r--r--   0 shaunak    (501) staff       (20)  4930620 2023-06-16 10:21:30.000000 accern_data-0.2.1rc1/tests/data/data-2022.json
+-rw-r--r--   0 shaunak    (501) staff       (20)     3658 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_by_date.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     3380 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_consistency.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     4961 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_data_iterator.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     4362 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_filters.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     1079 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_inconsistent_fields.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     4346 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_modes.py
+-rw-r--r--   0 shaunak    (501) staff       (20)     4130 2023-06-16 10:21:31.000000 accern_data-0.2.1rc1/tests/test_timestamps.py
```

### Comparing `accern_data-0.2.0rc1/LICENSE` & `accern_data-0.2.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.0rc1/PKG-INFO` & `accern_data-0.2.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accern_data
-Version: 0.2.0rc1
+Version: 0.2.1rc1
 Summary: Client for consuming Accern data feeds.
 Home-page: https://github.com/Accern/accern-data-client
 Author: Accern Corp.
 Author-email: datascience@accern.com
 License: MIT
 Keywords: api client data feed NLP processing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `accern_data-0.2.0rc1/README.md` & `accern_data-0.2.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.0rc1/packages/python/accern_data.egg-info/PKG-INFO` & `accern_data-0.2.1rc1/packages/python/accern_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accern-data
-Version: 0.2.0rc1
+Version: 0.2.1rc1
 Summary: Client for consuming Accern data feeds.
 Home-page: https://github.com/Accern/accern-data-client
 Author: Accern Corp.
 Author-email: datascience@accern.com
 License: MIT
 Keywords: api client data feed NLP processing
 Classifier: Development Status :: 4 - Beta
```

### Comparing `accern_data-0.2.0rc1/packages/python/accern_data.egg-info/SOURCES.txt` & `accern_data-0.2.1rc1/packages/python/accern_data.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -9,9 +9,16 @@
 packages/python/accern_data/py.typed
 packages/python/accern_data/util.py
 packages/python/accern_data.egg-info/PKG-INFO
 packages/python/accern_data.egg-info/SOURCES.txt
 packages/python/accern_data.egg-info/dependency_links.txt
 packages/python/accern_data.egg-info/requires.txt
 packages/python/accern_data.egg-info/top_level.txt
+tests/test_by_date.py
+tests/test_consistency.py
+tests/test_data_iterator.py
+tests/test_filters.py
+tests/test_inconsistent_fields.py
+tests/test_modes.py
+tests/test_timestamps.py
 tests/data/data-2022.csv
 tests/data/data-2022.json
```

### Comparing `accern_data-0.2.0rc1/pyproject.toml` & `accern_data-0.2.1rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.0rc1/setup.cfg` & `accern_data-0.2.1rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.0rc1/tests/data/data-2022.csv` & `accern_data-0.2.1rc1/tests/data/data-2022.csv`

 * *Files identical despite different names*

### Comparing `accern_data-0.2.0rc1/tests/data/data-2022.json` & `accern_data-0.2.1rc1/tests/data/data-2022.json`

 * *Files identical despite different names*

