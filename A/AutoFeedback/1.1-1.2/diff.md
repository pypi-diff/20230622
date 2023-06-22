# Comparing `tmp/AutoFeedback-1.1.tar.gz` & `tmp/AutoFeedback-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoFeedback-1.1.tar", last modified: Mon Mar 20 10:30:08 2023, max compression
+gzip compressed data, was "AutoFeedback-1.2.tar", last modified: Thu Jun 22 18:28:16 2023, max compression
```

## Comparing `AutoFeedback-1.1.tar` & `AutoFeedback-1.2.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-03-20 10:30:08.817019 AutoFeedback-1.1/
--rw-r--r--   0 abrown41   (502) staff       (20)      162 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AUTHORS.rst
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-03-20 10:30:08.817610 AutoFeedback-1.1/AutoFeedback/
--rw-r--r--   0 abrown41   (502) staff       (20)      214 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/__init__.py
--rw-r--r--   0 abrown41   (502) staff       (20)      495 2023-03-20 10:30:08.817651 AutoFeedback-1.1/AutoFeedback/_version.py
--rw-r--r--   0 abrown41   (502) staff       (20)      283 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/bcolors.py
--rw-r--r--   0 abrown41   (502) staff       (20)     7052 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/funcchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4557 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/function_error_messages.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4374 2023-03-20 10:13:20.000000 AutoFeedback-1.1/AutoFeedback/plot_error_messages.py
--rw-r--r--   0 abrown41   (502) staff       (20)     9000 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/plotchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4391 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/plotclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)    16126 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/randomclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)      431 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/utils.py
--rw-r--r--   0 abrown41   (502) staff       (20)     4119 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/varchecks.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3986 2023-03-20 10:13:58.000000 AutoFeedback-1.1/AutoFeedback/variable_error_messages.py
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-03-20 10:30:08.814145 AutoFeedback-1.1/AutoFeedback.egg-info/
--rw-r--r--   0 abrown41   (502) staff       (20)     2692 2023-03-20 10:30:08.000000 AutoFeedback-1.1/AutoFeedback.egg-info/PKG-INFO
--rw-r--r--   0 abrown41   (502) staff       (20)      960 2023-03-20 10:30:08.000000 AutoFeedback-1.1/AutoFeedback.egg-info/SOURCES.txt
--rw-r--r--   0 abrown41   (502) staff       (20)        1 2023-03-20 10:30:08.000000 AutoFeedback-1.1/AutoFeedback.egg-info/dependency_links.txt
--rw-r--r--   0 abrown41   (502) staff       (20)       63 2023-03-20 10:30:08.000000 AutoFeedback-1.1/AutoFeedback.egg-info/requires.txt
--rw-r--r--   0 abrown41   (502) staff       (20)       18 2023-03-20 10:30:08.000000 AutoFeedback-1.1/AutoFeedback.egg-info/top_level.txt
--rw-r--r--   0 abrown41   (502) staff       (20)     3081 2023-03-20 10:13:58.000000 AutoFeedback-1.1/CONTRIBUTING.rst
--rw-r--r--   0 abrown41   (502) staff       (20)     1520 2023-03-20 10:13:58.000000 AutoFeedback-1.1/LICENSE
--rw-r--r--   0 abrown41   (502) staff       (20)      398 2023-03-20 10:13:58.000000 AutoFeedback-1.1/MANIFEST.in
--rw-r--r--   0 abrown41   (502) staff       (20)     2692 2023-03-20 10:30:08.817142 AutoFeedback-1.1/PKG-INFO
--rw-r--r--   0 abrown41   (502) staff       (20)     2157 2023-03-20 10:13:58.000000 AutoFeedback-1.1/README.rst
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-03-20 10:30:08.814535 AutoFeedback-1.1/docs/
--rw-r--r--   0 abrown41   (502) staff       (20)      673 2023-03-20 10:13:58.000000 AutoFeedback-1.1/docs/Makefile
--rw-r--r--   0 abrown41   (502) staff       (20)      797 2023-03-20 10:13:58.000000 AutoFeedback-1.1/docs/make.bat
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-03-20 10:30:08.815231 AutoFeedback-1.1/docs/source/
--rw-r--r--   0 abrown41   (502) staff       (20)     6730 2023-03-20 10:13:58.000000 AutoFeedback-1.1/docs/source/conf.py
--rw-r--r--   0 abrown41   (502) staff       (20)      396 2023-03-20 10:13:58.000000 AutoFeedback-1.1/docs/source/index.rst
--rw-r--r--   0 abrown41   (502) staff       (20)     1083 2023-03-20 10:13:58.000000 AutoFeedback-1.1/docs/source/min_versions.rst
--rw-r--r--   0 abrown41   (502) staff       (20)    30606 2023-03-20 10:13:58.000000 AutoFeedback-1.1/docs/source/usage.rst
--rw-r--r--   0 abrown41   (502) staff       (20)       29 2023-03-20 10:13:58.000000 AutoFeedback-1.1/requirements.txt
--rw-r--r--   0 abrown41   (502) staff       (20)      408 2023-03-20 10:30:08.817434 AutoFeedback-1.1/setup.cfg
--rw-r--r--   0 abrown41   (502) staff       (20)     2414 2023-03-20 10:13:58.000000 AutoFeedback-1.1/setup.py
-drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-03-20 10:30:08.816899 AutoFeedback-1.1/test/
--rw-r--r--   0 abrown41   (502) staff       (20)        0 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/__init__.py
--rw-r--r--   0 abrown41   (502) staff       (20)       32 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/printtest.py
--rw-r--r--   0 abrown41   (502) staff       (20)     9518 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testerrors.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3525 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testfuncs.py
--rw-r--r--   0 abrown41   (502) staff       (20)     3497 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testplot.py
--rw-r--r--   0 abrown41   (502) staff       (20)     2780 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testplotclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)      578 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testprint.py
--rw-r--r--   0 abrown41   (502) staff       (20)    11743 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testrandomclass.py
--rw-r--r--   0 abrown41   (502) staff       (20)     1976 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testsymp.py
--rw-r--r--   0 abrown41   (502) staff       (20)      970 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testutils.py
--rw-r--r--   0 abrown41   (502) staff       (20)     2224 2023-03-20 10:13:58.000000 AutoFeedback-1.1/test/testvars.py
--rw-r--r--   0 abrown41   (502) staff       (20)    78254 2023-03-20 10:13:58.000000 AutoFeedback-1.1/versioneer.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.787516 AutoFeedback-1.2/
+-rw-r--r--   0 abrown41   (502) staff       (20)      162 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AUTHORS.rst
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.788144 AutoFeedback-1.2/AutoFeedback/
+-rw-r--r--   0 abrown41   (502) staff       (20)      214 2023-04-25 17:16:18.000000 AutoFeedback-1.2/AutoFeedback/__init__.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      495 2023-06-22 18:28:16.788186 AutoFeedback-1.2/AutoFeedback/_version.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      283 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/bcolors.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     7052 2023-06-22 17:57:56.000000 AutoFeedback-1.2/AutoFeedback/funcchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4557 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/function_error_messages.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4374 2023-06-22 18:26:48.000000 AutoFeedback-1.2/AutoFeedback/plot_error_messages.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     9009 2023-06-22 18:26:41.000000 AutoFeedback-1.2/AutoFeedback/plotchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4391 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/plotclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    16126 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/randomclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      431 2023-06-22 17:57:56.000000 AutoFeedback-1.2/AutoFeedback/utils.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     4119 2023-06-22 17:57:56.000000 AutoFeedback-1.2/AutoFeedback/varchecks.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3986 2023-03-20 10:13:58.000000 AutoFeedback-1.2/AutoFeedback/variable_error_messages.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.785342 AutoFeedback-1.2/AutoFeedback.egg-info/
+-rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/PKG-INFO
+-rw-r--r--   0 abrown41   (502) staff       (20)      999 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/SOURCES.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)        1 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/dependency_links.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       20 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/entry_points.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       63 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/requires.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)       18 2023-06-22 18:28:16.000000 AutoFeedback-1.2/AutoFeedback.egg-info/top_level.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)     3081 2023-03-20 10:13:58.000000 AutoFeedback-1.2/CONTRIBUTING.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)     1520 2023-03-20 10:13:58.000000 AutoFeedback-1.2/LICENSE
+-rw-r--r--   0 abrown41   (502) staff       (20)      398 2023-03-20 10:13:58.000000 AutoFeedback-1.2/MANIFEST.in
+-rw-r--r--   0 abrown41   (502) staff       (20)     2712 2023-06-22 18:28:16.787627 AutoFeedback-1.2/PKG-INFO
+-rw-r--r--   0 abrown41   (502) staff       (20)     2157 2023-03-20 10:13:58.000000 AutoFeedback-1.2/README.rst
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.785616 AutoFeedback-1.2/docs/
+-rw-r--r--   0 abrown41   (502) staff       (20)      673 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/Makefile
+-rw-r--r--   0 abrown41   (502) staff       (20)      797 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/make.bat
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.786085 AutoFeedback-1.2/docs/source/
+-rw-r--r--   0 abrown41   (502) staff       (20)     6730 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/source/conf.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      396 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/source/index.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)     1083 2023-03-20 10:13:58.000000 AutoFeedback-1.2/docs/source/min_versions.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)    30606 2023-06-22 17:57:56.000000 AutoFeedback-1.2/docs/source/usage.rst
+-rw-r--r--   0 abrown41   (502) staff       (20)       29 2023-06-22 17:57:53.000000 AutoFeedback-1.2/requirements.txt
+-rw-r--r--   0 abrown41   (502) staff       (20)      408 2023-06-22 18:28:16.787994 AutoFeedback-1.2/setup.cfg
+-rw-r--r--   0 abrown41   (502) staff       (20)     2414 2023-03-20 10:13:58.000000 AutoFeedback-1.2/setup.py
+drwxr-xr-x   0 abrown41   (502) staff       (20)        0 2023-06-22 18:28:16.787402 AutoFeedback-1.2/test/
+-rw-r--r--   0 abrown41   (502) staff       (20)        0 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/__init__.py
+-rw-r--r--   0 abrown41   (502) staff       (20)       32 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/printtest.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     9518 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testerrors.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3525 2023-06-22 17:57:56.000000 AutoFeedback-1.2/test/testfuncs.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     3497 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testplot.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     2780 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testplotclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      578 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testprint.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    11743 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testrandomclass.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     1976 2023-03-20 10:13:58.000000 AutoFeedback-1.2/test/testsymp.py
+-rw-r--r--   0 abrown41   (502) staff       (20)      970 2023-06-22 17:57:56.000000 AutoFeedback-1.2/test/testutils.py
+-rw-r--r--   0 abrown41   (502) staff       (20)     2224 2023-06-22 17:57:56.000000 AutoFeedback-1.2/test/testvars.py
+-rw-r--r--   0 abrown41   (502) staff       (20)    78254 2023-03-20 10:13:58.000000 AutoFeedback-1.2/versioneer.py
```

### Comparing `AutoFeedback-1.1/AutoFeedback/funcchecks.py` & `AutoFeedback-1.2/AutoFeedback/funcchecks.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/AutoFeedback/function_error_messages.py` & `AutoFeedback-1.2/AutoFeedback/function_error_messages.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/AutoFeedback/plot_error_messages.py` & `AutoFeedback-1.2/AutoFeedback/plot_error_messages.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/AutoFeedback/plotchecks.py` & `AutoFeedback-1.2/AutoFeedback/plotchecks.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,15 @@
         lines, patch, axes, labels, legends =\
             _extract_plot_elements(fighand, lines=(len(explines) > 0),
                                    patches=exppatch, axes=bool(expaxes),
                                    axislabels=bool(explabels),
                                    legend=explegend)
         explegends = [line.label for line in explines
                       if line.label is not None]
-        expline = ""
+        expline = explines[0]
         if not check_partial:
             if explines:
                 assert (len(lines) == len(explines)), "_datasets"
             if explegend:
                 assert (len(legends) == len(explegends)), "_legend"
 
         if (explines and not lines):
```

### Comparing `AutoFeedback-1.1/AutoFeedback/plotclass.py` & `AutoFeedback-1.2/AutoFeedback/plotclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/AutoFeedback/randomclass.py` & `AutoFeedback-1.2/AutoFeedback/randomclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/AutoFeedback/varchecks.py` & `AutoFeedback-1.2/AutoFeedback/varchecks.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/AutoFeedback/variable_error_messages.py` & `AutoFeedback-1.2/AutoFeedback/variable_error_messages.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/AutoFeedback.egg-info/PKG-INFO` & `AutoFeedback-1.2/AutoFeedback.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: AutoFeedback
-Version: 1.1
+Version: 1.2
 Summary: check basic python exercises with pretty feedback
 Home-page: https://github.com/abrown41/AutoFeedback
 Author: Andrew Brown
 Author-email: andrew.brown@qub.ac.uk
 License: BSD (3-clause)
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: sympy
@@ -72,7 +73,9 @@
     pip install -e .
 
 
 =====
 Usage
 =====
 Full usage instructions can be found `here. <https://abrown41.github.io/AutoFeedback/usage.html>`_
+
+
```

### Comparing `AutoFeedback-1.1/AutoFeedback.egg-info/SOURCES.txt` & `AutoFeedback-1.2/AutoFeedback.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 AutoFeedback/randomclass.py
 AutoFeedback/utils.py
 AutoFeedback/varchecks.py
 AutoFeedback/variable_error_messages.py
 AutoFeedback.egg-info/PKG-INFO
 AutoFeedback.egg-info/SOURCES.txt
 AutoFeedback.egg-info/dependency_links.txt
+AutoFeedback.egg-info/entry_points.txt
 AutoFeedback.egg-info/requires.txt
 AutoFeedback.egg-info/top_level.txt
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
 docs/source/min_versions.rst
```

### Comparing `AutoFeedback-1.1/CONTRIBUTING.rst` & `AutoFeedback-1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/LICENSE` & `AutoFeedback-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/PKG-INFO` & `AutoFeedback-1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: AutoFeedback
-Version: 1.1
+Version: 1.2
 Summary: check basic python exercises with pretty feedback
 Home-page: https://github.com/abrown41/AutoFeedback
 Author: Andrew Brown
 Author-email: andrew.brown@qub.ac.uk
 License: BSD (3-clause)
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: sympy
@@ -72,7 +73,9 @@
     pip install -e .
 
 
 =====
 Usage
 =====
 Full usage instructions can be found `here. <https://abrown41.github.io/AutoFeedback/usage.html>`_
+
+
```

### Comparing `AutoFeedback-1.1/README.rst` & `AutoFeedback-1.2/README.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/docs/Makefile` & `AutoFeedback-1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/docs/make.bat` & `AutoFeedback-1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/docs/source/conf.py` & `AutoFeedback-1.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/docs/source/min_versions.rst` & `AutoFeedback-1.2/docs/source/min_versions.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/docs/source/usage.rst` & `AutoFeedback-1.2/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/setup.py` & `AutoFeedback-1.2/setup.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testerrors.py` & `AutoFeedback-1.2/test/testerrors.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testfuncs.py` & `AutoFeedback-1.2/test/testfuncs.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testplot.py` & `AutoFeedback-1.2/test/testplot.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testplotclass.py` & `AutoFeedback-1.2/test/testplotclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testprint.py` & `AutoFeedback-1.2/test/testprint.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testrandomclass.py` & `AutoFeedback-1.2/test/testrandomclass.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testsymp.py` & `AutoFeedback-1.2/test/testsymp.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testutils.py` & `AutoFeedback-1.2/test/testutils.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/test/testvars.py` & `AutoFeedback-1.2/test/testvars.py`

 * *Files identical despite different names*

### Comparing `AutoFeedback-1.1/versioneer.py` & `AutoFeedback-1.2/versioneer.py`

 * *Files identical despite different names*

