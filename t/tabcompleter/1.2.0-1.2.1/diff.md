# Comparing `tmp/tabcompleter-1.2.0.tar.gz` & `tmp/tabcompleter-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tabcompleter-1.2.0.tar", last modified: Mon Apr 17 17:53:33 2023, max compression
+gzip compressed data, was "tabcompleter-1.2.1.tar", last modified: Thu Jun 22 14:39:09 2023, max compression
```

## Comparing `tabcompleter-1.2.0.tar` & `tabcompleter-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-17 17:53:33.409340 tabcompleter-1.2.0/
--rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 tabcompleter-1.2.0/.gitignore
--rwxr-xr-x   0 michael    (501) staff       (20)     1576 2022-11-28 07:10:47.000000 tabcompleter-1.2.0/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 michael    (501) staff       (20)     1704 2022-11-28 07:13:14.000000 tabcompleter-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 michael    (501) staff       (20)     1074 2022-11-28 07:13:28.000000 tabcompleter-1.2.0/LICENSE
--rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 tabcompleter-1.2.0/MANIFEST.in
--rw-r--r--   0 michael    (501) staff       (20)     3542 2023-04-17 17:53:33.409390 tabcompleter-1.2.0/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     1480 2022-11-29 01:41:11.000000 tabcompleter-1.2.0/README.md
--rwxr-xr-x   0 michael    (501) staff       (20)      327 2022-11-28 07:12:39.000000 tabcompleter-1.2.0/SECURITY.md
--rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-04-17 17:53:33.409557 tabcompleter-1.2.0/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     5239 2023-04-17 17:52:50.000000 tabcompleter-1.2.0/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-17 17:53:33.408754 tabcompleter-1.2.0/src/
--rwxr-xr-x   0 michael    (501) staff       (20)       28 2022-11-28 07:23:01.000000 tabcompleter-1.2.0/src/__init__.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-04-17 17:53:33.409243 tabcompleter-1.2.0/src/tabcompleter.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     3542 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      341 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)       45 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       13 2023-04-17 17:53:33.000000 tabcompleter-1.2.0/src/tabcompleter.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)    12516 2023-01-19 19:17:09.000000 tabcompleter-1.2.0/src/tabcompleter.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 14:39:09.001836 tabcompleter-1.2.1/
+-rw-r--r--   0 michael    (501) staff       (20)      774 2022-11-28 00:12:24.000000 tabcompleter-1.2.1/.gitignore
+-rwxr-xr-x   0 michael    (501) staff       (20)     1576 2022-11-28 07:10:47.000000 tabcompleter-1.2.1/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 michael    (501) staff       (20)     1704 2022-11-28 07:13:14.000000 tabcompleter-1.2.1/CONTRIBUTING.md
+-rw-r--r--   0 michael    (501) staff       (20)     1074 2022-11-28 07:13:28.000000 tabcompleter-1.2.1/LICENSE
+-rw-rw-r--   0 michael    (501) staff       (20)       34 2022-11-28 00:19:28.000000 tabcompleter-1.2.1/MANIFEST.in
+-rw-r--r--   0 michael    (501) staff       (20)     3542 2023-06-22 14:39:09.001897 tabcompleter-1.2.1/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     1480 2022-11-29 01:41:11.000000 tabcompleter-1.2.1/README.md
+-rwxr-xr-x   0 michael    (501) staff       (20)      327 2022-11-28 07:12:39.000000 tabcompleter-1.2.1/SECURITY.md
+-rwxr-xr-x   0 michael    (501) staff       (20)       88 2023-06-22 14:39:09.002086 tabcompleter-1.2.1/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     5317 2023-06-22 14:36:39.000000 tabcompleter-1.2.1/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 14:39:09.000933 tabcompleter-1.2.1/src/
+-rwxr-xr-x   0 michael    (501) staff       (20)       28 2022-11-28 07:23:01.000000 tabcompleter-1.2.1/src/__init__.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2023-06-22 14:39:09.001714 tabcompleter-1.2.1/src/tabcompleter.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     3542 2023-06-22 14:39:08.000000 tabcompleter-1.2.1/src/tabcompleter.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      341 2023-06-22 14:39:08.000000 tabcompleter-1.2.1/src/tabcompleter.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2023-06-22 14:39:08.000000 tabcompleter-1.2.1/src/tabcompleter.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)       45 2023-06-22 14:39:08.000000 tabcompleter-1.2.1/src/tabcompleter.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       13 2023-06-22 14:39:08.000000 tabcompleter-1.2.1/src/tabcompleter.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)    11952 2023-06-22 14:36:39.000000 tabcompleter-1.2.1/src/tabcompleter.py
```

### Comparing `tabcompleter-1.2.0/.gitignore` & `tabcompleter-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.2.0/CODE_OF_CONDUCT.md` & `tabcompleter-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.2.0/CONTRIBUTING.md` & `tabcompleter-1.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.2.0/LICENSE` & `tabcompleter-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.2.0/PKG-INFO` & `tabcompleter-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabcompleter
-Version: 1.2.0
+Version: 1.2.1
 Summary: tabcompleter --- Autocompletion in the Python console.
 Home-page: https://github.com/mdmintz/tabcompleter
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/tabcompleter/releases
```

### Comparing `tabcompleter-1.2.0/README.md` & `tabcompleter-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `tabcompleter-1.2.0/setup.py` & `tabcompleter-1.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,37 +20,37 @@
     long_description = "\n".join(long_description_lines)
 except IOError:
     long_description = "tabcompleter --- Autocompletion in the Python console."
 
 if sys.argv[-1] == "publish":
     reply = None
     input_method = input
-    if not sys.version_info[0] >= 3:
-        input_method = raw_input  # noqa: F821
     confirm_text = ">>> Confirm release PUBLISH to PyPI? (yes/no): "
     reply = str(input_method(confirm_text)).lower().strip()
     if reply == "yes":
+        if sys.version_info < (3, 9):
+            print("\nERROR! Publishing to PyPI requires Python>=3.9")
+            sys.exit()
         print("\n*** Checking code health with flake8:\n")
-        if sys.version_info >= (3, 9):
-            os.system("python -m pip install 'flake8==6.0.0'")
-        else:
-            os.system("python -m pip install 'flake8==5.0.4'")
+        os.system("python -m pip install 'flake8==6.0.0'")
         flake8_status = os.system("flake8 --exclude=.eggs,temp")
         if flake8_status != 0:
-            print("\nWARNING! Fix flake8 issues before publishing to PyPI!\n")
+            print("\nERROR! Fix flake8 issues before publishing to PyPI!\n")
             sys.exit()
         else:
             print("*** No flake8 issues detected. Continuing...")
         print("\n*** Removing existing distribution packages: ***\n")
         os.system("rm -f dist/*.egg; rm -f dist/*.tar.gz; rm -f dist/*.whl")
         os.system("rm -rf build/bdist.*; rm -rf build/lib")
         print("\n*** Installing build: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'build>=0.10.0'")
         print("\n*** Installing pkginfo: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'pkginfo>=1.9.6'")
+        print("\n*** Installing readme-renderer: *** (For PyPI uploads)\n")
+        os.system("python -m pip install --upgrade 'readme-renderer>=40.0'")
         print("\n*** Installing twine: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade 'twine>=4.0.2'")
         print("\n*** Installing tqdm: *** (Required for PyPI uploads)\n")
         os.system("python -m pip install --upgrade tqdm")
         print("\n*** Rebuilding distribution packages: ***\n")
         os.system("python -m build")  # Create new tar/wheel
         print("\n*** Publishing The Release to PyPI: ***\n")
@@ -58,15 +58,15 @@
         print("\n*** The Release was PUBLISHED SUCCESSFULLY to PyPI! :) ***\n")
     else:
         print("\n>>> The Release was NOT PUBLISHED to PyPI! <<<\n")
     sys.exit()
 
 setup(
     name="tabcompleter",
-    version="1.2.0",
+    version="1.2.1",
     description="tabcompleter --- Autocompletion in the Python console.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="tab completion console",
     url="https://github.com/mdmintz/tabcompleter",
     project_urls={
         "Changelog": "https://github.com/mdmintz/tabcompleter/releases",
```

### Comparing `tabcompleter-1.2.0/src/tabcompleter.egg-info/PKG-INFO` & `tabcompleter-1.2.1/src/tabcompleter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tabcompleter
-Version: 1.2.0
+Version: 1.2.1
 Summary: tabcompleter --- Autocompletion in the Python console.
 Home-page: https://github.com/mdmintz/tabcompleter
 Author: Michael Mintz
 Author-email: mdmintz@gmail.com
 Maintainer: Michael Mintz
 License: MIT
 Project-URL: Changelog, https://github.com/mdmintz/tabcompleter/releases
```

### Comparing `tabcompleter-1.2.0/src/tabcompleter.py` & `tabcompleter-1.2.1/src/tabcompleter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,19 @@
-"""tabcompleter: Python console tab-completion. Replaces fancycompleter."""
-
-from __future__ import with_statement
-from __future__ import print_function
+"""
+tabcompleter: Python console tab-completion. Replaces fancycompleter.
+=====================================================================
+"""
 import rlcompleter
 import sys
 import types
 import os.path
 from itertools import count
 
-PY3K = sys.version_info[0] >= 3
-
-# Python3 compatibility
-# ---------------------
-try:
-    from itertools import izip
-except ImportError:
-    izip = zip
-try:
-    from types import ClassType
-except ImportError:
-    ClassType = type
-try:
-    unicode
-except NameError:
-    unicode = str
-# ----------------------
-
 
 class LazyVersion(object):
-
     def __init__(self, pkg):
         self.pkg = pkg
         self.__version = None
 
     @property
     def version(self):
         if self.__version is None:
@@ -43,15 +24,14 @@
         try:
             from pkg_resources import get_distribution, DistributionNotFound
         except ImportError:
             return "N/A"
         try:
             return get_distribution(self.pkg).version
         except DistributionNotFound:
-            # Package is not installed
             return "N/A"
 
     def __repr__(self):
         return self.version
 
     def __eq__(self, other):
         return self.version == other
@@ -87,32 +67,29 @@
             color = getattr(cls, color)
         except AttributeError:
             pass
         return "\x1b[%sm%s\x1b[00m" % (color, string)
 
 
 class DefaultConfig:
-
     consider_getitems = True
     use_colors = "auto"
-    readline = None  # Set by setup()
+    readline = None
     color_by_type = {
         types.BuiltinMethodType: Color.turquoise,
         types.MethodType: Color.turquoise,
         type((42).__add__): Color.turquoise,
         type(int.__add__): Color.turquoise,
         type(str.replace): Color.turquoise,
         types.FunctionType: Color.blue,
         types.BuiltinFunctionType: Color.blue,
-        ClassType: Color.fuchsia,
         type: Color.fuchsia,
         types.ModuleType: Color.teal,
         type(None): Color.lightgray,
         str: Color.green,
-        unicode: Color.green,
         int: Color.yellow,
         float: Color.yellow,
         complex: Color.yellow,
         bool: Color.yellow,
     }
     color_by_baseclass = [
         ((BaseException,), Color.red),
@@ -269,16 +246,14 @@
                     word[:n] == attr
                     and not (noprefix and word[:n + 1] == noprefix)
                 ):
                     try:
                         val = getattr(thisobject, word)
                     except Exception:
                         val = None
-                    if not PY3K and isinstance(word, unicode):
-                        word = word.encode("utf-8")
                     names.append(word)
                     values.append(val)
             if names or not noprefix:
                 break
             if noprefix == "_":
                 noprefix = "__"
             else:
@@ -295,15 +270,15 @@
         if prefix:
             names += [" "]
         return names
 
     def color_matches(self, names, values):
         matches = [self.color_for_obj(i, name, obj)
                    for i, name, obj
-                   in izip(count(), names, values)]
+                   in zip(count(), names, values)]
         return matches + [" "]
 
     def color_for_obj(self, i, name, value):
         t = type(value)
         color = self.config.color_by_type.get(t, None)
         if color is None:
             for x, _color in self.config.color_by_baseclass:
@@ -345,15 +320,15 @@
     readline.set_completer(completer.complete)
     return completer
 
 
 def setup_history(completer, persist_history):
     import atexit
     readline = completer.config.readline
-    if isinstance(persist_history, (str, unicode)):
+    if isinstance(persist_history, str):
         filename = persist_history
     else:
         filename = "~/.history.py"
     filename = os.path.expanduser(filename)
     if os.path.isfile(filename):
         readline.read_history_file(filename)
```

