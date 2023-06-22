# Comparing `tmp/devcheck-0.3.tar.gz` & `tmp/devcheck-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcheck-0.3.tar", last modified: Thu Jun 22 14:36:03 2023, max compression
+gzip compressed data, was "devcheck-0.4.tar", last modified: Thu Jun 22 14:37:13 2023, max compression
```

## Comparing `devcheck-0.3.tar` & `devcheck-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-22 14:36:03.175713 devcheck-0.3/
--rw-r--r--   0 jwd2488    (501) staff       (20)       73 2023-06-22 14:36:03.175557 devcheck-0.3/PKG-INFO
--rw-r--r--   0 jwd2488    (501) staff       (20)        0 2023-06-20 02:17:54.000000 devcheck-0.3/README.md
-drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-22 14:36:03.174314 devcheck-0.3/devcheck/
--rw-r--r--   0 jwd2488    (501) staff       (20)        0 2023-06-20 02:17:54.000000 devcheck-0.3/devcheck/__init__.py
--rw-r--r--   0 jwd2488    (501) staff       (20)     8409 2023-06-22 14:20:28.000000 devcheck-0.3/devcheck/main.py
--rw-r--r--   0 jwd2488    (501) staff       (20)      859 2023-06-22 14:20:28.000000 devcheck-0.3/devcheck/mangocheck.py
-drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-22 14:36:03.175240 devcheck-0.3/devcheck.egg-info/
--rw-r--r--   0 jwd2488    (501) staff       (20)       73 2023-06-22 14:36:03.000000 devcheck-0.3/devcheck.egg-info/PKG-INFO
--rw-r--r--   0 jwd2488    (501) staff       (20)      242 2023-06-22 14:36:03.000000 devcheck-0.3/devcheck.egg-info/SOURCES.txt
--rw-r--r--   0 jwd2488    (501) staff       (20)        1 2023-06-22 14:36:03.000000 devcheck-0.3/devcheck.egg-info/dependency_links.txt
--rw-r--r--   0 jwd2488    (501) staff       (20)       48 2023-06-22 14:36:03.000000 devcheck-0.3/devcheck.egg-info/entry_points.txt
--rw-r--r--   0 jwd2488    (501) staff       (20)        9 2023-06-22 14:36:03.000000 devcheck-0.3/devcheck.egg-info/top_level.txt
--rw-r--r--   0 jwd2488    (501) staff       (20)       38 2023-06-22 14:36:03.175772 devcheck-0.3/setup.cfg
--rw-r--r--   0 jwd2488    (501) staff       (20)      273 2023-06-20 14:41:01.000000 devcheck-0.3/setup.py
+drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-22 14:37:13.040847 devcheck-0.4/
+-rw-r--r--   0 jwd2488    (501) staff       (20)       73 2023-06-22 14:37:13.040734 devcheck-0.4/PKG-INFO
+-rw-r--r--   0 jwd2488    (501) staff       (20)        0 2023-06-20 02:17:54.000000 devcheck-0.4/README.md
+drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-22 14:37:13.039981 devcheck-0.4/devcheck/
+-rw-r--r--   0 jwd2488    (501) staff       (20)        0 2023-06-20 02:17:54.000000 devcheck-0.4/devcheck/__init__.py
+-rw-r--r--   0 jwd2488    (501) staff       (20)     8409 2023-06-22 14:20:28.000000 devcheck-0.4/devcheck/main.py
+-rw-r--r--   0 jwd2488    (501) staff       (20)      990 2023-06-22 14:37:03.000000 devcheck-0.4/devcheck/mangocheck.py
+drwxr-xr-x   0 jwd2488    (501) staff       (20)        0 2023-06-22 14:37:13.040557 devcheck-0.4/devcheck.egg-info/
+-rw-r--r--   0 jwd2488    (501) staff       (20)       73 2023-06-22 14:37:13.000000 devcheck-0.4/devcheck.egg-info/PKG-INFO
+-rw-r--r--   0 jwd2488    (501) staff       (20)      242 2023-06-22 14:37:13.000000 devcheck-0.4/devcheck.egg-info/SOURCES.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)        1 2023-06-22 14:37:13.000000 devcheck-0.4/devcheck.egg-info/dependency_links.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)       48 2023-06-22 14:37:13.000000 devcheck-0.4/devcheck.egg-info/entry_points.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)        9 2023-06-22 14:37:13.000000 devcheck-0.4/devcheck.egg-info/top_level.txt
+-rw-r--r--   0 jwd2488    (501) staff       (20)       38 2023-06-22 14:37:13.040892 devcheck-0.4/setup.cfg
+-rw-r--r--   0 jwd2488    (501) staff       (20)      273 2023-06-22 14:37:07.000000 devcheck-0.4/setup.py
```

### Comparing `devcheck-0.3/devcheck/main.py` & `devcheck-0.4/devcheck/main.py`

 * *Files identical despite different names*

### Comparing `devcheck-0.3/devcheck/mangocheck.py` & `devcheck-0.4/devcheck/mangocheck.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from typing import Dict
 from main import Networking
 import json as j
+import sys
 
 
 def MangoCheck(data: Dict | str | None = None):
     """
     You can either give this function a raw dictionary or a string containing the filepath (relative paths should be based on the directory that you run devcheck from)
     """
 
     def wrap(f):
         def wrapper(*args, **kwargs):
-            json = {}
-            if isinstance(data, Dict):
-                json["inputs"] = data
-            elif isinstance(data, str):
-                with open(data) as file:
-                    json["inputs"] = j.loads(file.read())
-            else:
-                raise ValueError(f"{data} should not be done")
+            # very monkey but :shrug:
             result = f(*args, **kwargs)
-            json["lllml"] = result
-            Networking.post(f"{json}")
+            if sys.argv[0] == "devcheck":
+                json = {}
+                if isinstance(data, Dict):
+                    json["inputs"] = data
+                elif isinstance(data, str):
+                    with open(data) as file:
+                        json["inputs"] = j.loads(file.read())
+                else:
+                    raise ValueError(f"{data} should not be done")
+                json["lllml"] = result
+                Networking.post(f"{json}")
             return result
 
         return wrapper
 
     return wrap
```

