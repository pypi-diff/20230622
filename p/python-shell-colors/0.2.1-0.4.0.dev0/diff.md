# Comparing `tmp/python-shell-colors-0.2.1.tar.gz` & `tmp/python-shell-colors-0.4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-shell-colors-0.2.1.tar", last modified: Thu Sep  3 14:52:27 2020, max compression
+gzip compressed data, was "python-shell-colors-0.4.0.dev0.tar", last modified: Thu Jun 22 14:07:00 2023, max compression
```

## Comparing `python-shell-colors-0.2.1.tar` & `python-shell-colors-0.4.0.dev0.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2020-09-03 14:52:27.668501 python-shell-colors-0.2.1/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        0 2020-09-03 14:47:39.000000 python-shell-colors-0.2.1/COPYING
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      771 2020-09-03 14:52:27.668501 python-shell-colors-0.2.1/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        0 2020-09-03 14:47:39.000000 python-shell-colors-0.2.1/README.md
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2020-09-03 14:52:27.668501 python-shell-colors-0.2.1/pscolors/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1005 2020-09-03 14:47:39.000000 python-shell-colors-0.2.1/pscolors/__init__.py
-drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2020-09-03 14:52:27.668501 python-shell-colors-0.2.1/python_shell_colors.egg-info/
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      771 2020-09-03 14:52:27.000000 python-shell-colors-0.2.1/python_shell_colors.egg-info/PKG-INFO
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      271 2020-09-03 14:52:27.000000 python-shell-colors-0.2.1/python_shell_colors.egg-info/SOURCES.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2020-09-03 14:52:27.000000 python-shell-colors-0.2.1/python_shell_colors.egg-info/dependency_links.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2020-09-03 14:48:06.000000 python-shell-colors-0.2.1/python_shell_colors.egg-info/not-zip-safe
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        9 2020-09-03 14:52:27.000000 python-shell-colors-0.2.1/python_shell_colors.egg-info/top_level.txt
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1190 2020-09-03 14:52:27.668501 python-shell-colors-0.2.1/setup.cfg
--rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1265 2020-09-03 14:52:24.000000 python-shell-colors-0.2.1/setup.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-06-22 14:07:00.597067 python-shell-colors-0.4.0.dev0/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        0 2023-06-22 14:05:41.000000 python-shell-colors-0.4.0.dev0/COPYING
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      109 2023-06-22 14:05:41.000000 python-shell-colors-0.4.0.dev0/Makefile
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      759 2023-06-22 14:07:00.597067 python-shell-colors-0.4.0.dev0/PKG-INFO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        0 2023-06-22 14:05:41.000000 python-shell-colors-0.4.0.dev0/README.md
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       11 2023-06-22 14:06:54.000000 python-shell-colors-0.4.0.dev0/VERSION
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-06-22 14:07:00.593068 python-shell-colors-0.4.0.dev0/bcolors/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1005 2023-06-22 14:05:41.000000 python-shell-colors-0.4.0.dev0/bcolors/__init__.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-06-22 14:07:00.597067 python-shell-colors-0.4.0.dev0/python_shell_colors.egg-info/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      759 2023-06-22 14:07:00.000000 python-shell-colors-0.4.0.dev0/python_shell_colors.egg-info/PKG-INFO
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)      308 2023-06-22 14:07:00.000000 python-shell-colors-0.4.0.dev0/python_shell_colors.egg-info/SOURCES.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2023-06-22 14:07:00.000000 python-shell-colors-0.4.0.dev0/python_shell_colors.egg-info/dependency_links.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        1 2023-06-22 14:07:00.000000 python-shell-colors-0.4.0.dev0/python_shell_colors.egg-info/not-zip-safe
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)        8 2023-06-22 14:07:00.000000 python-shell-colors-0.4.0.dev0/python_shell_colors.egg-info/top_level.txt
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1195 2023-06-22 14:07:00.597067 python-shell-colors-0.4.0.dev0/setup.cfg
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)     1270 2023-06-22 14:06:54.000000 python-shell-colors-0.4.0.dev0/setup.py
+drwxrwxr-x   0 savchenk  (1000) savchenk  (1000)        0 2023-06-22 14:07:00.597067 python-shell-colors-0.4.0.dev0/tests/
+-rw-rw-r--   0 savchenk  (1000) savchenk  (1000)       92 2023-06-22 14:05:41.000000 python-shell-colors-0.4.0.dev0/tests/test_simple.py
```

### Comparing `python-shell-colors-0.2.1/pscolors/__init__.py` & `python-shell-colors-0.4.0.dev0/bcolors/__init__.py`

 * *Files identical despite different names*

### Comparing `python-shell-colors-0.2.1/setup.cfg` & `python-shell-colors-0.4.0.dev0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.1
+current_version = 0.4.0-dev0
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `python-shell-colors-0.2.1/setup.py` & `python-shell-colors-0.4.0.dev0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,10 +35,10 @@
     include_package_data=True,
     keywords='python_shell_colors',
     name='python-shell-colors',
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/volodymyrss/python-shell-colors',
-    version='0.2.1',
+    version='0.4.0-dev0',
     zip_safe=False,
 )
```

