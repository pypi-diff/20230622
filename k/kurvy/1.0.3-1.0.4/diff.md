# Comparing `tmp/kurvy-1.0.3.tar.gz` & `tmp/kurvy-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kurvy-1.0.3.tar", last modified: Tue Jun 20 14:53:15 2023, max compression
+gzip compressed data, was "kurvy-1.0.4.tar", last modified: Thu Jun 22 15:03:29 2023, max compression
```

## Comparing `kurvy-1.0.3.tar` & `kurvy-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 14:53:15.720199 kurvy-1.0.3/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1069 2023-05-19 09:22:17.000000 kurvy-1.0.3/LICENSE
--rw-r--r--   0 lucbatty   (501) staff       (20)     1956 2023-06-20 14:53:15.719536 kurvy-1.0.3/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)     1463 2023-06-20 14:50:34.000000 kurvy-1.0.3/README.md
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 14:53:15.715255 kurvy-1.0.3/kurvy/
--rw-r--r--   0 lucbatty   (501) staff       (20)       71 2023-05-19 09:51:28.000000 kurvy-1.0.3/kurvy/__init__.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    14489 2023-06-20 14:08:40.000000 kurvy-1.0.3/kurvy/plots.py
--rw-r--r--   0 lucbatty   (501) staff       (20)    28987 2023-06-20 14:08:41.000000 kurvy-1.0.3/kurvy/trig.py
--rw-r--r--   0 lucbatty   (501) staff       (20)     6692 2023-06-20 14:08:40.000000 kurvy-1.0.3/kurvy/utils.py
-drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-20 14:53:15.718561 kurvy-1.0.3/kurvy.egg-info/
--rw-r--r--   0 lucbatty   (501) staff       (20)     1956 2023-06-20 14:53:15.000000 kurvy-1.0.3/kurvy.egg-info/PKG-INFO
--rw-r--r--   0 lucbatty   (501) staff       (20)      219 2023-06-20 14:53:15.000000 kurvy-1.0.3/kurvy.egg-info/SOURCES.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-20 14:53:15.000000 kurvy-1.0.3/kurvy.egg-info/dependency_links.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-20 14:53:15.000000 kurvy-1.0.3/kurvy.egg-info/top_level.txt
--rw-r--r--   0 lucbatty   (501) staff       (20)      231 2023-06-20 08:47:52.000000 kurvy-1.0.3/pyproject.toml
--rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-20 14:53:15.720459 kurvy-1.0.3/setup.cfg
--rw-r--r--   0 lucbatty   (501) staff       (20)      700 2023-06-20 14:53:08.000000 kurvy-1.0.3/setup.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 15:03:29.408566 kurvy-1.0.4/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1069 2023-05-19 09:22:17.000000 kurvy-1.0.4/LICENSE
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1854 2023-06-22 15:03:29.408047 kurvy-1.0.4/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1463 2023-06-20 14:50:34.000000 kurvy-1.0.4/README.md
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 15:03:29.402812 kurvy-1.0.4/kurvy/
+-rw-r--r--   0 lucbatty   (501) staff       (20)       71 2023-05-19 09:51:28.000000 kurvy-1.0.4/kurvy/__init__.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    14489 2023-06-20 14:08:40.000000 kurvy-1.0.4/kurvy/plots.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)    28987 2023-06-20 14:08:41.000000 kurvy-1.0.4/kurvy/trig.py
+-rw-r--r--   0 lucbatty   (501) staff       (20)     6692 2023-06-20 14:08:40.000000 kurvy-1.0.4/kurvy/utils.py
+drwxr-xr-x   0 lucbatty   (501) staff       (20)        0 2023-06-22 15:03:29.407208 kurvy-1.0.4/kurvy.egg-info/
+-rw-r--r--   0 lucbatty   (501) staff       (20)     1854 2023-06-22 15:03:29.000000 kurvy-1.0.4/kurvy.egg-info/PKG-INFO
+-rw-r--r--   0 lucbatty   (501) staff       (20)      219 2023-06-22 15:03:29.000000 kurvy-1.0.4/kurvy.egg-info/SOURCES.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        1 2023-06-22 15:03:29.000000 kurvy-1.0.4/kurvy.egg-info/dependency_links.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)        6 2023-06-22 15:03:29.000000 kurvy-1.0.4/kurvy.egg-info/top_level.txt
+-rw-r--r--   0 lucbatty   (501) staff       (20)      231 2023-06-20 08:47:52.000000 kurvy-1.0.4/pyproject.toml
+-rw-r--r--   0 lucbatty   (501) staff       (20)       38 2023-06-22 15:03:29.408831 kurvy-1.0.4/setup.cfg
+-rw-r--r--   0 lucbatty   (501) staff       (20)      600 2023-06-22 15:02:55.000000 kurvy-1.0.4/setup.py
```

### Comparing `kurvy-1.0.3/LICENSE` & `kurvy-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.3/PKG-INFO` & `kurvy-1.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: kurvy
-Version: 1.0.3
+Version: 1.0.4
 Summary: Curve approximation toolkit
 Home-page: https://github.com/celerygemini/kurvy
 Author: celerygemini
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![pyfer_cover](aux/kurvy.png)
```

### Comparing `kurvy-1.0.3/README.md` & `kurvy-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.3/kurvy/plots.py` & `kurvy-1.0.4/kurvy/plots.py`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.3/kurvy/trig.py` & `kurvy-1.0.4/kurvy/trig.py`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.3/kurvy/utils.py` & `kurvy-1.0.4/kurvy/utils.py`

 * *Files identical despite different names*

### Comparing `kurvy-1.0.3/kurvy.egg-info/PKG-INFO` & `kurvy-1.0.4/kurvy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: kurvy
-Version: 1.0.3
+Version: 1.0.4
 Summary: Curve approximation toolkit
 Home-page: https://github.com/celerygemini/kurvy
 Author: celerygemini
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![pyfer_cover](aux/kurvy.png)
```

