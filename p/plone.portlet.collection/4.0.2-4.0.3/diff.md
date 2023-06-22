# Comparing `tmp/plone.portlet.collection-4.0.2.tar.gz` & `tmp/plone.portlet.collection-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.portlet.collection-4.0.2.tar", last modified: Thu Apr 13 23:41:48 2023, max compression
+gzip compressed data, was "plone.portlet.collection-4.0.3.tar", last modified: Thu Jun 22 19:18:11 2023, max compression
```

## Comparing `plone.portlet.collection-4.0.2.tar` & `plone.portlet.collection-4.0.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.024917 plone.portlet.collection-4.0.2/
--rw-r--r--   0 maurits    (501) staff       (20)     9287 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      162 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    10339 2023-04-13 23:41:48.025063 plone.portlet.collection-4.0.2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)       77 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.018319 plone.portlet.collection-4.0.2/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      686 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.018635 plone.portlet.collection-4.0.2/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.021289 plone.portlet.collection-4.0.2/plone/portlet/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.022804 plone.portlet.collection-4.0.2/plone/portlet/collection/
--rw-r--r--   0 maurits    (501) staff       (20)      395 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3986 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/collection.pt
--rw-r--r--   0 maurits    (501) staff       (20)    10066 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/collection.py
--rw-r--r--   0 maurits    (501) staff       (20)     1141 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/configure.zcml
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.015086 plone.portlet.collection-4.0.2/plone/portlet/collection/profiles/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.023435 plone.portlet.collection-4.0.2/plone/portlet/collection/profiles/default/
--rw-r--r--   0 maurits    (501) staff       (20)      187 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/profiles/default/metadata.xml
--rw-r--r--   0 maurits    (501) staff       (20)      415 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/profiles/default/portlets.xml
--rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/testing.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.024640 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     5876 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/functional.txt
--rw-r--r--   0 maurits    (501) staff       (20)      947 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/test_functional_doctest.py
--rw-r--r--   0 maurits    (501) staff       (20)    16311 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone/portlet/collection/tests/test_portlet_collection.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-04-13 23:41:48.020982 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    10339 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1035 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       20 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      327 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1682 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       62 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/requirements-6.0.x.txt
--rw-r--r--   0 maurits    (501) staff       (20)      224 2023-04-13 23:41:48.025613 plone.portlet.collection-4.0.2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-04-13 23:41:47.000000 plone.portlet.collection-4.0.2/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.274449 plone.portlet.collection-4.0.3/
+-rw-r--r--   0 maurits    (501) staff       (20)     9476 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      162 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    10528 2023-06-22 19:18:11.274094 plone.portlet.collection-4.0.3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)       77 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.267699 plone.portlet.collection-4.0.3/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      686 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.268011 plone.portlet.collection-4.0.3/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.270631 plone.portlet.collection-4.0.3/plone/portlet/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.271987 plone.portlet.collection-4.0.3/plone/portlet/collection/
+-rw-r--r--   0 maurits    (501) staff       (20)      395 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3986 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/collection.pt
+-rw-r--r--   0 maurits    (501) staff       (20)    10130 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/collection.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1141 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/configure.zcml
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.264959 plone.portlet.collection-4.0.3/plone/portlet/collection/profiles/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.272542 plone.portlet.collection-4.0.3/plone/portlet/collection/profiles/default/
+-rw-r--r--   0 maurits    (501) staff       (20)      187 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/profiles/default/metadata.xml
+-rw-r--r--   0 maurits    (501) staff       (20)      415 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/profiles/default/portlets.xml
+-rw-r--r--   0 maurits    (501) staff       (20)     1501 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/testing.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.273660 plone.portlet.collection-4.0.3/plone/portlet/collection/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5876 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/tests/functional.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      947 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/tests/test_functional_doctest.py
+-rw-r--r--   0 maurits    (501) staff       (20)    16311 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/plone/portlet/collection/tests/test_portlet_collection.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-06-22 19:18:11.270373 plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    10528 2023-06-22 19:18:11.000000 plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1025 2023-06-22 19:18:11.000000 plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:18:11.000000 plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       20 2023-06-22 19:18:11.000000 plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-06-22 19:18:11.000000 plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      327 2023-06-22 19:18:11.000000 plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2023-06-22 19:18:11.000000 plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3900 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       62 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/requirements-6.0.x.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2023-06-22 19:18:11.274519 plone.portlet.collection-4.0.3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1937 2023-06-22 19:18:10.000000 plone.portlet.collection-4.0.3/setup.py
```

### Comparing `plone.portlet.collection-4.0.2/CHANGES.rst` & `plone.portlet.collection-4.0.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Fix TypeError with "Select random items" option. @alecpm (#36)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (7723aeaf)
+
+
 4.0.2 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.portlet.collection-4.0.2/PKG-INFO` & `plone.portlet.collection-4.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.portlet.collection
-Version: 4.0.2
+Version: 4.0.3
 Summary: A portlet that fetches results from a collection
 Home-page: https://pypi.org/project/plone.portlet.collection/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection portlet
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,14 +34,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Fix TypeError with "Select random items" option. @alecpm (#36)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (7723aeaf)
+
+
 4.0.2 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.portlet.collection-4.0.2/docs/LICENSE.GPL` & `plone.portlet.collection-4.0.3/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.2/docs/LICENSE.txt` & `plone.portlet.collection-4.0.3/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.2/plone/portlet/collection/collection.pt` & `plone.portlet.collection-4.0.3/plone/portlet/collection/collection.pt`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.2/plone/portlet/collection/collection.py` & `plone.portlet.collection-4.0.3/plone/portlet/collection/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,17 +251,19 @@
             exclude_context = getattr(self.data, "exclude_context", False)
             results = collection.queryCatalog(sort_on=None)
             if results is None:
                 return []
             limit = self.data.limit and min(len(results), self.data.limit) or 1
 
             if exclude_context:
-                results = [
+                results = tuple(
                     brain for brain in results if brain.getPath() != context_path
-                ]
+                )
+            else:
+                results = tuple(results)
             if len(results) < limit:
                 limit = len(results)
             results = random.sample(results, limit)
 
         return results
 
     @memoize
```

### Comparing `plone.portlet.collection-4.0.2/plone/portlet/collection/configure.zcml` & `plone.portlet.collection-4.0.3/plone/portlet/collection/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.2/plone/portlet/collection/testing.py` & `plone.portlet.collection-4.0.3/plone/portlet/collection/testing.py`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.2/plone/portlet/collection/tests/functional.txt` & `plone.portlet.collection-4.0.3/plone/portlet/collection/tests/functional.txt`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.2/plone/portlet/collection/tests/test_functional_doctest.py` & `plone.portlet.collection-4.0.3/plone/portlet/collection/tests/test_functional_doctest.py`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.2/plone/portlet/collection/tests/test_portlet_collection.py` & `plone.portlet.collection-4.0.3/plone/portlet/collection/tests/test_portlet_collection.py`

 * *Files identical despite different names*

### Comparing `plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/PKG-INFO` & `plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.portlet.collection
-Version: 4.0.2
+Version: 4.0.3
 Summary: A portlet that fetches results from a collection
 Home-page: https://pypi.org/project/plone.portlet.collection/
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: collection portlet
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,14 +34,30 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+4.0.3 (2023-06-22)
+------------------
+
+Bug fixes:
+
+
+- Fix TypeError with "Select random items" option. @alecpm (#36)
+
+
+Internal:
+
+
+- Update configuration files.
+  [plone devs] (7723aeaf)
+
+
 4.0.2 (2023-04-14)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.portlet.collection-4.0.2/plone.portlet.collection.egg-info/SOURCES.txt` & `plone.portlet.collection-4.0.3/plone.portlet.collection.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CHANGES.rst
 CONTRIBUTING.rst
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements-6.0.x.txt
-setup.cfg
 setup.py
 docs/LICENSE.GPL
 docs/LICENSE.txt
 plone/__init__.py
 plone.portlet.collection.egg-info/PKG-INFO
 plone.portlet.collection.egg-info/SOURCES.txt
 plone.portlet.collection.egg-info/dependency_links.txt
```

### Comparing `plone.portlet.collection-4.0.2/setup.py` & `plone.portlet.collection-4.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "4.0.2"
+version = "4.0.3"
 
 setup(
     name="plone.portlet.collection",
     version=version,
     description="A portlet that fetches results from a collection",
     long_description=open("README.rst").read() + "\n" + open("CHANGES.rst").read(),
     classifiers=[
```

