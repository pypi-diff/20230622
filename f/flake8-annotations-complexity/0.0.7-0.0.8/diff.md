# Comparing `tmp/flake8_annotations_complexity-0.0.7.tar.gz` & `tmp/flake8_annotations_complexity-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_annotations_complexity-0.0.7.tar", last modified: Thu Feb 24 18:29:22 2022, max compression
+gzip compressed data, was "flake8_annotations_complexity-0.0.8.tar", last modified: Thu Jun 22 13:26:31 2023, max compression
```

## Comparing `flake8_annotations_complexity-0.0.7.tar` & `flake8_annotations_complexity-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 18:29:22.767195 flake8_annotations_complexity-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-02-24 18:28:57.000000 flake8_annotations_complexity-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-02-24 18:29:22.771195 flake8_annotations_complexity-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-02-24 18:28:57.000000 flake8_annotations_complexity-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 18:29:22.767195 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-24 18:28:57.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-02-24 18:28:57.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity/ast_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-02-24 18:28:57.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-24 18:29:22.767195 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3070 2022-02-24 18:29:22.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-02-24 18:29:22.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 18:29:22.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-24 18:29:22.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-24 18:29:22.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-02-24 18:29:22.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-02-24 18:29:22.000000 flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-02-24 18:29:22.771195 flake8_annotations_complexity-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1807 2022-02-24 18:28:57.000000 flake8_annotations_complexity-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:26:31.473257 flake8_annotations_complexity-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-22 13:25:53.000000 flake8_annotations_complexity-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-22 13:26:31.473257 flake8_annotations_complexity-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-22 13:25:53.000000 flake8_annotations_complexity-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:26:31.473257 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 13:25:53.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-22 13:25:53.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity/ast_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-22 13:25:53.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:26:31.473257 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-22 13:26:31.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-22 13:26:31.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:26:31.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 13:26:31.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:26:31.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 13:26:31.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-22 13:26:31.000000 flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-22 13:26:31.473257 flake8_annotations_complexity-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-22 13:25:53.000000 flake8_annotations_complexity-0.0.8/setup.py
```

### Comparing `flake8_annotations_complexity-0.0.7/LICENSE` & `flake8_annotations_complexity-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8_annotations_complexity-0.0.7/PKG-INFO` & `flake8_annotations_complexity-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: flake8_annotations_complexity
-Version: 0.0.7
+Version: 0.0.8
 Summary: A flake8 extension that checks for type annotations complexity
 Home-page: https://github.com/best-doctor/flake8-annotations-complexity
 Author: Ilya Lebedev
 Author-email: melevir@gmail.com
 License: MIT
 Keywords: flake8 annotations
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-annotations-complexity
 
 [![Build Status](https://github.com/best-doctor/flake8-annotations-complexity/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/best-doctor/flake8-annotations-complexity/actions/workflows/build.yml)
@@ -79,9 +79,7 @@
 Here are useful tips:
 
 - You can run all checks and tests with `make check`.
   Please do it before CI does.
 - We use [BestDoctor python styleguide](https://github.com/best-doctor/guides/blob/master/guides/en/python_styleguide.md).
 - We respect [Django CoC](https://www.djangoproject.com/conduct/).
   Make soft, not bullshit.
-
-
```

### Comparing `flake8_annotations_complexity-0.0.7/README.md` & `flake8_annotations_complexity-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `flake8_annotations_complexity-0.0.7/flake8_annotations_complexity/ast_helpers.py` & `flake8_annotations_complexity-0.0.8/flake8_annotations_complexity/ast_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,13 +58,13 @@
         complexity = get_annotation_complexity(annotation)
         if complexity > max_annotations_complexity:
             too_difficult_annotations.append((
                 annotation,
                 'TAE002 too complex annotation ({0} > {1})'.format(complexity, max_annotations_complexity),
             ))
         annotation_len = get_annotation_len(annotation)
-        if annotation_len > 7:
+        if annotation_len > max_annotations_len:
             too_difficult_annotations.append((
                 annotation,
                 'TAE003 too long annotation ({0} > {1})'.format(annotation_len, max_annotations_len),
             ))
     return too_difficult_annotations
```

### Comparing `flake8_annotations_complexity-0.0.7/flake8_annotations_complexity/checker.py` & `flake8_annotations_complexity-0.0.8/flake8_annotations_complexity/checker.py`

 * *Files identical despite different names*

### Comparing `flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/PKG-INFO` & `flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: flake8-annotations-complexity
-Version: 0.0.7
+Version: 0.0.8
 Summary: A flake8 extension that checks for type annotations complexity
 Home-page: https://github.com/best-doctor/flake8-annotations-complexity
 Author: Ilya Lebedev
 Author-email: melevir@gmail.com
 License: MIT
 Keywords: flake8 annotations
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Framework :: Flake8
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # flake8-annotations-complexity
 
 [![Build Status](https://github.com/best-doctor/flake8-annotations-complexity/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/best-doctor/flake8-annotations-complexity/actions/workflows/build.yml)
@@ -79,9 +79,7 @@
 Here are useful tips:
 
 - You can run all checks and tests with `make check`.
   Please do it before CI does.
 - We use [BestDoctor python styleguide](https://github.com/best-doctor/guides/blob/master/guides/en/python_styleguide.md).
 - We respect [Django CoC](https://www.djangoproject.com/conduct/).
   Make soft, not bullshit.
-
-
```

### Comparing `flake8_annotations_complexity-0.0.7/flake8_annotations_complexity.egg-info/SOURCES.txt` & `flake8_annotations_complexity-0.0.8/flake8_annotations_complexity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flake8_annotations_complexity-0.0.7/setup.cfg` & `flake8_annotations_complexity-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `flake8_annotations_complexity-0.0.7/setup.py` & `flake8_annotations_complexity-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Software Development :: Quality Assurance',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     python_requires='>=3.7',
     packages=find_packages(),
     include_package_data=True,
     keywords='flake8 annotations',
```

