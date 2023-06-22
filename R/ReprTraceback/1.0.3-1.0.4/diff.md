# Comparing `tmp/ReprTraceback-1.0.3.tar.gz` & `tmp/ReprTraceback-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReprTraceback-1.0.3.tar", last modified: Wed Jun 21 08:09:14 2023, max compression
+gzip compressed data, was "ReprTraceback-1.0.4.tar", last modified: Thu Jun 22 04:43:04 2023, max compression
```

## Comparing `ReprTraceback-1.0.3.tar` & `ReprTraceback-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 08:09:14.056437 ReprTraceback-1.0.3/
--rw-rw-rw-   0        0        0     1898 2023-06-21 08:09:14.056437 ReprTraceback-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1498 2023-06-20 04:41:42.000000 ReprTraceback-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 08:09:14.042914 ReprTraceback-1.0.3/ReprTraceback/
--rw-rw-rw-   0        0        0     3414 2023-06-21 08:06:34.000000 ReprTraceback-1.0.3/ReprTraceback/ReprTraceback.py
--rw-rw-rw-   0        0        0        0 2023-06-20 04:32:24.000000 ReprTraceback-1.0.3/ReprTraceback/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 08:09:14.054935 ReprTraceback-1.0.3/ReprTraceback.egg-info/
--rw-rw-rw-   0        0        0     1898 2023-06-21 08:09:13.000000 ReprTraceback-1.0.3/ReprTraceback.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-06-21 08:09:14.000000 ReprTraceback-1.0.3/ReprTraceback.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 08:09:13.000000 ReprTraceback-1.0.3/ReprTraceback.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-21 08:09:13.000000 ReprTraceback-1.0.3/ReprTraceback.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-21 08:09:14.057448 ReprTraceback-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      582 2023-06-21 08:09:06.000000 ReprTraceback-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:43:04.371110 ReprTraceback-1.0.4/
+-rw-rw-rw-   0        0        0     1898 2023-06-22 04:43:04.370110 ReprTraceback-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1498 2023-06-20 04:41:42.000000 ReprTraceback-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 04:43:04.336553 ReprTraceback-1.0.4/ReprTraceback/
+-rw-rw-rw-   0        0        0     3411 2023-06-22 04:38:43.000000 ReprTraceback-1.0.4/ReprTraceback/ReprTraceback.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 04:32:24.000000 ReprTraceback-1.0.4/ReprTraceback/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 04:43:04.365085 ReprTraceback-1.0.4/ReprTraceback.egg-info/
+-rw-rw-rw-   0        0        0     1898 2023-06-22 04:43:03.000000 ReprTraceback-1.0.4/ReprTraceback.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-06-22 04:43:04.000000 ReprTraceback-1.0.4/ReprTraceback.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 04:43:03.000000 ReprTraceback-1.0.4/ReprTraceback.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-22 04:43:03.000000 ReprTraceback-1.0.4/ReprTraceback.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 04:43:04.371110 ReprTraceback-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      582 2023-06-22 04:42:39.000000 ReprTraceback-1.0.4/setup.py
```

### Comparing `ReprTraceback-1.0.3/PKG-INFO` & `ReprTraceback-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReprTraceback
-Version: 1.0.3
+Version: 1.0.4
 Summary: Improve stack traces with the values associated with each argument in each frame.
 Home-page: https://github.com/NateRiz/ReprTraceback
 Author: NateRiz
 Author-email: natezriz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `ReprTraceback-1.0.3/README.md` & `ReprTraceback-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `ReprTraceback-1.0.3/ReprTraceback/ReprTraceback.py` & `ReprTraceback-1.0.4/ReprTraceback/ReprTraceback.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         # If immediate lookup was desired, trigger lookups now.
         if lookup_lines:
             for f in result:
                 formatted_line = ReprTraceback.get_formatted_function_exception(f)
                 if formatted_line:
                     f._line = formatted_line
                 f.line
-                f.locals.clear()
+                f.locals = {}
         return result
 
     @staticmethod
     def get_formatted_function_exception(current_frame: ReprFrameSummary):
         if current_frame.f_back is None:
             return ""
         args, varargs, kwargs = inspect.getargs(current_frame.f_code)
```

### Comparing `ReprTraceback-1.0.3/ReprTraceback.egg-info/PKG-INFO` & `ReprTraceback-1.0.4/ReprTraceback.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReprTraceback
-Version: 1.0.3
+Version: 1.0.4
 Summary: Improve stack traces with the values associated with each argument in each frame.
 Home-page: https://github.com/NateRiz/ReprTraceback
 Author: NateRiz
 Author-email: natezriz@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `ReprTraceback-1.0.3/setup.py` & `ReprTraceback-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ReprTraceback',
-    version='1.0.3',
+    version='1.0.4',
     description='Improve stack traces with the values associated with each argument in each frame.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='NateRiz',
     author_email='natezriz@gmail.com',
     url='https://github.com/NateRiz/ReprTraceback',
     packages=find_packages(),
```

