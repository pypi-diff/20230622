# Comparing `tmp/snaptext-0.1.0.tar.gz` & `tmp/snaptext-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snaptext-0.1.0.tar", last modified: Tue May 23 12:49:11 2023, max compression
+gzip compressed data, was "snaptext-0.1.1.tar", last modified: Thu Jun 22 12:36:58 2023, max compression
```

## Comparing `snaptext-0.1.0.tar` & `snaptext-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 12:49:11.167526 snaptext-0.1.0/
--rw-r--r--   0 simon      (501) staff       (20)     1611 2023-05-23 12:49:11.167399 snaptext-0.1.0/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      439 2023-05-23 12:48:27.000000 snaptext-0.1.0/pyproject.toml
--rw-r--r--   0 simon      (501) staff       (20)     1319 2023-05-23 12:45:17.000000 snaptext-0.1.0/readme.md
--rw-r--r--   0 simon      (501) staff       (20)       38 2023-05-23 12:49:11.167563 snaptext-0.1.0/setup.cfg
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 12:49:11.166423 snaptext-0.1.0/snaptext/
--rw-r--r--   0 simon      (501) staff       (20)       63 2023-05-18 00:11:31.000000 snaptext-0.1.0/snaptext/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)     7595 2023-05-23 09:29:26.000000 snaptext-0.1.0/snaptext/core.py
--rw-r--r--   0 simon      (501) staff       (20)     3520 2023-05-23 09:30:04.000000 snaptext-0.1.0/snaptext/json.py
--rw-r--r--   0 simon      (501) staff       (20)     6679 2023-05-23 10:35:18.000000 snaptext-0.1.0/snaptext/string.py
--rw-r--r--   0 simon      (501) staff       (20)      816 2023-05-23 09:30:42.000000 snaptext-0.1.0/snaptext/value.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-23 12:49:11.167182 snaptext-0.1.0/snaptext.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     1611 2023-05-23 12:49:11.000000 snaptext-0.1.0/snaptext.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      244 2023-05-23 12:49:11.000000 snaptext-0.1.0/snaptext.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-23 12:49:11.000000 snaptext-0.1.0/snaptext.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)        9 2023-05-23 12:49:11.000000 snaptext-0.1.0/snaptext.egg-info/top_level.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-22 12:36:58.074703 snaptext-0.1.1/
+-rw-r--r--   0 simon      (501) staff       (20)     1611 2023-06-22 12:36:58.074580 snaptext-0.1.1/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      439 2023-06-22 12:36:21.000000 snaptext-0.1.1/pyproject.toml
+-rw-r--r--   0 simon      (501) staff       (20)     1319 2023-05-23 12:45:17.000000 snaptext-0.1.1/readme.md
+-rw-r--r--   0 simon      (501) staff       (20)       38 2023-06-22 12:36:58.074735 snaptext-0.1.1/setup.cfg
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-22 12:36:58.073628 snaptext-0.1.1/snaptext/
+-rw-r--r--   0 simon      (501) staff       (20)       63 2023-05-18 00:11:31.000000 snaptext-0.1.1/snaptext/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)     7595 2023-05-23 09:29:26.000000 snaptext-0.1.1/snaptext/core.py
+-rw-r--r--   0 simon      (501) staff       (20)     3520 2023-05-23 09:30:04.000000 snaptext-0.1.1/snaptext/json.py
+-rw-r--r--   0 simon      (501) staff       (20)     6737 2023-06-05 11:47:51.000000 snaptext-0.1.1/snaptext/string.py
+-rw-r--r--   0 simon      (501) staff       (20)      854 2023-06-06 13:54:14.000000 snaptext-0.1.1/snaptext/value.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-06-22 12:36:58.074400 snaptext-0.1.1/snaptext.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     1611 2023-06-22 12:36:58.000000 snaptext-0.1.1/snaptext.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      244 2023-06-22 12:36:58.000000 snaptext-0.1.1/snaptext.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-06-22 12:36:58.000000 snaptext-0.1.1/snaptext.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)        9 2023-06-22 12:36:58.000000 snaptext-0.1.1/snaptext.egg-info/top_level.txt
```

### Comparing `snaptext-0.1.0/PKG-INFO` & `snaptext-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snaptext
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for manipulating strings while retaining source positions in the resulting object
 License: EUPL-1.2
 Project-URL: repository, https://github.com/slietar/snaptext
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Snaptext
```

### Comparing `snaptext-0.1.0/readme.md` & `snaptext-0.1.1/readme.md`

 * *Files identical despite different names*

### Comparing `snaptext-0.1.0/snaptext/core.py` & `snaptext-0.1.1/snaptext/core.py`

 * *Files identical despite different names*

### Comparing `snaptext-0.1.0/snaptext/json.py` & `snaptext-0.1.1/snaptext/json.py`

 * *Files identical despite different names*

### Comparing `snaptext-0.1.0/snaptext/string.py` & `snaptext-0.1.1/snaptext/string.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,21 +17,20 @@
     ...
 
   @overload
   def __init__(self, value: Self | str, /):
     ...
 
   def __init__(self, value: Self | str, area: Optional[LocationArea] = None, *, symbolic: bool = False):
-    if isinstance(value, LocatedString):
-      pass
-
     if area is not None:
       LocatedValue.__init__(self, value, area)
-    elif isinstance(value, LocatedString):
-      LocatedValue.__init__(self, value.value, value.area)
+    elif hasattr(value, 'area'):
+      LocatedValue.__init__(self, value.value, value.area) # type: ignore
+    # elif isinstance(value, LocatedString):
+    #   LocatedValue.__init__(self, value.value, value.area)
     else:
       LocatedValue.__init__(self, value, Source(value).area)
 
     self.symbolic = symbolic
 
   # Overriden methods
```

### Comparing `snaptext-0.1.0/snaptext/value.py` & `snaptext-0.1.1/snaptext/value.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from .core import LocationArea
 
 
 T = TypeVar('T')
 
 class LocatedValue(Generic[T]):
+  __match_args__ = ('value', 'area')
+
   def __init__(self, value: T, area: LocationArea):
     self.area = area
     self.value = value
 
   @property
   def source(self):
     return self.area.source
```

### Comparing `snaptext-0.1.0/snaptext.egg-info/PKG-INFO` & `snaptext-0.1.1/snaptext.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snaptext
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for manipulating strings while retaining source positions in the resulting object
 License: EUPL-1.2
 Project-URL: repository, https://github.com/slietar/snaptext
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # Snaptext
```

